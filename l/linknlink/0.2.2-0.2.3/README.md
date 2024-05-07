# Comparing `tmp/linknlink-0.2.2.tar.gz` & `tmp/linknlink-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linknlink-0.2.2.tar", last modified: Tue Apr 30 13:47:18 2024, max compression
+gzip compressed data, was "linknlink-0.2.3.tar", last modified: Tue May  7 02:09:45 2024, max compression
```

## Comparing `linknlink-0.2.2.tar` & `linknlink-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-30 13:47:18.857034 linknlink-0.2.2/
--rw-rw-r--   0 user      (1000) user      (1000)     1068 2023-11-08 09:39:11.000000 linknlink-0.2.2/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      503 2024-04-30 13:47:18.857034 linknlink-0.2.2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)       77 2023-11-14 06:52:53.000000 linknlink-0.2.2/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-30 13:47:18.857034 linknlink-0.2.2/linknlink/
--rw-rw-r--   0 user      (1000) user      (1000)     4080 2024-04-10 10:04:04.000000 linknlink-0.2.2/linknlink/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      269 2024-04-02 02:50:19.000000 linknlink-0.2.2/linknlink/const.py
--rw-rw-r--   0 user      (1000) user      (1000)    12633 2024-04-30 13:41:20.000000 linknlink-0.2.2/linknlink/device.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-11-10 07:16:08.000000 linknlink-0.2.2/linknlink/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1847 2023-11-10 07:09:54.000000 linknlink-0.2.2/linknlink/protocol.py
--rw-rw-r--   0 user      (1000) user      (1000)     9017 2024-04-30 13:37:50.000000 linknlink-0.2.2/linknlink/remote.py
--rw-rw-r--   0 user      (1000) user      (1000)     1774 2024-03-25 06:45:21.000000 linknlink-0.2.2/linknlink/sensor.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-30 13:47:18.857034 linknlink-0.2.2/linknlink.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      503 2024-04-30 13:47:18.000000 linknlink-0.2.2/linknlink.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      369 2024-04-30 13:47:18.000000 linknlink-0.2.2/linknlink.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-30 13:47:18.000000 linknlink-0.2.2/linknlink.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-11-10 08:42:09.000000 linknlink-0.2.2/linknlink.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       18 2024-04-30 13:47:18.000000 linknlink-0.2.2/linknlink.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2024-04-30 13:47:18.000000 linknlink-0.2.2/linknlink.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-30 13:47:18.857034 linknlink-0.2.2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      743 2024-04-30 13:45:58.000000 linknlink-0.2.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-07 02:09:45.248275 linknlink-0.2.3/
+-rw-rw-r--   0 user      (1000) user      (1000)     1068 2023-11-08 09:39:11.000000 linknlink-0.2.3/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      503 2024-05-07 02:09:45.244275 linknlink-0.2.3/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)       77 2023-11-14 06:52:53.000000 linknlink-0.2.3/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-07 02:09:45.244275 linknlink-0.2.3/linknlink/
+-rw-rw-r--   0 user      (1000) user      (1000)     4080 2024-04-10 10:04:04.000000 linknlink-0.2.3/linknlink/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      269 2024-04-02 02:50:19.000000 linknlink-0.2.3/linknlink/const.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12633 2024-04-30 13:41:20.000000 linknlink-0.2.3/linknlink/device.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-11-10 07:16:08.000000 linknlink-0.2.3/linknlink/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1847 2023-11-10 07:09:54.000000 linknlink-0.2.3/linknlink/protocol.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9042 2024-05-07 02:07:54.000000 linknlink-0.2.3/linknlink/remote.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1774 2024-03-25 06:45:21.000000 linknlink-0.2.3/linknlink/sensor.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-07 02:09:45.244275 linknlink-0.2.3/linknlink.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      503 2024-05-07 02:09:45.000000 linknlink-0.2.3/linknlink.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      369 2024-05-07 02:09:45.000000 linknlink-0.2.3/linknlink.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-07 02:09:45.000000 linknlink-0.2.3/linknlink.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-11-10 08:42:09.000000 linknlink-0.2.3/linknlink.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       18 2024-05-07 02:09:45.000000 linknlink-0.2.3/linknlink.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2024-05-07 02:09:45.000000 linknlink-0.2.3/linknlink.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-07 02:09:45.248275 linknlink-0.2.3/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      743 2024-05-07 02:09:16.000000 linknlink-0.2.3/setup.py
```

### Comparing `linknlink-0.2.2/LICENSE` & `linknlink-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.2/linknlink/__init__.py` & `linknlink-0.2.3/linknlink/__init__.py`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.2/linknlink/device.py` & `linknlink-0.2.3/linknlink/device.py`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.2/linknlink/exceptions.py` & `linknlink-0.2.3/linknlink/exceptions.py`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.2/linknlink/protocol.py` & `linknlink-0.2.3/linknlink/protocol.py`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.2/linknlink/remote.py` & `linknlink-0.2.3/linknlink/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,18 @@
     """Controls a LinknLink ehub."""
 
     TYPE = "EHUB"
     
     # sensor function
     def _send(self, command: int, data: bytes = b"") -> bytes:
         """Send a packet to the device."""
