# Comparing `tmp/Hebill_Pypi-1.0.0-py3-none-any.whl.zip` & `tmp/Hebill_Pypi-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5472 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     1079 b- defN 24-May-07 01:17 hebill_pypi/README.MD
+Zip file size: 5554 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     1132 b- defN 24-May-07 02:06 hebill_pypi/README.MD
 -rw-rw-rw-  2.0 fat       50 b- defN 24-May-07 01:37 hebill_pypi/__init__.py
--rw-rw-rw-  2.0 fat      306 b- defN 24-May-07 00:52 hebill_pypi/constants.py
+-rw-rw-rw-  2.0 fat      306 b- defN 24-May-07 02:08 hebill_pypi/constants.py
 -rw-rw-rw-  2.0 fat     9555 b- defN 24-May-07 01:46 hebill_pypi/core.py
--rw-rw-rw-  2.0 fat     1336 b- defN 24-May-07 01:51 Hebill_Pypi-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 01:51 Hebill_Pypi-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-May-07 01:51 Hebill_Pypi-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      626 b- defN 24-May-07 01:51 Hebill_Pypi-1.0.0.dist-info/RECORD
-8 files, 13056 bytes uncompressed, 4380 bytes compressed:  66.5%
+-rw-rw-rw-  2.0 fat     1420 b- defN 24-May-07 02:08 Hebill_Pypi-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 02:08 Hebill_Pypi-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-May-07 02:08 Hebill_Pypi-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      626 b- defN 24-May-07 02:08 Hebill_Pypi-1.0.1.dist-info/RECORD
+8 files, 13193 bytes uncompressed, 4462 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: hebill_pypi/constants.py
 Comment: 
 
 Filename: hebill_pypi/core.py
 Comment: 
 
-Filename: Hebill_Pypi-1.0.0.dist-info/METADATA
+Filename: Hebill_Pypi-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: Hebill_Pypi-1.0.0.dist-info/WHEEL
+Filename: Hebill_Pypi-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: Hebill_Pypi-1.0.0.dist-info/top_level.txt
+Filename: Hebill_Pypi-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: Hebill_Pypi-1.0.0.dist-info/RECORD
+Filename: Hebill_Pypi-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hebill_pypi/README.MD

```diff
@@ -35,12 +35,12 @@
     AUTHOR_URL = 'http://www.project.url/'
     ```
 3. 编写 pypi.py 内容
    ```python
    from hebill_pypi import Pypi
    import myProject
    
-   pypi = Pypi(myProject)
+   pypi = Pypi(myProject, r'D:\SDK\Environments\myProject\Scripts\python.exe')
    pypi.pack()
    ```
 
 4. 运行 pypi.py
```

## hebill_pypi/constants.py

```diff
@@ -1,8 +1,8 @@
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 NAME = 'Hebill Pypi'
 DESCRIPTION = 'Pack and upload the python projects to pypi.com'
 LONG_DESCRIPTION = 'README.MD'
 LONG_DESCRIPTION_TYPE = 'text/markdown'
 URL = 'http://www.hebill.net/'
 AUTHOR = 'He Bill'
 AUTHOR_EMAIL = 'hebill@hebill.net'
```

## Comparing `Hebill_Pypi-1.0.0.dist-info/METADATA` & `Hebill_Pypi-1.0.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: Hebill-Pypi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pack and upload the python projects to pypi.com
 Requires-Python: >=3.12
 Description-Content-Type: text/plain
 Requires-Dist: twine ==5.0.0
+Requires-Dist: wheel ==0.43.0
 
 ## 说明
 快速打包上传到项目到 pypi.org。  
 模块在WIN系统pyCharm中测试，不做其他环境使用。
 
 ## 设置 .pypi
 在你的/~user/里面创建 .pypi，用记事本编辑以下内容并保存
@@ -43,12 +44,12 @@
     AUTHOR_URL = 'http://www.project.url/'
     ```
 3. 编写 pypi.py 内容
    ```python
    from hebill_pypi import Pypi
    import myProject
    
-   pypi = Pypi(myProject)
+   pypi = Pypi(myProject, r'D:\SDK\Environments\myProject\Scripts\python.exe')
    pypi.pack()
    ```
 
 4. 运行 pypi.py
```

