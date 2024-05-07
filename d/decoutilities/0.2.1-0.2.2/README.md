# Comparing `tmp/decoutilities-0.2.1.tar.gz` & `tmp/decoutilities-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.2.1.tar", last modified: Mon May  6 07:13:56 2024, max compression
+gzip compressed data, was "decoutilities-0.2.2.tar", last modified: Tue May  7 13:01:33 2024, max compression
```

## Comparing `decoutilities-0.2.1.tar` & `decoutilities-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 07:13:56.443682 decoutilities-0.2.1/
--rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     9043 2024-05-06 07:13:56.427681 decoutilities-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     8572 2024-04-30 13:10:29.000000 decoutilities-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 07:13:56.137611 decoutilities-0.2.1/decoutilities/
--rw-rw-rw-   0        0        0     4791 2024-05-06 07:06:49.000000 decoutilities-0.2.1/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:13:56.327106 decoutilities-0.2.1/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.1/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.1/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.1/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:13:56.398679 decoutilities-0.2.1/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.1/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      483 2024-04-29 13:14:09.000000 decoutilities-0.2.1/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:13:56.409681 decoutilities-0.2.1/decoutilities.egg-info/
--rw-rw-rw-   0        0        0     9043 2024-05-06 07:13:55.000000 decoutilities-0.2.1/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2024-05-06 07:13:55.000000 decoutilities-0.2.1/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 07:13:55.000000 decoutilities-0.2.1/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-06 07:13:55.000000 decoutilities-0.2.1/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 07:13:56.443682 decoutilities-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-06 07:09:43.000000 decoutilities-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:01:33.076781 decoutilities-0.2.2/
+-rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    10146 2024-05-07 13:01:33.054928 decoutilities-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9675 2024-05-07 12:58:21.000000 decoutilities-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 13:01:32.721167 decoutilities-0.2.2/decoutilities/
+-rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.2.2/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:01:32.879109 decoutilities-0.2.2/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.2/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.2/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.2/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:01:32.931755 decoutilities-0.2.2/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.2/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      483 2024-04-29 13:14:09.000000 decoutilities-0.2.2/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:01:32.978442 decoutilities-0.2.2/decoutilities/queue/
+-rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.2.2/decoutilities/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:01:33.014202 decoutilities-0.2.2/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0    10146 2024-05-07 13:01:32.000000 decoutilities-0.2.2/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2024-05-07 13:01:32.000000 decoutilities-0.2.2/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 13:01:32.000000 decoutilities-0.2.2/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-07 13:01:32.000000 decoutilities-0.2.2/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 13:01:33.076781 decoutilities-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-07 13:00:25.000000 decoutilities-0.2.2/setup.py
```

### Comparing `decoutilities-0.2.1/LICENSE` & `decoutilities-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.1/PKG-INFO` & `decoutilities-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.1
+Version: 0.2.2
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -298,14 +298,48 @@
 # Use the injector to get the function
 greet_func = injector_instance.inject('greet')
 
 # Call the function
 print(greet_func('World'))  # Outputs: Hello, World!
 ```
 
+### Queue
+
+The `Queue` class provides a simple implementation of a queue data structure. It also logs every action performed on the queue.
+
+```python
+from decoutilities.queue import Queue
+
+# Create a Queue instance
+queue = Queue()
+
+# Add an item to the queue
+queue.add_item('item1')
+
+# Remove an item from the queue
+removed_item = queue.remove_item()
+
+# Check the first item in the queue without removing it
+first_item = queue.check_item()
+
+# Clear the queue
+queue.clear_queue()
+
+# Print the log of actions performed on the queue
+queue.print_log()
+```
+
+#### Methods
+
+- `add_item(item)`: Adds an item to the end of the queue.
+- `remove_item()`: Removes and returns the first item in the queue. If the queue is empty, it returns `None`.
+- `check_item()`: Returns the first item in the queue without removing it. If the queue is empty, it returns `None`.
+- `clear_queue()`: Clears all items from the queue.
+- `print_log()`: Prints the log of actions performed on the queue. Each log entry includes the timestamp, action, item, and the size of the queue after the action.
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
```

