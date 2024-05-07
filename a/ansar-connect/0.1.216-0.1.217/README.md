# Comparing `tmp/ansar_connect-0.1.216.tar.gz` & `tmp/ansar_connect-0.1.217.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.216.tar", last modified: Mon May  6 20:55:07 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.217.tar", last modified: Tue May  7 00:48:59 2024, max compression
```

## Comparing `ansar_connect-0.1.216.tar` & `ansar_connect-0.1.217.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 20:55:07.714729 ansar_connect-0.1.216/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.216/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 20:55:07.714729 ansar_connect-0.1.216/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.216/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.216/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-06 20:55:07.714729 ansar_connect-0.1.216/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.216/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 20:55:07.710729 ansar_connect-0.1.216/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 20:55:07.710729 ansar_connect-0.1.216/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 20:55:07.710729 ansar_connect-0.1.216/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.216/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.216/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.216/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.216/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 20:55:07.710729 ansar_connect-0.1.216/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-06 20:55:04.000000 ansar_connect-0.1.216/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.216/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    87313 2024-05-06 20:55:01.000000 ansar_connect-0.1.216/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8884 2024-05-06 19:54:12.000000 ansar_connect-0.1.216/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.216/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.216/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.216/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.216/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.216/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.216/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.216/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.216/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.216/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.216/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.216/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.216/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.216/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.216/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.216/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 20:55:07.714729 ansar_connect-0.1.216/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 20:55:07.000000 ansar_connect-0.1.216/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-06 20:55:07.000000 ansar_connect-0.1.216/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-06 20:55:07.000000 ansar_connect-0.1.216/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-06 20:55:07.000000 ansar_connect-0.1.216/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-06 20:55:07.000000 ansar_connect-0.1.216/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-06 20:55:07.000000 ansar_connect-0.1.216/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 00:48:59.245938 ansar_connect-0.1.217/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.217/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-07 00:48:59.245938 ansar_connect-0.1.217/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.217/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.217/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-07 00:48:59.245938 ansar_connect-0.1.217/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.217/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 00:48:59.241938 ansar_connect-0.1.217/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 00:48:59.241938 ansar_connect-0.1.217/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 00:48:59.241938 ansar_connect-0.1.217/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.217/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.217/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.217/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.217/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 00:48:59.245938 ansar_connect-0.1.217/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-07 00:48:56.000000 ansar_connect-0.1.217/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.217/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    87388 2024-05-07 00:48:01.000000 ansar_connect-0.1.217/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9104 2024-05-07 00:25:17.000000 ansar_connect-0.1.217/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.217/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.217/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.217/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.217/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.217/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.217/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.217/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.217/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.217/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.217/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    40495 2024-05-07 00:48:01.000000 ansar_connect-0.1.217/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.217/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 00:41:36.000000 ansar_connect-0.1.217/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.217/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.217/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 00:48:59.245938 ansar_connect-0.1.217/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-07 00:48:59.000000 ansar_connect-0.1.217/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-07 00:48:59.000000 ansar_connect-0.1.217/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-07 00:48:59.000000 ansar_connect-0.1.217/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-07 00:48:59.000000 ansar_connect-0.1.217/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-07 00:48:59.000000 ansar_connect-0.1.217/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-07 00:48:59.000000 ansar_connect-0.1.217/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.216/LICENSE` & `ansar_connect-0.1.217/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/PKG-INFO` & `ansar_connect-0.1.217/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.216
+Version: 0.1.217
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.216/README.md` & `ansar_connect-0.1.217/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/pyproject.toml` & `ansar_connect-0.1.217/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/setup.py` & `ansar_connect-0.1.217/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.217/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.217/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.217/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.217/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/__init__.py` & `ansar_connect-0.1.217/src/ansar/connect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: upgrade-pub-sub-messages
-Commit: d010ae95ec3fc75bcb133b596725ddb5f9c70959
-Version: 0.1.215 (2024-05-07@08:55:04+NZST)
+Commit: d6bc546c0f99d5aac45600fc497588b40c6701bf
+Version: 0.1.216 (2024-05-07@12:48:56+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.216/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.217/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/directory.py` & `ansar_connect-0.1.217/src/ansar/connect/directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -808,15 +808,15 @@
 	self.assign(self.ctd, CONNECT_ABOVE)
 
 	# Acceptance of connections from lower directories.
 	if isinstance(self.accept_below, HostPort):
 		if self.accept_below.host is None:
 			self.send(HostPort(host=None), self.parent_address)
 		else:
-			listen(self, self.accept_below, tag='directory-accept', encrypted=self.encrypted)
+			listen(self, self.accept_below, encrypted=self.encrypted)
 			return OPENING
 	else:
 		pass	# Acceptance arranged externally. May be a
 				# Listening object for diagnosis.
 
 	return NORMAL
 
@@ -1194,16 +1194,17 @@
 		self.session_address = self.created_session
 		self.origin_address = self.created_session
 	else:
 		self.session_address = self.publisher_address
 		self.origin_address = self.remote_session
 
 	self.send(LoopOpened(self.session_address, self.route_key), self.remote_loop)
+	opened_at = ar.world_now()
 	delivered = Delivered(matched_search=self.route.matched_search, matched_name=self.route.matched_name,
-			matched_scope=self.route.matched_scope,
+			matched_scope=self.route.matched_scope, opened_at=opened_at,
 			route_key=self.route_key, agent_address=self.parent_address)
 	self.forward(delivered, self.publisher_address, self.origin_address)
 	return LOOPED
 
 # Methods of termination;
 ### PS-pub-8 Loop terminates by session completion.
 def PublisherLoop_LOOPED_Completed(self, message):
@@ -1715,16 +1716,17 @@
 			# Latch clears additional session alias on stop
 			hand = ar.SwitchOver()
 		# Sending session control message from Latch is flawed - doesnt know
 		# about "origin_address".
 		s = address_to_text(self.subscriber_address)
 		p = address_to_text(self.origin_address)
 		self.trace(f'Loop opened between subscriber [{s}] and publisher [{p}]')
+		opened_at = ar.world_now()
 		available = Available(matched_search=self.route.matched_search, matched_name=self.route.matched_name,
-			matched_scope=self.route.matched_scope,
+			matched_scope=self.route.matched_scope, opened_at=opened_at,
 			route_key=message.route_key, agent_address=self.parent_address)
 		self.forward(available, self.subscriber_address, self.origin_address)
 		self.send(hand, self.latch)
 		# LATCH MUST CONTINUE FOR THOSE MESSAGES THAT WERE
 		# SITTING IN THE QUEUE AFTER THE HANDOVER MESSAGE
 	
 	def latch_loop(self):
```

### Comparing `ansar_connect-0.1.216/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.217/src/ansar/connect/directory_if.py`

 * *Files 13% similar despite different names*

```diff
@@ -75,18 +75,19 @@
 
 # The actual service directory with listings and searches.
 #
 
 # Session messages to publish/listen controllers.
 # Subscribe/client/calling/outbound end.
 class Available(object):
-	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, agent_address=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, opened_at=None, route_key=None, agent_address=None):
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
+		self.opened_at = opened_at
 		self.route_key = route_key
 		self.agent_address = agent_address
 
 class NotAvailable(ar.Faulted):
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, reason=None, agent_address=None):
 		self.matched_search = matched_search
 		self.matched_name = matched_name
