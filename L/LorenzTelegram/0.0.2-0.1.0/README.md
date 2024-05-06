# Comparing `tmp/lorenztelegram-0.0.2.tar.gz` & `tmp/lorenztelegram-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lorenztelegram-0.0.2.tar", last modified: Fri May  3 23:16:01 2024, max compression
+gzip compressed data, was "lorenztelegram-0.1.0.tar", last modified: Mon May  6 23:38:31 2024, max compression
```

## Comparing `lorenztelegram-0.0.2.tar` & `lorenztelegram-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       18 2024-04-30 20:46:05.645859 lorenztelegram-0.0.2/README.md
--rw-r--r--   0        0        0      597 2024-05-03 23:16:01.526323 lorenztelegram-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-30 20:46:05.645859 lorenztelegram-0.0.2/src/lorenztelegram/__init__.py
--rw-r--r--   0        0        0    11941 2024-05-03 22:40:50.502110 lorenztelegram-0.0.2/src/lorenztelegram/telegram.py
--rw-r--r--   0        0        0        0 2024-04-30 20:46:05.648187 lorenztelegram-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      465 1970-01-01 00:00:00.000000 lorenztelegram-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      692 2024-05-04 12:17:08.012216 lorenztelegram-0.1.0/README.md
+-rw-r--r--   0        0        0      597 2024-05-06 23:38:31.708267 lorenztelegram-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-30 20:46:05.645859 lorenztelegram-0.1.0/src/lorenztelegram/__init__.py
+-rw-r--r--   0        0        0    12307 2024-05-06 23:38:16.004246 lorenztelegram-0.1.0/src/lorenztelegram/configBlocks.py
+-rw-r--r--   0        0        0    14634 2024-05-06 23:38:16.004246 lorenztelegram-0.1.0/src/lorenztelegram/telegram.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:46:05.648187 lorenztelegram-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 lorenztelegram-0.1.0/PKG-INFO
```

### Comparing `lorenztelegram-0.0.2/pyproject.toml` & `lorenztelegram-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "LorenzTelegram"
-version = "0.0.2"
+version = "0.1.0"
 description = "A library to communicate with Lorenz Messtechnik sensors"
 authors = [
     { name = "Mikkel Jeppesen", email = "2756925+Duckle29@users.noreply.github.com" },
 ]
 dependencies = [
     "pyserial>=3.5",
 ]
```

### Comparing `lorenztelegram-0.0.2/src/lorenztelegram/telegram.py` & `lorenztelegram-0.1.0/src/lorenztelegram/telegram.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #!/usr/bin/env python3
 import warnings
 
 import serial
-import threading
-import time
-import math
+from pathlib import Path
 
 from enum import IntEnum
 
+from lorenztelegram.configBlocks import Config
+
+class UnsupportedCommand(Exception):
+    pass
+
 class Error(IntEnum):
     OK =                            0
     GENERIC =                       1
     WATCHDOG =                      2
     ROTOR_GENERIC =                 3
     ROTOR_WRONG_SPEED =             4
     ROTOR_TOO_SLOW =                5
@@ -45,15 +48,14 @@
     BAD_PARM =                      43
     BAD_ADDR =                      44
     CANT_OVERWRITE =                45
 
     STACK_OVERFLOW =                60
     ANGLE_OVERFLOW =                61
 
-
 class Command(IntEnum):
     STX =                           0x02,
     SCMD_ACK =                      0x06,
     SCMD_NACK =                     0x15,
     SCMD_Hello =                    0x40,
     SCMD_ReadRaw =                  0x41,
     SCMD_ReadStatus =               0x42,
@@ -88,59 +90,60 @@
 }
 
 class Telegram:
     def __init__(self, command: Command=None, addr_from: int=0xFF, addr_to: int=0x01, parameters: list[int] = []) -> None:
         self.command = command
         self.addr_to = addr_to
         self.addr_from = addr_from
+
+        if type(parameters) in [bytes, bytearray]:
+            parameters = list(parameters)
         self.parameters = parameters
 
         self.parameter_cnt = len(parameters)
         self.checksum = 0
         self.wchecksum = 0
 
         self.stuffed = False
         self.valid = False
         if command is not None:
