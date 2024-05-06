# Comparing `tmp/supernovacontroller-1.1.0.tar.gz` & `tmp/supernovacontroller-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supernovacontroller-1.1.0.tar", last modified: Tue Feb  6 19:06:56 2024, max compression
+gzip compressed data, was "supernovacontroller-1.2.0.tar", last modified: Mon May  6 22:12:05 2024, max compression
```

## Comparing `supernovacontroller-1.1.0.tar` & `supernovacontroller-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:06:56.666517 supernovacontroller-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18902 2024-02-06 19:06:56.666517 supernovacontroller-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18388 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:06:56.666517 supernovacontroller-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/examples/ICM42605_i3c_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/examples/basic_i2c_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/examples/basic_i3c_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/examples/basic_i3c_target_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/examples/basic_uart_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/examples/ibi_example.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 19:06:56.666517 supernovacontroller-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:06:56.666517 supernovacontroller-1.1.0/supernovacontroller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/supernovacontroller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:06:56.666517 supernovacontroller-1.1.0/supernovacontroller/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/supernovacontroller/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/supernovacontroller/errors/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:06:56.666517 supernovacontroller-1.1.0/supernovacontroller/sequential/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/supernovacontroller/sequential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/supernovacontroller/sequential/i2c.py
--rw-r--r--   0 runner    (1001) docker     (127)    64690 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/supernovacontroller/sequential/i3c.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/supernovacontroller/sequential/i3c_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/supernovacontroller/sequential/supernova_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/supernovacontroller/sequential/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:06:56.666517 supernovacontroller-1.1.0/supernovacontroller/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/supernovacontroller/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-06 19:06:46.000000 supernovacontroller-1.1.0/supernovacontroller/utils/mctp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 19:06:56.666517 supernovacontroller-1.1.0/supernovacontroller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18902 2024-02-06 19:06:56.000000 supernovacontroller-1.1.0/supernovacontroller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-02-06 19:06:56.000000 supernovacontroller-1.1.0/supernovacontroller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 19:06:56.000000 supernovacontroller-1.1.0/supernovacontroller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-06 19:06:56.000000 supernovacontroller-1.1.0/supernovacontroller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-06 19:06:56.000000 supernovacontroller-1.1.0/supernovacontroller.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:12:05.970657 supernovacontroller-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28537 2024-05-06 22:12:05.970657 supernovacontroller-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    28023 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:12:05.966657 supernovacontroller-1.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/examples/ICM42605_i3c_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/examples/basic_i2c_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/examples/basic_i3c_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/examples/basic_i3c_target_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/examples/basic_spi_controller_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/examples/basic_uart_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/examples/ibi_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 22:12:05.970657 supernovacontroller-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:12:05.966657 supernovacontroller-1.2.0/supernovacontroller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/supernovacontroller/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:12:05.970657 supernovacontroller-1.2.0/supernovacontroller/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/supernovacontroller/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/supernovacontroller/errors/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:12:05.970657 supernovacontroller-1.2.0/supernovacontroller/sequential/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/supernovacontroller/sequential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/supernovacontroller/sequential/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64934 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/supernovacontroller/sequential/i3c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/supernovacontroller/sequential/i3c_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15828 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/supernovacontroller/sequential/spi_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/supernovacontroller/sequential/supernova_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/supernovacontroller/sequential/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:12:05.970657 supernovacontroller-1.2.0/supernovacontroller/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/supernovacontroller/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 22:11:57.000000 supernovacontroller-1.2.0/supernovacontroller/utils/mctp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:12:05.970657 supernovacontroller-1.2.0/supernovacontroller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28537 2024-05-06 22:12:05.000000 supernovacontroller-1.2.0/supernovacontroller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-06 22:12:05.000000 supernovacontroller-1.2.0/supernovacontroller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 22:12:05.000000 supernovacontroller-1.2.0/supernovacontroller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-06 22:12:05.000000 supernovacontroller-1.2.0/supernovacontroller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 22:12:05.000000 supernovacontroller-1.2.0/supernovacontroller.egg-info/top_level.txt
```

### Comparing `supernovacontroller-1.1.0/PKG-INFO` & `supernovacontroller-1.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,16 @@
-Metadata-Version: 2.1
-Name: supernovacontroller
-Version: 1.1.0
-Summary: A blocking API for interacting with the Supernova host-adapter device
-Home-page: https://github.com/binhollc/SupernovaController
-Author: Binho LLC
-Author-email: support@binho.io
-License: Private
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-
 # SupernovaController
 Manages communications with the Supernova host-adapter USB HID device.
 
 ## Introduction
 SupernovaController is a Python-based tool designed to interface with the Supernova host-adapter USB HID device. Offering a blocking API, it simplifies command sequences and interactions in the context of asynchronous operation environments like the one offered by the Supernova host-adapter. This approach enhances usability and efficiency, providing a streamlined experience for developers working with the Supernova device.
 
 ## Features
 - **Blocking API:** A streamlined approach to interact with the Supernova device, minimizing the complexity of handling asynchronous callbacks.
-- **Multi-Interface:** Easily communicate with UART, I2C and I3C Devices in an All-In-One package.
+- **Multi-Interface:** Easily communicate with SPI, UART, I2C and I3C Devices in an All-In-One package.
 - **Communication:** Seamlessly manages command responses and notifications, facilitating easier and more intuitive command sequencing.
 - **Examples:** Comprehensive examples demonstrating the practical application of the blocking API.
 
 ## Installation
 
 To install the SupernovaController package, follow these steps:
 
@@ -283,47 +268,299 @@
 
 The fact that the memory is not circular obligates to take into account border cases:
 
 * If the user tries to start the transfer in an address surpassing the target memory range, the target will ignore the address and will start the transfer from the end of the the previous one.
 
 * If the transfer starts in an allowed memory address but tries to surpass the range during the transaction, it will only modify the bytes in the allowed range and discard the rest. The end of the transfer is taken as the end of the memory.
 