@@ -98,18 +99,19 @@
 		#self.condition = cannot
 		#self.explanation = reason
 		self.error_code = None
 		self.error_text = None
 
 # Publish/service/answering/inbound end.
 class Delivered(object):
-	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, agent_address=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, opened_at=None, route_key=None, agent_address=None):
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
+		self.opened_at = opened_at
 		self.route_key = route_key
 		self.agent_address = agent_address
 
 class NotDelivered(ar.Faulted):
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, reason=None, agent_address=None):
 		self.matched_search = matched_search
 		self.matched_name = matched_name
@@ -142,43 +144,44 @@
 		self.route_key = route_key
 		self.reason = reason
 		ar.Faulted.__init__(self, 'peer lost', reason)
 		self.error_code = None
 		self.error_text = None
 
 ENDING_SCHEMA = {
-	'matched_search': str,
-	'matched_name': str,
+	'matched_search': ar.Unicode(),
+	'matched_name': ar.Unicode(),
 	'matched_scope': ScopeOfService,
-	'route_key': str,
+	'opened_at': ar.WorldTime(),
+	'route_key': ar.Unicode(),
 	'session': ar.Any,
 	'value': ar.Any,
-	'reason': str,
-	'condition': str,
-	'explanation': str,
-	'error_text': str,
+	'reason': ar.Unicode(),
+	'condition': ar.Unicode(),
+	'explanation': ar.Unicode(),
+	'error_text': ar.Unicode(),
 	'error_code': ar.Integer8(),
 	'exit_code': ar.Integer8(),
 }
 
 ar.bind(Clear, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Cleared, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Dropped, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 
 SHARED_SCHEMA = {
 	#'route_key': ar.VectorOf(ar.Integer8()),
-	'name': str,
-	'requested_name': str,
-	'requested_search': str,
-	'requested_name': str,
+	'name': ar.Unicode(),
+	'requested_name': ar.Unicode(),
+	'requested_search': ar.Unicode(),
+	'requested_name': ar.Unicode(),
 	'remote_address': ar.Address(),
 	'session_address': ar.Address(),
 	'requested_scope': ScopeOfService,
 	'service_scope': ScopeOfService,
-	'reason': ar.String(),
+	'reason': ar.Unicode(),
 	'listening_ipp': ar.UserDefined(HostPort),
 	'agent_address': ar.Address(),
 	'address': ar.Address(),
 	'published_at': ar.WorldTime(),
 	'subscribed_at': ar.WorldTime(),
 }
```

### Comparing `ansar_connect-0.1.216/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.217/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/group_if.py` & `ansar_connect-0.1.217/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/grouping.py` & `ansar_connect-0.1.217/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/moving.py` & `ansar_connect-0.1.217/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/networking.py` & `ansar_connect-0.1.217/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.217/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/node.py` & `ansar_connect-0.1.217/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.217/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/procedure.py` & `ansar_connect-0.1.217/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/product.py` & `ansar_connect-0.1.217/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/socketry.py` & `ansar_connect-0.1.217/src/ansar/connect/socketry.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,95 +131,86 @@
 		self.object_type = object_type
 		self.args = args
 		self.kw = kw
 
 # Control messages sent to the sockets thread
 # via the control channel.
 class ListenForStream(object):
-	def __init__(self, requested_ipp=None, create_session=None, tag=None, upgrade=None, encrypted=False):
+	def __init__(self, requested_ipp=None, create_session=None, upgrade=None, encrypted=False):
 		self.requested_ipp = requested_ipp or HostPort()
 		self.create_session = create_session
-		self.tag = tag
 		self.upgrade = upgrade
 		self.encrypted = encrypted
 
 class ConnectStream(object):
-	def __init__(self, requested_ipp=None, create_session=None, tag=None, upgrade=None, encrypted=False):
+	def __init__(self, requested_ipp=None, create_session=None, upgrade=None, encrypted=False):
 		self.requested_ipp = requested_ipp or HostPort()
 		self.create_session = create_session
-		self.tag = tag
 		self.upgrade = upgrade
 		self.encrypted = encrypted
 
 class StopListening(object):
 	def __init__(self, listening_ipp=None):
 		self.listening_ipp = listening_ipp or HostPort()
 
 # Update messages from sockets thread to app.
 class Listening(object):
-	def __init__(self, requested_ipp=None, listening_ipp=None, tag=None, encrypted=False):
+	def __init__(self, requested_ipp=None, listening_ipp=None, encrypted=False):
 		self.requested_ipp = requested_ipp or HostPort()
 		self.listening_ipp = listening_ipp or HostPort()
-		self.tag = tag
 		self.encrypted = encrypted
 
 class Accepted(object):
-	def __init__(self, listening_ipp=None, accepted_ipp=None, remote_address=None, opened_at=None, tag=None):
+	def __init__(self, listening_ipp=None, accepted_ipp=None, remote_address=None, opened_at=None):
 		self.listening_ipp = listening_ipp or HostPort()
 		self.accepted_ipp = accepted_ipp or HostPort()
 		self.remote_address = remote_address
 		self.opened_at = opened_at
-		self.tag = tag
 
 class Connected(object):
-	def __init__(self, requested_ipp=None, connected_ipp=None, remote_address=None, opened_at=None, tag=None):
+	def __init__(self, requested_ipp=None, connected_ipp=None, remote_address=None, opened_at=None):
 		self.requested_ipp = requested_ipp or HostPort()
 		self.connected_ipp = connected_ipp or HostPort()
 		self.remote_address = remote_address
 		self.opened_at = opened_at
-		self.tag = tag
 
 class NotListening(ar.Faulted):
-	def __init__(self, requested_ipp=None, error_code=0, error_text=None, tag=None):
+	def __init__(self, requested_ipp=None, error_code=0, error_text=None):
 		cannot = f'cannot listen at "{requested_ipp}"'
 		reason = error_text
 		ar.Faulted.__init__(self, cannot, reason, exit_code=error_code)
 		self.requested_ipp = requested_ipp or HostPort()
 		self.error_code = error_code
 		self.error_text = error_text
-		self.tag = tag
 
 class NotAccepted(ar.Faulted):
-	def __init__(self, listening_ipp=None, error_code=0, error_text=None, tag=None):
+	def __init__(self, listening_ipp=None, error_code=0, error_text=None):
 		cannot = f'cannot accept at "{listening_ipp}"'
 		reason = error_text
 		ar.Faulted.__init__(self, cannot, reason, exit_code=error_code)
 		self.listening_ipp = listening_ipp or HostPort()
 		self.error_code = error_code
 		self.error_text = error_text
-		self.tag = tag
 
 class NotConnected(ar.Faulted):
-	def __init__(self, requested_ipp=None, error_code=0, error_text=None, tag=None):
+	def __init__(self, requested_ipp=None, error_code=0, error_text=None):
 		cannot = f'cannot connect to "{requested_ipp}"'
 		reason = error_text
 		ar.Faulted.__init__(self, cannot, reason, exit_code=error_code)
 		#self.condition = cannot
 		#self.explanation = reason
 		#self.exit_code = error_code
 		self.requested_ipp = requested_ipp or HostPort()
 		self.error_code = error_code
 		self.error_text = error_text
-		self.tag = tag
 
 CONTROL_SCHEMA = {
 	'requested_ipp': ar.UserDefined(HostPort),
 	'controller_address': ar.Address(),
 	'remote_address': ar.Address(),
-	'tag': str,
 	'opened_at': ar.WorldTime(),
 	'upgrade': ar.Type(),
 	'create_session': ar.Type(),
 	'connected_ipp': ar.UserDefined(HostPort),
 	'listening_ipp': ar.UserDefined(HostPort),
 	'accepted_ipp': ar.UserDefined(HostPort),
 	'condition': ar.Unicode(),
@@ -242,36 +233,33 @@
 # Session termination messages. Handshake between app
 # and sockets thread to cleanly terminate a connection.
 class Close(object):
 	def __init__(self, value=None):
 		self.value = value
 
 class Closed(ar.Faulted):
-	def __init__(self, value=None, reason=None, opened_ipp=None, opened_at=None, closed_at=None, tag=None):
+	def __init__(self, value=None, reason=None, opened_ipp=None, opened_at=None, closed_at=None):
 		self.value = value
 		self.opened_ipp = opened_ipp or HostPort()
 		cannot = f'closed {self.opened_ipp}'
 		ar.Faulted.__init__(self, cannot, reason)
 		self.opened_at = opened_at
 		self.closed_at = closed_at
-		self.tag = tag
 
 class Abandoned(ar.Faulted):
-	def __init__(self, opened_ipp=None, opened_at=None, closed_at=None, tag=None):
+	def __init__(self, opened_ipp=None, opened_at=None, closed_at=None):
 		self.opened_ipp = opened_ipp or HostPort()
 		cannot = f'abandoned by {self.opened_ipp}'
 		reason = None
 		ar.Faulted.__init__(self, cannot, reason)
 		self.opened_at = opened_at
 		self.closed_at = closed_at
-		self.tag = tag
 
 ENDING_SCHEMA = {
 	'value': ar.Any,
-	'tag': str,
 	'opened_ipp': ar.UserDefined(HostPort),
 	'condition': ar.Unicode(),
 	'explanation': ar.Unicode(),
 	'exit_code': ar.Integer8(),
 	'error_code': ar.Integer8(),
 	'opened_at': ar.WorldTime(),
 	'closed_at': ar.WorldTime(),
@@ -559,23 +547,22 @@
 			encoded_bytes += str(n).encode('ascii')
 			encoded_bytes += b'\n'
 			encoded_bytes += e
 			encoded_bytes += b'\n'
 		return len(encoded_bytes)
 
 class TcpStream(StreamingIn, StreamingOut):
-	def __init__(self, parent, controller_address, upgrade, opened, tag):
+	def __init__(self, parent, controller_address, upgrade, opened):
 		StreamingIn.__init__(self)
 		StreamingOut.__init__(self)
 		self.parent = parent
 		self.controller_address = controller_address
 		self.remote_address = None
 		self.upgrade = upgrade
 		self.opened = opened
-		self.tag = tag
 		self.closing = False
 		self.value = None
 		self.codec = None
 		self.encoded_bytes = bytearray()
 		self.diffie_hellman = None
 		self.private_key = None
 		self.key_box = None
@@ -736,20 +723,20 @@
 
 def ControlChannel_ListenForStream(self, control, mr):
 	m, r = mr
 	requested_ipp = m.requested_ipp
 	try:
 		server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 	except socket.error as e:
-		self.send(NotListening(requested_ipp, e.errno, str(e), m.tag), r)
+		self.send(NotListening(requested_ipp, e.errno, str(e)), r)
 		return
 
 	def server_not_listening(e):
 		server.close()
-		self.send(NotListening(requested_ipp, e.errno, str(e), m.tag), r)
+		self.send(NotListening(requested_ipp, e.errno, str(e)), r)
 
 	try:
 		server.setblocking(False)
 		server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 		server.bind(requested_ipp.inet())
 		server.listen(5)
 	except socket.herror as e:
@@ -759,28 +746,28 @@
 		server_not_listening(e)
 		return
 	except socket.error as e:
 		server_not_listening(e)
 		return
 	except OverflowError as e:
 		server.close()
-		self.send(NotListening(requested_ipp, 0, str(e), m.tag), r)
+		self.send(NotListening(requested_ipp, 0, str(e)), r)
 		return
 
 	hap = server.getsockname()
 	listening_ipp=HostPort(hap[0], hap[1])
 
 	if m.encrypted:
 		self.trace(f'Listening (encrypted) on "{listening_ipp}", requested "{requested_ipp}"')
 	else:
 		self.trace(f'Listening on "{listening_ipp}", requested "{requested_ipp}"')
 
 	listening = Listening(requested_ipp=requested_ipp,
 		listening_ipp=listening_ipp,
-		tag=m.tag, encrypted=m.encrypted)
+		encrypted=m.encrypted)
 
 	self.networking[server] = TcpServer(server, m, listening, r, m.upgrade)
 	self.receiving.append(server)
 	self.faulting.append(server)
 
 	self.send(listening, r)
 
@@ -791,15 +778,15 @@
 	def ending(value, parent, address):
 		ar.send_a_message(Close(value), proxy, address)
 	return ending
 
 def open_stream(self, parent, s, opened):
 	controller_address = parent.controller_address
 
-	stream = TcpStream(parent, controller_address, parent.upgrade, opened, parent.request.tag)
+	stream = TcpStream(parent, controller_address, parent.upgrade, opened)
 	proxy_address = self.create(SocketProxy, s, self.channel, stream, object_ending=no_ending)
 
 	cs = parent.request.create_session
 	if cs:
 		# Create the ending function that swaps the Completed message to the parent for a
 		# Close message to the proxy.
 
@@ -818,29 +805,29 @@
 def ControlChannel_ConnectStream(self, control, mr):
 	m, r = mr
 	requested_ipp = m.requested_ipp
 	try:
 		client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 		client.setblocking(False)
 	except socket.error as e:
-		self.send(NotConnected(requested_ipp, e.errno, str(e), m.tag), r)
+		self.send(NotConnected(requested_ipp, e.errno, str(e)), r)
 		return
 
 	def client_not_connected(e):
 		client.close()
-		self.send(NotConnected(requested_ipp, e.errno, str(e), m.tag), r)
+		self.send(NotConnected(requested_ipp, e.errno, str(e)), r)
 
 	try:
 		e = client.connect_ex(requested_ipp.inet())
 		if e:
 			# Connect request cannot complete. Check for codes indicating
 			# async issue. If not it's a real error.
 			if e not in (errno.EINPROGRESS, errno.EWOULDBLOCK, errno.EAGAIN):
 				client.close()
-				self.send(NotConnected(requested_ipp, e, 'Connect incomplete and no pending indication.', m.tag), r)
+				self.send(NotConnected(requested_ipp, e, 'Connect incomplete and no pending indication.'), r)
 				return
 
 			# Build a transient "session" that just exists to catch
 			# an initial, either send or fault (a receive is treated
 			# as an error). True session is constructed on receiving
 			# a "normal" send event.
 			pending = TcpClient(client, m, None, r, m.upgrade, m.encrypted)
@@ -858,37 +845,36 @@
 		client_not_connected(e)
 		return
 	except socket.error as e:
 		client_not_connected(e)
 		return
 	except OverflowError as e:
 		client.close()
-		self.send(NotConnected(requested_ipp, 0, str(e), m.tag), r)
+		self.send(NotConnected(requested_ipp, 0, str(e)), r)
 		return
 
 	hap = client.getsockname()
 	connected_ipp = HostPort(hap[0], hap[1])
 
 	connected = Connected(requested_ipp=requested_ipp,
 		connected_ipp=connected_ipp,
-		opened_at=ar.world_now(),
-		tag=m.tag)
+		opened_at=ar.world_now())
 
 	parent = TcpClient(client, m, connected, r, m.upgrade, m.encrypted)
 	stream, proxy_address = open_stream(self, parent, client, connected)
 	connected.remote_address = proxy_address
 
 	self.networking[client] = stream
 	self.receiving.append(client)
 	self.sending.append(client)
 	self.faulting.append(client)
 
 	if m.encrypted:
 		self.trace(f'Connected (encrypted) to "{requested_ipp}", at local address "{connected_ipp}"')
-		not_connected = NotConnected(requested_ipp, None, None, m.tag)
+		not_connected = NotConnected(requested_ipp, None, None)
 		stream.diffie_hellman = (
 			(connected, r, stream.remote_address),
 			(not_connected, r))
 		# Start the exchange. Public key filled out during
 		# streaming.
 		self.send(Diffie(), proxy_address)
 		return
@@ -972,33 +958,33 @@
 
 def TcpServer_ReceiveBlock(self, server, s):
 	listening = server.listening
 	try:
 		accepted, hap = s.accept()
 		accepted.setblocking(False)
 	except socket.error as e:
-		self.send(NotAccepted(listening.requested_ipp, e.errno, str(e), listening.tag), server.controller_address)
+		self.send(NotAccepted(listening.requested_ipp, e.errno, str(e)), server.controller_address)
 		return
 
 	opened_at = ar.world_now()
 	stream, proxy_address = open_stream(self, server, accepted, None)
 	self.receiving.append(accepted)
 	self.sending.append(accepted)
 	self.faulting.append(accepted)
 
 	accepted_ipp = HostPort(hap[0], hap[1])
 
 	accepted = Accepted(listening_ipp=listening.listening_ipp,
 		accepted_ipp=accepted_ipp, remote_address=stream.remote_address,
-		opened_at=opened_at, tag=listening.tag)
+		opened_at=opened_at)
 	stream.opened = accepted
 
 	if listening.encrypted:
 		self.trace(f'Accepted (encrypted) "{accepted_ipp}", requested "{listening.listening_ipp}"')
