# Comparing `tmp/istr_python-1.0.0.tar.gz` & `tmp/istr_python-1.0.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-1.0.0.tar", last modified: Mon May  6 13:49:54 2024, max compression
+gzip compressed data, was "istr_python-1.0.0.post0.tar", last modified: Tue May  7 15:27:01 2024, max compression
```

## Comparing `istr_python-1.0.0.tar` & `istr_python-1.0.0.post0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 13:49:54.787606 istr_python-1.0.0/
--rw-rw-rw-   0        0        0    15702 2024-05-06 13:49:54.785577 istr_python-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    14565 2024-05-06 13:47:27.000000 istr_python-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 13:49:54.759491 istr_python-1.0.0/istr/
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-1.0.0/istr/__init__.py
--rw-rw-rw-   0        0        0    24194 2024-05-06 11:38:16.000000 istr_python-1.0.0/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:49:54.783062 istr_python-1.0.0/istr_python.egg-info/
--rw-rw-rw-   0        0        0    15702 2024-05-06 13:49:54.000000 istr_python-1.0.0/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-05-06 13:49:54.000000 istr_python-1.0.0/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 13:49:54.000000 istr_python-1.0.0/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-06 13:49:54.000000 istr_python-1.0.0/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      658 2024-05-06 13:49:48.000000 istr_python-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 13:49:54.787606 istr_python-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 13:49:54.781067 istr_python-1.0.0/tests/
--rw-rw-rw-   0        0        0    16198 2024-05-06 11:40:02.000000 istr_python-1.0.0/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:27:01.200452 istr_python-1.0.0.post0/
+-rw-rw-rw-   0        0        0    16564 2024-05-07 15:27:01.194781 istr_python-1.0.0.post0/PKG-INFO
+-rw-rw-rw-   0        0        0     3506 2024-05-07 14:46:38.000000 istr_python-1.0.0.post0/changelog.md
+drwxrwxrwx   0        0        0        0 2024-05-07 15:27:01.044344 istr_python-1.0.0.post0/istr/
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-1.0.0.post0/istr/__init__.py
+-rw-rw-rw-   0        0        0    22612 2024-05-07 15:26:00.000000 istr_python-1.0.0.post0/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:27:01.189048 istr_python-1.0.0.post0/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    16564 2024-05-07 15:27:00.000000 istr_python-1.0.0.post0/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-07 15:27:01.000000 istr_python-1.0.0.post0/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 15:27:00.000000 istr_python-1.0.0.post0/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-07 15:27:00.000000 istr_python-1.0.0.post0/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      713 2024-05-07 15:26:52.000000 istr_python-1.0.0.post0/pyproject.toml
+-rw-rw-rw-   0        0        0    15395 2024-05-07 15:20:46.000000 istr_python-1.0.0.post0/readme.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 15:27:01.202010 istr_python-1.0.0.post0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 15:27:01.179779 istr_python-1.0.0.post0/tests/
+-rw-rw-rw-   0        0        0    16873 2024-05-07 14:59:26.000000 istr_python-1.0.0.post0/tests/test_istr.py
```

### Comparing `istr_python-1.0.0/PKG-INFO` & `istr_python-1.0.0.post0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 1.0.0
+Version: 1.0.0.post0
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
  <img src="https://www.salabim.org/istr_logo.png" width=500>
 
 ### Introduction
 
-The istr module has exactly one class: istr.
-
-With this it is possible to interpret strings as if they were integers.
+With  `istr` is possible to interpret strings as if they were integers.
 
 This can be very handy for solving puzzles, but also for other purposes.
 For instance the famous send more money puzzle, where each letter has to be replaced by a unique digit (0-9)
 
 ```
   S E N D
   M O R E
@@ -93,15 +91,15 @@
 
 or
 
 ```
 twenty = four * 5
 ```
 
-And now `twenty` can be used as if it was an int as well. So:
+And now `twenty` can be used as if it was an int as well. So
 
 ```
 twenty - four
 ```
 
 is `istr('16')`
 
@@ -109,22 +107,22 @@
 
 ```
 -four + (twenty / 2)
 ```
 
 is `istr('6')`
 
-And we can test for equality, So:
+And we can test for equality. So:
 
 ```
 twenty == 20
 ```
 is True.
 
-But as istrs are also strings. So
+But istrs are also strings. So
 
 ```
 twenty == '20'
 ```
 
 is also True!
 
@@ -137,60 +135,64 @@
 ```
 are `True`.
 
 In contrast to an ordinary string
 ```
 print(four + five)
 ```
-prints `9`, as istr are treated as ints.
+prints `9`, as istr are treated as ints (if possible).
 
 Please note that `four`  could have also been initialized with
 ```
 four = istr(4)
 ```
 or even
 ```
 four, five = istr(4, 5)
 ```
 
-> [!NOTE]
->
-> All calculations are strictly integer calculations. That means that if a float variale is ever produced it will be converted to an int.
-> Also divisions are always floor divisions!
+> > [!IMPORTANT]
+> >
+> > All calculations are strictly integer calculations. That means that if a float or decimal variable is ever produced it will be converted to an int.
+> > Also divisions are always floor divisions!
 
 #### Use istrs as string
 
 We should realize that istrs are in fact strings.
 
-In order to concatenate two istrs (or an istr and a str), we cannot use the `four + five` operator as
-
-that would be `istr(9)`.
+In order to concatenate two istrs (or an istr and a str), we cannot use the `+` operator (remember `four + five` is `istr('9')`).
 
 In order to concatenate istrs,  we use the or operator (`|`). So
 
 ```
 four | five
 ```
 will be `istr(`45`).
 
-That means that
+And
 ```
 (four | five) / 3
 ```
 is `istr('9')`.
 
-In order to repeat a string in the usual sense, you cannot use `3 * four`, as that would be `12`. 
+In order to repeat a string in the usual sense, you cannot use the `*` operator (remember `3 * four` is `istr(12)`. 
 
 In order to repeat we use the matrix multiplication operator (`@`). So
 
  `3 @ four`
 
- is istr(`444`). As is `four @ 3`.
+ is `istr('444')`
+
+And 
+
+```four @ 3```
+
+is also `istr('444')`
 
-> [!NOTE]
+> Note:
 >
 > It is not allowed to use the `@` operator for two istrs. So, `four @ five` raises a TypeError.
 
 #### istrs that can't be interpreted as an int
 
 Although usualy, istrs are to be interpreted as an int, that's not a requirement.
 
@@ -199,52 +201,52 @@
 ```
 istr('abc')
 ```
 
 or
 
 ```