-### Next Steps
+## UART protocol
+
+### UART features
+
+This section describes how to get you started with the `SupernovaController` focusing on the UART protocol.
+
+* The supported features are: 
+    * Bus initialization.
+    * Setting of bus parameters such as baudrate, hardware handshake, parity, data size and stop bit.
+    * UART TX/RX transactions of up to 1024 bytes.
+
+### Basic UART Communication
+
+#### Generic operations
+
+1. ***Initializing the Supernova Device:***
+
+   Imports and initializes the `SupernovaDevice`. Optionally, specifies the USB HID path if multiple devices are connected:
+
+   ```python
+   from supernovacontroller.sequential import SupernovaDevice
+
+   device = SupernovaDevice()
+   # Optionally specify the USB HID path
+   device.open(usb_address='your_usb_hid_path')
+   ```
+
+   Call `open()` without parameters if you don't need to specify a particular device.
+
+2. ***Creating a UART controller Interface:***
+
+   Creates a UART controller interface:
+
+   ```python
+   uart = device.create_interface("uart")
+   ``` 
+
+3. ***Closing the Device:***
+
+   Closes the device when done:
+
+   ```python
+   device.close()
+   ```
+
+### Operations intended for the Supernova UART peripheral
+
+1. ***Setting Bus Voltage:***
+
+   Sets the bus voltage (in mV) for the UART bus. This step is required before initializing the bus:
+
+   ```python
+   success, response = uart.set_bus_voltage(3300)
+   ```
+
+2. ***Initializing the Supernova UART peripheral:***
+
+    Initializes the Supernova UART peripheral:
+
+    ```python
+   success, response = uart.init_bus()
+   ```
+    Without any parameters, the UART peripheral initializes with the default values for baudrate (9600bps), parity (no parity), data size (8 bit), stop bit (one stop bit) and hardware handshake (no hardware handshake). Optionally, it is possible to set any of these parameters by specifying them in the init_bus function:
+
+    ```python
+   success, response = uart.init_bus(baudrate=UartControllerBaudRate.UART_BAUD_115200, parity=UartControllerParity.UART_EVEN_PARITY)
+   ```
+3. ***Modifying the UART peripheral parameters***
 
-After installing the `SupernovaController` package, you can further explore its capabilities by trying out the examples included in the installation. These examples demonstrate practical applications of UART, I2C and I3C protocols:
+    It is also possible to configure/set any parameter after initialization (baudrate, parity, data size, stop bit and hardware handshake):
+
+    ```python
+   success, response = uart.set_parameters(stop_bit = UartControllerStopBit.UART_TWO_STOP_BIT, baudrate = UartControllerBaudRate.UART_BAUD_56000)
+   ```
+
+   If parameters are provided, it configures the parameters; otherwise, it retains the current settings.
+
+4. ***Read the current UART peripheral configuration***
+
+    The following method retrieves the current UART peripheral communication parameters, including baudrate, parity, data size, stop bit and hardware handshake.
+
+    ```python
+   success, response = uart.get_parameters()
+   ```
+
+    The variable ```response``` is a tuple containing the current UART controller communication parameters:
+    *(baudrate, parity, data_size, stop_bit, hardware_handshake)*
+
+5. ***Send data over UART bus***
+
+    If the bus is initialized, sends the provided data over the UART TX channel. 
+
+    ```python
+    data = [0x00, 0x01, 0x02, 0x3, 0x04, 0x05, 0x06]
+    success, response = uart.send(data, transferLength)
+    ```
+    - If no errors arises while sending the data, ```success``` will be _true_ and the ```response``` will be a success message.
+    - If an error arises while sending the data, ```success``` will be _false_ and the ```response``` will be an error message.
+
+6. ***Receive data over UART bus***
+
+    If the bus is initialized, awaits reception of data over the UART RX channel. A timeout can be set to the waiting process to exit if no data is received in the timeout's time specified time (use None to ignore the timeout feature). 
+
+    ```python
+    success, response = uart.wait_for_notification(timeout = None)
+    ```
+    - If data is received before the configured timeout, ```success``` will be _true_ and the ```response``` will be the array of received data.
+    - If data is not received before the configured timeout,  ```success``` will be _false_ and the ```response``` will be a timeout error message.
+    - If an error arises while receiving the data, ```success``` will be _false_ and the ```response``` will be an error message.
+
+## SPI protocol
+
+### SPI features
+
+This section describes how to get you started with the `SupernovaController` focusing on the SPI protocol.
+In a SPI bus, the Supernova can act as a controller.
+
+* In controller mode the Supernova supports several features: 
+    * Supernova initialization in SPI controller mode.
+    * Bus initialization.
+    * Setting of bus parameters such as bit order, SPI mode, chip select, chip select polarity and frequency.
+    * SPI transfers of up to 1024 bytes.
+    * 8 bits data width frames.
+
+* Coming soon:
+  * For the SPI controller mode:
+    - Pre and post delays.
+    - Keep chip select active between transfers.
+    - Support for 16 bits data width.
+  * Support for SPI target mode.
+
+### Basic SPI Communication
+
+#### Generic operations
+
+1. ***Initializing the Supernova Device:***
+
+   Imports and initializes the `SupernovaDevice`. Optionally, specifies the USB HID path if multiple devices are connected:
+
+   ```python
+   from supernovacontroller.sequential import SupernovaDevice
+
+   device = SupernovaDevice()
+   
+   # Optionally specify the USB HID path
+   device.open(usb_address='your_usb_hid_path')
+   ```
+
+   Call `open()` without parameters if you don't need to specify a particular device.
+
+2. ***Creating a SPI controller Interface:***
+
+   Creates a SPI controller interface:
+
+   ```python
+   spi_controller = device.create_interface("spi.controller")
+   ``` 
+
+3. ***Closing the Device:***
+
+   Closes the device when done:
+
+   ```python
+   device.close()
+   ```
+
+### Operations intended for the Supernova in SPI controller mode
+
+1. ***Setting Bus Voltage:***
+
+   Sets the bus voltage (in mV) for the SPI bus. This step is required before initializing the bus:
+
+   ```python
+   success, response = spi_controller.set_bus_voltage(3300)
+   ```
+
+2. ***Initializing the Supernova as a SPI controller:***
+
+    Initializes the Supernova in SPI controller mode:
+
+    ```python
+   success, response = spi_controller.init_bus()
+   ```
+    Without any parameters, the SPI controller initializes with the default values for bit order (MSB first), mode (Mode 0), chip select (CS0), chip select polarity (Active low) and frequency (10 MHz). Optionally, it is possible to set any of these parameters by specifying in the init_bus function:
+
+    ```python
+   success, response = spi_controller.init_bus(bit_order=SpiControllerBitOrder.LSB, frequency=20000000)
+   ```
+
+3. ***Modifying the SPI controller parameters***
+
+    It is possible to set a new configuration for each parameter (bit order, mode, chip select, chip select polarity and frequency):
+
+    ```python
+   success, response = spi_controller.set_parameters(bit_order = SpiControllerBitOrder.MSB, mode = SpiControllerMode.MODE_1)
+   ```
+
+   If parameters are provided, it configures the parameters; otherwise, it retains the current settings.
+
+4. ***Read the current SPI controller configuration***
+
+    The following method retrieves the current SPI controller communication parameters, including bit order, spi mode, data width, chip select, chip select polarity and frequency.
+
+    ```python
+   success, response = spi_controller.get_parameters()
+   ```
+
+    The variable ```response``` is a tuple containing the current SPI controller communication parameters:
+    (bit_order, mode, data_width, chip_select, chip_select_pol, frequency)
+
+5. ***Transfer data over SPI bus***
+
+    Transfers the provided data over the SPI bus if the bus is initialized. It is necessary to indicate the length of the transfer to generate the SPI clock cycles. This length could be more than the length of the transferred data to a SPI target, in the cases where the response (data on the MISO line) consists of more bytes than the transferred.
+
+    ```python
+    data = [0x01, 0x02, 0x03, 0x04, 0x05, 0x06]
+    transfer_length = 6
+    success, response = spi_controller.transfer(data, transfer_length)
+    ```
+
+    For a particular case of a SPI target device that interprets instructions via opcodes, an example of use could be the following:
+    
+    ```python
+    # Read opcode: 0x03
+    # Address to read: 0x0002
+    # Transferred data: [opcode, address_H, address_L]
+    data = [0x03, 0x00, 0x02]
+    
+    # Transfer length includes the length of the transferred data to the target and the read length to generate SPI clock cycles for the read operation
+    # Read length: 6 bytes to read
+    # Data to target: 3 bytes
+    read_length = 6
+    data_to_target = len(data)
+    transfer_length = data_to_target + read_length
+
+    success, response = spi_controller.transfer(data, transfer_length)
+
+    # The response consists of the entire MISO line since the transfer started.
+    # If the SPI target device doesn't send information while the instruction is transferred, the first bytes of the response are in IDLE state with the value 0x00
+    # response: [0x00, 0x00, 0x00, 0xFA, 0xFB, 0xFC, 0xFD, 0xFE, 0xFF]
+    data_from_target = response[3:]
+    ```
+
+## Next Steps
+
+After installing the `SupernovaController` package, you can further explore its capabilities by trying out the examples included in the installation. These examples demonstrate practical applications of SPI, UART, I2C and I3C protocols:
 
 - **Basic I3C Example (`basic_i3c_example.py`):** Learn the basics of I3C bus initialization and device communication using the Supernova as an I3C controller.
 - **Basic I3C Target Mode Example (`basic_i3c_target_example.py`):** Learn the basics of I3C target mode implementation using two Supernovas, one as an I3C target and the other one as a controller.
 - **Basic I2C Example (`basic_i2c_example.py`):** Get started with fundamental I2C operations.
 - **Basic UART Example (`basic_uart_example.py`):** Try out the UART protocol Hands-On.
