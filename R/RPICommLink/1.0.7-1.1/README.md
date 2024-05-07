# Comparing `tmp/RPICommLink-1.0.7.tar.gz` & `tmp/RPICommLink-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RPICommLink-1.0.7.tar", last modified: Tue May  7 10:00:27 2024, max compression
+gzip compressed data, was "dist\RPICommLink-1.1.tar", last modified: Tue May  7 17:06:04 2024, max compression
```

## Comparing `RPICommLink-1.0.7.tar` & `RPICommLink-1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/
--rw-rw-rw-   0        0        0     1749 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/RPICommLink/
--rw-rw-rw-   0        0        0    15711 2024-05-07 09:48:52.000000 RPICommLink-1.0.7/RPICommLink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/RPICommLink.egg-info/
--rw-rw-rw-   0        0        0     1749 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/RPICommLink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/RPICommLink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/RPICommLink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/RPICommLink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 10:00:27.000000 RPICommLink-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1753 2024-05-07 09:52:36.000000 RPICommLink-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:06:04.000000 RPICommLink-1.1/
+-rw-rw-rw-   0        0        0     2022 2024-05-07 17:06:04.000000 RPICommLink-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 17:06:04.000000 RPICommLink-1.1/RPICommLink/
+-rw-rw-rw-   0        0        0    19316 2024-05-07 16:43:48.000000 RPICommLink-1.1/RPICommLink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:06:04.000000 RPICommLink-1.1/RPICommLink.egg-info/
+-rw-rw-rw-   0        0        0     2022 2024-05-07 17:06:04.000000 RPICommLink-1.1/RPICommLink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-05-07 17:06:04.000000 RPICommLink-1.1/RPICommLink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 17:06:04.000000 RPICommLink-1.1/RPICommLink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-07 17:06:04.000000 RPICommLink-1.1/RPICommLink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 17:06:04.000000 RPICommLink-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2035 2024-05-07 17:05:57.000000 RPICommLink-1.1/setup.py
```

### Comparing `RPICommLink-1.0.7/PKG-INFO` & `RPICommLink-1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: RPICommLink
-Version: 1.0.7
+Version: 1.1
 Summary: A library for communication on Raspberry Pi
 Home-page: UNKNOWN
 Author: adixu
 Author-email: adixu7@gmail.com
 License: UNKNOWN
 Description: RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。
         
@@ -45,8 +45,14 @@
         1.0.6 -修复了潜在bug
         
         
         
         
         
         1.0.7 -轻量化
+        
+        
+        
+        
+        
+        1.1   -增加了传输摄像头帧的函数，需要自行下载opencv-python库。注意：该版本为测试版，将会有许多未发现的报错，建议在在服务器端发送摄像头帧而不是客户端。
 Platform: UNKNOWN
```

### Comparing `RPICommLink-1.0.7/RPICommLink/__init__.py` & `RPICommLink-1.1/RPICommLink/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,25 +13,29 @@
         self.thread_now:当前正在运行的线程列表，用于存储正在等待接受数据的线程。
         self.data_event:线程间的事件通信。
         self.rpi_port:服务器打开的端口与客户端连接的端口，默认为11451。
         self.password:发送请求的密码。
         self.target_name:存储扫描到的设备名。
         self.connect_device:客户端已连接的设备。
         self.send_server_socket:发送的服务器套接字。
+        self.state:状态，如果为False则为普通的发信息状态，True为发图片
+        self._device_state:私有变量，表示当前设备为服务器或客户端
         """
         self.return_data = None
         self.socket_list = []
         self.threading_now = []
         self.data_event = threading.Event()
         self.data_event.clear()
         self.rpi_port = rpi_port
         self.password = password
         self.target_name = []
         self.connect_device = []
         self._send_server_socket = []
+        self.state = False
+        self._device_state = None
 
     def open(self, device_name: str = 'default', max_connect: int = 0, ip: str = None):
         """打开_server线程的函数
 
         它使用线程来启动服务器是为了实现非阻塞式的服务器启动。如果直接调用 _server 方法而不使用线程，
         那么在服务器启动过程中，主程序会被阻塞，直到服务器关闭或者达到最大连接数为止。
 
@@ -41,14 +45,19 @@
 
         因此，使用线程来启动服务器可以提高程序的并发性和响应性，使程序更加灵活和高效。
 
         :param ip: ip地址，如果无法正确打开IP地址，请自行查看本地IP地址设置
         :param device_name:该设备名称，用于将设备名称发送给客户端
         :param max_connect:最大的客户端连接数量，如果它为0，则不作限制
         """
+        if self._device_state is None:
+            self._device_state = 'server'
+        else:
+            print(f'\033[91mError:当前为客户端，无法作为服务器打开 \033[0m')
+            exit()
         listen_thread = threading.Thread(target=self._server, args=(device_name, max_connect, ip), daemon=True)
         listen_thread.start()
 
     def _server(self, device_name, max_connect, ip):
         """_server 的作用是启动一个服务器，用于监听客户端的连接请求，并根据一定条件接受或拒绝连接的线程。
 
         它负责创建一个 TCP 套接字，绑定到本机的 IP 地址和指定的端口号，然后在一个无限循环中等待客户端的连接请求。
