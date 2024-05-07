# Comparing `tmp/selftest-0.4.0.tar.gz` & `tmp/selftest-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selftest-0.4.0.tar", last modified: Wed Sep 20 13:12:27 2023, max compression
+gzip compressed data, was "selftest-0.4.1.tar", last modified: Tue May  7 17:57:07 2024, max compression
```

## Comparing `selftest-0.4.0.tar` & `selftest-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:12:27.985133 selftest-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-09-20 13:12:18.000000 selftest-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-20 13:12:18.000000 selftest-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23023 2023-09-20 13:12:27.985133 selftest-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22405 2023-09-20 13:12:18.000000 selftest-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:12:27.985133 selftest-0.4.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2023-09-20 13:12:18.000000 selftest-0.4.0/bin/selftest
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:12:27.985133 selftest-0.4.0/selftest/
--rwxr-xr-x   0 runner    (1001) docker     (127)    16098 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5806 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/asyncer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/binder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/diffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20045 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/integrationtests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/prrint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15460 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:12:27.985133 selftest-0.4.0/selftest/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/tests/sub_module_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/tests/sub_module_ok.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/tests/temporary_class_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/tests/tryout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/tests/tryout2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-09-20 13:12:18.000000 selftest-0.4.0/selftest/wildcard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 13:12:27.985133 selftest-0.4.0/selftest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23023 2023-09-20 13:12:27.000000 selftest-0.4.0/selftest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-09-20 13:12:27.000000 selftest-0.4.0/selftest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-20 13:12:27.000000 selftest-0.4.0/selftest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-20 13:12:27.000000 selftest-0.4.0/selftest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-20 13:12:27.985133 selftest-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2023-09-20 13:12:18.000000 selftest-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:57:07.463199 selftest-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 17:57:01.000000 selftest-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 17:57:01.000000 selftest-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23375 2024-05-07 17:57:07.463199 selftest-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22744 2024-05-07 17:57:01.000000 selftest-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:57:07.459200 selftest-0.4.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-05-07 17:57:01.000000 selftest-0.4.1/bin/selftest
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:57:07.463199 selftest-0.4.1/selftest/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16098 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/asyncer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/binder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/diffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20045 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/integrationtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/prrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15460 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:57:07.463199 selftest-0.4.1/selftest/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/tests/sub_module_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/tests/sub_module_ok.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/tests/temporary_class_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/tests/tryout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/tests/tryout2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-07 17:57:01.000000 selftest-0.4.1/selftest/wildcard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:57:07.463199 selftest-0.4.1/selftest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23375 2024-05-07 17:57:07.000000 selftest-0.4.1/selftest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-07 17:57:07.000000 selftest-0.4.1/selftest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:57:07.000000 selftest-0.4.1/selftest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 17:57:07.000000 selftest-0.4.1/selftest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:57:07.463199 selftest-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-07 17:57:01.000000 selftest-0.4.1/setup.py
```

### Comparing `selftest-0.4.0/LICENSE` & `selftest-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/PKG-INFO` & `selftest-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: selftest
-Version: 0.4.0
-Summary: Python Testing Library
-Home-page: https://github.com/seecr/selftest
+Version: 0.4.1
+Summary: Python In-Source Testing Library
+Home-page: https://github.com/ejgroene/selftest
 Author: Erik Groeneveld
 Author-email: erik@seecr.nl
 Maintainer: Thijs Janssen
 Maintainer-email: thijs@seecr.nl
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Software Development :: Testing
@@ -15,14 +15,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://github.com/seecr/selftest/actions/workflows/python-package.yml/badge.svg
    :alt: Python Package Check
 
+.. image:: https://img.shields.io/badge/created_by-seecr-orange
+   :alt: Created by Seecr
+
 ========
 Selftest
 ========
 
 1. Introduction
 ===============
 
@@ -33,20 +36,26 @@
 
 - tests are *ordinary functions*, anywhere in the application code,
 - gathering and running tests is *automatic* and follows the structure of your code,
 - testing *stops on first failure* with a standard Python stack trace,
 
 The benefit of this approach are:
 
-- there is no seprate test tree to maintain,
+- there is no separate test tree to maintain,
 - dependencies are automatically tested,
 - quicker cycles, more focus.
 
 The core is extremely small and support for `async`, `filters`, `operators`, `fixtures`, `diffs`, `wildcards`, `guards`, etc are all implemented in `hooks`.
 