+- **Basic SPI Controller Example (`basic_spi_controller_example.py`):** Explore the fundamental SPI controller operations communicating with a SPI Target device.
 - **IBI Example (`ibi_example.py`):** Understand handling In-Band Interrupts (IBI) in I3C.
 - **ICM42605 I3C Example (`ICM42605_i3c_example.py`):** Explore a real-world application of I3C with the ICM42605 sensor.
 
 #### Accessing the Examples
 
-The example scripts are installed in a directory named `SupernovaExamples`, which is located in your Python environment's directory. To find this directory, you can use the following Python commands:
+The example scripts are installed in your site-packages folder as `supernovacontrollerexamples`, and you can access them just like you would any other package in Python. To find this directory, you can use the following Python commands:
 
 ```python
 import sys
 import os
 
-examples_dir_name = "SupernovaExamples"
-examples_path = os.path.join(sys.prefix, examples_dir_name)
+examples_dir_name = "supernovacontrollerexamples"
+examples_path = os.path.join(sys.prefix, "lib", "site-packages", examples_dir_name)
 print(f"Examples are located in: {examples_path}")
 ```
 
 This will print the path to the `SupernovaExamples` directory. Navigate to this directory to find the example scripts.
 
 You can run an example directly from this directory using Python. For instance:
 
 ```sh
-python /path/to/SupernovaExamples/basic_i2c_example.py
+python /path/to/supernovacontrollerexamples/basic_i2c_example.py
 ```
 
-Replace `/path/to/SupernovaExamples/` with the actual path printed in the previous step and `basic_i2c_example.py` with the name of the example you wish to run.
+Replace `/path/to/supernovacontrollerexamples/` with the actual path printed in the previous step and `basic_i2c_example.py` with the name of the example you wish to run.
+
+Or by calling the main method from the example directly from your Python script, as so:
+
+```python
+from supernovacontrollerexamples import basic_i2c_example
+
+basic_i2c_example.main()
+```
 
 #### Exploring Further
 
 Each example is designed to provide insights into different aspects of the `SupernovaController` usage. By running and modifying these examples, you'll gain a deeper understanding of how to effectively use the package in various scenarios.
 
 ## Error Handling
```

### Comparing `supernovacontroller-1.1.0/README.md` & `supernovacontroller-1.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,31 @@
+Metadata-Version: 2.1
+Name: supernovacontroller
+Version: 1.2.0
+Summary: A blocking API for interacting with the Supernova host-adapter device
+Home-page: https://github.com/binhollc/SupernovaController
+Author: Binho LLC
+Author-email: support@binho.io
+License: Private
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 # SupernovaController
 Manages communications with the Supernova host-adapter USB HID device.
 
 ## Introduction
 SupernovaController is a Python-based tool designed to interface with the Supernova host-adapter USB HID device. Offering a blocking API, it simplifies command sequences and interactions in the context of asynchronous operation environments like the one offered by the Supernova host-adapter. This approach enhances usability and efficiency, providing a streamlined experience for developers working with the Supernova device.
 
 ## Features
 - **Blocking API:** A streamlined approach to interact with the Supernova device, minimizing the complexity of handling asynchronous callbacks.
-- **Multi-Interface:** Easily communicate with UART, I2C and I3C Devices in an All-In-One package.
+- **Multi-Interface:** Easily communicate with SPI, UART, I2C and I3C Devices in an All-In-One package.
 - **Communication:** Seamlessly manages command responses and notifications, facilitating easier and more intuitive command sequencing.
 - **Examples:** Comprehensive examples demonstrating the practical application of the blocking API.
 
 ## Installation
 
 To install the SupernovaController package, follow these steps:
 
@@ -268,47 +283,299 @@
 
 The fact that the memory is not circular obligates to take into account border cases:
 
 * If the user tries to start the transfer in an address surpassing the target memory range, the target will ignore the address and will start the transfer from the end of the the previous one.
 
 * If the transfer starts in an allowed memory address but tries to surpass the range during the transaction, it will only modify the bytes in the allowed range and discard the rest. The end of the transfer is taken as the end of the memory.
 