-		not_accepted = NotAccepted(listening.requested_ipp, None, None, listening.tag)
+		not_accepted = NotAccepted(listening.requested_ipp, None, None)
 		stream.diffie_hellman = (
 			(accepted, server.controller_address, stream.remote_address),
 			(not_accepted, server.controller_address))
 		return
 	self.trace(f'Accepted "{accepted_ipp}", requested "{listening.listening_ipp}"')
 
 	self.forward(accepted, server.controller_address, stream.remote_address)
@@ -1022,39 +1008,37 @@
 	requested_ipp = request.requested_ipp
 
 	# CANNOT BUILD A STREAM AND IMMEDIATELY TEAR IT DOWN ON AN EXCEPTION.
 	# THIS WILL MAY CREATE A SESSION OBJECT WHEN THERE IS NO REMOTE AND MAY
 	# NEVER BE. DO IT AFTER A SUCCESSFUL RECV().
 	#connected = Connected(requested_ipp=request.requested_ipp,
 	#	connected_ipp=HostPort(hap[0], hap[1]),
-	#	opened_at=ar.world_now(),
-	#	tag=request.tag)
+	#	opened_at=ar.world_now())
 	#selector.connected = connected
 
 	#stream, proxy_address = open_stream(self, selector, client, connected.opened_at)
 	#connected.remote_address = proxy_address
 
 	try:
 		scrap = s.recv(TCP_RECV)
 
 		# No exception. New stream.
 		connected = Connected(requested_ipp=requested_ipp,
 			connected_ipp=connected_ipp,
-			opened_at=ar.world_now(),
-			tag=request.tag)
+			opened_at=ar.world_now())
 
 		selector.connected = connected
 		stream, proxy_address = open_stream(self, selector, client, connected)
 		connected.remote_address = proxy_address
 
 		self.trace(f'Connected to "{requested_ipp}", at local address "{connected_ipp}"')
 
 		if selector.encrypted:
 			self.trace(f'Connected (encrypted) to "{requested_ipp}", at local address "{connected_ipp}"')