+In-source testing
+-----------------
+Selttest runs tests within the source code alongside the implementation, similar to Rust's module tests and Vitest in-source testing.
+
+This makes the tests share closure with the implementation and enables it to test against private state without exporting. Meanwhile, it also brings a closer feedback loop for development.
+
 
 History
 -------
 Selftest began, as a recalcitrant move away from the frameworks, with the following decorator above my tests:
 
 .. code:: python
 
@@ -59,21 +68,19 @@
 
   @test                                   # marks and runs the test
   def a_test():
       assert 42 == i_need_testing(42)
 
 It would just run the test every time I imported it. That turned out to work so well that it grew out to what we have here today.
 
-Selftest was first named Autotest, due to conflicting names in the Python Package Index it was renamed to Selftest.
-
 
 Features
 --------
 
-Meanwhile autotest gained some features. It
+Meanwhile selftest gained some features. It
 
 #) works in a familiar *Pythonic* way, no magic,
 #) has one simple *API* via the test object,
 #) is based on *standard modules* operator, pdb, logger, difflib, inspect, etc,
 #) seamlessly scales from *microtests* to *systemtests*,
 #) discovers tests automatically through the *importing mechanism*,
 #) crosses module, package and project boundaries easily,
@@ -83,39 +90,39 @@
 #) supports *levels*: unit, integration, performance etc.,
 #) there are *fixtures* (context managers) like in other test tools,
 #) *async tests and fixtures* are fully supported,
 #) most functionality is in *hooks* which you can extend easily,
 #) there is a *root* tester which can have *subtesters*,
 #) output is send to a *logger*.
 
-Although autotest promotes an agile, rigorous and Pythonic way of testing, since there is little magic and tests are just functions, you are free to organise them as you wish. You can even do it the Python unittest way, if you want.
+Although selftest promotes an agile, rigorous and Pythonic way of testing, since there is little magic and tests are just functions, you are free to organise them as you wish. You can even do it the Python unittest way, if you want.
 
 
 
 An example
 ----------
 
 Selftest has a global root tester that can have an arbitrarily deep and wide tree of child testers. A typical module uses it as follows:
 
 .. code:: python
 
-    import autotest
-    test = autotest.get_tester(__name__)
+    import selftest
+    test = selftest.get_tester(__name__)
 
     def area(w, h):
         return w * h
 
     @test
     def area_basics():
         assert 9 == area(3, 3)
         assert 6 == area(2, 3)
 
-Its creates a subtester using ``get_tester()``. The resulting tester object is the main access point to all functionality of autotest.  In this case, it is used as a decorator to mark and execute a test function.
+Its creates a subtester using ``get_tester()``. The resulting tester object is the main access point to all functionality of selftest.  In this case, it is used as a decorator to mark and execute a test function.
 
-More on assert later.
+More on ``assert`` later.
 
 
 
 2. Basic API
 ============
 
 General
@@ -150,29 +157,29 @@
 - hooks API.
 - APIs introduced by hooks
 
 
 Module Level API
 ----------------
 
-The autotest core consist of two module level functions:
+The selftest core consist of two module level functions:
 
 
 ``basic_config(**options)``
 
 Sets options for the root tester. This can be called only once, before ``get_tester()``. If not called, default options are used. This typicalliy happens in the main of an application or in a program for running tests.
 
 
 ``get_tester(name=None)``
 
 When name is ``None`` returns the root tester. Otherwise it returns a named child of the root.  Name is a potentially hierarchical name separated by dots. Each level in this hierarchy becomes a child of the one preceding it. The last tester object is returned. Thus, ``get_tester("main.sub")`` creates a child ``main`` of the root and a child ``sub`` of the child ``main``. It returns the latter.
 
 Testers created this way become globally available. A call to ``get_tester()`` with the same name repeatedly will return the same tester.
 
-Recommended is to use ``test = get_tester(__name__)`` at the start of your module. Using subtesters is a powerful way of organising tests. See the source code of autotest for many examples.
+Recommended is to use ``test = get_tester(__name__)`` at the start of your module. Using subtesters is a powerful way of organising tests. See the source code of selftest for many examples.
 
 
 Tester Objects API
 ------------------
 
 A tester object as returned from ``get_tester()`` support the following methods:
 
@@ -226,15 +233,15 @@
 
 ``child(**options)``
 
 This creates a child and returns a context manager.
 
 .. code:: python
 
-   test = autotest.get_tester(__name__)
+   test = selftest.get_tester(__name__)
    with test.child(level=CRITICAL) as crit:
        @crit
        def a_critical_test_function():
            pass
 
 
 ``fail(*args, **kwargs)``