-istr(1,2,3)
+istr('1,2,3')
 ```
 
 are accepted.
 
 But, we can't do any arithmetic with them. 
 
 If we try
 
 ```
 istr('abc') + 5
 ```
 
-a TypeError will be raised.
+a `TypeError` will be raised.
 
 That holds for any arithmetic we try.
 
 If we want to test if an istr can be interpreted (and thus used in an arithmetic expression). we can use the `is_int()` method. So
 
 ```ìstr(20).is_int()```
 
-is `True`, wherea
+is `True`, whereas
 
 ```ìstr('abc').is_int()```
 
 is `False`.
 
 
 
 The bool operator works normally on the integer value of an istr. So
 
 `bool(istr('0'))` ==> `False`
 `bool(istr('1'))` ==> `True`
 
-If the istr can't be interpreted as an int, the string will be used to test. So
+If the istr can't be interpreted as an int, the string value will be used to test. So
 
-`bool(istr('abc'))` ==> `False`
-`bool(istr(''))` ==> `True`
+`bool(istr('abc'))` ==> `True`
+`bool(istr(''))` ==> `False`
 
 #### Other operators
 
 For the `in` operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
 
 ```
 '34' in istr(1234)
@@ -275,15 +277,15 @@
 
 is 
 
 ```
 '0 1 2 3 4 5 6 7 8 9 10 11'
 ```
 
-#### Using other values for istr than numeric value or str
+#### Using values to inialitize istr other than numeric value or str
 Apart from with simple numeric (to be interpreted as an int) or str, istr can be initialized with
 several other types:
 
 - if a dict (or subtype of dict), the same type dict will be returned with all *values* istr'ed
 
     ```
     istr({0: 0, 1: 1, 2: 4}) ==> {0: istr('0'), 1: istr('1'), 2: istr('4')}
@@ -304,15 +306,15 @@
     istr({0, 1, 4}) ==> `{istr('4'), istr('0'), istr('1')}  # or similar
     ```
 
 - if a range, an istr.range instance will be returned
   
     ```
   istr(range(3))` ==> `istr.range(3)
-    list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]
+  list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]
   len(istr(range(3)))` ==> `3
   ```
 
 - if an istr.range instance, the same istr.range will be returned
 
 - if an istr, the same istr will be used
 
@@ -326,48 +328,62 @@
 to unpack multiple values, e.g.
 
 ```
 a, b, c = istr(5, 6, 7) ==> a=istr('5') , b=istr('6'), c=istr('7') 
 ```
 
 #### test for even/odd
-It is possible to test for even/odd (provided the istt can be interpreted as an int) with the
+It is possible to test for even/odd (provided the istr can be interpreted as an int) with the
 
 `is_even` and `is_odd` method, e.g.
 
 ```
 istr(4).is_even()) ==> True
 istr(5).is_odd()) ==> True
 ```
+#### test whether all characters are distinct
+
+With the `all_distinct` method, it is possible to test whether all characters are distinct (i.e. no character appearts more than once).
+
+```
+istr('01234').all_distict() ==> True
+istr('012340').all_distict() ==> False
+n98 = istr(98)
+n100 = n98 + 2
+istr(n98).all_distinct() ==> True
+istr(n100).all_distinct() ==> False
+```
+
 #### reverse an istr
+
 The method `istr.reversed()` will return the an istr with the reversed content:
 ```
 istr(456).reversed() ==> istr('654')
 istr('0456').reversed() ==> istr('6540')
 ```
 The same can -of course- be achieved with
 ```
 istr(456)[::-1] ==> istr('654')
 istr('0456')[::-1] ==> istr('6540')
 ```
-> [!NOTE]
->
-> It is possible to reverse a negative istr, but the result can't be interpreted as an int anymore.
->
-> ```
-> istr(-456) ==> TypeError
-> ```
+> > [!NOTE]
+> >
+> > It is possible to reverse a negative istr, but the result can't be interpreted as an int anymore.
+> >
+> > ```
+> > istr(-456) ==> TypeError
+> > ```
 
 #### enumerate with istrs
 
 The `istr.enumerate` method can be used just as the builtin enumerate function.
 The iteration counter however is an istr rather than an int. E.g. 
 
 ```
-    for i,c in istr.enumerate('abc'):
+    for i, c in istr.enumerate('abc'):
         print(f'{repr(i)} {c}')
 ```
 prints
 ```
 istr('0') a
 istr('1') b
 istr('2') c
@@ -387,38 +403,48 @@
 ```
 
 #### generate istr with digits
 
 The class method `digits` can be used to return an istr of digits according to a given specification.
 The method takes either no or a number of arguments.
 
-If no arguments are given, the result will be istr('0123456789').
+If no arguments are given, the result will be `istr('0123456789')`.
 
 The given argument(s) result in a range of digits.
 
 - `<n>` ==> n
 - `<n-m>` ==> n, n+1, ..., m
 - `-n>` ==> 0, 1, ... n
 - `n->` ==> n, n+1, ..., 9
 - `''` ==> 0, 1, ..., 9
 
-(n and m must be digits between 0 and 9)
+(n and m must be digits between 0 and 9 or letters letters between A and Z)
+
+When no stop value is specified, it will be
+
+* 9 if the start value is between 0 and 9
+* Z if the start value is between A and Z 
 
 The final result is an istr composed of the given range(s).
 
 Here are some examples:
 
 ```
 istr.digits() ==> istr('0123456789')
 istr.digits('') ==> istr('0123456789')
 istr.digits('1') ==> istr('1')
 istr.digits('3-') ==> istr('3456789')
 istr.digits('-3') ==> istr('0123')
 istr('1-4', '6', '8-9') ==> istr('1234689')
 istr('1', '1-2', '1-3') ==> istr('11213')