-### Next Steps
+## UART protocol
+
+### UART features
+
+This section describes how to get you started with the `SupernovaController` focusing on the UART protocol.
+
+* The supported features are: 
+    * Bus initialization.
+    * Setting of bus parameters such as baudrate, hardware handshake, parity, data size and stop bit.
+    * UART TX/RX transactions of up to 1024 bytes.
+
+### Basic UART Communication
+
+#### Generic operations
+
+1. ***Initializing the Supernova Device:***
+
+   Imports and initializes the `SupernovaDevice`. Optionally, specifies the USB HID path if multiple devices are connected:
+
+   ```python
+   from supernovacontroller.sequential import SupernovaDevice
+
+   device = SupernovaDevice()
+   # Optionally specify the USB HID path
+   device.open(usb_address='your_usb_hid_path')
+   ```
+
+   Call `open()` without parameters if you don't need to specify a particular device.
+
+2. ***Creating a UART controller Interface:***
+
+   Creates a UART controller interface:
+
+   ```python
+   uart = device.create_interface("uart")
+   ``` 
+
+3. ***Closing the Device:***
+
+   Closes the device when done:
+
+   ```python
+   device.close()
+   ```
+
+### Operations intended for the Supernova UART peripheral
+
+1. ***Setting Bus Voltage:***
+
+   Sets the bus voltage (in mV) for the UART bus. This step is required before initializing the bus:
+
+   ```python
+   success, response = uart.set_bus_voltage(3300)
+   ```
+
+2. ***Initializing the Supernova UART peripheral:***
+
+    Initializes the Supernova UART peripheral:
+
+    ```python
+   success, response = uart.init_bus()
+   ```
+    Without any parameters, the UART peripheral initializes with the default values for baudrate (9600bps), parity (no parity), data size (8 bit), stop bit (one stop bit) and hardware handshake (no hardware handshake). Optionally, it is possible to set any of these parameters by specifying them in the init_bus function:
+
+    ```python
+   success, response = uart.init_bus(baudrate=UartControllerBaudRate.UART_BAUD_115200, parity=UartControllerParity.UART_EVEN_PARITY)
+   ```
+3. ***Modifying the UART peripheral parameters***
 
-After installing the `SupernovaController` package, you can further explore its capabilities by trying out the examples included in the installation. These examples demonstrate practical applications of UART, I2C and I3C protocols:
+    It is also possible to configure/set any parameter after initialization (baudrate, parity, data size, stop bit and hardware handshake):
+
+    ```python
+   success, response = uart.set_parameters(stop_bit = UartControllerStopBit.UART_TWO_STOP_BIT, baudrate = UartControllerBaudRate.UART_BAUD_56000)
+   ```
+
+   If parameters are provided, it configures the parameters; otherwise, it retains the current settings.
+
+4. ***Read the current UART peripheral configuration***
+
+    The following method retrieves the current UART peripheral communication parameters, including baudrate, parity, data size, stop bit and hardware handshake.
+
+    ```python
+   success, response = uart.get_parameters()
+   ```
+
+    The variable ```response``` is a tuple containing the current UART controller communication parameters:
+    *(baudrate, parity, data_size, stop_bit, hardware_handshake)*
+
+5. ***Send data over UART bus***
+
+    If the bus is initialized, sends the provided data over the UART TX channel. 
+
+    ```python
+    data = [0x00, 0x01, 0x02, 0x3, 0x04, 0x05, 0x06]
+    success, response = uart.send(data, transferLength)
+    ```
+    - If no errors arises while sending the data, ```success``` will be _true_ and the ```response``` will be a success message.
+    - If an error arises while sending the data, ```success``` will be _false_ and the ```response``` will be an error message.
+
+6. ***Receive data over UART bus***
+
+    If the bus is initialized, awaits reception of data over the UART RX channel. A timeout can be set to the waiting process to exit if no data is received in the timeout's time specified time (use None to ignore the timeout feature). 
+
+    ```python
+    success, response = uart.wait_for_notification(timeout = None)
+    ```
+    - If data is received before the configured timeout, ```success``` will be _true_ and the ```response``` will be the array of received data.
+    - If data is not received before the configured timeout,  ```success``` will be _false_ and the ```response``` will be a timeout error message.
+    - If an error arises while receiving the data, ```success``` will be _false_ and the ```response``` will be an error message.
+
+## SPI protocol
+
+### SPI features
+
+This section describes how to get you started with the `SupernovaController` focusing on the SPI protocol.
+In a SPI bus, the Supernova can act as a controller.
+
+* In controller mode the Supernova supports several features: 
+    * Supernova initialization in SPI controller mode.
+    * Bus initialization.
+    * Setting of bus parameters such as bit order, SPI mode, chip select, chip select polarity and frequency.
+    * SPI transfers of up to 1024 bytes.
+    * 8 bits data width frames.
+
+* Coming soon:
+  * For the SPI controller mode:
+    - Pre and post delays.
+    - Keep chip select active between transfers.
+    - Support for 16 bits data width.
+  * Support for SPI target mode.
+
+### Basic SPI Communication
+
+#### Generic operations
+
+1. ***Initializing the Supernova Device:***
+
+   Imports and initializes the `SupernovaDevice`. Optionally, specifies the USB HID path if multiple devices are connected:
+
+   ```python
+   from supernovacontroller.sequential import SupernovaDevice
+
+   device = SupernovaDevice()
+   
+   # Optionally specify the USB HID path
+   device.open(usb_address='your_usb_hid_path')
+   ```
+
+   Call `open()` without parameters if you don't need to specify a particular device.
+
+2. ***Creating a SPI controller Interface:***
+
+   Creates a SPI controller interface:
+
+   ```python
+   spi_controller = device.create_interface("spi.controller")
+   ``` 
+
+3. ***Closing the Device:***
+
+   Closes the device when done:
+
+   ```python
+   device.close()
+   ```
+
+### Operations intended for the Supernova in SPI controller mode
+
+1. ***Setting Bus Voltage:***
+
+   Sets the bus voltage (in mV) for the SPI bus. This step is required before initializing the bus:
+
+   ```python
+   success, response = spi_controller.set_bus_voltage(3300)
+   ```
+
+2. ***Initializing the Supernova as a SPI controller:***
+
+    Initializes the Supernova in SPI controller mode:
+
+    ```python
+   success, response = spi_controller.init_bus()
+   ```
+    Without any parameters, the SPI controller initializes with the default values for bit order (MSB first), mode (Mode 0), chip select (CS0), chip select polarity (Active low) and frequency (10 MHz). Optionally, it is possible to set any of these parameters by specifying in the init_bus function:
+
+    ```python
+   success, response = spi_controller.init_bus(bit_order=SpiControllerBitOrder.LSB, frequency=20000000)
+   ```
+
+3. ***Modifying the SPI controller parameters***
+
+    It is possible to set a new configuration for each parameter (bit order, mode, chip select, chip select polarity and frequency):
+
+    ```python
+   success, response = spi_controller.set_parameters(bit_order = SpiControllerBitOrder.MSB, mode = SpiControllerMode.MODE_1)
+   ```
+
+   If parameters are provided, it configures the parameters; otherwise, it retains the current settings.
+
+4. ***Read the current SPI controller configuration***
+
+    The following method retrieves the current SPI controller communication parameters, including bit order, spi mode, data width, chip select, chip select polarity and frequency.
+
+    ```python
+   success, response = spi_controller.get_parameters()
+   ```
+
+    The variable ```response``` is a tuple containing the current SPI controller communication parameters:
+    (bit_order, mode, data_width, chip_select, chip_select_pol, frequency)
+
+5. ***Transfer data over SPI bus***
+
+    Transfers the provided data over the SPI bus if the bus is initialized. It is necessary to indicate the length of the transfer to generate the SPI clock cycles. This length could be more than the length of the transferred data to a SPI target, in the cases where the response (data on the MISO line) consists of more bytes than the transferred.
+
+    ```python
+    data = [0x01, 0x02, 0x03, 0x04, 0x05, 0x06]
+    transfer_length = 6
+    success, response = spi_controller.transfer(data, transfer_length)
+    ```
+
+    For a particular case of a SPI target device that interprets instructions via opcodes, an example of use could be the following:
+    
+    ```python
+    # Read opcode: 0x03
+    # Address to read: 0x0002
+    # Transferred data: [opcode, address_H, address_L]
+    data = [0x03, 0x00, 0x02]
+    
+    # Transfer length includes the length of the transferred data to the target and the read length to generate SPI clock cycles for the read operation
+    # Read length: 6 bytes to read
+    # Data to target: 3 bytes
+    read_length = 6
+    data_to_target = len(data)
+    transfer_length = data_to_target + read_length
+
+    success, response = spi_controller.transfer(data, transfer_length)
+
+    # The response consists of the entire MISO line since the transfer started.
+    # If the SPI target device doesn't send information while the instruction is transferred, the first bytes of the response are in IDLE state with the value 0x00
+    # response: [0x00, 0x00, 0x00, 0xFA, 0xFB, 0xFC, 0xFD, 0xFE, 0xFF]
+    data_from_target = response[3:]
+    ```
+
+## Next Steps
+
+After installing the `SupernovaController` package, you can further explore its capabilities by trying out the examples included in the installation. These examples demonstrate practical applications of SPI, UART, I2C and I3C protocols:
 
 - **Basic I3C Example (`basic_i3c_example.py`):** Learn the basics of I3C bus initialization and device communication using the Supernova as an I3C controller.
 - **Basic I3C Target Mode Example (`basic_i3c_target_example.py`):** Learn the basics of I3C target mode implementation using two Supernovas, one as an I3C target and the other one as a controller.
 - **Basic I2C Example (`basic_i2c_example.py`):** Get started with fundamental I2C operations.
 - **Basic UART Example (`basic_uart_example.py`):** Try out the UART protocol Hands-On.