@@ -265,15 +272,15 @@
 ==========  =======  =======   ==========================================================
 keep        boolean  False     Keep the function instead of discarding it.
 run         boolean  True      Run immediately.
 hooks       list     []        List of hooks that are invoked in order.
 subprocess  boolean  False     Runs test when inside a subprocess.
 ==========  =======  =======   ==========================================================
 
-Normally, autotest runs a test as soon as it discovers it and then discards it. The example below show how tests can be run later by keeping and invoking them.
+Normally, selftest runs a test as soon as it discovers it and then discards it. The example below show how tests can be run later by keeping and invoking them.
 
 .. code:: python
 
   @test
   def this_test_runs_immediately():
     pass
 
@@ -385,22 +392,22 @@
     @test
     def another_test():
         test.all(x > 1 for x in [1,2,3])      # use builtin all()
         test.startswith("rumbush", "rum")     # use method of first argument
 
 When the given operator returns ``False`` according to ``bool()`` it raises ``AssertionError`` with the actual values of the arguments.
 
-This shows how autotest stays close to Python as we know it. It does nothing more than looking up the given attribute in four places:
+This shows how selftest stays close to Python as we know it. It does nothing more than looking up the given attribute in four places:
 
 #) module ``operator``, e.g.: ``test.gt(2, 1)``,
 #) module ``builtins``, e.g.: ``test.isinstance('aa', str)``,
 #) module ``inspect``, e.g.: ``test.isfunction(len)``,
 #) the first argument, e.g.: ``test.isupper("ABC")``.
 
-The benefits of this is that we do not have to learn new methods, that the assert functions are not limited, and that autotest can print the arguments for us on failure.
+The benefits of this is that we do not have to learn new methods, that the assert functions are not limited, and that selftest can print the arguments for us on failure.
 
 **diff**
 
 All operators obtained this way support a keyword ``diff=<function>`` that, when present, is invoked with the actual arguments. The result is then given to the ``AssertionError`` instead of the actual arguments.
 
 .. code:: python
 
@@ -624,44 +631,44 @@
 
   $ python <mymodule.py>
   $ python -c "import mymodule"
 
 When you only want to develop a submodule, just ``cd`` down into that directory and do the same. Only the tests of that submodule (and everything in imports) will be tested.
 
 
-The methode above just prints crude messages and has no way to use options. For that use the main that comes with autotest:
+The methode above just prints crude messages and has no way to use options. For that use the main that comes with selftest:
 
 .. code:: bash
 
-  $ autotest --help
-  Usage: autotest [options] module
+  $ selftest --help
+  Usage: selftest [options] module
 
   Options:
     -h, --help            show this help message and exit
     -f FILTER, --filter=FILTER
                         only run tests whose qualified name contains FILTER
     -t , --threshold=THRESHOLD
                         only run tests whose level is >= THRESHOLD
 
 
 For example to run your tests but not the imported ones from other packages:
 
 .. code:: bash
 
-  $ autotest --filter mymodule mymodule
+  $ selftest --filter mymodule mymodule
 
 
-If you want to run the tests for autotests itself, go to the autotest project directory and use:
+If you want to run the tests for selftest itself, go to the selftest project directory and use:
 
 .. code:: bash
 
-  $ python -c "import autotest"  autotest.selftest
+  $ python -c "import selftest"  selftest.selftest
 
-The argument ``autotest.selftest`` lets autotest run its own tests, which are normally skipped.
-Also, this avoids using the autotest main program because it is not guaranteed that an installed old version of autotest can run its own test from the future.
+The argument ``selftest.selftest`` lets selftest run its own tests, which are normally skipped.
+Also, this avoids using the selftest main program because it is not guaranteed that an installed old version of selftest can run its own test from the future.
 
 
 **Production**
 
 During production, all tests are automatically run during startup when all needed modules are imported. If an the application configures a specific root, for example by calling ``logging.basicConfig()``, the tests will automatically log there. Alternatively, you can setup a separate ``Logger`` for running tests. See Core API.
 
 You can als filter tests or run tests for a specific level only. Or suppress them all. See the source code of ``__main__.py`` for ideas.
```

### Comparing `selftest-0.4.0/README.rst` & `selftest-0.4.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 .. image:: https://github.com/seecr/selftest/actions/workflows/python-package.yml/badge.svg
    :alt: Python Package Check
 