-			not_connected = NotConnected(requested_ipp, None, None, request.tag)
+			not_connected = NotConnected(requested_ipp, None, None)
 			stream.diffie_hellman = (
 				(connected, stream.controller_address, stream.remote_address),
 				(not_connected, selector.controller_address))
 			self.send(Diffie(), proxy_address)
 			return
 		self.trace(f'Connected to "{requested_ipp}", at local address "{connected_ipp}"')
 
@@ -1071,17 +1055,17 @@
 		except (ar.CodecFailed, OverflowError, ValueError) as e:
 			value = ar.Faulted(condition='cannot stream inbound', explanation=str(e))
 			self.warning(str(value))
 			close_session(stream, value, s)
 		return
 
 	except socket.error as e:
-		self.send(NotConnected(request.requested_ipp, e.errno, str(e), request.tag), selector.controller_address)
+		self.send(NotConnected(request.requested_ipp, e.errno, str(e)), selector.controller_address)
 		self.clear(s, TcpClient)
-		#self.send(NotConnected(request.requested_ipp, e.errno, str(e), request.tag), stream.controller_address)
+		#self.send(NotConnected(request.requested_ipp, e.errno, str(e)), stream.controller_address)
 		#self.send(ar.Stop(), stream.remote_address)
 		#self.clear(s, TcpStream)
 		return
 
 def TcpClient_ReadyToSend(self, selector, s):
 	client = s
 	#self.sending.remove(client)
