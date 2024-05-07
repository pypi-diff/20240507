# Comparing `tmp/arch_flow-0.1.4.tar.gz` & `tmp/arch_flow-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch_flow-0.1.4.tar", last modified: Sat Apr 27 03:10:55 2024, max compression
+gzip compressed data, was "arch_flow-0.1.5.tar", last modified: Tue May  7 01:34:18 2024, max compression
```

## Comparing `arch_flow-0.1.4.tar` & `arch_flow-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 03:10:55.068301 arch_flow-0.1.4/
--rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.4/LICENCE
--rw-rw-rw-   0        0        0      981 2024-04-27 03:10:55.067299 arch_flow-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6622 2024-04-25 23:30:53.000000 arch_flow-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 03:10:54.973144 arch_flow-0.1.4/arch_flow/
--rw-rw-rw-   0        0        0     4361 2024-04-26 04:45:37.000000 arch_flow-0.1.4/arch_flow/ArchFlow.py
--rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.4/arch_flow/DirectoryCreator.py
--rw-rw-rw-   0        0        0     3301 2024-04-21 06:07:10.000000 arch_flow-0.1.4/arch_flow/DirectoryExplorer.py
--rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.4/arch_flow/StringManipulator.py
--rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.4/arch_flow/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 03:10:55.013299 arch_flow-0.1.4/arch_flow/exceptions/
--rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.4/arch_flow/exceptions/ExceptionHandler.py
--rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.4/arch_flow/exceptions/FileOrDirectoryExistsError.py
--rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.4/arch_flow/exceptions/NotFoundException.py
-drwxrwxrwx   0        0        0        0 2024-04-27 03:10:55.040329 arch_flow-0.1.4/arch_flow/implementations/
--rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.4/arch_flow/implementations/DirectoryCreatorImplementation.py
--rw-rw-rw-   0        0        0     7196 2024-04-21 05:43:57.000000 arch_flow-0.1.4/arch_flow/implementations/DirectoryExplorerImplementation.py
--rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.4/arch_flow/implementations/StringManipulatorImplementation.py
-drwxrwxrwx   0        0        0        0 2024-04-27 03:10:55.049329 arch_flow-0.1.4/arch_flow/output/
--rw-rw-rw-   0        0        0     2372 2024-03-15 22:56:29.000000 arch_flow-0.1.4/arch_flow/output/OutputHandler.py
-drwxrwxrwx   0        0        0        0 2024-04-27 03:10:55.064301 arch_flow-0.1.4/arch_flow/utils/
--rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.4/arch_flow/utils/DirectoryExplorerUtil.py
--rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.4/arch_flow/utils/Filter.py
-drwxrwxrwx   0        0        0        0 2024-04-27 03:10:55.066303 arch_flow-0.1.4/arch_flow.egg-info/
--rw-rw-rw-   0        0        0      981 2024-04-27 03:10:54.000000 arch_flow-0.1.4/arch_flow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      743 2024-04-27 03:10:54.000000 arch_flow-0.1.4/arch_flow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 03:10:54.000000 arch_flow-0.1.4/arch_flow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-27 03:10:54.000000 arch_flow-0.1.4/arch_flow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-27 03:10:54.000000 arch_flow-0.1.4/arch_flow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 03:10:55.068301 arch_flow-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1182 2024-04-27 03:00:32.000000 arch_flow-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:34:18.975493 arch_flow-0.1.5/
+-rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.5/LICENCE
+-rw-rw-rw-   0        0        0      981 2024-05-07 01:34:18.974494 arch_flow-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6622 2024-04-25 23:30:53.000000 arch_flow-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 01:34:18.902733 arch_flow-0.1.5/arch_flow/
+-rw-rw-rw-   0        0        0     4419 2024-05-07 01:28:08.000000 arch_flow-0.1.5/arch_flow/ArchFlow.py
+-rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.5/arch_flow/DirectoryCreator.py
+-rw-rw-rw-   0        0        0     3301 2024-05-04 03:27:18.000000 arch_flow-0.1.5/arch_flow/DirectoryExplorer.py
+-rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.5/arch_flow/StringManipulator.py
+-rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.5/arch_flow/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:34:18.932392 arch_flow-0.1.5/arch_flow/exceptions/
+-rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.5/arch_flow/exceptions/ExceptionHandler.py
+-rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.5/arch_flow/exceptions/FileOrDirectoryExistsError.py
+-rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.5/arch_flow/exceptions/NotFoundException.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:34:18.959555 arch_flow-0.1.5/arch_flow/implementations/
+-rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.5/arch_flow/implementations/DirectoryCreatorImplementation.py
+-rw-rw-rw-   0        0        0     7196 2024-04-21 05:43:57.000000 arch_flow-0.1.5/arch_flow/implementations/DirectoryExplorerImplementation.py
+-rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.5/arch_flow/implementations/StringManipulatorImplementation.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:34:18.961983 arch_flow-0.1.5/arch_flow/output/
+-rw-rw-rw-   0        0        0     2372 2024-03-15 22:56:29.000000 arch_flow-0.1.5/arch_flow/output/OutputHandler.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:34:18.971494 arch_flow-0.1.5/arch_flow/utils/
+-rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.5/arch_flow/utils/DirectoryExplorerUtil.py
+-rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.5/arch_flow/utils/Filter.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:34:18.973493 arch_flow-0.1.5/arch_flow.egg-info/
+-rw-rw-rw-   0        0        0      981 2024-05-07 01:34:18.000000 arch_flow-0.1.5/arch_flow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2024-05-07 01:34:18.000000 arch_flow-0.1.5/arch_flow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 01:34:18.000000 arch_flow-0.1.5/arch_flow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 01:34:18.000000 arch_flow-0.1.5/arch_flow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-07 01:34:18.000000 arch_flow-0.1.5/arch_flow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 01:34:18.975493 arch_flow-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1182 2024-05-07 01:28:08.000000 arch_flow-0.1.5/setup.py
```

### Comparing `arch_flow-0.1.4/LICENCE` & `arch_flow-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/PKG-INFO` & `arch_flow-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.4
+Version: 0.1.5
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `arch_flow-0.1.4/README.md` & `arch_flow-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/arch_flow/ArchFlow.py` & `arch_flow-0.1.5/arch_flow/ArchFlow.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,17 @@
         if args:
             content = self.StringManipulator.replace_args(content, args)
         content = self.StringManipulator.replace_tags(content)
         self.DirectoryCreator.create_file(file_destination, file_name, content)
 
     @staticmethod
     def handle_args():
-        args_input = sys.argv
-        return args_input[1:]
+        args_input = sys.argv[1:]
+        args_lower = [arg.lower() for arg in args_input]
+        return args_lower
 
     def handler_input(self, args, json_content):
         if len(args) == 0:
             self.OutputHandler.information_message("Whoopsie-daisy! It seems like you forgot to provide a function. "
                                                "How about trying --help for some magic commands?")
             return None
         name_function = args[0]
```