@@ -172,30 +181,31 @@
         如果接收到了数据，将其解码为 UTF-8 格式，并存储在 self.return_data 属性中。
         通过 self.data_event.set() 设置数据事件，表示数据已经接收到。
 
         从 self.threading_now 列表中移除当前处理的套接字，表示该线程已完成。
 
         :param sock:需要接受到数据的套接字
         """
-        try:
-            recv_data = sock[0].recv(1024)
-            if not recv_data:
-                sock[0].close()
-                self.socket_list.remove(sock)
-                print(f"\033[93mError:一台设备断开了连接，当前设备数为{len(self.socket_list)}\033[0m")
-            else:
-                self.return_data = recv_data.decode('utf-8')
-                self.data_event.set()  # 设置数据事件，表示数据已经接收到
-            self.threading_now.remove(sock)
-        except Exception:
-            if sock in self.threading_now:
+        if not self.state:
+            try:
+                recv_data = sock[0].recv(1024)
+                if not recv_data:
+                    sock[0].close()
+                    self.socket_list.remove(sock)
+                    print(f"\033[93mError:一台设备断开了连接，当前设备数为{len(self.socket_list)}\033[0m")
+                else:
+                    self.return_data = recv_data.decode('utf-8')
+                    self.data_event.set()  # 设置数据事件，表示数据已经接收到
                 self.threading_now.remove(sock)
-            if sock in self.socket_list:
-                self.socket_list.remove(sock)
-            print(f"\033[91mError:一台设备连接异常中止 \033[0m")
+            except Exception:
+                if sock in self.threading_now:
+                    self.threading_now.remove(sock)
+                if sock in self.socket_list:
+                    self.socket_list.remove(sock)
+                print(f"\033[91mError:一台设备连接异常中止 \033[0m")
 
     def _scan_port(self, ip, port, target):
         """扫描指定 IP 地址和端口，扫描局域网内的多个设备是否开放了指定的端口，并且尝试与这些设备建立连接。
 
         创建一个 TCP 套接字并设置超时时间为 1 秒。尝试连接指定的 IP 地址和端口。
         如果连接成功，发送密码给服务器端。
         接收服务器端返回的设备名字，并将其存储在 self.target_name 中。