+- **Basic SPI Controller Example (`basic_spi_controller_example.py`):** Explore the fundamental SPI controller operations communicating with a SPI Target device.
 - **IBI Example (`ibi_example.py`):** Understand handling In-Band Interrupts (IBI) in I3C.
 - **ICM42605 I3C Example (`ICM42605_i3c_example.py`):** Explore a real-world application of I3C with the ICM42605 sensor.
 
 #### Accessing the Examples
 
-The example scripts are installed in a directory named `SupernovaExamples`, which is located in your Python environment's directory. To find this directory, you can use the following Python commands:
+The example scripts are installed in your site-packages folder as `supernovacontrollerexamples`, and you can access them just like you would any other package in Python. To find this directory, you can use the following Python commands:
 
 ```python
 import sys
 import os
 
-examples_dir_name = "SupernovaExamples"
-examples_path = os.path.join(sys.prefix, examples_dir_name)
+examples_dir_name = "supernovacontrollerexamples"
+examples_path = os.path.join(sys.prefix, "lib", "site-packages", examples_dir_name)
 print(f"Examples are located in: {examples_path}")
 ```
 
 This will print the path to the `SupernovaExamples` directory. Navigate to this directory to find the example scripts.
 
 You can run an example directly from this directory using Python. For instance:
 
 ```sh
-python /path/to/SupernovaExamples/basic_i2c_example.py
+python /path/to/supernovacontrollerexamples/basic_i2c_example.py
 ```
 
-Replace `/path/to/SupernovaExamples/` with the actual path printed in the previous step and `basic_i2c_example.py` with the name of the example you wish to run.
+Replace `/path/to/supernovacontrollerexamples/` with the actual path printed in the previous step and `basic_i2c_example.py` with the name of the example you wish to run.
+
+Or by calling the main method from the example directly from your Python script, as so:
+
+```python
+from supernovacontrollerexamples import basic_i2c_example
+
+basic_i2c_example.main()
+```
 
 #### Exploring Further
 
 Each example is designed to provide insights into different aspects of the `SupernovaController` usage. By running and modifying these examples, you'll gain a deeper understanding of how to effectively use the package in various scenarios.
 
 ## Error Handling
```

### Comparing `supernovacontroller-1.1.0/examples/ICM42605_i3c_example.py` & `supernovacontroller-1.2.0/examples/ICM42605_i3c_example.py`

 * *Files identical despite different names*

### Comparing `supernovacontroller-1.1.0/examples/basic_i2c_example.py` & `supernovacontroller-1.2.0/examples/basic_i2c_example.py`

 * *Files identical despite different names*

### Comparing `supernovacontroller-1.1.0/examples/basic_i3c_example.py` & `supernovacontroller-1.2.0/examples/basic_i3c_example.py`

 * *Files identical despite different names*

### Comparing `supernovacontroller-1.1.0/examples/basic_i3c_target_example.py` & `supernovacontroller-1.2.0/examples/basic_i3c_target_example.py`

 * *Files identical despite different names*

### Comparing `supernovacontroller-1.1.0/examples/basic_uart_example.py` & `supernovacontroller-1.2.0/examples/basic_uart_example.py`

 * *Files identical despite different names*

### Comparing `supernovacontroller-1.1.0/examples/ibi_example.py` & `supernovacontroller-1.2.0/examples/ibi_example.py`

 * *Files identical despite different names*

### Comparing `supernovacontroller-1.1.0/setup.py` & `supernovacontroller-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import os
 from setuptools import setup, find_packages
 
-# Read GH_TOKEN from environment variables // Remove when transfer_controller v0.3.0 is approved
+# Read GH_TOKEN from environment variables
 gh_token = os.environ.get('GH_TOKEN')
 