+istr.digits('-z') ==> istr('0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ')
+istr.digits('A-F') ==> istr('ABCDEF')
+istr.digits('C') ==> istr('C')
+istr.digits('3-') ==> istr('34567879')
+istr.digits('X-') ==> istr('XYZ')
 ```
 
 
 #### Subclassing istr
 When a class is derived from istr, all methods will return that newly derived class. 
 
 E.g.
@@ -430,26 +456,26 @@
 ```
 will print `jstr('20')`
 
 #### Changing the way repr works
 
 It is possible to control the way an `istr` instance will be repr'ed.
 
-By default, the `istr('5')` is represented as `istr('5')`.
+By default, the `istr(5)` is represented as `istr('5')`.
 
 With the istr.repr_mode() context manager, that can be changed:
 ```
 with istr.repr_mode('str'):
-    five = istr('5')
+    five = istr(5)
     print(repr(five))
 with istr.repr_mode('int'):
-    five = istr('5')
+    five = istr(5)
     print(repr(five))
 with istr.repr_mode('istr'):
-    five = istr('5')
+    five = istr(5)
     print(repr(five))
 ```
 This will print
 ```
 '5'
 5
 istr('5')
@@ -464,17 +490,17 @@
 
 This will print
 
 ```
 nan
 ```
 
-> [!NOTE]
->
-> The way an `istr` is represented is determined at initialization.
+> > [!NOTE]
+> >
+> > The way an `istr` is represented is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 
 ```
 istr.repr_mode('str')
 five = istr('5')
 print(repr(five))
@@ -576,32 +602,32 @@
 will print
 ```
 istr('001')
 istr('012')
 istr('123')
 istr('1234')
 ```
-> [!NOTE]
->
->  if a string is used to initialize an istr AND that string can be interpreted as an int. the string will reformatted:
->
-> ```
-> with istr.int_format('03'):
->     print(repr(istr('  12 ')))
-> ```
->
-> will result in
->
-> ```
-> istr('0012')
-> ```
-
-> [!NOTE]
+> > [!NOTE]
+> >
+> > if a string is used to initialize an istr AND that string can be interpreted as an int. the string will reformatted:
+> >
+> > ```
+> > with istr.int_format('03'):
+> >    print(repr(istr(12)))
+> > ```
+> >
+> > will result in
+> >
+> > ```
+> > istr('0012')
+> > ```
 >
-> For bases other than 10, the string will never be reformatted!
+> > [!NOTE]
+> >
+> > For bases other than 10, the string will never be reformatted!
 
 ### Overview of operations
 
 The table below shows whether the string or the int version of istr is applied.
 
 ```
 operator/function   int  str   Example
```

### Comparing `istr_python-1.0.0/README.md` & `istr_python-1.0.0.post0/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
  <img src="https://www.salabim.org/istr_logo.png" width=500>
 
 ### Introduction
 
-The istr module has exactly one class: istr.
-
-With this it is possible to interpret strings as if they were integers.
+With  `istr` is possible to interpret strings as if they were integers.
 
 This can be very handy for solving puzzles, but also for other purposes.
 For instance the famous send more money puzzle, where each letter has to be replaced by a unique digit (0-9)
 
 ```
   S E N D
   M O R E
@@ -80,15 +78,15 @@
 
 or
 
 ```
 twenty = four * 5
 ```
 
-And now `twenty` can be used as if it was an int as well. So:
+And now `twenty` can be used as if it was an int as well. So
 
 ```
 twenty - four
 ```
 
 is `istr('16')`
 
@@ -96,22 +94,22 @@
 
 ```
 -four + (twenty / 2)
 ```
 
 is `istr('6')`
 
-And we can test for equality, So:
+And we can test for equality. So:
 
 ```
 twenty == 20
 ```
 is True.
 
-But as istrs are also strings. So
+But istrs are also strings. So
 
 ```
 twenty == '20'
 ```
 
 is also True!
 
@@ -124,60 +122,64 @@
 ```
 are `True`.
 
 In contrast to an ordinary string
 ```
 print(four + five)
 ```
-prints `9`, as istr are treated as ints.
+prints `9`, as istr are treated as ints (if possible).
 
 Please note that `four`  could have also been initialized with
 ```
 four = istr(4)
 ```
 or even
 ```
 four, five = istr(4, 5)
 ```
 
-> [!NOTE]
->
-> All calculations are strictly integer calculations. That means that if a float variale is ever produced it will be converted to an int.
-> Also divisions are always floor divisions!
+> > [!IMPORTANT]
+> >
+> > All calculations are strictly integer calculations. That means that if a float or decimal variable is ever produced it will be converted to an int.
+> > Also divisions are always floor divisions!
 
 #### Use istrs as string
 
 We should realize that istrs are in fact strings.
 
-In order to concatenate two istrs (or an istr and a str), we cannot use the `four + five` operator as
-
-that would be `istr(9)`.
+In order to concatenate two istrs (or an istr and a str), we cannot use the `+` operator (remember `four + five` is `istr('9')`).
 
 In order to concatenate istrs,  we use the or operator (`|`). So
 
 ```
 four | five
 ```
 will be `istr(`45`).
 
-That means that
+And
 ```
 (four | five) / 3
 ```
 is `istr('9')`.
 
-In order to repeat a string in the usual sense, you cannot use `3 * four`, as that would be `12`. 
+In order to repeat a string in the usual sense, you cannot use the `*` operator (remember `3 * four` is `istr(12)`. 
 
 In order to repeat we use the matrix multiplication operator (`@`). So
 
  `3 @ four`
 
- is istr(`444`). As is `four @ 3`.
+ is `istr('444')`
+
+And 
+
+```four @ 3```
+
+is also `istr('444')`
 
-> [!NOTE]
+> Note:
 >
 > It is not allowed to use the `@` operator for two istrs. So, `four @ five` raises a TypeError.
 
 #### istrs that can't be interpreted as an int
 
 Although usualy, istrs are to be interpreted as an int, that's not a requirement.
 
@@ -186,52 +188,52 @@
 ```
 istr('abc')
 ```
 
 or
 
 ```
