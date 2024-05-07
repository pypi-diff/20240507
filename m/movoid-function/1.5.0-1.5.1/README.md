# Comparing `tmp/movoid_function-1.5.0.tar.gz` & `tmp/movoid_function-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_function-1.5.0.tar", last modified: Sun Apr 14 08:04:10 2024, max compression
+gzip compressed data, was "movoid_function-1.5.1.tar", last modified: Tue May  7 14:03:27 2024, max compression
```

## Comparing `movoid_function-1.5.0.tar` & `movoid_function-1.5.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 08:04:10.289501 movoid_function-1.5.0/
--rw-rw-rw-   0        0        0      213 2024-04-14 08:04:10.288515 movoid_function-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_function-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 08:04:10.278538 movoid_function-1.5.0/movoid_function/
--rw-rw-rw-   0        0        0      562 2024-04-13 09:15:08.000000 movoid_function-1.5.0/movoid_function/__init__.py
--rw-rw-rw-   0        0        0     9812 2024-02-20 05:59:20.000000 movoid_function-1.5.0/movoid_function/check.py
--rw-rw-rw-   0        0        0    16565 2024-02-20 11:49:02.000000 movoid_function-1.5.0/movoid_function/decorator.py
--rw-rw-rw-   0        0        0     1557 2024-04-14 08:03:48.000000 movoid_function-1.5.0/movoid_function/function.py
--rw-rw-rw-   0        0        0    12734 2024-02-20 05:59:20.000000 movoid_function-1.5.0/movoid_function/type.py
-drwxrwxrwx   0        0        0        0 2024-04-14 08:04:10.287510 movoid_function-1.5.0/movoid_function.egg-info/
--rw-rw-rw-   0        0        0      213 2024-04-14 08:04:10.000000 movoid_function-1.5.0/movoid_function.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-04-14 08:04:10.000000 movoid_function-1.5.0/movoid_function.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 08:04:10.000000 movoid_function-1.5.0/movoid_function.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-14 08:04:10.000000 movoid_function-1.5.0/movoid_function.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 08:04:10.289501 movoid_function-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0      462 2024-04-14 07:24:11.000000 movoid_function-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:03:27.165840 movoid_function-1.5.1/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_function-1.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      213 2024-05-07 14:03:27.164842 movoid_function-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_function-1.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 14:03:27.157673 movoid_function-1.5.1/movoid_function/
+-rw-rw-rw-   0        0        0      562 2024-04-13 09:15:08.000000 movoid_function-1.5.1/movoid_function/__init__.py
+-rw-rw-rw-   0        0        0     9812 2024-02-20 05:59:20.000000 movoid_function-1.5.1/movoid_function/check.py
+-rw-rw-rw-   0        0        0    16565 2024-02-20 11:49:02.000000 movoid_function-1.5.1/movoid_function/decorator.py
+-rw-rw-rw-   0        0        0     1557 2024-04-14 08:03:48.000000 movoid_function-1.5.1/movoid_function/function.py
+-rw-rw-rw-   0        0        0    13000 2024-05-07 13:18:50.000000 movoid_function-1.5.1/movoid_function/type.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:03:27.163750 movoid_function-1.5.1/movoid_function.egg-info/
+-rw-rw-rw-   0        0        0      213 2024-05-07 14:03:27.000000 movoid_function-1.5.1/movoid_function.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-07 14:03:27.000000 movoid_function-1.5.1/movoid_function.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:03:27.000000 movoid_function-1.5.1/movoid_function.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-07 14:03:27.000000 movoid_function-1.5.1/movoid_function.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 14:03:27.165840 movoid_function-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      462 2024-05-07 14:02:58.000000 movoid_function-1.5.1/setup.py
```

### Comparing `movoid_function-1.5.0/movoid_function/__init__.py` & `movoid_function-1.5.1/movoid_function/__init__.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.0/movoid_function/check.py` & `movoid_function-1.5.1/movoid_function/check.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.0/movoid_function/decorator.py` & `movoid_function-1.5.1/movoid_function/decorator.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.0/movoid_function/function.py` & `movoid_function-1.5.1/movoid_function/function.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.0/movoid_function/type.py` & `movoid_function-1.5.1/movoid_function/type.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 
 class Bool(Type):
     def __init__(self, convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
 
     def __repr__(self):
-        return 'bool'
+        return f'Bool(convert={self._convert})'
 
     def check(self, check_target, convert=None) -> bool:
         check_target = self.convert(check_target, convert)
         return isinstance(check_target, bool)
 
     def _convert_function(self, check_target) -> bool:
         return bool(check_target)
@@ -71,15 +71,15 @@
 class Int(Type):
     def __init__(self, limit='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._limit = CheckFormula(limit, NumberCheck)
 
     def __repr__(self):
         limit_text = f'limit={self._limit}, ' if self._limit._str_formula else ''
-        return f'int({limit_text}convert={self._convert})'
+        return f'Int({limit_text}convert={self._convert})'
 
     def check(self, check_target, convert=None) -> bool:
         check_target = self.convert(check_target, convert)
         if isinstance(check_target, int):
             re_bool = self._limit.check(check_target)
         else:
             re_bool = False
@@ -99,15 +99,15 @@
 class Float(Type):
     def __init__(self, limit='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._limit = CheckFormula(limit, NumberCheck)
 
     def __repr__(self):
         limit_text = f'limit={self._limit}, ' if self._limit._str_formula else ''
-        return f'float({limit_text}convert={self._convert})'
+        return f'Float({limit_text}convert={self._convert})'
 
     def check(self, check_target, convert=None) -> bool:
         check_target = self.convert(check_target, convert)
         if isinstance(check_target, float):
             re_bool = self._limit.check(check_target)
         else:
             re_bool = False
@@ -127,15 +127,15 @@
 class Number(Type):
     def __init__(self, limit='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._limit = CheckFormula(limit, NumberCheck)
 
     def __repr__(self):
         limit_text = f'limit={self._limit}, ' if self._limit._str_formula else ''
-        return f'number({limit_text}convert={self._convert})'
+        return f'Number({limit_text}convert={self._convert})'
 
     def check(self, check_target, convert=None) -> bool:
         check_target = self.convert(check_target, convert)
         if isinstance(check_target, float) or isinstance(check_target, int):
             re_bool = self._limit.check(check_target)
         else:
             re_bool = False
@@ -163,15 +163,15 @@
         self._length = CheckFormula(length, NumberCheck)
         self._regex = regex
 
     def __repr__(self):
         char_text = f'char={self._char}, ' if self._char else ''
         limit_text = f'length={self._length}, ' if self._length._str_formula else ''
         regex_text = f'regex={self._regex}, ' if self._regex else ''
-        return f'str({char_text}{limit_text}{regex_text}convert={self._convert})'
+        return f'Str({char_text}{limit_text}{regex_text}convert={self._convert})'
 
     def check(self, check_target, convert=None) -> bool:
         check_target = self.convert(check_target, convert)
         if isinstance(check_target, str):
             re_bool = True
             if self._char:
                 re_bool = re_bool and all([_ in self._char for _ in check_target])
@@ -193,15 +193,15 @@
 class List(Type):
     def __init__(self, length='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._length = CheckFormula(length, NumberCheck)
 
     def __repr__(self):
         length_text = f'length={self._length}, ' if self._length._str_formula else ''
-        return f'list({length_text}convert={self._convert})'
+        return f'List({length_text}convert={self._convert})'
 
     def check(self, check_target, convert=None) -> bool:
         check_target = self.convert(check_target, convert)
         if isinstance(check_target, list):
             re_bool = True
             re_bool = re_bool and self._length.check(len(check_target))
         else:
@@ -224,15 +224,15 @@
 class Tuple(Type):
     def __init__(self, length='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._length = CheckFormula(length, NumberCheck)
 
     def __repr__(self):
         length_text = f'length={self._length}, ' if self._length._str_formula else ''
-        return f'tuple({length_text}convert={self._convert})'
+        return f'Tuple({length_text}convert={self._convert})'
 
     def check(self, check_target, convert=None) -> bool:
         check_target = self.convert(check_target, convert)
         if isinstance(check_target, tuple):
             re_bool = True
             re_bool = re_bool and self._length.check(len(check_target))
         else:
@@ -255,15 +255,15 @@
 class Set(Type):
     def __init__(self, length='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._length = CheckFormula(length, NumberCheck)
 
     def __repr__(self):
         length_text = f'length={self._length}, ' if self._length._str_formula else ''
-        return f'set({length_text}convert={self._convert})'
+        return f'Set({length_text}convert={self._convert})'
 
     def check(self, check_target, convert=None) -> bool:
         check_target = self.convert(check_target, convert)
         if isinstance(check_target, set):
             re_bool = True
             re_bool = re_bool and self._length.check(len(check_target))
         else:
@@ -286,15 +286,15 @@
 class Dict(Type):
     def __init__(self, length='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._length = CheckFormula(length, NumberCheck)
 
     def __repr__(self):
         length_text = f'length={self._length}, ' if self._length._str_formula else ''
-        return f'dict({length_text}convert={self._convert})'
+        return f'Dict({length_text}convert={self._convert})'
 
     def check(self, check_target, convert=None) -> bool:
         check_target = self.convert(check_target, convert)
         if isinstance(check_target, dict):
             re_bool = True
             re_bool = re_bool and self._length.check(len(check_target))
         else:
@@ -311,25 +311,32 @@
         if self._convert:
             return Union[dict, str]
         else:
             return dict
 
 
 class Path(Type):
-    def __init__(self, convert=False, **kwargs):
+    def __init__(self, should_exist=True, convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
+        self._should_exist = should_exist
 
     def __repr__(self):
-        return f'path(convert={self._convert})'
+        return f'Path(convert={self._convert})'
 
     def check(self, check_target, convert=None) -> bool:
         check_target = self.convert(check_target, convert)
         if isinstance(check_target, str):
-            re_bool = True
-            re_bool = re_bool and pathlib.Path(check_target).exists()
+            try:
+                tar_path = pathlib.Path(check_target)
+                if self._should_exist:
+                    re_bool = tar_path.exists()
+                else:
+                    re_bool = True
+            except:
+                re_bool = False
         else:
             re_bool = False
         return re_bool
 
     def _convert_function(self, check_target):
         return str(check_target)
 
@@ -370,15 +377,15 @@
                     return_annotation[_i] = real_annotation
             else:
                 if check_arguments:
                     argument_annotation[_i] = real_annotation
         func.__annotations__ = change_annotation
 
         @recover_signature_from_function_func(func)
-        def wrapper(kwargs):
+        def wrapper(**kwargs):
             for _i2, _v2 in kwargs.items():
                 if _i2 in argument_annotation:
                     _v3 = argument_annotation[_i2]
                     check_result = _v3.check(_v2)
                     if not check_result:
                         raise TypeError(f'{_i2} is {_v2}({type(_v2).__name__}),but it should be a {_v3}')
                     kwargs[_i2] = _v3.convert(_v2)
```

