# Comparing `tmp/pyircsdk-1.1.0.tar.gz` & `tmp/pyircsdk-1.2.0.tar.gz`

## Comparing `pyircsdk-1.1.0.tar` & `pyircsdk-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/__about__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/command.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/message.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/pyircsdk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/event/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyircsdk/event/event.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/LICENSE
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/README.md
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/__about__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/command.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/message.py
+-rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/pyircsdk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/event/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/event/event.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/LICENSE
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/README.md
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/PKG-INFO
```

### Comparing `pyircsdk-1.1.0/pyircsdk/command.py` & `pyircsdk-1.2.0/pyircsdk/command.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.1.0/pyircsdk/message.py` & `pyircsdk-1.2.0/pyircsdk/message.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.1.0/pyircsdk/pyircsdk.py` & `pyircsdk-1.2.0/pyircsdk/pyircsdk.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,101 @@
 import socket
 import sys
 
 from .event.event import Event
 from .message import Message
 
+class IRCSDKConfig:
+    def __init__(self, host, port, nick, channel, user, realname):
+        self.host = host
+        self.port = port
+        self.nick = nick
+        self.channel = channel
+        self.user = user
+        self.realname = realname
+
+    def __str__(self):
+        return f'Host: {self.host}, Port: {self.port}, Nick: {self.nick}, Channel: {self.channel}, User: {self.user}'
+
+    def __repr__(self):
+        return f'Host: {self.host}, Port: {self.port}, Nick: {self.nick}, Channel: {self.channel}, User: {self.user}'
+
 
 class IRCSDK:
-    def __init__(self, config):
-        self.event = Event()
+    def __init__(self, config: IRCSDKConfig = None) -> None:
+        self.event: Event = Event()
         if config:
             self.config = config
             self.irc = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
-    def privmsg(self, receiver, msg):
+    def privmsg(self, receiver: str, msg: str) -> None:
         command = "PRIVMSG %s :%s\r\n" % (receiver, msg)
         self.irc.send(command.encode('utf-8'))
 
-    def sendRaw(self, msg):
+    def sendRaw(self, msg: str) -> None:
         self.irc.send(msg.encode('utf-8'))
 
-    def close(self):
+    def close(self) -> None:
         message = "QUIT :%s\r\n" % self.config.nick
         self.irc.send(message.encode('utf-8'))
         self.irc.close()
 
-    def connect(self, config):
+    def connect(self, config: IRCSDKConfig = None) -> None:
         # if no config use __init__ config
         if not config:
             config = self.config
 
         # if no config is passed throw an error
         if not self.config:
             raise ValueError('No config passed to connect')
 
-        self.irc = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.irc: socket.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         # print config
         print(config)
 
         self.irc.connect((self.config.host, self.config.port))
         self.event.emit('connected', 'Connected to host %s:%s' % (self.config.host, self.config.port))
 
         self.event.on('raw', self.log)
         self.event.on('raw', self.handle_raw_message)
-        self.setUser(self.config.user)
+        self.setUser(self.config.user, self.config.realname)
         self.setNick(self.config.nick)
+
         self.event.on('connected', lambda data: self.join(self.config.channel))
         self.startRecv()
 
-    def startRecv(self):
+    def startRecv(self) -> None:
         while 1:
             try:
                 text = self.irc.recv(2048)
                 self.event.emit('raw', text)
 
             except OSError as e:
                 print(e)
                 # exit program
                 sys.exit(1)
-                break
 
-    def log(self, data):
+    def log(self, data: bytes) -> None:
         # convert bytes to string
         data = data.decode('utf-8')
         # print(data)
 
-    def join(self, channel):
+    def join(self, channel: str) -> None:
         buffer = "JOIN %s\r\n" % channel
         self.irc.send(buffer.encode('utf-8'))
 