### Comparing `arch_flow-0.1.4/arch_flow/DirectoryCreator.py` & `arch_flow-0.1.5/arch_flow/DirectoryCreator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/arch_flow/DirectoryExplorer.py` & `arch_flow-0.1.5/arch_flow/DirectoryExplorer.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/arch_flow/StringManipulator.py` & `arch_flow-0.1.5/arch_flow/StringManipulator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/arch_flow/exceptions/ExceptionHandler.py` & `arch_flow-0.1.5/arch_flow/exceptions/ExceptionHandler.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/arch_flow/exceptions/FileOrDirectoryExistsError.py` & `arch_flow-0.1.5/arch_flow/exceptions/FileOrDirectoryExistsError.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/arch_flow/exceptions/NotFoundException.py` & `arch_flow-0.1.5/arch_flow/exceptions/NotFoundException.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/arch_flow/implementations/DirectoryCreatorImplementation.py` & `arch_flow-0.1.5/arch_flow/implementations/DirectoryCreatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/arch_flow/implementations/DirectoryExplorerImplementation.py` & `arch_flow-0.1.5/arch_flow/implementations/DirectoryExplorerImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/arch_flow/implementations/StringManipulatorImplementation.py` & `arch_flow-0.1.5/arch_flow/implementations/StringManipulatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/arch_flow/output/OutputHandler.py` & `arch_flow-0.1.5/arch_flow/output/OutputHandler.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/arch_flow/utils/Filter.py` & `arch_flow-0.1.5/arch_flow/utils/Filter.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/arch_flow.egg-info/PKG-INFO` & `arch_flow-0.1.5/arch_flow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.4
+Version: 0.1.5
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `arch_flow-0.1.4/arch_flow.egg-info/SOURCES.txt` & `arch_flow-0.1.5/arch_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.4/setup.py` & `arch_flow-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='arch-flow',
-    version='0.1.4',
+    version='0.1.5',
     license='MIT License',
     author='Carlos Vinicius Da Silva',
     long_description="O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações. Inspirado no conceito de peças de Lego, o ArchFlow oferece uma variedade de módulos independentes, cada um com funcionalidades específicas. Esses módulos podem ser combinados de forma flexível para atender às necessidades de automação de diferentes projetos. Com uma arquitetura modular e uma ampla gama de funções, o ArchFlow permite aos desenvolvedores criar soluções eficientes e personalizadas, reduzindo o tempo e esforço necessários para o desenvolvimento de software.",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='arch flow',
     description=u'O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.',
```