-istr(1,2,3)
+istr('1,2,3')
 ```
 
 are accepted.
 
 But, we can't do any arithmetic with them. 
 
 If we try
 
 ```
 istr('abc') + 5
 ```
 
-a TypeError will be raised.
+a `TypeError` will be raised.
 
 That holds for any arithmetic we try.
 
 If we want to test if an istr can be interpreted (and thus used in an arithmetic expression). we can use the `is_int()` method. So
 
 ```ìstr(20).is_int()```
 
-is `True`, wherea
+is `True`, whereas
 
 ```ìstr('abc').is_int()```
 
 is `False`.
 
 
 
 The bool operator works normally on the integer value of an istr. So
 
 `bool(istr('0'))` ==> `False`
 `bool(istr('1'))` ==> `True`
 
-If the istr can't be interpreted as an int, the string will be used to test. So
+If the istr can't be interpreted as an int, the string value will be used to test. So
 
-`bool(istr('abc'))` ==> `False`
-`bool(istr(''))` ==> `True`
+`bool(istr('abc'))` ==> `True`
+`bool(istr(''))` ==> `False`
 
 #### Other operators
 
 For the `in` operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
 
 ```
 '34' in istr(1234)
@@ -262,15 +264,15 @@
 
 is 
 
 ```
 '0 1 2 3 4 5 6 7 8 9 10 11'
 ```
 
-#### Using other values for istr than numeric value or str
+#### Using values to inialitize istr other than numeric value or str
 Apart from with simple numeric (to be interpreted as an int) or str, istr can be initialized with
 several other types:
 
 - if a dict (or subtype of dict), the same type dict will be returned with all *values* istr'ed
 
     ```
     istr({0: 0, 1: 1, 2: 4}) ==> {0: istr('0'), 1: istr('1'), 2: istr('4')}
@@ -291,15 +293,15 @@
     istr({0, 1, 4}) ==> `{istr('4'), istr('0'), istr('1')}  # or similar
     ```
 
 - if a range, an istr.range instance will be returned
   
     ```
   istr(range(3))` ==> `istr.range(3)
-    list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]
+  list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]
   len(istr(range(3)))` ==> `3
   ```
 
 - if an istr.range instance, the same istr.range will be returned
 
 - if an istr, the same istr will be used
 
@@ -313,48 +315,62 @@
 to unpack multiple values, e.g.
 
 ```
 a, b, c = istr(5, 6, 7) ==> a=istr('5') , b=istr('6'), c=istr('7') 
 ```
 
 #### test for even/odd
-It is possible to test for even/odd (provided the istt can be interpreted as an int) with the
+It is possible to test for even/odd (provided the istr can be interpreted as an int) with the
 
 `is_even` and `is_odd` method, e.g.
 
 ```
 istr(4).is_even()) ==> True
 istr(5).is_odd()) ==> True
 ```
+#### test whether all characters are distinct
+
+With the `all_distinct` method, it is possible to test whether all characters are distinct (i.e. no character appearts more than once).
+
+```
+istr('01234').all_distict() ==> True
+istr('012340').all_distict() ==> False
+n98 = istr(98)
+n100 = n98 + 2
+istr(n98).all_distinct() ==> True
+istr(n100).all_distinct() ==> False
+```
+
 #### reverse an istr
+
 The method `istr.reversed()` will return the an istr with the reversed content:
 ```
 istr(456).reversed() ==> istr('654')
 istr('0456').reversed() ==> istr('6540')
 ```
 The same can -of course- be achieved with
 ```
 istr(456)[::-1] ==> istr('654')
 istr('0456')[::-1] ==> istr('6540')
 ```
-> [!NOTE]
->
-> It is possible to reverse a negative istr, but the result can't be interpreted as an int anymore.
->
-> ```
-> istr(-456) ==> TypeError
-> ```
+> > [!NOTE]
+> >
+> > It is possible to reverse a negative istr, but the result can't be interpreted as an int anymore.
+> >
+> > ```
+> > istr(-456) ==> TypeError
+> > ```
 
 #### enumerate with istrs
 
 The `istr.enumerate` method can be used just as the builtin enumerate function.
 The iteration counter however is an istr rather than an int. E.g. 
 
 ```
-    for i,c in istr.enumerate('abc'):
+    for i, c in istr.enumerate('abc'):
         print(f'{repr(i)} {c}')
 ```
 prints
 ```
 istr('0') a
 istr('1') b
 istr('2') c
@@ -374,38 +390,48 @@
 ```
 
 #### generate istr with digits
 
 The class method `digits` can be used to return an istr of digits according to a given specification.
 The method takes either no or a number of arguments.
 
-If no arguments are given, the result will be istr('0123456789').
+If no arguments are given, the result will be `istr('0123456789')`.
 
 The given argument(s) result in a range of digits.
 
 - `<n>` ==> n
 - `<n-m>` ==> n, n+1, ..., m
 - `-n>` ==> 0, 1, ... n
 - `n->` ==> n, n+1, ..., 9
 - `''` ==> 0, 1, ..., 9
 
-(n and m must be digits between 0 and 9)
+(n and m must be digits between 0 and 9 or letters letters between A and Z)
+
+When no stop value is specified, it will be
+
+* 9 if the start value is between 0 and 9
+* Z if the start value is between A and Z 
 
 The final result is an istr composed of the given range(s).
 
 Here are some examples:
 
 ```
 istr.digits() ==> istr('0123456789')
 istr.digits('') ==> istr('0123456789')
 istr.digits('1') ==> istr('1')
 istr.digits('3-') ==> istr('3456789')
 istr.digits('-3') ==> istr('0123')
 istr('1-4', '6', '8-9') ==> istr('1234689')
 istr('1', '1-2', '1-3') ==> istr('11213')