@@ -1089,39 +1073,38 @@
 	request = selector.request
 	hap = client.getsockname()
 	connected_ipp = HostPort(hap[0], hap[1])
 	requested_ipp = request.requested_ipp
 
 	connected = Connected(requested_ipp=requested_ipp,
 		connected_ipp=connected_ipp,
-		opened_at=ar.world_now(),
-		tag=request.tag)
+		opened_at=ar.world_now())
 	selector.connected = connected
 
 	stream, proxy_address = open_stream(self, selector, client, connected)
 	connected.remote_address = proxy_address
 	#receiving.append( client)
 	#self.faulting.append( client)
 
 	if selector.encrypted:
 		self.trace(f'Connected (encrypted) to "{requested_ipp}", at local address "{connected_ipp}"')
-		not_connected = NotConnected(requested_ipp, None, None, request.tag)
+		not_connected = NotConnected(requested_ipp, None, None)
 		stream.diffie_hellman = (
 			(connected, stream.controller_address, stream.remote_address),
 			(not_connected, selector.controller_address))
 		# Start the exchange of public keys.
 		self.send(Diffie(), proxy_address)
 		return
 	self.trace(f'Connected to "{requested_ipp}", at local address "{connected_ipp}"')
 
 	self.forward(connected, stream.controller_address, stream.remote_address)
 
 def TcpClient_BrokenTransport(self, selector, s):
 	text = 'fault on pending connect, unreachable, no service at that address or blocked'