@@ -244,14 +254,20 @@
         在连接成功时，发送密码给服务器端，并接收服务器返回的设备名称和状态。
         打印扫描到的设备名称。
         根据连接状态输出相应的信息。
 
         :param subnet_ip:子网，IP地址前三个数，格式为str’xxx.xxx.xx‘
         :param target_name: 指定的设备名字
         """
+        if self._device_state is None:
+            self._device_state = 'client'
+        else:
+            print(f'\033[91mError:当前为服务器，无法连接第二个服务器，只能等待其它连接 \033[0m')
+            exit()
+
         if subnet_ip is None:
             local_ip = get_host_ip()  # 获取本地主机的IP地址
             subnet = '.'.join(local_ip.split('.')[:-1])  # 获取局域网子网
         else:
             subnet = subnet_ip
         port = self.rpi_port  # 要扫描的端口号
         threads = []
@@ -289,14 +305,91 @@
             except Exception:
                 print('\033[91mError:一个服务器发送失败！请确认是否有连接服务器 \033[0m')
                 self._send_server_socket.remove(sock)
                 if len(self._send_server_socket) == 0:
                     print('\033[91mError:无服务器连接 \033[0m')
                     sys.exit()
 
+    def auto_frame(self):
+        if self._device_state == 'server':
+            threading.Thread(target=self._auto_frame, daemon=True).start()
+        elif self._device_state is None:
+            print(f'\033[91mError:未开启或连接服务器 \033[0m')
+        else:
+            threading.Thread(target=self._auto_frame, daemon=True).start()
+            print(f'\033[93mWarning:客户端发送系统冲突！这会导致无法发送正常数据以及其它报错！'
+                  f'这不是一个正常用法，强烈建议使用send_frame自行进行发送！ \033[0m')
+
+    def _auto_frame(self):
+        import cv2
+
+        cap = cv2.VideoCapture(0)
+        while True:
+            print(1)
+            ret, _frame = cap.read()
+            self.send_frame(_frame)
+
+    def send_frame(self, frame):
+        """读摄像头数据 发送给服务器"""
+        import cv2
+        import numpy
+        import struct
+
+        sock_list = []
+        if self._device_state == 'server':
+            sock_list = self.socket_list
+        elif self._device_state is None:
+            print(f'\033[91mError:未开启或连接服务器 \033[0m')
+        else:
+            sock_list.append(self._send_server_socket)
+
+        resolution = (640, 480)
+        try:
+            frame = cv2.resize(frame, resolution)
+            ret, img = cv2.imencode('.jpg', frame, [cv2.IMWRITE_JPEG_QUALITY, 100])
+            img_code = numpy.array(img)
+            img = img_code.tobytes()
+            length = len(img)
+            all_data = struct.pack('ihh', length, resolution[0], resolution[1]) + img
+            for sock in sock_list:
+                sock[0].send(all_data)
+                time.sleep(0.01)
+                print('send')
+        except Exception as e:
+            print(e)
+
+    def recv_frame(self):
+        import struct
+        import numpy
+        import cv2
+
+        sock_list = []
+        if self._device_state == 'client':
+            sock_list.append(self._send_server_socket)
+        elif self._device_state is None:
+            print(f'\033[91mError:未开启或连接服务器 \033[0m')
+        else:
+            self.state = True
+            sock_list = self.socket_list
+            self.wait()
+        for sock in sock_list:
+            data = sock[0].recv(8)
+
+        length, width, height = struct.unpack('ihh', data)
+        img_data = b''  # 存放最终的图片数据
+        while length:
+            for sock in sock_list:
+                temp_size = sock[0].recv(length)
+                length -= len(temp_size)
+                img_data += temp_size
+        data = numpy.frombuffer(img_data, dtype='uint8')
+        image = cv2.imdecode(data, cv2.IMREAD_UNCHANGED)
+        self.state = False
+        return image
+
 
 def get_host_ip():
     """
     查询本机IP地址
     :return:本机IP地址
     """
     try:
```

### Comparing `RPICommLink-1.0.7/RPICommLink.egg-info/PKG-INFO` & `RPICommLink-1.1/RPICommLink.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: RPICommLink
-Version: 1.0.7
+Version: 1.1
 Summary: A library for communication on Raspberry Pi
 Home-page: UNKNOWN
 Author: adixu
 Author-email: adixu7@gmail.com
 License: UNKNOWN
 Description: RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。
         
@@ -45,8 +45,14 @@
         1.0.6 -修复了潜在bug
         
         
         
         
         
         1.0.7 -轻量化
+        
+        
+        
+        
+        
+        1.1   -增加了传输摄像头帧的函数，需要自行下载opencv-python库。注意：该版本为测试版，将会有许多未发现的报错，建议在在服务器端发送摄像头帧而不是客户端。
 Platform: UNKNOWN
```

### Comparing `RPICommLink-1.0.7/setup.py` & `RPICommLink-1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from setuptools import setup
 
 setup(
     name='RPICommLink',
-    version='1.0.7',
+    version='1.1',
     author='adixu',
     author_email='adixu7@gmail.com',
     description='A library for communication on Raspberry Pi',
     long_description="RPICommLink 是一个用于在不同设备之间建立通信连接的 Python 类。提供了一系列方法使设备能够通过 TCP/IP 协议进行数据交换。"
                      "灵活的通信设置可以轻松地在设备之间建立通信连接，无论是在局域网内部还是通过互联网。"
                      "具备完善的错误处理机制及时发现并处理连接中断、超时等异常情况，保证通信的稳定性和可靠性。"
                      "使用简单易用的接口可以方便地发送和接收数据，无需过多关注底层网络细节，让设备之间的通信变得更加简单和高效。"
                      "通过 RPICommLink 类，可以实现设备之间的数据交换，为项目提供强大的通信支持。"
                      "\n\n\n\n\n\n历代版本更新："
                      "\n\n\n\n\n\n1.0.2 -优化了函数的命名，发送模块不再进行死循环。"
                      "\n\n\n\n\n\n1.0.3 -修复了潜在bug，优化了获取IP的方式，现在可以不命名而使用默认设备名称了。添加了中文介绍。"
                      "\n\n\n\n\n\n1.0.4 -重新了上传中文介绍。"
                      "\n\n\n\n\n\n1.0.5 -修复了无法在无互联网下获取IP的报错，修复了无法同时连接两个服务器的bug。"
                      "\n\n\n\n\n\n1.0.6 -修复了潜在bug"
-                     "\n\n\n\n\n\n1.0.7 -轻量化",
+                     "\n\n\n\n\n\n1.0.7 -轻量化"
+                     "\n\n\n\n\n\n1.1   -增加了传输摄像头帧的函数，需要自行下载opencv-python库。注意：该版本为测试版，将会有许多未发现的报错，建议在在服务器端发送摄像头帧而不是客户端。",
     packages=['RPICommLink'],
+    include_package_data=True,
     install_requires=[],
 )
```