-            self.calc_checksums()
+            self.checksum, self.wchecksum = self.calc_checksums()
     
     def from_bytes(self, bytes_obj: bytes):
         """Construct a Telegram object from a bytes object
 
         Args:
             bytes_obj (bytes): The serialized telegram
         """
 
         if bytes_obj[1] == Command.STX:
             bytes_obj = bytes_obj[2:] # Telegram must be stuffed with an extra STX, remove both
             self.stuffed = True
         else:
             bytes_obj = bytes_obj[1:] # Remove STX
         
-        self.command = bytes_obj[0]
+        self.command = Command(bytes_obj[0])
         self.addr_to = bytes_obj[1]
         self.addr_from = bytes_obj[2]
         self.parameter_cnt = bytes_obj[3]
         
         if self.parameter_cnt > 0:
+            self.parameters = []
             for b in bytes_obj[4:-2]:
                 self.parameters.append(b)
         
-        self.calc_checksums()
+        self.checksum, self.wchecksum = self.calc_checksums()
         self.valid = self.checksum == bytes_obj[-2] and self.wchecksum == bytes_obj[-1]
 
     def calc_checksums(self):
         """Generates checksums of telegram
            
            checksum: 1-byte sum of all the bytes in the message excluding stx and checksums
            wchecksum: 1-byte sum of all the checksums, with 1 added on overflows
 
-        Args:
-            telegram (list[int]): The telegram as 1-byte sized integers
-
         Returns:
             tuple[int, int]: The checksum and weighted checksum
         """
 
         tg = [self.command, self.addr_to, self.addr_from, self.parameter_cnt] + self.parameters
         
         checksum = 0
@@ -150,35 +153,53 @@
             checksum = checksum & 0xFF
             
             wchecksum += checksum
             if wchecksum > 0xFF:
                 wchecksum += 1
             wchecksum = wchecksum & 0xFF
         
-        self.checksum = checksum
-        self.wchecksum = wchecksum
+        return checksum, wchecksum
+
+    def stuff(self, payload: list[int]) -> list[int]:
+        out = []
+        for itm in payload:
+            out.append(itm)
+            if itm == Command.STX:
+                out.append(itm)
+        return out
 
     def serialize(self) -> bytes:
         """Serialize the Telegram to a bytes string for sending
 
         Returns:
             bytes: bytes string to send to sensor
         """
         tg = [self.command, self.addr_to, self.addr_from, self.parameter_cnt] + self.parameters
-        tg += [self.checksum, self.wchecksum]
+        tg += list(self.calc_checksums())
 
-        if Command.STX in tg:
-            # Stuff an extra STX in there
-            tg = [Command.STX] + tg
+        tg = self.stuff(tg)
 
         return bytes([Command.STX] + tg)
-        
 
 class LorenzConnector:
 
+    SAMPLE_RATES = {
+            20:     0xFA,
+            25:     0xC8,
+            50:     0x64,
+            100:    0x32,
+            200:    0x19,
+            250:    0x14,
+            500:    0x0A,
+            1000:   0x05,
+            1250:   0x04,
+            2500:   0x02,
+            5000:   0x01
+        }
+
     def __init__(self, port: str, timeout=0.01, **kwargs):
         """Create an object with a connection to a serial device
 
         Args:
             port (str): The serial port to connect to the device
             timeout (float): The timeout in to wait for new bytes from device when reading [s]
 
@@ -198,43 +219,43 @@
             del kwargs['port']
 
         self.ser = serial.Serial(**kwargs)
         self.ser.port = port
         self.ser.timeout = timeout
 
         self.mode = "undefined"
+
+        self.config = Config()
     
     def __enter__(self):
         self.ser.open()
         return self
     
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.ser.close()
     
-    def send_telegram(self, tg: Telegram) -> Telegram | None:
+    def _send_telegram(self, tg: Telegram) -> Telegram | None:
         """Send a Telegram and return the response (if any)
 
         Args:
             tg (Telegram): The Telegram object to send
 
         Returns:
             Telegram: Telegram response. None if sent telegram was a broadcast
         """
 
+        if tg.command in self.UNSUPPORTED_COMMANDS:
+            raise UnsupportedCommand(f'{self.__class__.__name__} does not support {tg.command}')
+
         self.ser.write(tg.serialize())
         if tg.addr_to != 0:
-            rx_tg = self.recv_telegram(tg)
-
-            if rx_tg.command == Command.SCMD_NACK:
-                #err = Error(rx_tg.parameters[0])
-                print("err")
-
+            rx_tg = self._recv_telegram(tg)
             return rx_tg
                 
-    def recv_telegram(self, tx_tg: Telegram) -> Telegram:
+    def _recv_telegram(self, tx_tg: Telegram) -> Telegram:
         """Recieve a telegram from a sensor
 
         Args:
             tx_tg (Telegram): The telegram that was sent to the sensor prior to the response
 
         Returns:
             Telegram: The telegram from the sensor