+dev_dependencies = []
+
+if gh_token:
+    dev_dependencies.append(f'binhosimulators @ git+https://{gh_token}@github.com/binhollc/BinhoSimulators.git@v0.1.1')
+
 setup(
     name='supernovacontroller',
-    version='1.1.0',
+    version='1.2.0',
     packages=find_packages(),
     data_files=[
-        ('SupernovaExamples', ['examples/basic_i2c_example.py', 'examples/basic_i3c_example.py', 'examples/ibi_example.py', 'examples/ICM42605_i3c_example.py', 'examples/basic_i3c_target_example.py'])
+        ('lib/site-packages/supernovacontrollerexamples', ['examples/basic_i2c_example.py', 'examples/basic_i3c_example.py', 'examples/ibi_example.py', 'examples/ICM42605_i3c_example.py', 'examples/basic_i3c_target_example.py',
+                               'examples/basic_uart_example.py', 'examples/basic_spi_controller_example.py'])
     ],
     description='A blocking API for interacting with the Supernova host-adapter device',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Binho LLC',
     author_email='support@binho.io',
     url='https://github.com/binhollc/SupernovaController',
     license='Private',
     install_requires=[
-      'transfer_controller==0.3.1',
-      'BinhoSupernova==2.0.1'
-    ],
+      'transfer_controller==0.4.0',
+      'BinhoSupernova==2.0.1',
+    ] + dev_dependencies,
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.5',
+    python_requires='>=3.9',
 )
```

### Comparing `supernovacontroller-1.1.0/supernovacontroller/errors/exceptions.py` & `supernovacontroller-1.2.0/supernovacontroller/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `supernovacontroller-1.1.0/supernovacontroller/sequential/i2c.py` & `supernovacontroller-1.2.0/supernovacontroller/sequential/i2c.py`

 * *Files identical despite different names*

### Comparing `supernovacontroller-1.1.0/supernovacontroller/sequential/i3c.py` & `supernovacontroller-1.2.0/supernovacontroller/sequential/i3c.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,25 +325,34 @@
         else:
             result = (False, responses[0]["errors"])
 
         return result
 
     def _process_response(self, command_name, responses, extra_data=None):
         def format_response_payload(command_name, response):
-            match command_name:
-                case "write": return None
-                case "read": return response["data"]
-                case "ccc_getpid": return [int(item[2:], 16) for item in response["pid"]]
-                case "ccc_getbcr": return response["bcr"]["value"][2][2:].upper()
-                case "ccc_getdcr": return response["dcr"][2:].upper()
-                case "ccc_getmrl": return response["maxReadLength"]
-                case "ccc_getmwl": return response["maxWriteLength"]
-                case "ccc_get_status": return response["data"]
-                case "ccc_setnewda": return None
-                case "ccc_unicast_setmrl" | "ccc_unicast_setmwl" | "ccc_broadcast_setmwl" | "ccc_broadcast_setmrl" : return response["data"]
+            if command_name == "write":
+                return None
+            elif command_name == "read":
+                return response["data"]
+            elif command_name == "ccc_getpid":
+                return [int(item[2:], 16) for item in response["pid"]]
+            elif command_name == "ccc_getbcr":
+                return response["bcr"]["value"][2][2:].upper()
+            elif command_name == "ccc_getdcr":
+                return response["dcr"][2:].upper()
+            elif command_name == "ccc_getmrl":
+                return response["maxReadLength"]
+            elif command_name == "ccc_getmwl":
+                return response["maxWriteLength"]
+            elif command_name == "ccc_get_status":
+                return response["data"]
+            elif command_name == "ccc_setnewda":
+                return None
+            elif command_name in ["ccc_unicast_setmrl", "ccc_unicast_setmwl", "ccc_broadcast_setmwl", "ccc_broadcast_setmrl"]:
+                return response["data"]
             return None
 
         response = responses[0]
         if response["header"]["result"] == "I3C_TRANSFER_SUCCESS":
             data = format_response_payload(command_name, response)
             result_data = data
             if extra_data:
```

### Comparing `supernovacontroller-1.1.0/supernovacontroller/sequential/i3c_target.py` & `supernovacontroller-1.2.0/supernovacontroller/sequential/i3c_target.py`

 * *Files identical despite different names*

### Comparing `supernovacontroller-1.1.0/supernovacontroller/sequential/supernova_device.py` & `supernovacontroller-1.2.0/supernovacontroller/sequential/supernova_device.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from supernovacontroller.errors import BackendError
 import queue
 import threading
 from .i2c import SupernovaI2CBlockingInterface
 from .i3c import SupernovaI3CBlockingInterface
 from .uart import SupernovaUARTBlockingInterface
 from .i3c_target import SupernovaI3CTargetBlockingInterface
+from .spi_controller import SupernovaSPIControllerBlockingInterface
 
 def id_gen(start=0):
     i = start
     while True:
         i += 1
         yield i
 
@@ -38,14 +39,15 @@
       self.driver = Supernova()
 
       self.interfaces = {
           "i2c": [None, SupernovaI2CBlockingInterface],
           "i3c.controller": [None, SupernovaI3CBlockingInterface],
           "uart":[None, SupernovaUARTBlockingInterface],
           "i3c.target": [None, SupernovaI3CTargetBlockingInterface],
+          "spi.controller": [None, SupernovaSPIControllerBlockingInterface],
       }
 
       self.mounted = False
 
     def open(self, usb_address=None):
         if self.mounted:
             raise DeviceAlreadyMountedError
```

### Comparing `supernovacontroller-1.1.0/supernovacontroller/sequential/uart.py` & `supernovacontroller-1.2.0/supernovacontroller/sequential/uart.py`

 * *Files identical despite different names*

### Comparing `supernovacontroller-1.1.0/supernovacontroller.egg-info/PKG-INFO` & `supernovacontroller-1.2.0/supernovacontroller.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: supernovacontroller
-Version: 1.1.0
+Version: 1.2.0
 Summary: A blocking API for interacting with the Supernova host-adapter device
 Home-page: https://github.com/binhollc/SupernovaController
 Author: Binho LLC
 Author-email: support@binho.io
 License: Private
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # SupernovaController
 Manages communications with the Supernova host-adapter USB HID device.
 
 ## Introduction
 SupernovaController is a Python-based tool designed to interface with the Supernova host-adapter USB HID device. Offering a blocking API, it simplifies command sequences and interactions in the context of asynchronous operation environments like the one offered by the Supernova host-adapter. This approach enhances usability and efficiency, providing a streamlined experience for developers working with the Supernova device.
 
 ## Features
 - **Blocking API:** A streamlined approach to interact with the Supernova device, minimizing the complexity of handling asynchronous callbacks.
-- **Multi-Interface:** Easily communicate with UART, I2C and I3C Devices in an All-In-One package.
+- **Multi-Interface:** Easily communicate with SPI, UART, I2C and I3C Devices in an All-In-One package.
 - **Communication:** Seamlessly manages command responses and notifications, facilitating easier and more intuitive command sequencing.
 - **Examples:** Comprehensive examples demonstrating the practical application of the blocking API.
 
 ## Installation
 
 To install the SupernovaController package, follow these steps:
 