-	self.send(NotConnected(selector.requested_ipp, 0, text, selector.tag), selector.controller_address)
+	self.send(NotConnected(selector.requested_ipp, 0, text), selector.controller_address)
 	self.clear(s, TcpClient)
 
 def close_session(stream, value, s):
 	stream.closing = True
 	stream.value = value
 	s.shutdown(socket.SHUT_RDWR)
 
@@ -1134,23 +1117,21 @@
 		ipp = None
 
 	if stream.closing:
 		c = Closed(value=stream.value,
 			reason=reason,
 			opened_ipp=ipp,
 			opened_at=stream.opened.opened_at,
-			closed_at=ar.world_now(),
-			tag=stream.tag)
+			closed_at=ar.world_now())
 		self.forward(c, stream.controller_address, stream.remote_address)
 	else:
 		self.send(ar.Stop(), stream.remote_address)
 		a = Abandoned(opened_ipp=ipp,
 			opened_at=stream.opened.opened_at,
-			closed_at=ar.world_now(),
-			tag=stream.tag)
+			closed_at=ar.world_now())
 		self.forward(a, stream.controller_address, stream.remote_address)
 	self.clear(s, TcpStream)
 
 def TcpStream_ReadyToSend(self, stream, s):
 	try:
 		if stream.send_a_block(s):
 			return