@@ -247,88 +268,127 @@
         if rx_params == Command.SCMD_ACK:
             rx_params = 0
         if rx_params == Command.SCMD_Hello:
             rx_params = 1
 
         expected_len = rx_params + 7
         
-        resp = self.ser.read()
-        rx_tg = [resp]
-
-        while resp != b'' and len(rx_tg) < expected_len:
+        resp = None
+        while resp != Command.STX.to_bytes(1,'big') and resp != b'':
+            resp = self.ser.read()
+        rx = [resp]
 
-            if len(rx_tg) == 2:
-                if rx_tg[0] == rx_tg[1] == Command.STX:
-                    expected_len += 1
-                
+        while resp != b'' and len(rx) < expected_len:
             resp = self.ser.read()
-            rx_tg.append(resp)
+            if resp == Command.STX.to_bytes(1,'big'):
+                resp = self.ser.read()
+            rx.append(resp)
+        
+        if resp == b'':
+            return None
 
-        rx_tg = [int.from_bytes(b, "big") for b in rx_tg]
+        rx = [int.from_bytes(b, "big") for b in rx]
         
         tg = Telegram()
-        tg.from_bytes(bytes(rx_tg))
+        tg.from_bytes(bytes(rx))
         return tg
-        
-    def get_value(self) -> tuple[tuple[int, int], tuple[int, int]]:
+
+    def hello(self, addr_to: int=1) -> Telegram | None:
+        return self._send_telegram(Telegram(Command.SCMD_Hello, addr_to=addr_to))
+
+    def get_raw(self) -> tuple[tuple[int, int], tuple[int, int]]:
         """Return a single set of raw and calibrated values from channel 0 and 1
 
         Returns:
             tuple[tuple[int, int], tuple[int, int]]: Returns a tuple of channel 0 and 1. (raw, cal)
         """
 
         tg = Telegram(Command.SCMD_ReadRaw)
         
-        resp_tg = self.send_telegram(tg)
+        resp_tg = self._send_telegram(tg)
 
         raw0 = (resp_tg.parameters[0] << 8) + resp_tg.parameters[1]
         raw1 = (resp_tg.parameters[2] << 8) + resp_tg.parameters[3]
 
         cal0 = (resp_tg.parameters[4] << 8) + resp_tg.parameters[5]
         cal1 = (resp_tg.parameters[6] << 8) + resp_tg.parameters[7]
         return (raw0, cal0), (raw1, cal1)
 
-    def get_status_short(self):
+    def get_status_short(self, addr_to: int=1) -> Telegram:
+        return self._send_telegram(Telegram(Command.SCMD_ReadStatusShort, addr_to=addr_to))
+    
+    def get_status(self, addr_to: int=1) -> Telegram:
+        return self._send_telegram(Telegram(Command.SCMD_ReadStatus, addr_to=addr_to))
 
