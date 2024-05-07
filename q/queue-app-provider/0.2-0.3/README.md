# Comparing `tmp/queue_app_provider-0.2.tar.gz` & `tmp/queue_app_provider-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue_app_provider-0.2.tar", last modified: Mon May  6 17:58:10 2024, max compression
+gzip compressed data, was "queue_app_provider-0.3.tar", last modified: Tue May  7 06:12:50 2024, max compression
```

## Comparing `queue_app_provider-0.2.tar` & `queue_app_provider-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidrodriguezalfayate   (501) staff       (20)        0 2024-05-06 17:58:10.812460 queue_app_provider-0.2/
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)      822 2024-05-06 17:58:10.812597 queue_app_provider-0.2/PKG-INFO
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1978 2023-06-05 14:48:05.799242 queue_app_provider-0.2/README
-drwxr-xr-x   0 davidrodriguezalfayate   (501) staff       (20)        0 2024-05-06 17:58:10.810747 queue_app_provider-0.2/queue_app_provider/
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     2937 2023-06-02 09:51:06.498136 queue_app_provider-0.2/queue_app_provider/AppProvider.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1967 2024-05-06 17:39:44.760644 queue_app_provider-0.2/queue_app_provider/HandlerOutput.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1440 2024-05-06 17:48:37.443999 queue_app_provider-0.2/queue_app_provider/InputEntry.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     2087 2024-05-06 17:31:07.272714 queue_app_provider-0.2/queue_app_provider/QueueThread.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)      189 2024-04-04 19:16:40.600584 queue_app_provider-0.2/queue_app_provider/__init__.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)       39 2024-04-04 19:22:08.004721 queue_app_provider-0.2/setup.cfg
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1686 2024-05-06 17:52:29.378428 queue_app_provider-0.2/setup.py
-drwxr-xr-x   0 davidrodriguezalfayate   (501) staff       (20)        0 2024-05-06 17:58:10.812394 queue_app_provider-0.2/test/
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     2485 2023-06-06 11:38:00.287220 queue_app_provider-0.2/test/test_AppProviderTest.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1468 2023-06-05 14:48:05.799708 queue_app_provider-0.2/test/test_HandlerOutputTest.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1346 2023-06-05 14:48:05.799807 queue_app_provider-0.2/test/test_InputEntryTest.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1386 2023-06-05 14:48:05.799872 queue_app_provider-0.2/test/test_QueueThreadTest.py
+drwxr-xr-x   0 davidrodriguezalfayate   (501) staff       (20)        0 2024-05-07 06:12:50.624200 queue_app_provider-0.3/
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)      822 2024-05-07 06:12:50.624342 queue_app_provider-0.3/PKG-INFO
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1978 2023-06-05 14:48:05.799242 queue_app_provider-0.3/README
+drwxr-xr-x   0 davidrodriguezalfayate   (501) staff       (20)        0 2024-05-07 06:12:50.622394 queue_app_provider-0.3/queue_app_provider/
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     3440 2024-05-07 06:08:54.162763 queue_app_provider-0.3/queue_app_provider/AppProvider.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     2077 2024-05-07 06:09:21.069385 queue_app_provider-0.3/queue_app_provider/HandlerOutput.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1475 2024-05-07 06:10:02.291969 queue_app_provider-0.3/queue_app_provider/InputEntry.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     2148 2024-05-07 06:10:23.492448 queue_app_provider-0.3/queue_app_provider/QueueThread.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)      189 2024-04-04 19:16:40.600584 queue_app_provider-0.3/queue_app_provider/__init__.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)       39 2024-04-04 19:22:08.004721 queue_app_provider-0.3/setup.cfg
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1676 2024-05-07 06:11:18.595899 queue_app_provider-0.3/setup.py
+drwxr-xr-x   0 davidrodriguezalfayate   (501) staff       (20)        0 2024-05-07 06:12:50.624122 queue_app_provider-0.3/test/
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     2485 2023-06-06 11:38:00.287220 queue_app_provider-0.3/test/test_AppProviderTest.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1468 2023-06-05 14:48:05.799708 queue_app_provider-0.3/test/test_HandlerOutputTest.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1346 2023-06-05 14:48:05.799807 queue_app_provider-0.3/test/test_InputEntryTest.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1386 2023-06-05 14:48:05.799872 queue_app_provider-0.3/test/test_QueueThreadTest.py
```

### Comparing `queue_app_provider-0.2/PKG-INFO` & `queue_app_provider-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: queue_app_provider
-Version: 0.2
+Version: 0.3
 Summary: Simple backend processor that receives binary data and stores it in a queue that its processed in a background thread.
 Home-page: https://github.com/drodriguezalfayate/flask-binary-queue/
 Author: David Rodriguez Alfayate
 Author-email: david.rodriguez.alfayate@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: QUEUE BACKGROUND PROCESSOR