+.. image:: https://img.shields.io/badge/created_by-seecr-orange
+   :alt: Created by Seecr
+
 ========
 Selftest
 ========
 
 1. Introduction
 ===============
 
@@ -15,20 +18,26 @@
 
 - tests are *ordinary functions*, anywhere in the application code,
 - gathering and running tests is *automatic* and follows the structure of your code,
 - testing *stops on first failure* with a standard Python stack trace,
 
 The benefit of this approach are:
 
-- there is no seprate test tree to maintain,
+- there is no separate test tree to maintain,
 - dependencies are automatically tested,
 - quicker cycles, more focus.
 
 The core is extremely small and support for `async`, `filters`, `operators`, `fixtures`, `diffs`, `wildcards`, `guards`, etc are all implemented in `hooks`.
 
+In-source testing
+-----------------
+Selttest runs tests within the source code alongside the implementation, similar to Rust's module tests and Vitest in-source testing.
+
+This makes the tests share closure with the implementation and enables it to test against private state without exporting. Meanwhile, it also brings a closer feedback loop for development.
+
 
 History
 -------
 Selftest began, as a recalcitrant move away from the frameworks, with the following decorator above my tests:
 
 .. code:: python
 
@@ -41,21 +50,19 @@
 
   @test                                   # marks and runs the test
   def a_test():
       assert 42 == i_need_testing(42)
 
 It would just run the test every time I imported it. That turned out to work so well that it grew out to what we have here today.
 
-Selftest was first named Autotest, due to conflicting names in the Python Package Index it was renamed to Selftest.
-
 
 Features
 --------
 
-Meanwhile autotest gained some features. It
+Meanwhile selftest gained some features. It
 
 #) works in a familiar *Pythonic* way, no magic,
 #) has one simple *API* via the test object,
 #) is based on *standard modules* operator, pdb, logger, difflib, inspect, etc,
 #) seamlessly scales from *microtests* to *systemtests*,
 #) discovers tests automatically through the *importing mechanism*,
 #) crosses module, package and project boundaries easily,
@@ -65,39 +72,39 @@
 #) supports *levels*: unit, integration, performance etc.,
 #) there are *fixtures* (context managers) like in other test tools,
 #) *async tests and fixtures* are fully supported,
 #) most functionality is in *hooks* which you can extend easily,
 #) there is a *root* tester which can have *subtesters*,
 #) output is send to a *logger*.
 
-Although autotest promotes an agile, rigorous and Pythonic way of testing, since there is little magic and tests are just functions, you are free to organise them as you wish. You can even do it the Python unittest way, if you want.
+Although selftest promotes an agile, rigorous and Pythonic way of testing, since there is little magic and tests are just functions, you are free to organise them as you wish. You can even do it the Python unittest way, if you want.
 
 
 
 An example
 ----------
 
 Selftest has a global root tester that can have an arbitrarily deep and wide tree of child testers. A typical module uses it as follows:
 
 .. code:: python
 
-    import autotest
-    test = autotest.get_tester(__name__)
+    import selftest
+    test = selftest.get_tester(__name__)
 
     def area(w, h):
         return w * h
 
     @test
     def area_basics():
         assert 9 == area(3, 3)
         assert 6 == area(2, 3)
 
-Its creates a subtester using ``get_tester()``. The resulting tester object is the main access point to all functionality of autotest.  In this case, it is used as a decorator to mark and execute a test function.
+Its creates a subtester using ``get_tester()``. The resulting tester object is the main access point to all functionality of selftest.  In this case, it is used as a decorator to mark and execute a test function.
 
-More on assert later.
+More on ``assert`` later.
 
 
 
 2. Basic API
 ============
 
 General
@@ -132,29 +139,29 @@
 - hooks API.
 - APIs introduced by hooks
 
 
 Module Level API
 ----------------
 
-The autotest core consist of two module level functions:
+The selftest core consist of two module level functions:
 
 
 ``basic_config(**options)``
 
 Sets options for the root tester. This can be called only once, before ``get_tester()``. If not called, default options are used. This typicalliy happens in the main of an application or in a program for running tests.
 
 
 ``get_tester(name=None)``
 
 When name is ``None`` returns the root tester. Otherwise it returns a named child of the root.  Name is a potentially hierarchical name separated by dots. Each level in this hierarchy becomes a child of the one preceding it. The last tester object is returned. Thus, ``get_tester("main.sub")`` creates a child ``main`` of the root and a child ``sub`` of the child ``main``. It returns the latter.
 
 Testers created this way become globally available. A call to ``get_tester()`` with the same name repeatedly will return the same tester.
 