-        tg = Telegram(Command.SCMD_ReadStatusShort)
-        resp_tg = self.send_telegram(tg)
+    def restart_device(self, addr_to: int=1) -> Telegram:
+        return self._send_telegram(Telegram(Command.SCMD_RestartDevice, addr_to=addr_to))
+
+    def zero_angle(self, addr_to: int=1) -> Telegram:
+        return self._send_telegram(Telegram(Command.SCMD_SetAngleToZero, addr_to=addr_to))
+
+    def _dump_all_blocks(self, addr_to: int=1):
+        with (Path(__file__).parent / 'dump.txt').open('w') as fp:
+            for block in range(0xFF):
+                tg = Telegram(Command.SCMD_ReadConfig, parameters=[block])
+                
+                fp.write(f'BLOCK{block:>3}:\n\tTX:')
+                for b in tg.serialize():
+                    fp.write(f'{b:02X} ')
+                fp.write('\n\tRX:')
+                
+                rx_tg = self._send_telegram(tg)
+                if rx_tg is None:
+                    fp.write(f'Failed to read: {block}\n')
+                    continue
+
+                for b in rx_tg.serialize():
+                    fp.write(f'{b:02X} ')
+                fp.write('\n')
+
+
+
+    def read_config(self, addr_to: int=1):
+        for block in self.config:
+            tg = Telegram(Command.SCMD_ReadConfig, parameters=[block.BLOCK])
+            rx_tg = self._send_telegram(tg)
+            if rx_tg is None:
+                print(f'Failed to read: {block.__class__.__name__}')
+                continue
+            
+            block.from_payload(rx_tg.parameters)
+
+    def write_config(self, addr_to: int=1):
+        for block in self.config:
+            if not block.READONLY:
+                payload = block.serialize()
+                params = block.BLOCK.to_bytes(1, 'big') + payload
+                tg = Telegram(Command.SCMD_WriteConfig, addr_to=addr_to, parameters=params)
+                self._send_telegram(tg)
 
-        return resp_tg
-    
     def start_streaming(self, sample_rate: int, count: int=0, channel: str='A'):
-        sample_rates = {
-            20:     0xFA,
-            25:     0xC8,
-            50:     0x64,
-            100:    0x32,
-            200:    0x19,
-            250:    0x14,
-            500:    0x0A,
-            1000:   0x05,
-            1250:   0x04,
-            2500:   0x02,
-            5000:   0x01
-        }
+
+        if channel not in ['A', 'B', 'C']:
+            raise ValueError('Channel can only be A B or C')
 
         if channel == 'C':
             self.mode = 'SOSM_DUAL'
         else:
             self.mode = 'SOSM_SINGLE'
 
-        channel = ord(channel) # Convert char to int
-
-        params = [3, sample_rates[sample_rate]]
-        if count <= 255:
+        params = [3, self.SAMPLE_RATES[sample_rate]]
+        
+        count = min(0xFFFF, max(0, count))
+        if count <= 0xFF:
             params.append(0)
         params.append(count)
-        params.append(channel)
+        params.append(ord(channel))
         
         # Switch to SOSM mode #3
         tg = Telegram(Command.SCMD_GotoSpecialMode, parameters=params)
-        return self.send_telegram(tg)
+        return self._send_telegram(tg)
     
     def streaming_recv_poll(self):
         if not 'SOSM' in self.mode:
             return None
         
         expected_bytes = 5 if self.mode == 'SOSM_DUAL' else 3
 
@@ -344,35 +404,37 @@
         self.ser.write(Command.STX.to_bytes(1, 'big'))
         self.ser.write(Command.STX.to_bytes(1, 'big'))
         self.ser.write(Command.STX.to_bytes(1, 'big'))
 
         self.mode = 'idle'
 
 class LCV_USB(LorenzConnector):
-
+    UNSUPPORTED_COMMANDS = [
+        Command.SCMD_SetAngleToZero,
+    ]
+    
     def __init__(self, port: str, **kwargs) -> None:
 
         if 'baudrate' in kwargs:
             if kwargs['baudrate'] not in [115200, 230400]:
                 kwargs['baudrate'] = 115200
                 warnings.warn('Device only supports 115.2 or 230.4 kbaud. Defaulted to 115.2k')
         else:
             kwargs['baudrate'] = 115200
         
         super().__init__(port, timeout=0.1, **kwargs)
     
 
 if __name__ == '__main__':
     with LCV_USB('COM7') as lc:
-        start = time.time()
-        ret = lc.start_streaming(1000)
-
-        while time.time() < start+5:
-            idx, val = lc.streaming_recv_poll()
-            if val is not None:
-                print(f'{idx:3d}: {val}')
-            #time.sleep(0.01)
-        
-        lc.stop_streaming()
-        print(lc.ser.in_waiting)
-        time.sleep(1)
-        print(lc.ser.in_waiting)
+        lc.read_config()
+        #lc.dump_all_blocks()
+        print('horse')
+        #start = time.time()
+        #ret = lc.start_streaming(1000)
+
+        # while time.time() < start+5:
+        #     idx, val = lc.streaming_recv_poll()
+        #     if val is not None:
+        #         print(f'{idx:3d}: {val}')
+        #     #time.sleep(0.01)
+        # lc.stop_streaming()
```