@@ -283,47 +283,299 @@
 
 The fact that the memory is not circular obligates to take into account border cases:
 
 * If the user tries to start the transfer in an address surpassing the target memory range, the target will ignore the address and will start the transfer from the end of the the previous one.
 
 * If the transfer starts in an allowed memory address but tries to surpass the range during the transaction, it will only modify the bytes in the allowed range and discard the rest. The end of the transfer is taken as the end of the memory.
 
-### Next Steps
+## UART protocol
 
-After installing the `SupernovaController` package, you can further explore its capabilities by trying out the examples included in the installation. These examples demonstrate practical applications of UART, I2C and I3C protocols:
+### UART features
+
+This section describes how to get you started with the `SupernovaController` focusing on the UART protocol.
+
+* The supported features are: 
+    * Bus initialization.
+    * Setting of bus parameters such as baudrate, hardware handshake, parity, data size and stop bit.
+    * UART TX/RX transactions of up to 1024 bytes.
+
+### Basic UART Communication
+
+#### Generic operations
+
+1. ***Initializing the Supernova Device:***
+
+   Imports and initializes the `SupernovaDevice`. Optionally, specifies the USB HID path if multiple devices are connected:
+
+   ```python
+   from supernovacontroller.sequential import SupernovaDevice
+
+   device = SupernovaDevice()
+   # Optionally specify the USB HID path
+   device.open(usb_address='your_usb_hid_path')
+   ```
+
+   Call `open()` without parameters if you don't need to specify a particular device.
+
+2. ***Creating a UART controller Interface:***
+
+   Creates a UART controller interface:
+
+   ```python
+   uart = device.create_interface("uart")
+   ``` 
+
+3. ***Closing the Device:***
+
+   Closes the device when done:
+
+   ```python
+   device.close()
+   ```
+
+### Operations intended for the Supernova UART peripheral
+
+1. ***Setting Bus Voltage:***
+
+   Sets the bus voltage (in mV) for the UART bus. This step is required before initializing the bus:
+
+   ```python
+   success, response = uart.set_bus_voltage(3300)
+   ```
+
+2. ***Initializing the Supernova UART peripheral:***
+
+    Initializes the Supernova UART peripheral:
+
+    ```python
+   success, response = uart.init_bus()
+   ```
+    Without any parameters, the UART peripheral initializes with the default values for baudrate (9600bps), parity (no parity), data size (8 bit), stop bit (one stop bit) and hardware handshake (no hardware handshake). Optionally, it is possible to set any of these parameters by specifying them in the init_bus function:
+
+    ```python
+   success, response = uart.init_bus(baudrate=UartControllerBaudRate.UART_BAUD_115200, parity=UartControllerParity.UART_EVEN_PARITY)
+   ```
+3. ***Modifying the UART peripheral parameters***
+
+    It is also possible to configure/set any parameter after initialization (baudrate, parity, data size, stop bit and hardware handshake):
+
+    ```python
+   success, response = uart.set_parameters(stop_bit = UartControllerStopBit.UART_TWO_STOP_BIT, baudrate = UartControllerBaudRate.UART_BAUD_56000)
+   ```
+
+   If parameters are provided, it configures the parameters; otherwise, it retains the current settings.
+
+4. ***Read the current UART peripheral configuration***
+
+    The following method retrieves the current UART peripheral communication parameters, including baudrate, parity, data size, stop bit and hardware handshake.
+
+    ```python
+   success, response = uart.get_parameters()
+   ```
+
+    The variable ```response``` is a tuple containing the current UART controller communication parameters:
+    *(baudrate, parity, data_size, stop_bit, hardware_handshake)*
+
+5. ***Send data over UART bus***
+
+    If the bus is initialized, sends the provided data over the UART TX channel. 
+
+    ```python
+    data = [0x00, 0x01, 0x02, 0x3, 0x04, 0x05, 0x06]
+    success, response = uart.send(data, transferLength)
+    ```
+    - If no errors arises while sending the data, ```success``` will be _true_ and the ```response``` will be a success message.
+    - If an error arises while sending the data, ```success``` will be _false_ and the ```response``` will be an error message.
+
+6. ***Receive data over UART bus***
+
+    If the bus is initialized, awaits reception of data over the UART RX channel. A timeout can be set to the waiting process to exit if no data is received in the timeout's time specified time (use None to ignore the timeout feature). 
+
+    ```python
+    success, response = uart.wait_for_notification(timeout = None)
+    ```
+    - If data is received before the configured timeout, ```success``` will be _true_ and the ```response``` will be the array of received data.
+    - If data is not received before the configured timeout,  ```success``` will be _false_ and the ```response``` will be a timeout error message.
+    - If an error arises while receiving the data, ```success``` will be _false_ and the ```response``` will be an error message.
+
+## SPI protocol
+
+### SPI features
+
+This section describes how to get you started with the `SupernovaController` focusing on the SPI protocol.
+In a SPI bus, the Supernova can act as a controller.
+
+* In controller mode the Supernova supports several features: 
+    * Supernova initialization in SPI controller mode.
+    * Bus initialization.
+    * Setting of bus parameters such as bit order, SPI mode, chip select, chip select polarity and frequency.
+    * SPI transfers of up to 1024 bytes.
+    * 8 bits data width frames.
+
+* Coming soon:
+  * For the SPI controller mode:
+    - Pre and post delays.
+    - Keep chip select active between transfers.
+    - Support for 16 bits data width.
+  * Support for SPI target mode.
+
+### Basic SPI Communication
+
+#### Generic operations
+
+1. ***Initializing the Supernova Device:***
+
+   Imports and initializes the `SupernovaDevice`. Optionally, specifies the USB HID path if multiple devices are connected:
+
+   ```python
+   from supernovacontroller.sequential import SupernovaDevice
+
+   device = SupernovaDevice()
+   
+   # Optionally specify the USB HID path
+   device.open(usb_address='your_usb_hid_path')
+   ```
+
+   Call `open()` without parameters if you don't need to specify a particular device.
+
+2. ***Creating a SPI controller Interface:***
+
+   Creates a SPI controller interface:
+
+   ```python
+   spi_controller = device.create_interface("spi.controller")
+   ``` 
+
+3. ***Closing the Device:***
+
+   Closes the device when done:
+
+   ```python
+   device.close()
+   ```
+
+### Operations intended for the Supernova in SPI controller mode
+
+1. ***Setting Bus Voltage:***
+
+   Sets the bus voltage (in mV) for the SPI bus. This step is required before initializing the bus:
+
+   ```python
+   success, response = spi_controller.set_bus_voltage(3300)
+   ```
+
+2. ***Initializing the Supernova as a SPI controller:***
+
+    Initializes the Supernova in SPI controller mode:
+
+    ```python
+   success, response = spi_controller.init_bus()
+   ```
+    Without any parameters, the SPI controller initializes with the default values for bit order (MSB first), mode (Mode 0), chip select (CS0), chip select polarity (Active low) and frequency (10 MHz). Optionally, it is possible to set any of these parameters by specifying in the init_bus function:
+
+    ```python
+   success, response = spi_controller.init_bus(bit_order=SpiControllerBitOrder.LSB, frequency=20000000)
+   ```
+
+3. ***Modifying the SPI controller parameters***
+
+    It is possible to set a new configuration for each parameter (bit order, mode, chip select, chip select polarity and frequency):
+
+    ```python
+   success, response = spi_controller.set_parameters(bit_order = SpiControllerBitOrder.MSB, mode = SpiControllerMode.MODE_1)
+   ```
+
+   If parameters are provided, it configures the parameters; otherwise, it retains the current settings.
+
+4. ***Read the current SPI controller configuration***
+
+    The following method retrieves the current SPI controller communication parameters, including bit order, spi mode, data width, chip select, chip select polarity and frequency.
+
+    ```python
+   success, response = spi_controller.get_parameters()
+   ```
+
+    The variable ```response``` is a tuple containing the current SPI controller communication parameters:
+    (bit_order, mode, data_width, chip_select, chip_select_pol, frequency)
+
+5. ***Transfer data over SPI bus***
+
+    Transfers the provided data over the SPI bus if the bus is initialized. It is necessary to indicate the length of the transfer to generate the SPI clock cycles. This length could be more than the length of the transferred data to a SPI target, in the cases where the response (data on the MISO line) consists of more bytes than the transferred.
+
+    ```python
+    data = [0x01, 0x02, 0x03, 0x04, 0x05, 0x06]
+    transfer_length = 6
+    success, response = spi_controller.transfer(data, transfer_length)
+    ```
+
+    For a particular case of a SPI target device that interprets instructions via opcodes, an example of use could be the following:
+    
+    ```python
+    # Read opcode: 0x03
+    # Address to read: 0x0002
+    # Transferred data: [opcode, address_H, address_L]
+    data = [0x03, 0x00, 0x02]
+    
+    # Transfer length includes the length of the transferred data to the target and the read length to generate SPI clock cycles for the read operation
+    # Read length: 6 bytes to read
+    # Data to target: 3 bytes
+    read_length = 6
+    data_to_target = len(data)
+    transfer_length = data_to_target + read_length
+
+    success, response = spi_controller.transfer(data, transfer_length)
+
+    # The response consists of the entire MISO line since the transfer started.
+    # If the SPI target device doesn't send information while the instruction is transferred, the first bytes of the response are in IDLE state with the value 0x00
+    # response: [0x00, 0x00, 0x00, 0xFA, 0xFB, 0xFC, 0xFD, 0xFE, 0xFF]
+    data_from_target = response[3:]
+    ```
+
+## Next Steps
+
+After installing the `SupernovaController` package, you can further explore its capabilities by trying out the examples included in the installation. These examples demonstrate practical applications of SPI, UART, I2C and I3C protocols:
 
 - **Basic I3C Example (`basic_i3c_example.py`):** Learn the basics of I3C bus initialization and device communication using the Supernova as an I3C controller.
 - **Basic I3C Target Mode Example (`basic_i3c_target_example.py`):** Learn the basics of I3C target mode implementation using two Supernovas, one as an I3C target and the other one as a controller.
 - **Basic I2C Example (`basic_i2c_example.py`):** Get started with fundamental I2C operations.
 - **Basic UART Example (`basic_uart_example.py`):** Try out the UART protocol Hands-On.