```

### Comparing `queue_app_provider-0.2/README` & `queue_app_provider-0.3/README`

 * *Files identical despite different names*

### Comparing `queue_app_provider-0.2/queue_app_provider/AppProvider.py` & `queue_app_provider-0.3/queue_app_provider/AppProvider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import queue
 import signal
 import sys
 import threading
+import logging
 from typing import Callable
 
 from flask import Request
 from flask import abort
 
 from queue_app_provider.HandlerOutput import HandlerOutput
 from queue_app_provider.InputEntry import InputEntry
 from queue_app_provider.QueueThread import QueueThread
 
+logger = logging.getLogger('queue-app-provider:app-provider')
+
 
 # This is the main class and the one that should be used from the external flask app,
 # it can be configured using the handler (the processor from the input file), timeout
 # and accepted content-types for this AppProvider
 #
 # Created by: David Rodríguez Alfayate
 # Version: 1.0
@@ -51,20 +54,28 @@
     # Main processing of request, it verifies that input data is correctly defined, meaning
     # that a file and a callback url is provided, and check if content-type is valid
     # for the intended use-case. If demands are satisfied, a new InputEntry is created and
     # stored in queue.
     # When the request is properly processed we send requester - as soon as possible - a 204
     # if conditions are not satisfied, our response is just a simple 404.
     def process(self, request: Request):
+        logger.debug('New request from %s ', request.remote_addr)
         if 'file' not in request.files.keys() or 'callback' not in request.form.keys():
+            logger.debug('There is no file or callback input data')
             abort(404)
         file = request.files['file']
         callback = request.form['callback']
-        if not file.filename or not callback or not file.content_type in self.accepted_types:
+        if not file.filename or not callback:
+            logger.debug('File or callback are invalid, aborting')
+            abort(404)
+        if file.content_type not in self.accepted_types:
+            logger.debug('Input content-type %s is not allowed, aborting', file.content_type)
             abort(404)
 
         # We create the entry, enqueueing it properly
         entry = InputEntry(file, callback)
         self.queue.put_nowait(entry)
 
+        logger.debug('Initial processing is successful, enqueuing request for further analysis')
+
         # Just a no-content response is enough, we are not returning anything especially interesting indeed.
         return "", 204
```

### Comparing `queue_app_provider-0.2/queue_app_provider/HandlerOutput.py` & `queue_app_provider-0.3/queue_app_provider/HandlerOutput.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 import requests
 
-logger = logging.getLogger('HandlerOutput')
+logger = logging.getLogger('queue-app-provider:handler-output')
 
 
 # This class is a holder for all information regarding the processing
 # of a handler, a handler is the function accountable of working on
 # a image or binary data to create proper output.
 #
 # It's just a wrapper of a `success` a `text` or a `file` if the
@@ -35,14 +35,15 @@
                 return
             # On success, but a file
             if self.file:
                 logger.debug('Sending success file to % endpoint', callback)
                 requests.post(callback, json={"success": True}, files={'file': open(self.file, 'rb')})
                 return
             # Normal text
+            logger.debug('Sending success message %s to % endpoint', self.text, callback)
             requests.post(callback, json={"success": True, "data": self.text})
         except requests.exceptions.RequestException as e:
             # In a more complex scenario we should, perhaps, enqueue this callback response, expecting
             # than in the near future the remote server could be up again. For this simple example,
             # we are just ignoring the request, logging the error event
             logger.exception(e, exc_info=True)
             return
```

### Comparing `queue_app_provider-0.2/queue_app_provider/InputEntry.py` & `queue_app_provider-0.3/queue_app_provider/InputEntry.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,32 +13,33 @@
 # after that the local file is purged from system
 #
 # Created by: David Rodríguez Alfayate
 # Version: 1.0
 from queue_app_provider.HandlerOutput import HandlerOutput
 import logging
 
-logger = logging.getLogger('InputEntry')
+logger = logging.getLogger('queue-app-provider:input-entry')
 
 
 class InputEntry:
     def __init__(self, file_storage: FileStorage, callback):
         self.callback = callback
         self.fh, self.file = tempfile.mkstemp()