+istr.digits('-z') ==> istr('0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ')
+istr.digits('A-F') ==> istr('ABCDEF')
+istr.digits('C') ==> istr('C')
+istr.digits('3-') ==> istr('34567879')
+istr.digits('X-') ==> istr('XYZ')
 ```
 
 
 #### Subclassing istr
 When a class is derived from istr, all methods will return that newly derived class. 
 
 E.g.
@@ -417,26 +443,26 @@
 ```
 will print `jstr('20')`
 
 #### Changing the way repr works
 
 It is possible to control the way an `istr` instance will be repr'ed.
 
-By default, the `istr('5')` is represented as `istr('5')`.
+By default, the `istr(5)` is represented as `istr('5')`.
 
 With the istr.repr_mode() context manager, that can be changed:
 ```
 with istr.repr_mode('str'):
-    five = istr('5')
+    five = istr(5)
     print(repr(five))
 with istr.repr_mode('int'):
-    five = istr('5')
+    five = istr(5)
     print(repr(five))
 with istr.repr_mode('istr'):
-    five = istr('5')
+    five = istr(5)
     print(repr(five))
 ```
 This will print
 ```
 '5'
 5
 istr('5')
@@ -451,17 +477,17 @@
 
 This will print
 
 ```
 nan
 ```
 
-> [!NOTE]
->
-> The way an `istr` is represented is determined at initialization.
+> > [!NOTE]
+> >
+> > The way an `istr` is represented is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 
 ```
 istr.repr_mode('str')
 five = istr('5')
 print(repr(five))
@@ -563,32 +589,32 @@
 will print
 ```
 istr('001')
 istr('012')
 istr('123')
 istr('1234')
 ```
-> [!NOTE]
->
->  if a string is used to initialize an istr AND that string can be interpreted as an int. the string will reformatted:
->
-> ```
-> with istr.int_format('03'):
->     print(repr(istr('  12 ')))
-> ```
->
-> will result in
->
-> ```
-> istr('0012')
-> ```
-
-> [!NOTE]
+> > [!NOTE]
+> >
+> > if a string is used to initialize an istr AND that string can be interpreted as an int. the string will reformatted:
+> >
+> > ```
+> > with istr.int_format('03'):
+> >    print(repr(istr(12)))
+> > ```
+> >
+> > will result in
+> >
+> > ```
+> > istr('0012')
+> > ```
 >
-> For bases other than 10, the string will never be reformatted!
+> > [!NOTE]
+> >
+> > For bases other than 10, the string will never be reformatted!
 
 ### Overview of operations
 
 The table below shows whether the string or the int version of istr is applied.
 
 ```
 operator/function   int  str   Example
```

### Comparing `istr_python-1.0.0/istr/istr.py` & `istr_python-1.0.0.post0/istr/istr.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,93 +6,15 @@
 # strings you can count on
 
 __version__ = "1.0.0"
 import functools
 import math
 
 """
-changelog
-
-version 1.0.0 2024-05-06
-------------------------
-With this version, istrs do not have to be interpretable as an int anymore.
-Only when arithmetic and friends are to be carried with an istr, that's a requirement.
-
-So now we can say
-    a = istr('1 2 3')
-    print(a.split())
-and get
-    [istr('1'), istr('2'), istr('3')]
-But
-    a = istr('1 2 3')
-    b = a + 1
-will raise
-    TypeError: unsupported operand for +: istr('1 2 3') and 1
-    
-It is possible to check if an istr can be interpreted as an int with the is_int method:
-    a = istr('1 2 3')
-    print(a.is_int()) 
-will give
-    False 
-    
-This also means that there is no reason for istr('') to be interpretable as 0. So it isn't anymore.
-And reversed() now also works with negative numbers, although the result can't be used in calculations.
-
-The method / context manager format has been renamed to int_format.
-
-The bool method now operates on the string if it can not be interpreted as an int.
-That means that bool(istr('')) is False. For any other istr where is_int() is True, bool will be True.
-
-version 0.2.0 2024-04-30
-----------------------
-Added __iter__ method__ .
-    So now,
-        for c in istr('123'):
-            ...
-        results in c values that are istrs 
-
-Added istr.digits method:
-Examples
---------
-istr.digits() ==> istr('0123456789')
-istr.digits('') ==> istr('0123456789')
-istr.digits('1') ==> istr('1')
-istr.digits('3-') ==> istr('3456789')
-istr.digits('-3') ==> istr('0123')
-istr('1-4', '6', '8-9') ==> istr('1234689')
-istr.digits('1', '1-2', '1-3') ==> istr('112123')
-
-    Note that a digit can occur more than once.
-
-version 0.1.2  2024-04-26  
--------------------------
-Added all relevant string methods to return istrs or data structures with istrs.
-Added corresponding tests.
-
-version 0.1.0  2024-04-22  
--------------------------
-Changed the way istr.range is implemennted.
-
-Changed the context manager istr.format() to be used directly without the with statement.
-Also, noww istr.format() works without any argument and then returns the current format.
-
-istr class now uses __slots__
-
-All internal values and methods now start with an underscore.
-
-Introduced istr.repr_mode()
-
-Introduced istr.base()
-
-Extended tests for new functionality
-
-
-version 0.0.8  2024-04-18  
--------------------------
-initial version with changelog
+Note: the changelog is now in changelog.md
 """
 
 
 class _range:
     """
     based on https://codereview.stackexchange.com/questions/229073/pure-python-range-implementation
     """
@@ -269,14 +191,15 @@
     __slots__ = ("_as_int", "_as_repr")
 
     _int_format = ""
     _repr_mode = "istr"
     _base = 10
     _nan = "nan"
     _force_istr_repr = False
+    _digits_cache = {}
 
     @staticmethod
     def _to_base(number, base):
         if number < 0:
             raise ValueError(f"negative numbers are not allowed for base {base}")
         result = ""
         while number:
@@ -520,14 +443,17 @@
         self._check_is_int("is_even")
         return self._as_int % 2 == 0
 
     def is_odd(self):
         self._check_is_int("is_odd")
         return self._as_int % 2 == 1
 
+    def all_distinct(self):
+        return len(self) == len(set(self))
+
     def is_int(self):
         return self._as_int != self._nan
 
     def reversed(self):
         return self[::-1]
 
     def __getitem__(self, key):
@@ -604,69 +530,82 @@
             self.saved_cls._base = self.saved_base
 
     @classmethod
     def range(cls, start, stop=None, step=1):
         return _range(cls, start, stop, step)
 
     @classmethod
-    @functools.lru_cache
     def digits(cls, *args):
         """
         return an istr of istr'ed digits as specified with args
 
         if no args, 0-9 will be used
 
         all given args will be used
         each arg has to be either null string, <digit>, <digit>-<digit> or -<digit>
 
-        examples
+        the digits may be '0' through '9' and 'A' through 'Z' (not case sensitive)
+        The returned value will always be in uppercase (if applicable).
+
+        Examples
         --------
         istr.digits() ==> istr('0123456789')
         istr.digits('') ==> istr('0123456789')
         istr.digits('1') ==> istr('1')
         istr.digits('3-') ==> istr('3456789')
         istr.digits('-3') ==> istr('0123')
         istr('1-4', '6', '8-9') ==> istr('1234689')
         istr('1', '1-2', '1-3') ==> istr('11213')
+        istr.digits('-z') ==> istr('0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ')
+        istr.digits('C') ==> istr('C')
+        istr.digits('A-F') ==> istr('ABCDEF')
+        istr.digits('X-') ==> istr('XYZ')
 
         Note
         ----
         A digit can occur more than once.
-
         """
+        key = (args, cls._base, cls._int_format, cls._repr_mode)
+        if key in cls._digits_cache:
+            return cls.digits_cache[key]
+        sequence = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ"
         result = []
         if not args:
             args = ["0-9"]
         for arg in args:
             if arg.strip() == "":
                 arg = "0-9"
-            pre, *post = arg.split("-")
+            pre, *post = arg.split("-", 1)
             if pre.strip() == "":
                 pre = "0"
-            try:
-                start = int(pre)
-            except ValueError:
-                raise ValueError(f"incorrect specifier: {repr(arg)}")
-            if not 0 <= start <= 9:
-                raise ValueError(f"incorrect specifier: {repr(arg)}")
-            if len(post) > 1:
+            pre = pre.upper()
+            if len(pre) > 1 or pre not in sequence:
                 raise ValueError(f"incorrect specifier: {repr(arg)}")
+            start = sequence.index(pre)
+
             if post:
-                if post[0].strip() == "":
-                    post = "9"
-                try:
-                    stop = int(post[0])
-                except ValueError:
+                post = post[0]
+                if post.strip() == "":
+                    if pre in "0123456789":
+                        post = "9"
+                    else:
+                        post = "Z"
+                post = post.upper()
+                if len(post) > 1 or post not in sequence:
                     raise ValueError(f"incorrect specifier: {repr(arg)}")
-                if (not 0 <= start <= 9) or start > stop:
+                stop = sequence.index(post)
+                if start > stop:
                     raise ValueError(f"incorrect specifier: {repr(arg)}")
             else:
                 stop = start
-            result.extend(range(start, stop + 1))
-        return cls("").join(istr(result))
+            result.extend(sequence[i] for i in range(start, stop + 1))
+
+        result = istr("".join(result))
+        cls._digits_cache[key] = result
+        return result
 
     def capitalize(self, *args, **kwargs):
         return self.__class__(super().capitalize(*args, **kwargs))
 
     def casefold(self, *args, **kwargs):
         return self.__class__(super().casefold(*args, **kwargs))
 
@@ -736,9 +675,10 @@
     def zfill(self, *args, **kwargs):
         return self.__class__(super().zfill(*args, **kwargs))
 
 
 def main():
     ...
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `istr_python-1.0.0/istr_python.egg-info/PKG-INFO` & `istr_python-1.0.0.post0/istr_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 1.0.0
+Version: 1.0.0.post0
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
  <img src="https://www.salabim.org/istr_logo.png" width=500>
 
 ### Introduction
 
-The istr module has exactly one class: istr.
-
-With this it is possible to interpret strings as if they were integers.
+With  `istr` is possible to interpret strings as if they were integers.
 
 This can be very handy for solving puzzles, but also for other purposes.
 For instance the famous send more money puzzle, where each letter has to be replaced by a unique digit (0-9)
 
 ```
   S E N D
   M O R E
@@ -93,15 +91,15 @@
 
 or
 
 ```
 twenty = four * 5
 ```
 
-And now `twenty` can be used as if it was an int as well. So:
+And now `twenty` can be used as if it was an int as well. So
 
 ```
 twenty - four
 ```
 
 is `istr('16')`
 
@@ -109,22 +107,22 @@
 
 ```
 -four + (twenty / 2)
 ```
 
 is `istr('6')`
 
-And we can test for equality, So:
+And we can test for equality. So:
 
 ```
 twenty == 20
 ```
 is True.
 
-But as istrs are also strings. So
+But istrs are also strings. So
 
 ```
 twenty == '20'
 ```
 
 is also True!
 
@@ -137,60 +135,64 @@
 ```
 are `True`.
 
 In contrast to an ordinary string
 ```
 print(four + five)
 ```
-prints `9`, as istr are treated as ints.
+prints `9`, as istr are treated as ints (if possible).
 
 Please note that `four`  could have also been initialized with
 ```
 four = istr(4)
 ```
 or even
 ```
 four, five = istr(4, 5)
 ```
 
-> [!NOTE]
->
-> All calculations are strictly integer calculations. That means that if a float variale is ever produced it will be converted to an int.
-> Also divisions are always floor divisions!
+> > [!IMPORTANT]
+> >
+> > All calculations are strictly integer calculations. That means that if a float or decimal variable is ever produced it will be converted to an int.
+> > Also divisions are always floor divisions!
 
 #### Use istrs as string
 
 We should realize that istrs are in fact strings.
 
-In order to concatenate two istrs (or an istr and a str), we cannot use the `four + five` operator as
-
-that would be `istr(9)`.
+In order to concatenate two istrs (or an istr and a str), we cannot use the `+` operator (remember `four + five` is `istr('9')`).
 
 In order to concatenate istrs,  we use the or operator (`|`). So
 
 ```
 four | five
 ```
 will be `istr(`45`).
 