-Recommended is to use ``test = get_tester(__name__)`` at the start of your module. Using subtesters is a powerful way of organising tests. See the source code of autotest for many examples.
+Recommended is to use ``test = get_tester(__name__)`` at the start of your module. Using subtesters is a powerful way of organising tests. See the source code of selftest for many examples.
 
 
 Tester Objects API
 ------------------
 
 A tester object as returned from ``get_tester()`` support the following methods:
 
@@ -208,15 +215,15 @@
 
 ``child(**options)``
 
 This creates a child and returns a context manager.
 
 .. code:: python
 
-   test = autotest.get_tester(__name__)
+   test = selftest.get_tester(__name__)
    with test.child(level=CRITICAL) as crit:
        @crit
        def a_critical_test_function():
            pass
 
 
 ``fail(*args, **kwargs)``
@@ -247,15 +254,15 @@
 ==========  =======  =======   ==========================================================
 keep        boolean  False     Keep the function instead of discarding it.
 run         boolean  True      Run immediately.
 hooks       list     []        List of hooks that are invoked in order.
 subprocess  boolean  False     Runs test when inside a subprocess.
 ==========  =======  =======   ==========================================================
 
-Normally, autotest runs a test as soon as it discovers it and then discards it. The example below show how tests can be run later by keeping and invoking them.
+Normally, selftest runs a test as soon as it discovers it and then discards it. The example below show how tests can be run later by keeping and invoking them.
 
 .. code:: python
 
   @test
   def this_test_runs_immediately():
     pass
 
@@ -367,22 +374,22 @@
     @test
     def another_test():
         test.all(x > 1 for x in [1,2,3])      # use builtin all()
         test.startswith("rumbush", "rum")     # use method of first argument
 
 When the given operator returns ``False`` according to ``bool()`` it raises ``AssertionError`` with the actual values of the arguments.
 
-This shows how autotest stays close to Python as we know it. It does nothing more than looking up the given attribute in four places:
+This shows how selftest stays close to Python as we know it. It does nothing more than looking up the given attribute in four places:
 
 #) module ``operator``, e.g.: ``test.gt(2, 1)``,
 #) module ``builtins``, e.g.: ``test.isinstance('aa', str)``,
 #) module ``inspect``, e.g.: ``test.isfunction(len)``,
 #) the first argument, e.g.: ``test.isupper("ABC")``.
 
-The benefits of this is that we do not have to learn new methods, that the assert functions are not limited, and that autotest can print the arguments for us on failure.
+The benefits of this is that we do not have to learn new methods, that the assert functions are not limited, and that selftest can print the arguments for us on failure.
 
 **diff**
 
 All operators obtained this way support a keyword ``diff=<function>`` that, when present, is invoked with the actual arguments. The result is then given to the ``AssertionError`` instead of the actual arguments.
 
 .. code:: python
 
@@ -606,44 +613,44 @@
 
   $ python <mymodule.py>
   $ python -c "import mymodule"
 
 When you only want to develop a submodule, just ``cd`` down into that directory and do the same. Only the tests of that submodule (and everything in imports) will be tested.
 
 
-The methode above just prints crude messages and has no way to use options. For that use the main that comes with autotest:
+The methode above just prints crude messages and has no way to use options. For that use the main that comes with selftest:
 
 .. code:: bash
 
-  $ autotest --help
-  Usage: autotest [options] module
+  $ selftest --help
+  Usage: selftest [options] module
 
   Options:
     -h, --help            show this help message and exit
     -f FILTER, --filter=FILTER
                         only run tests whose qualified name contains FILTER
     -t , --threshold=THRESHOLD
                         only run tests whose level is >= THRESHOLD
 
 
 For example to run your tests but not the imported ones from other packages:
 
 .. code:: bash
 
-  $ autotest --filter mymodule mymodule
+  $ selftest --filter mymodule mymodule
 
 
-If you want to run the tests for autotests itself, go to the autotest project directory and use:
+If you want to run the tests for selftest itself, go to the selftest project directory and use:
 
 .. code:: bash
 
-  $ python -c "import autotest"  autotest.selftest
+  $ python -c "import selftest"  selftest.selftest
 