-    def setUser(self, user):
-        command = "USER %s 0 * :%s\r\n" % (user, user)
+    def setUser(self, user: str, realname: str) -> None:
+        command = "USER %s 0 * :%s\r\n" % (user, realname)
         self.irc.send(command.encode('utf-8'))
 
-    def setNick(self, nick):
+    def setNick(self, nick: str) -> None:
         command = "NICK %s\r\n" % nick
         self.irc.send(command.encode('utf-8'))
 
-    def handle_raw_message(self, data):
+    def handle_raw_message(self, data: bytes) -> None:
         # parse message
         data = data.decode('utf-8')
         for line in data.split('\r\n'):
             if line:
                 message, message_list, prefix, command, params, trailing = self.parse_message(line.encode('utf-8'))
                 # print('Message: %s' % message)
                 # print('Message List: %s' % message_list)
@@ -99,15 +114,15 @@
                     self.event.emit('connected', 'End of /MOTD command.')
 
                 # # find To connect type /QUOTE PONG
                 # if data.find('To connect type /QUOTE PONG') != -1:
                 #     print(data.split(':')[1])
                 #     self.sendRaw('QUOTE PONG ' + data.split(':')[1] + '\r\n')
 
-    def parse_message(self, data):
+    def parse_message(self, data: bytes) -> tuple:
         # convert bytes to string
         data = data.decode('utf-8')
 
         # <message>  ::= [':' <prefix> <SPACE> ] <command> <params> <crlf>
         # <prefix>   ::= <servername> | <nick> [ '!' <user> ] [ '@' <host> ]
         # <command>  ::= <letter> { <letter> } | <number> <number> <number>
         # <SPACE>    ::= ' ' { ' ' }
@@ -135,33 +150,20 @@
 
         if params:
             if params[0].startswith(':'):
                 trailing = params[0][1:]
                 params = params[1:]
             else:
                 trailing = None
-        messageFrom = prefix.split('!')[0] if prefix else None
-        messageTo = params[0] if params else None
+        messageFrom: str = prefix.split('!')[0] if prefix else None
+        messageTo: str = params[0] if params else None
         # remove the first element from params
-        actualMessage = ' '.join(params[1:]) if params else None
+        actualMessage: str = ' '.join(params[1:]) if params else None
         # remove the ":" from the actual message
         if actualMessage:
-            actualMessage = actualMessage[1:]
+            actualMessage: str = actualMessage[1:]
 
         self.event.emit('message',
                         Message(data, prefix, command, params, trailing, messageFrom, messageTo, actualMessage))
 
         return data, message, prefix, command, params, trailing
 
-class IRCSDKConfig:
-    def __init__(self, host, port, nick, channel, user):
-        self.host = host
-        self.port = port
-        self.nick = nick
-        self.channel = channel
-        self.user = user
-
-    def __str__(self):
-        return f'Host: {self.host}, Port: {self.port}, Nick: {self.nick}, Channel: {self.channel}, User: {self.user}'
-
-    def __repr__(self):
-        return f'Host: {self.host}, Port: {self.port}, Nick: {self.nick}, Channel: {self.channel}, User: {self.user}'
```

### Comparing `pyircsdk-1.1.0/pyircsdk/event/event.py` & `pyircsdk-1.2.0/pyircsdk/event/event.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.1.0/.gitignore` & `pyircsdk-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.1.0/LICENSE` & `pyircsdk-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.1.0/README.md` & `pyircsdk-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.1.0/pyproject.toml` & `pyircsdk-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "pyircsdk"
 authors = [
   { name="Bludot", email="admin@floretos.com" },
 ]
-version = "1.1.0"
+version = "1.2.0"
 description = "pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyircsdk-1.1.0/PKG-INFO` & `pyircsdk-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyircsdk
-Version: 1.1.0
+Version: 1.2.0
 Summary: pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages.
 Project-URL: Homepage, https://github.com/bludot/pyircsdk
 Project-URL: Issues, https://github.com/bludot/pyircsdk/issues
 Author-email: Bludot <admin@floretos.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