```

### Comparing `ansar_connect-0.1.216/src/ansar/connect/standard.py` & `ansar_connect-0.1.217/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/transporting.py` & `ansar_connect-0.1.217/src/ansar/connect/transporting.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,19 +40,19 @@
 	ts.channel.send(ar.Stop(), root.address)
 	root.select(ar.Completed)
 
 ar.AddOn(create_sockets, stop_sockets)
 
 #
 #
-def connect(self, requested_ipp, session=None, tag=None, encrypted=False):
-	ts.channel.send(ConnectStream(requested_ipp=requested_ipp, create_session=session, tag=tag, encrypted=encrypted), self.address)
+def connect(self, requested_ipp, session=None, encrypted=False):
+	ts.channel.send(ConnectStream(requested_ipp=requested_ipp, create_session=session, encrypted=encrypted), self.address)
 
 #
 #
-def listen(self, requested_ipp, session=None, tag=None, encrypted=False):
-	ts.channel.send(ListenForStream(requested_ipp=requested_ipp, create_session=session, tag=tag, encrypted=encrypted), self.address)
+def listen(self, requested_ipp, session=None, encrypted=False):
+	ts.channel.send(ListenForStream(requested_ipp=requested_ipp, create_session=session, encrypted=encrypted), self.address)
 
 #
 #
 def stop_listen(self, requested_ipp):
 	ts.channel.send(StopListening(requested_ipp), self.address)
```

### Comparing `ansar_connect-0.1.216/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.217/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar/connect/wan.py` & `ansar_connect-0.1.217/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.216/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.217/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.216
+Version: 0.1.217
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.216/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.217/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