-The argument ``autotest.selftest`` lets autotest run its own tests, which are normally skipped.
-Also, this avoids using the autotest main program because it is not guaranteed that an installed old version of autotest can run its own test from the future.
+The argument ``selftest.selftest`` lets selftest run its own tests, which are normally skipped.
+Also, this avoids using the selftest main program because it is not guaranteed that an installed old version of selftest can run its own test from the future.
 
 
 **Production**
 
 During production, all tests are automatically run during startup when all needed modules are imported. If an the application configures a specific root, for example by calling ``logging.basicConfig()``, the tests will automatically log there. Alternatively, you can setup a separate ``Logger`` for running tests. See Core API.
 
 You can als filter tests or run tests for a specific level only. Or suppress them all. See the source code of ``__main__.py`` for ideas.
```

### Comparing `selftest-0.4.0/bin/selftest` & `selftest-0.4.1/bin/selftest`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/__init__.py` & `selftest-0.4.1/selftest/__init__.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/__main__.py` & `selftest-0.4.1/selftest/__main__.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/asyncer.py` & `selftest-0.4.1/selftest/asyncer.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/binder.py` & `selftest-0.4.1/selftest/binder.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/diffs.py` & `selftest-0.4.1/selftest/diffs.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/filter.py` & `selftest-0.4.1/selftest/filter.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/fixtures.py` & `selftest-0.4.1/selftest/fixtures.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/integrationtests.py` & `selftest-0.4.1/selftest/integrationtests.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/levels.py` & `selftest-0.4.1/selftest/levels.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/mocks.py` & `selftest-0.4.1/selftest/mocks.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/operators.py` & `selftest-0.4.1/selftest/operators.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/prrint.py` & `selftest-0.4.1/selftest/prrint.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/tester.py` & `selftest-0.4.1/selftest/tester.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/tests/__init__.py` & `selftest-0.4.1/selftest/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/tests/sub_module_fail.py` & `selftest-0.4.1/selftest/tests/sub_module_fail.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/tests/sub_module_ok.py` & `selftest-0.4.1/selftest/tests/sub_module_ok.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/tests/temporary_class_namespace.py` & `selftest-0.4.1/selftest/tests/temporary_class_namespace.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/tests/tryout.py` & `selftest-0.4.1/selftest/tests/tryout.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/tests/tryout2.py` & `selftest-0.4.1/selftest/tests/tryout2.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/utils.py` & `selftest-0.4.1/selftest/utils.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest/wildcard.py` & `selftest-0.4.1/selftest/wildcard.py`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/selftest.egg-info/PKG-INFO` & `selftest-0.4.1/selftest.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: selftest
-Version: 0.4.0
-Summary: Python Testing Library
-Home-page: https://github.com/seecr/selftest
+Version: 0.4.1
+Summary: Python In-Source Testing Library
+Home-page: https://github.com/ejgroene/selftest
 Author: Erik Groeneveld
 Author-email: erik@seecr.nl
 Maintainer: Thijs Janssen
 Maintainer-email: thijs@seecr.nl
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Software Development :: Testing
@@ -15,14 +15,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://github.com/seecr/selftest/actions/workflows/python-package.yml/badge.svg
    :alt: Python Package Check
 
+.. image:: https://img.shields.io/badge/created_by-seecr-orange
+   :alt: Created by Seecr
+
 ========
 Selftest
 ========
 
 1. Introduction
 ===============
 
@@ -33,20 +36,26 @@
 
 - tests are *ordinary functions*, anywhere in the application code,
 - gathering and running tests is *automatic* and follows the structure of your code,
 - testing *stops on first failure* with a standard Python stack trace,
 
 The benefit of this approach are:
 
-- there is no seprate test tree to maintain,
+- there is no separate test tree to maintain,
 - dependencies are automatically tested,
 - quicker cycles, more focus.
 
 The core is extremely small and support for `async`, `filters`, `operators`, `fixtures`, `diffs`, `wildcards`, `guards`, etc are all implemented in `hooks`.
 
+In-source testing
+-----------------
+Selttest runs tests within the source code alongside the implementation, similar to Rust's module tests and Vitest in-source testing.
+
+This makes the tests share closure with the implementation and enables it to test against private state without exporting. Meanwhile, it also brings a closer feedback loop for development.
+
 
 History
 -------
 Selftest began, as a recalcitrant move away from the frameworks, with the following decorator above my tests:
 
 .. code:: python
 
@@ -59,21 +68,19 @@
 
   @test                                   # marks and runs the test
   def a_test():
       assert 42 == i_need_testing(42)
 
 It would just run the test every time I imported it. That turned out to work so well that it grew out to what we have here today.
 