-That means that
+And
 ```
 (four | five) / 3
 ```
 is `istr('9')`.
 
-In order to repeat a string in the usual sense, you cannot use `3 * four`, as that would be `12`. 
+In order to repeat a string in the usual sense, you cannot use the `*` operator (remember `3 * four` is `istr(12)`. 
 
 In order to repeat we use the matrix multiplication operator (`@`). So
 
  `3 @ four`
 
- is istr(`444`). As is `four @ 3`.
+ is `istr('444')`
+
+And 
+
+```four @ 3```
+
+is also `istr('444')`
 
-> [!NOTE]
+> Note:
 >
 > It is not allowed to use the `@` operator for two istrs. So, `four @ five` raises a TypeError.
 
 #### istrs that can't be interpreted as an int
 
 Although usualy, istrs are to be interpreted as an int, that's not a requirement.
 
@@ -199,52 +201,52 @@
 ```
 istr('abc')
 ```
 
 or
 
 ```
-istr(1,2,3)
+istr('1,2,3')
 ```
 
 are accepted.
 
 But, we can't do any arithmetic with them. 
 
 If we try
 
 ```
 istr('abc') + 5
 ```
 
-a TypeError will be raised.
+a `TypeError` will be raised.
 
 That holds for any arithmetic we try.
 
 If we want to test if an istr can be interpreted (and thus used in an arithmetic expression). we can use the `is_int()` method. So
 
 ```ìstr(20).is_int()```
 
-is `True`, wherea
+is `True`, whereas
 
 ```ìstr('abc').is_int()```
 
 is `False`.
 
 
 
 The bool operator works normally on the integer value of an istr. So
 
 `bool(istr('0'))` ==> `False`
 `bool(istr('1'))` ==> `True`
 
-If the istr can't be interpreted as an int, the string will be used to test. So
+If the istr can't be interpreted as an int, the string value will be used to test. So
 
-`bool(istr('abc'))` ==> `False`
-`bool(istr(''))` ==> `True`
+`bool(istr('abc'))` ==> `True`
+`bool(istr(''))` ==> `False`
 
 #### Other operators
 
 For the `in` operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
 
 ```
 '34' in istr(1234)
@@ -275,15 +277,15 @@
 
 is 
 
 ```
 '0 1 2 3 4 5 6 7 8 9 10 11'
 ```
 
-#### Using other values for istr than numeric value or str
+#### Using values to inialitize istr other than numeric value or str
 Apart from with simple numeric (to be interpreted as an int) or str, istr can be initialized with
 several other types:
 
 - if a dict (or subtype of dict), the same type dict will be returned with all *values* istr'ed
 
     ```
     istr({0: 0, 1: 1, 2: 4}) ==> {0: istr('0'), 1: istr('1'), 2: istr('4')}
@@ -304,15 +306,15 @@
     istr({0, 1, 4}) ==> `{istr('4'), istr('0'), istr('1')}  # or similar
     ```
 
 - if a range, an istr.range instance will be returned
   
     ```
   istr(range(3))` ==> `istr.range(3)
-    list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]
+  list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]
   len(istr(range(3)))` ==> `3
   ```
 
 - if an istr.range instance, the same istr.range will be returned
 
 - if an istr, the same istr will be used
 
@@ -326,48 +328,62 @@
 to unpack multiple values, e.g.
 
 ```
 a, b, c = istr(5, 6, 7) ==> a=istr('5') , b=istr('6'), c=istr('7') 
 ```
 
 #### test for even/odd
-It is possible to test for even/odd (provided the istt can be interpreted as an int) with the
+It is possible to test for even/odd (provided the istr can be interpreted as an int) with the
 
 `is_even` and `is_odd` method, e.g.
 
 ```
 istr(4).is_even()) ==> True
 istr(5).is_odd()) ==> True
 ```
+#### test whether all characters are distinct
+
+With the `all_distinct` method, it is possible to test whether all characters are distinct (i.e. no character appearts more than once).
+
+```
+istr('01234').all_distict() ==> True
+istr('012340').all_distict() ==> False
+n98 = istr(98)
+n100 = n98 + 2
+istr(n98).all_distinct() ==> True
+istr(n100).all_distinct() ==> False
+```
+
 #### reverse an istr
+
 The method `istr.reversed()` will return the an istr with the reversed content:
 ```
 istr(456).reversed() ==> istr('654')
 istr('0456').reversed() ==> istr('6540')
 ```
 The same can -of course- be achieved with
 ```
 istr(456)[::-1] ==> istr('654')
 istr('0456')[::-1] ==> istr('6540')
 ```
-> [!NOTE]
->
-> It is possible to reverse a negative istr, but the result can't be interpreted as an int anymore.
->
-> ```
-> istr(-456) ==> TypeError
-> ```
+> > [!NOTE]
+> >
+> > It is possible to reverse a negative istr, but the result can't be interpreted as an int anymore.
+> >
+> > ```
+> > istr(-456) ==> TypeError
+> > ```
 
 #### enumerate with istrs
 
 The `istr.enumerate` method can be used just as the builtin enumerate function.
 The iteration counter however is an istr rather than an int. E.g. 
 
 ```
-    for i,c in istr.enumerate('abc'):
+    for i, c in istr.enumerate('abc'):
         print(f'{repr(i)} {c}')
 ```
 prints
 ```
 istr('0') a
 istr('1') b
 istr('2') c
@@ -387,38 +403,48 @@
 ```
 
 #### generate istr with digits
 
 The class method `digits` can be used to return an istr of digits according to a given specification.
 The method takes either no or a number of arguments.
 
-If no arguments are given, the result will be istr('0123456789').
+If no arguments are given, the result will be `istr('0123456789')`.
 
 The given argument(s) result in a range of digits.
 
 - `<n>` ==> n
 - `<n-m>` ==> n, n+1, ..., m
 - `-n>` ==> 0, 1, ... n
 - `n->` ==> n, n+1, ..., 9
 - `''` ==> 0, 1, ..., 9
 
-(n and m must be digits between 0 and 9)
+(n and m must be digits between 0 and 9 or letters letters between A and Z)
+
+When no stop value is specified, it will be
+
+* 9 if the start value is between 0 and 9
+* Z if the start value is between A and Z 
 
 The final result is an istr composed of the given range(s).
 
 Here are some examples:
 
 ```
 istr.digits() ==> istr('0123456789')
 istr.digits('') ==> istr('0123456789')
 istr.digits('1') ==> istr('1')
 istr.digits('3-') ==> istr('3456789')
 istr.digits('-3') ==> istr('0123')
 istr('1-4', '6', '8-9') ==> istr('1234689')
 istr('1', '1-2', '1-3') ==> istr('11213')
+istr.digits('-z') ==> istr('0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ')
+istr.digits('A-F') ==> istr('ABCDEF')
+istr.digits('C') ==> istr('C')
+istr.digits('3-') ==> istr('34567879')
+istr.digits('X-') ==> istr('XYZ')
 ```
 
 
 #### Subclassing istr
 When a class is derived from istr, all methods will return that newly derived class. 
 
 E.g.
@@ -430,26 +456,26 @@
 ```
 will print `jstr('20')`
 
 #### Changing the way repr works
 
 It is possible to control the way an `istr` instance will be repr'ed.
 
-By default, the `istr('5')` is represented as `istr('5')`.
+By default, the `istr(5)` is represented as `istr('5')`.
 
 With the istr.repr_mode() context manager, that can be changed:
 ```
 with istr.repr_mode('str'):
-    five = istr('5')
+    five = istr(5)
     print(repr(five))
 with istr.repr_mode('int'):
-    five = istr('5')
+    five = istr(5)
     print(repr(five))
 with istr.repr_mode('istr'):
-    five = istr('5')
+    five = istr(5)
     print(repr(five))
 ```
 This will print
 ```
 '5'
 5
 istr('5')
@@ -464,17 +490,17 @@
 
 This will print
 
 ```
 nan
 ```
 
-> [!NOTE]
->
-> The way an `istr` is represented is determined at initialization.
+> > [!NOTE]
+> >
+> > The way an `istr` is represented is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 
 ```
 istr.repr_mode('str')
 five = istr('5')
 print(repr(five))
@@ -576,32 +602,32 @@
 will print
 ```
 istr('001')
 istr('012')
 istr('123')
 istr('1234')
 ```
-> [!NOTE]
->
->  if a string is used to initialize an istr AND that string can be interpreted as an int. the string will reformatted:
->
-> ```
-> with istr.int_format('03'):
->     print(repr(istr('  12 ')))
-> ```
->
-> will result in
->
-> ```
-> istr('0012')
-> ```
-
-> [!NOTE]
+> > [!NOTE]
+> >
+> > if a string is used to initialize an istr AND that string can be interpreted as an int. the string will reformatted:
+> >
+> > ```
+> > with istr.int_format('03'):
+> >    print(repr(istr(12)))
+> > ```
+> >
+> > will result in
+> >
+> > ```
+> > istr('0012')
+> > ```
 >
-> For bases other than 10, the string will never be reformatted!
+> > [!NOTE]
+> >
+> > For bases other than 10, the string will never be reformatted!
 
 ### Overview of operations
 
 The table below shows whether the string or the int version of istr is applied.
 
 ```
 operator/function   int  str   Example
```

### Comparing `istr_python-1.0.0/pyproject.toml` & `istr_python-1.0.0.post0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "istr-python"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "istr - strings you can count on"
-version = "1.0.0"
+version = "1.0.0-0"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
@@ -20,7 +20,10 @@
 ]
 [project.urls]
 Homepage = "https://github.com/salabim/istr"
 Repository = "https://github.com/salabim/istr"
 
 [tool.setuptools]
 packages = ["istr"]