-        logger.debug('Storing temporary file in %s', self.file)
+        logger.debug('Storing temporary file in %r', self.file)
         file_storage.save(self.file)
 
     # Temporary file removal
     def clear(self):
         os.close(self.fh)
         os.remove(self.file)
 
     # Data processing function called from `QueueThread` main queue
     # we just execute the handler method
     def handle(self, handler: Callable[[str], HandlerOutput]):
-        # Generamos la salida de la clase, y tenemos con ella
-        # que enviar estos datos al sistema de procesado externo
+        # We process input, sending response to external
+        # processing system
         output = handler(self.file)
         try:
+            logger.debug('Handler result is %r', output)
             output.notify(self.callback)
         finally:
             self.clear()
```

### Comparing `queue_app_provider-0.2/queue_app_provider/QueueThread.py` & `queue_app_provider-0.3/queue_app_provider/QueueThread.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import logging
 import queue
 import threading
 
 
-# This is an independent queue processor thread, it just makes non blocking read
+# This is an independent queue processor thread, it just makes non-blocking read
 # on a queue and, process results using the handler input method.
 # Queue is stopped using provided event_handler
 #
 # Created by: David Rodríguez Alfayate
 # Version: 1.0
 from typing import Callable
 
 from queue_app_provider.HandlerOutput import HandlerOutput
-import logging
 
-logger = logging.getLogger('QueueThread')
+logger = logging.getLogger('queue-app-provider:queue-thread')
 
 
 class QueueThread(threading.Thread):
     def __init__(self, handler: Callable[[str], HandlerOutput], shared_queue: queue.Queue,
                  event_handler: threading.Event, timeout=30):
         threading.Thread.__init__(self)
         self.handler = handler
@@ -37,19 +36,20 @@
             # if it's set, processing is stopped and this thread "dies" gracefully
             global_break = False
             while not self.queue.empty():
                 if self.event_handler.is_set():
                     global_break = True
                     break
                 entry = self.queue.get_nowait()
+                logger.debug('Analyzing input entry')
                 entry.handle(self.handler)
 
             if global_break:
                 logger.debug("Breaking thread due to user interrupt")
                 break
 
-            # As stated above we wait til handler is set or timeout is exceded,
-            # if timeout is exceded we continue with normal workflow, that is
+            # As stated above we wait til handler is set or timeout is exceeded,
+            # if timeout is exceeded we continue with normal workflow, that is
             # run forever ;)
             if self.event_handler.wait(timeout=self.timeout):
                 logger.debug("Breaking thread due to user interrupt")
                 break
```

### Comparing `queue_app_provider-0.2/setup.py` & `queue_app_provider-0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from distutils.core import setup
 
 setup(
     name='queue_app_provider',  # How you named your package folder (MyLib)
     packages=['queue_app_provider'],  # Chose the same as "name"
-    version='0.2',  # Start with a small number and increase it with every change you make
+    version='0.3',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Simple backend processor that receives binary data and stores it in a queue that it''s processed in '
                 'a background thread.',  # Give a short description about your library
     author='David Rodriguez Alfayate',  # Type in your name
     author_email='david.rodriguez.alfayate@gmail.com',  # Type in your E-Mail
     url='https://github.com/drodriguezalfayate/flask-binary-queue/',  # Provide either the link to your github or to your website
     keywords=['QUEUE BACKGROUND PROCESSOR'],  # Keywords that define your package best
-    install_requires=[  # I get to this in a second
+    install_requires=[
         'flask',
         'requests',
+        'werkzeug'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',  # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',  # Again, pick a license
```

### Comparing `queue_app_provider-0.2/test/test_AppProviderTest.py` & `queue_app_provider-0.3/test/test_AppProviderTest.py`

 * *Files identical despite different names*

### Comparing `queue_app_provider-0.2/test/test_HandlerOutputTest.py` & `queue_app_provider-0.3/test/test_HandlerOutputTest.py`

 * *Files identical despite different names*

### Comparing `queue_app_provider-0.2/test/test_InputEntryTest.py` & `queue_app_provider-0.3/test/test_InputEntryTest.py`

 * *Files identical despite different names*

### Comparing `queue_app_provider-0.2/test/test_QueueThreadTest.py` & `queue_app_provider-0.3/test/test_QueueThreadTest.py`

 * *Files identical despite different names*