-Selftest was first named Autotest, due to conflicting names in the Python Package Index it was renamed to Selftest.
-
 
 Features
 --------
 
-Meanwhile autotest gained some features. It
+Meanwhile selftest gained some features. It
 
 #) works in a familiar *Pythonic* way, no magic,
 #) has one simple *API* via the test object,
 #) is based on *standard modules* operator, pdb, logger, difflib, inspect, etc,
 #) seamlessly scales from *microtests* to *systemtests*,
 #) discovers tests automatically through the *importing mechanism*,
 #) crosses module, package and project boundaries easily,
@@ -83,39 +90,39 @@
 #) supports *levels*: unit, integration, performance etc.,
 #) there are *fixtures* (context managers) like in other test tools,
 #) *async tests and fixtures* are fully supported,
 #) most functionality is in *hooks* which you can extend easily,
 #) there is a *root* tester which can have *subtesters*,
 #) output is send to a *logger*.
 
-Although autotest promotes an agile, rigorous and Pythonic way of testing, since there is little magic and tests are just functions, you are free to organise them as you wish. You can even do it the Python unittest way, if you want.
+Although selftest promotes an agile, rigorous and Pythonic way of testing, since there is little magic and tests are just functions, you are free to organise them as you wish. You can even do it the Python unittest way, if you want.
 
 
 
 An example
 ----------
 
 Selftest has a global root tester that can have an arbitrarily deep and wide tree of child testers. A typical module uses it as follows:
 
 .. code:: python
 
-    import autotest
-    test = autotest.get_tester(__name__)
+    import selftest
+    test = selftest.get_tester(__name__)
 
     def area(w, h):
         return w * h
 
     @test
     def area_basics():
         assert 9 == area(3, 3)
         assert 6 == area(2, 3)
 
-Its creates a subtester using ``get_tester()``. The resulting tester object is the main access point to all functionality of autotest.  In this case, it is used as a decorator to mark and execute a test function.
+Its creates a subtester using ``get_tester()``. The resulting tester object is the main access point to all functionality of selftest.  In this case, it is used as a decorator to mark and execute a test function.
 
-More on assert later.
+More on ``assert`` later.
 
 
 
 2. Basic API
 ============
 
 General
@@ -150,29 +157,29 @@
 - hooks API.
 - APIs introduced by hooks
 
 
 Module Level API
 ----------------
 
-The autotest core consist of two module level functions:
+The selftest core consist of two module level functions:
 
 
 ``basic_config(**options)``
 
 Sets options for the root tester. This can be called only once, before ``get_tester()``. If not called, default options are used. This typicalliy happens in the main of an application or in a program for running tests.
 
 
 ``get_tester(name=None)``
 
 When name is ``None`` returns the root tester. Otherwise it returns a named child of the root.  Name is a potentially hierarchical name separated by dots. Each level in this hierarchy becomes a child of the one preceding it. The last tester object is returned. Thus, ``get_tester("main.sub")`` creates a child ``main`` of the root and a child ``sub`` of the child ``main``. It returns the latter.
 
 Testers created this way become globally available. A call to ``get_tester()`` with the same name repeatedly will return the same tester.
 
-Recommended is to use ``test = get_tester(__name__)`` at the start of your module. Using subtesters is a powerful way of organising tests. See the source code of autotest for many examples.
+Recommended is to use ``test = get_tester(__name__)`` at the start of your module. Using subtesters is a powerful way of organising tests. See the source code of selftest for many examples.
 
 
 Tester Objects API
 ------------------
 
 A tester object as returned from ``get_tester()`` support the following methods:
 
@@ -226,15 +233,15 @@
 
 ``child(**options)``
 
 This creates a child and returns a context manager.
 
 .. code:: python
 
-   test = autotest.get_tester(__name__)
+   test = selftest.get_tester(__name__)
    with test.child(level=CRITICAL) as crit:
        @crit
        def a_critical_test_function():
            pass
 
 
 ``fail(*args, **kwargs)``
@@ -265,15 +272,15 @@
 ==========  =======  =======   ==========================================================
 keep        boolean  False     Keep the function instead of discarding it.
 run         boolean  True      Run immediately.
 hooks       list     []        List of hooks that are invoked in order.
 subprocess  boolean  False     Runs test when inside a subprocess.
 ==========  =======  =======   ==========================================================
 
-Normally, autotest runs a test as soon as it discovers it and then discards it. The example below show how tests can be run later by keeping and invoking them.
+Normally, selftest runs a test as soon as it discovers it and then discards it. The example below show how tests can be run later by keeping and invoking them.
 
 .. code:: python
 
   @test
   def this_test_runs_immediately():
     pass
 