### Comparing `decoutilities-0.2.1/README.md` & `decoutilities-0.2.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -285,14 +285,48 @@
 # Use the injector to get the function
 greet_func = injector_instance.inject('greet')
 
 # Call the function
 print(greet_func('World'))  # Outputs: Hello, World!
 ```
 
+### Queue
+
+The `Queue` class provides a simple implementation of a queue data structure. It also logs every action performed on the queue.
+
+```python
+from decoutilities.queue import Queue
+
+# Create a Queue instance
+queue = Queue()
+
+# Add an item to the queue
+queue.add_item('item1')
+
+# Remove an item from the queue
+removed_item = queue.remove_item()
+
+# Check the first item in the queue without removing it
+first_item = queue.check_item()
+
+# Clear the queue
+queue.clear_queue()
+
+# Print the log of actions performed on the queue
+queue.print_log()
+```
+
+#### Methods
+
+- `add_item(item)`: Adds an item to the end of the queue.
+- `remove_item()`: Removes and returns the first item in the queue. If the queue is empty, it returns `None`.
+- `check_item()`: Returns the first item in the queue without removing it. If the queue is empty, it returns `None`.
+- `clear_queue()`: Clears all items from the queue.
+- `print_log()`: Prints the log of actions performed on the queue. Each log entry includes the timestamp, action, item, and the size of the queue after the action.
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
```

### Comparing `decoutilities-0.2.1/decoutilities/__init__.py` & `decoutilities-0.2.2/decoutilities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,26 +58,24 @@
         return wrapper
     return decorator
 
 # @deprecated
 # Mark a function as deprecated and print a log when its used for the first time, also raise a warning and show in the editor as a warning.
 def deprecated(func):
     import warnings
-    import inspect
 
     def wrapper(*args, **kwargs):
         warnings.warn(f"Function {func.__name__} is deprecated and will be removed in the future.", DeprecationWarning, stacklevel=2)
         return func(*args, **kwargs)
     return wrapper
 
 # @experimental
 # Mark a function as experimental and print a log when its used for the first time, also raise a warning and show in the editor as a warning.
 def experimental(func):
     import warnings
-    import inspect
 
     def wrapper(*args, **kwargs):
         warnings.warn(f"Function {func.__name__} is experimental and may not work as expected.", UserWarning, stacklevel=2)
         return func(*args, **kwargs)
     return wrapper
 
 # @notnull
@@ -100,21 +98,19 @@
             time.sleep(seconds)
             return func(*args, **kwargs)
         return wrapper
     return decorator
 
 # @timeout(seconds)
 # Timeout a function after a number of seconds.
-from threading import Thread
-import time
-
 class TimeoutException(Exception):
     pass
 
 def timeout(seconds):
+    from threading import Thread
     def decorator(func):
         def wrapper(*args, **kwargs):
             res = [TimeoutException('Function timed out!')]
             def target():
                 try:
                     res[0] = func(*args, **kwargs)
                 except Exception as e:
```

### Comparing `decoutilities-0.2.1/decoutilities/config/config.py` & `decoutilities-0.2.2/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.1/decoutilities/config/configContainer.py` & `decoutilities-0.2.2/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.1/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.2.2/decoutilities.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.1
+Version: 0.2.2
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -298,14 +298,48 @@
 # Use the injector to get the function
 greet_func = injector_instance.inject('greet')
 
 # Call the function
 print(greet_func('World'))  # Outputs: Hello, World!
 ```
 
+### Queue
+
+The `Queue` class provides a simple implementation of a queue data structure. It also logs every action performed on the queue.
+
+```python
+from decoutilities.queue import Queue
+
+# Create a Queue instance
+queue = Queue()
+
+# Add an item to the queue
+queue.add_item('item1')
+
+# Remove an item from the queue
+removed_item = queue.remove_item()
+
+# Check the first item in the queue without removing it
+first_item = queue.check_item()
+
+# Clear the queue
+queue.clear_queue()
+
+# Print the log of actions performed on the queue
+queue.print_log()
+```
+
+#### Methods
+
+- `add_item(item)`: Adds an item to the end of the queue.
+- `remove_item()`: Removes and returns the first item in the queue. If the queue is empty, it returns `None`.
+- `check_item()`: Returns the first item in the queue without removing it. If the queue is empty, it returns `None`.
+- `clear_queue()`: Clears all items from the queue.
+- `print_log()`: Prints the log of actions performed on the queue. Each log entry includes the timestamp, action, item, and the size of the queue after the action.
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
```

### Comparing `decoutilities-0.2.1/setup.py` & `decoutilities-0.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.2.1',
+version='0.2.2',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