-        packet = struct.pack("<HI", len(data) + 4, command) + data
+        if 20000 <= self.devtype <= 29999:
+            packet = struct.pack("<HI", len(data) + 4, command) + data
+        else:
+            packet = struct.pack("<I", command) + data
         resp = self.send_packet(0x6A, packet)
         e.check_error(resp[0x22:0x24])
         payload = self.decrypt(resp[0x38:])
         p_len = struct.unpack("<H", payload[:0x2])[0]
         return payload[0x6 : p_len + 2]
     
     def check_sensors(self) -> dict:
@@ -91,15 +94,18 @@
 
     TYPE = "EREMOTE"
     UdpFlag = False
     Port = 61212
     
     def _send(self, command: int, data: bytes = b"") -> bytes:
         """Send a packet to the device."""
-        packet = struct.pack("<HI", len(data) + 4, command) + data
+        if 20000 <= self.devtype <= 29999:
+            packet = struct.pack("<HI", len(data) + 4, command) + data
+        else:
+            packet = struct.pack("<I", command) + data
         resp = self.send_packet(0x6A, packet)
         e.check_error(resp[0x22:0x24])
         payload = self.decrypt(resp[0x38:])
         p_len = struct.unpack("<H", payload[:0x2])[0]
         return payload[0x6 : p_len + 2]
     
     def _sendV2(self, command: int, data: bytes = b"") -> bytes:
@@ -129,16 +135,14 @@
 
         # print(f"UDP 服务器已在{self.Port}启动，等待客户端连接...")
 
         # 接收数据并发送响应
         while True:
             # 接收数据
             data, client_address = udp_server_socket.recvfrom(1024)
-            print(f"收到来自 {client_address} 的消息：{data.decode('utf-8')}")
-
             if self.cb:
                 try:
                     data_dict = json.loads(data.decode('utf-8'))
                     for key, value in data_dict.items():
                         if key.startswith("rmkey") and value != 0:
                             # print(f"键: {key}, 值: {value}")
                             self.cb(key)
@@ -149,24 +153,20 @@
             response = "ok"
             udp_server_socket.sendto(response.encode('utf-8'), client_address)
 
     def sendTimeout(self) -> bytes:
         """Send a packet to the device."""
         while True:
             data = (("""{"port":%s, "timeout":60}""") % (self.Port)).encode('utf-8')
-            print(data)
-            print(len(data) + 4)
             packet = struct.pack("<I", 20000) + data
             # packet = struct.pack("<HI", len(data) + 4, 20000) + data
-            print(packet.hex())
             try: 
                 resp = self.send_packet(0x6A, packet)
             except Exception as e:
                 print(e)
-            print(resp.hex())
             time.sleep(60)
     
     def getalldev(self) -> dict:
         """Return the all devices."""
         resp = self._sendV2(0x0b0e, """{"count":16,"index":0,}""".encode('utf-8')) # max 16dev
         try:
             json_string = resp.decode('utf-8')
```

### Comparing `linknlink-0.2.2/linknlink/sensor.py` & `linknlink-0.2.3/linknlink/sensor.py`

 * *Files identical despite different names*

### Comparing `linknlink-0.2.2/setup.py` & `linknlink-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 
 from setuptools import setup, find_packages
 
 
-version = '0.2.2'
+version = '0.2.3'
 
 setup(
     name="linknlink",
     version=version,
     author="Zhao Zehua",
     author_email="huahua.zzh@gmail.com",
     url="https://github.com/xuanxuan000/python-linknlink",
```