@@ -385,22 +392,22 @@
     @test
     def another_test():
         test.all(x > 1 for x in [1,2,3])      # use builtin all()
         test.startswith("rumbush", "rum")     # use method of first argument
 
 When the given operator returns ``False`` according to ``bool()`` it raises ``AssertionError`` with the actual values of the arguments.
 
-This shows how autotest stays close to Python as we know it. It does nothing more than looking up the given attribute in four places:
+This shows how selftest stays close to Python as we know it. It does nothing more than looking up the given attribute in four places:
 
 #) module ``operator``, e.g.: ``test.gt(2, 1)``,
 #) module ``builtins``, e.g.: ``test.isinstance('aa', str)``,
 #) module ``inspect``, e.g.: ``test.isfunction(len)``,
 #) the first argument, e.g.: ``test.isupper("ABC")``.
 
-The benefits of this is that we do not have to learn new methods, that the assert functions are not limited, and that autotest can print the arguments for us on failure.
+The benefits of this is that we do not have to learn new methods, that the assert functions are not limited, and that selftest can print the arguments for us on failure.
 
 **diff**
 
 All operators obtained this way support a keyword ``diff=<function>`` that, when present, is invoked with the actual arguments. The result is then given to the ``AssertionError`` instead of the actual arguments.
 
 .. code:: python
 
@@ -624,44 +631,44 @@
 
   $ python <mymodule.py>
   $ python -c "import mymodule"
 
 When you only want to develop a submodule, just ``cd`` down into that directory and do the same. Only the tests of that submodule (and everything in imports) will be tested.
 
 
-The methode above just prints crude messages and has no way to use options. For that use the main that comes with autotest:
+The methode above just prints crude messages and has no way to use options. For that use the main that comes with selftest:
 
 .. code:: bash
 
-  $ autotest --help
-  Usage: autotest [options] module
+  $ selftest --help
+  Usage: selftest [options] module
 
   Options:
     -h, --help            show this help message and exit
     -f FILTER, --filter=FILTER
                         only run tests whose qualified name contains FILTER
     -t , --threshold=THRESHOLD
                         only run tests whose level is >= THRESHOLD
 
 
 For example to run your tests but not the imported ones from other packages:
 
 .. code:: bash
 
-  $ autotest --filter mymodule mymodule
+  $ selftest --filter mymodule mymodule
 
 
-If you want to run the tests for autotests itself, go to the autotest project directory and use:
+If you want to run the tests for selftest itself, go to the selftest project directory and use:
 
 .. code:: bash
 
-  $ python -c "import autotest"  autotest.selftest
+  $ python -c "import selftest"  selftest.selftest
 
-The argument ``autotest.selftest`` lets autotest run its own tests, which are normally skipped.
-Also, this avoids using the autotest main program because it is not guaranteed that an installed old version of autotest can run its own test from the future.
+The argument ``selftest.selftest`` lets selftest run its own tests, which are normally skipped.
+Also, this avoids using the selftest main program because it is not guaranteed that an installed old version of selftest can run its own test from the future.
 
 
 **Production**
 
 During production, all tests are automatically run during startup when all needed modules are imported. If an the application configures a specific root, for example by calling ``logging.basicConfig()``, the tests will automatically log there. Alternatively, you can setup a separate ``Logger`` for running tests. See Core API.
 
 You can als filter tests or run tests for a specific level only. Or suppress them all. See the source code of ``__main__.py`` for ideas.
```

### Comparing `selftest-0.4.0/selftest.egg-info/SOURCES.txt` & `selftest-0.4.1/selftest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selftest-0.4.0/setup.py` & `selftest-0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.rst").read_text(encoding="utf-8")
 
-version = "0.4.0"
+version = "0.4.1"
 
 setup(
     name="selftest",
     version=version,
-    description="Python Testing Library",
+    description="Python In-Source Testing Library",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     packages=find_packages(),
     author="Erik Groeneveld",
     author_email="erik@seecr.nl",
     maintainer="Thijs Janssen",
     maintainer_email="thijs@seecr.nl",
-    url="https://github.com/seecr/selftest",
+    url="https://github.com/ejgroene/selftest",
     scripts=["bin/selftest"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Topic :: Software Development :: Testing",
         "Topic :: Software Development :: Testing :: Unit",
         "Programming Language :: Python :: 3",
```