+- **Basic SPI Controller Example (`basic_spi_controller_example.py`):** Explore the fundamental SPI controller operations communicating with a SPI Target device.
 - **IBI Example (`ibi_example.py`):** Understand handling In-Band Interrupts (IBI) in I3C.
 - **ICM42605 I3C Example (`ICM42605_i3c_example.py`):** Explore a real-world application of I3C with the ICM42605 sensor.
 
 #### Accessing the Examples
 
-The example scripts are installed in a directory named `SupernovaExamples`, which is located in your Python environment's directory. To find this directory, you can use the following Python commands:
+The example scripts are installed in your site-packages folder as `supernovacontrollerexamples`, and you can access them just like you would any other package in Python. To find this directory, you can use the following Python commands:
 
 ```python
 import sys
 import os
 
-examples_dir_name = "SupernovaExamples"
-examples_path = os.path.join(sys.prefix, examples_dir_name)
+examples_dir_name = "supernovacontrollerexamples"
+examples_path = os.path.join(sys.prefix, "lib", "site-packages", examples_dir_name)
 print(f"Examples are located in: {examples_path}")
 ```
 
 This will print the path to the `SupernovaExamples` directory. Navigate to this directory to find the example scripts.
 
 You can run an example directly from this directory using Python. For instance:
 
 ```sh
-python /path/to/SupernovaExamples/basic_i2c_example.py
+python /path/to/supernovacontrollerexamples/basic_i2c_example.py
 ```
 
-Replace `/path/to/SupernovaExamples/` with the actual path printed in the previous step and `basic_i2c_example.py` with the name of the example you wish to run.
+Replace `/path/to/supernovacontrollerexamples/` with the actual path printed in the previous step and `basic_i2c_example.py` with the name of the example you wish to run.
+
+Or by calling the main method from the example directly from your Python script, as so:
+
+```python
+from supernovacontrollerexamples import basic_i2c_example
+
+basic_i2c_example.main()
+```
 
 #### Exploring Further
 
 Each example is designed to provide insights into different aspects of the `SupernovaController` usage. By running and modifying these examples, you'll gain a deeper understanding of how to effectively use the package in various scenarios.
 
 ## Error Handling
```

### Comparing `supernovacontroller-1.1.0/supernovacontroller.egg-info/SOURCES.txt` & `supernovacontroller-1.2.0/supernovacontroller.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 MANIFEST.in
 README.md
 setup.py
 examples/ICM42605_i3c_example.py
 examples/basic_i2c_example.py
 examples/basic_i3c_example.py
 examples/basic_i3c_target_example.py
+examples/basic_spi_controller_example.py
 examples/basic_uart_example.py
 examples/ibi_example.py
 supernovacontroller/__init__.py
 supernovacontroller.egg-info/PKG-INFO
 supernovacontroller.egg-info/SOURCES.txt
 supernovacontroller.egg-info/dependency_links.txt
 supernovacontroller.egg-info/requires.txt
 supernovacontroller.egg-info/top_level.txt
 supernovacontroller/errors/__init__.py
 supernovacontroller/errors/exceptions.py
 supernovacontroller/sequential/__init__.py
 supernovacontroller/sequential/i2c.py
 supernovacontroller/sequential/i3c.py
 supernovacontroller/sequential/i3c_target.py
+supernovacontroller/sequential/spi_controller.py
 supernovacontroller/sequential/supernova_device.py
 supernovacontroller/sequential/uart.py
 supernovacontroller/utils/__init__.py
 supernovacontroller/utils/mctp.py
```