+
+[tool.setuptools.package-data]
+"*" = ["../*.md"]
```

### Comparing `istr_python-1.0.0/tests/test_istr.py` & `istr_python-1.0.0.post0/tests/test_istr.py`

 * *Files 2% similar despite different names*

```diff
@@ -544,15 +544,34 @@
     assert istr.digits().equals(istr("0123456789"))
     assert istr.digits("").equals(istr("0123456789"))
     assert istr.digits("1").equals(istr("1"))
     assert istr.digits("3-").equals(istr("3456789"))
     assert istr.digits("-3").equals(istr("0123"))
     assert istr.digits("1-4", "6", "8-9").equals(istr("1234689"))
     assert istr.digits("1", "1-2", "1-3").equals(istr("112123"))
+    a= istr.digits("a")
+    assert a.equals(istr("A"))
+    assert not a.is_int()
+    with istr.base(36): 
+        a=istr.digits("a")
+        assert a == 10
+        assert a =="A"
+        assert istr.digits("-a").equals(istr("0123456789A"))
+        assert istr.digits("x-").equals(istr("XYZ"))
+        assert istr.digits("B-d").equals(istr("BCD"))
+        assert istr.digits("-").equals(istr("0123456789"))
+    with istr.base(16):
+        ef = istr.digits("e-f")
+        assert (ef+1).equals(istr("F0"))
+        assert ef == 239
 
+def test_all_distinct():
+    assert istr("abcdef").all_distinct()
+    assert not istr("aabcdef").all_distinct()
+    assert istr("").all_distinct()
 
 def test_subclassing():
     class jstr(istr):
         ...
 
     assert jstr(5).equals(jstr(5))
     assert repr(jstr(*range(3))) == "(jstr('0'), jstr('1'), jstr('2'))"
```

