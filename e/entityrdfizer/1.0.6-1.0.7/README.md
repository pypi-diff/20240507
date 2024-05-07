# Comparing `tmp/entityrdfizer-1.0.6.tar.gz` & `tmp/entityrdfizer-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\entityrdfizer-1.0.6.tar", last modified: Tue Apr  5 23:17:53 2022, max compression
+gzip compressed data, was "entityrdfizer-1.0.7.tar", last modified: Tue May  7 15:34:01 2024, max compression
```

## Comparing `entityrdfizer-1.0.6.tar` & `entityrdfizer-1.0.7.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/
--rw-rw-rw-   0        0        0     1168 2022-04-05 14:29:34.000000 entityrdfizer-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      163 2022-04-05 14:29:34.000000 entityrdfizer-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3734 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2804 2022-04-05 14:29:34.000000 entityrdfizer-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/entityrdfizer/
--rw-rw-rw-   0        0        0       19 2022-04-05 14:29:34.000000 entityrdfizer-1.0.6/entityrdfizer/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/entityrdfizer/aboxgenerator/
--rw-rw-rw-   0        0        0     1573 2022-04-05 14:29:34.000000 entityrdfizer-1.0.6/entityrdfizer/aboxgenerator/ABoxGeneration.py
--rw-rw-rw-   0        0        0    12482 2022-04-05 14:29:34.000000 entityrdfizer-1.0.6/entityrdfizer/aboxgenerator/ABoxTemplateCSVFileToRDF.py
--rw-rw-rw-   0        0        0      968 2022-04-05 14:29:34.000000 entityrdfizer-1.0.6/entityrdfizer/aboxgenerator/ABoxTemplateCSVFilesToRDF.py
--rw-rw-rw-   0        0        0     2544 2022-04-05 14:29:34.000000 entityrdfizer-1.0.6/entityrdfizer/aboxgenerator/PropertyReader.py
--rw-rw-rw-   0        0        0        0 2022-04-05 14:29:34.000000 entityrdfizer-1.0.6/entityrdfizer/aboxgenerator/__init__.py
--rw-rw-rw-   0        0        0      523 2022-04-05 14:29:34.000000 entityrdfizer-1.0.6/entityrdfizer/aboxgenerator/csv2abox.py
--rw-rw-rw-   0        0        0      523 2022-04-05 14:29:34.000000 entityrdfizer-1.0.6/entityrdfizer/app.py
-drwxrwxrwx   0        0        0        0 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/entityrdfizer/conf/
--rw-rw-rw-   0        0        0      274 2022-04-05 14:29:34.000000 entityrdfizer-1.0.6/entityrdfizer/conf/EntityRDFizer.properties
--rw-rw-rw-   0        0        0      698 2022-04-05 23:02:38.000000 entityrdfizer-1.0.6/entityrdfizer/driver.py
-drwxrwxrwx   0        0        0        0 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/entityrdfizer/javagateway/
--rw-rw-rw-   0        0        0        0 2022-04-05 14:29:35.000000 entityrdfizer-1.0.6/entityrdfizer/javagateway/__init__.py
--rw-rw-rw-   0        0        0      100 2022-04-05 14:29:35.000000 entityrdfizer-1.0.6/entityrdfizer/javagateway/gateway.py
-drwxrwxrwx   0        0        0        0 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/entityrdfizer/tboxgenerator/
--rw-rw-rw-   0        0        0        0 2022-04-05 14:29:35.000000 entityrdfizer-1.0.6/entityrdfizer/tboxgenerator/__init__.py
--rw-rw-rw-   0        0        0     1840 2022-04-05 14:29:35.000000 entityrdfizer-1.0.6/entityrdfizer/tboxgenerator/csv2tbox.py
-drwxrwxrwx   0        0        0        0 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/entityrdfizer.egg-info/
--rw-rw-rw-   0        0        0     3734 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/entityrdfizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/entityrdfizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/entityrdfizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/entityrdfizer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/entityrdfizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/entityrdfizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-04-05 23:17:53.000000 entityrdfizer-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      799 2022-04-05 23:17:17.000000 entityrdfizer-1.0.6/setup.py
+drwxr-xr-x   0 sm453     (1000) sm453     (1000)        0 2024-05-07 15:34:01.272311 entityrdfizer-1.0.7/
+-rw-r--r--   0 sm453     (1000) sm453     (1000)     1162 2022-02-17 15:59:51.000000 entityrdfizer-1.0.7/LICENSE
+-rw-r--r--   0 sm453     (1000) sm453     (1000)      160 2022-02-17 15:59:51.000000 entityrdfizer-1.0.7/MANIFEST.in
+-rw-r--r--   0 sm453     (1000) sm453     (1000)     6783 2024-05-07 15:34:01.272311 entityrdfizer-1.0.7/PKG-INFO
+-rw-r--r--   0 sm453     (1000) sm453     (1000)     5331 2024-05-07 11:51:08.000000 entityrdfizer-1.0.7/README.md
+drwxr-xr-x   0 sm453     (1000) sm453     (1000)        0 2024-05-07 15:34:01.272311 entityrdfizer-1.0.7/entityrdfizer/
+-rw-r--r--   0 sm453     (1000) sm453     (1000)       19 2022-02-17 15:59:51.000000 entityrdfizer-1.0.7/entityrdfizer/__init__.py
+drwxr-xr-x   0 sm453     (1000) sm453     (1000)        0 2024-05-07 15:34:01.272311 entityrdfizer-1.0.7/entityrdfizer/aboxgenerator/
+-rw-r--r--   0 sm453     (1000) sm453     (1000)     1533 2022-02-17 15:59:51.000000 entityrdfizer-1.0.7/entityrdfizer/aboxgenerator/ABoxGeneration.py
+-rw-r--r--   0 sm453     (1000) sm453     (1000)    27395 2024-05-07 11:51:08.000000 entityrdfizer-1.0.7/entityrdfizer/aboxgenerator/ABoxTemplateCSVFileToRDF.py
+-rw-r--r--   0 sm453     (1000) sm453     (1000)      986 2024-05-07 11:51:08.000000 entityrdfizer-1.0.7/entityrdfizer/aboxgenerator/ABoxTemplateCSVFilesToRDF.py
+-rw-r--r--   0 sm453     (1000) sm453     (1000)     2460 2022-02-17 15:59:51.000000 entityrdfizer-1.0.7/entityrdfizer/aboxgenerator/PropertyReader.py
+-rw-r--r--   0 sm453     (1000) sm453     (1000)        0 2022-02-17 15:59:51.000000 entityrdfizer-1.0.7/entityrdfizer/aboxgenerator/__init__.py
+-rw-r--r--   0 sm453     (1000) sm453     (1000)      538 2024-05-07 11:51:08.000000 entityrdfizer-1.0.7/entityrdfizer/aboxgenerator/csv2abox.py
+-rw-r--r--   0 sm453     (1000) sm453     (1000)    61063 2024-05-07 11:51:08.000000 entityrdfizer-1.0.7/entityrdfizer/aboxgenerator/tboxtools.py
+-rw-r--r--   0 sm453     (1000) sm453     (1000)      616 2024-05-07 11:51:08.000000 entityrdfizer-1.0.7/entityrdfizer/app.py
+drwxr-xr-x   0 sm453     (1000) sm453     (1000)        0 2024-05-07 15:34:01.272311 entityrdfizer-1.0.7/entityrdfizer/conf/
+-rw-r--r--   0 sm453     (1000) sm453     (1000)      268 2022-02-17 15:59:51.000000 entityrdfizer-1.0.7/entityrdfizer/conf/EntityRDFizer.properties
+-rw-r--r--   0 sm453     (1000) sm453     (1000)      811 2024-05-07 11:51:08.000000 entityrdfizer-1.0.7/entityrdfizer/driver.py
+drwxr-xr-x   0 sm453     (1000) sm453     (1000)        0 2024-05-07 15:34:01.272311 entityrdfizer-1.0.7/entityrdfizer/javagateway/
+-rw-r--r--   0 sm453     (1000) sm453     (1000)        0 2022-02-17 15:59:51.000000 entityrdfizer-1.0.7/entityrdfizer/javagateway/__init__.py
+-rw-r--r--   0 sm453     (1000) sm453     (1000)       97 2022-02-17 15:59:51.000000 entityrdfizer-1.0.7/entityrdfizer/javagateway/gateway.py
+drwxr-xr-x   0 sm453     (1000) sm453     (1000)        0 2024-05-07 15:34:01.272311 entityrdfizer-1.0.7/entityrdfizer/tboxgenerator/
+-rw-r--r--   0 sm453     (1000) sm453     (1000)        0 2022-02-17 15:59:51.000000 entityrdfizer-1.0.7/entityrdfizer/tboxgenerator/__init__.py
+-rw-r--r--   0 sm453     (1000) sm453     (1000)     1797 2022-02-17 15:59:51.000000 entityrdfizer-1.0.7/entityrdfizer/tboxgenerator/csv2tbox.py
+drwxr-xr-x   0 sm453     (1000) sm453     (1000)        0 2024-05-07 15:34:01.272311 entityrdfizer-1.0.7/entityrdfizer.egg-info/
+-rw-r--r--   0 sm453     (1000) sm453     (1000)     6783 2024-05-07 15:34:01.000000 entityrdfizer-1.0.7/entityrdfizer.egg-info/PKG-INFO
+-rw-r--r--   0 sm453     (1000) sm453     (1000)      858 2024-05-07 15:34:01.000000 entityrdfizer-1.0.7/entityrdfizer.egg-info/SOURCES.txt
+-rw-r--r--   0 sm453     (1000) sm453     (1000)        1 2024-05-07 15:34:01.000000 entityrdfizer-1.0.7/entityrdfizer.egg-info/dependency_links.txt
+-rw-r--r--   0 sm453     (1000) sm453     (1000)       55 2024-05-07 15:34:01.000000 entityrdfizer-1.0.7/entityrdfizer.egg-info/entry_points.txt
+-rw-r--r--   0 sm453     (1000) sm453     (1000)       38 2024-05-07 15:34:01.000000 entityrdfizer-1.0.7/entityrdfizer.egg-info/requires.txt
+-rw-r--r--   0 sm453     (1000) sm453     (1000)       14 2024-05-07 15:34:01.000000 entityrdfizer-1.0.7/entityrdfizer.egg-info/top_level.txt
+-rw-r--r--   0 sm453     (1000) sm453     (1000)       38 2024-05-07 15:34:01.272311 entityrdfizer-1.0.7/setup.cfg
+-rw-r--r--   0 sm453     (1000) sm453     (1000)      843 2024-05-07 15:33:42.000000 entityrdfizer-1.0.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `entityrdfizer-1.0.6/LICENSE` & `entityrdfizer-1.0.7/LICENSE`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (C) 2021 Prof. Markus Kraft (mk306@cam.ac.uk) and the Computational Modelling Group, Cambridge, UK (cheng-como@lists.cam.ac.uk).
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright (C) 2021 Prof. Markus Kraft (mk306@cam.ac.uk) and the Computational Modelling Group, Cambridge, UK (cheng-como@lists.cam.ac.uk).
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `entityrdfizer-1.0.6/entityrdfizer/aboxgenerator/ABoxGeneration.py` & `entityrdfizer-1.0.7/entityrdfizer/aboxgenerator/ABoxGeneration.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-##########################################
-# Author: Feroz Farazi (msff2@cam.ac.uk) #
-# Date: 30 Nov 2020                      #
-##########################################
-
-"""This module is designed and developed to allow users to create and link
-instances and add data properties to instances."""
-
-from rdflib import URIRef, Literal
-from rdflib.namespace import RDF, RDFS, XSD
-
-"""Creates an instance"""
-def create_instance(graph, class_iri, instance_iri, instance_name):
-    instance = URIRef(instance_iri)
-    graph.add((instance, RDF.type, class_iri))
-    link_data_with_type(graph, RDFS.label, instance, instance_name, XSD.string)
-    return graph
-
-"""Creates an instance"""
-def create_instance_without_name(graph, class_iri, instance_iri):
-    instance = URIRef(instance_iri)
-    graph.add((instance, RDF.type, class_iri))
-    return graph
-
-"""Links a source instance with a target instance"""
-def link_instance(graph, object_property, source_instance_iri, target_instance_iri):
-    graph.add((source_instance_iri, object_property, target_instance_iri))
-    return graph
-
-"""Adds a data property to an instance"""
-def link_data(graph, data_property, instance_iri, value):
-    data = Literal(value)
-    graph.add((instance_iri, data_property, data))
-    return graph
-
-"""Adds a data property including the data type to an instance"""
-def link_data_with_type(graph, data_property, instance_iri, value, data_type):
-    data = Literal(value, datatype=data_type)
-    graph.add((instance_iri, data_property, data))
-    return graph
+##########################################
+# Author: Feroz Farazi (msff2@cam.ac.uk) #
+# Date: 30 Nov 2020                      #
+##########################################
+
+"""This module is designed and developed to allow users to create and link
+instances and add data properties to instances."""
+
+from rdflib import URIRef, Literal
+from rdflib.namespace import RDF, RDFS, XSD
+
+"""Creates an instance"""
+def create_instance(graph, class_iri, instance_iri, instance_name):
+    instance = URIRef(instance_iri)
+    graph.add((instance, RDF.type, class_iri))
+    link_data_with_type(graph, RDFS.label, instance, instance_name, XSD.string)
+    return graph
+
+"""Creates an instance"""
+def create_instance_without_name(graph, class_iri, instance_iri):
+    instance = URIRef(instance_iri)
+    graph.add((instance, RDF.type, class_iri))
+    return graph
+
+"""Links a source instance with a target instance"""
+def link_instance(graph, object_property, source_instance_iri, target_instance_iri):
+    graph.add((source_instance_iri, object_property, target_instance_iri))
+    return graph
+
+"""Adds a data property to an instance"""
+def link_data(graph, data_property, instance_iri, value):
+    data = Literal(value)
+    graph.add((instance_iri, data_property, data))
+    return graph
+
+"""Adds a data property including the data type to an instance"""
+def link_data_with_type(graph, data_property, instance_iri, value, data_type):
+    data = Literal(value, datatype=data_type)
+    graph.add((instance_iri, data_property, data))
+    return graph
```

### Comparing `entityrdfizer-1.0.6/entityrdfizer/aboxgenerator/PropertyReader.py` & `entityrdfizer-1.0.7/entityrdfizer/aboxgenerator/PropertyReader.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-##########################################
-# Author: Feroz Farazi (msff2@cam.ac.uk) #
-# Date: 07 Dec 2020                      #
-##########################################
-import configparser
-import pkg_resources
-import os
-
-ENTRDF_PROP_FILE = pkg_resources.resource_filename(__name__,os.path.join('..','conf','EntityRDFizer.properties'))
-
-config = configparser.RawConfigParser()
-config.read(ENTRDF_PROP_FILE)
-
-"""Created variables to be used globally to maintain the values
-read from a property file and to update the variables if users set
-new values via setter functions"""
-tboxIRI=''
-aboxIRI=''
-aboxFileName=''
-aboxFileExtension=''
-instanceLabelCreationOption=''
-
-def getTBoxIRI():
-    return tboxIRI
-
-def setTBoxIRI(iri):
-    global tboxIRI
-    tboxIRI = iri
-
-def getABoxIRI():
-    return aboxIRI
-
-def setABoxIRI(iri):
-    global aboxIRI
-    aboxIRI=iri
-
-def getABoxFileName():
-    return aboxFileName
-
-def setABoxFileName(fileName):
-    global aboxFileName
-    aboxFileName = fileName
-
-def getInstanceLabelCreationOption():
-    return instanceLabelCreationOption
-
-def setInstanceLabelCreationOption(labelCreationOption):
-    global instanceLabelCreationOption
-    instanceLabelCreationOption = labelCreationOption
-
-def readInstanceLabelCreationOption():
-    global instanceLabelCreationOption
-    instanceLabelCreationOption = config.get('InstanceParameter', 'create.label.using.instance.name')
-    return instanceLabelCreationOption
-
-def getABoxFileExtension():
-    return aboxFileExtension
-
-def setABoxFileExtension(fileExtension):
-    global aboxFileExtension
-    aboxFileExtension = fileExtension
-
-def readABoxFileExtension():
-    global aboxFileExtension
-    aboxFileExtension = config.get('FileSection', 'kb.abox.file.extension')
-    return aboxFileExtension
-
-
-if __name__ == '__main__':
-    """Shows the default values available in the property file"""
-    print(readInstanceLabelCreationOption())
-    print(readABoxFileExtension())
-    """Sets new values to update the ones read from the property file"""
-    setTBoxIRI("http://a/test/tbox/iri")
-    setABoxIRI("http://a/test/abox/iri")
-    setABoxFileName("a-test-a-box-file-name")
-    setInstanceLabelCreationOption("no")
-    setABoxFileExtension("a-test-a-box-file-extension")
-    """Shows the new values set via setter functions above"""
-    print(getTBoxIRI())
-    print(getABoxIRI())
-    print(getABoxFileName())
-    print(getInstanceLabelCreationOption())
-    print(getABoxFileExtension())
+##########################################
+# Author: Feroz Farazi (msff2@cam.ac.uk) #
+# Date: 07 Dec 2020                      #
+##########################################
+import configparser
+import pkg_resources
+import os
+
+ENTRDF_PROP_FILE = pkg_resources.resource_filename(__name__,os.path.join('..','conf','EntityRDFizer.properties'))
+
+config = configparser.RawConfigParser()
+config.read(ENTRDF_PROP_FILE)
+
+"""Created variables to be used globally to maintain the values
+read from a property file and to update the variables if users set
+new values via setter functions"""
+tboxIRI=''
+aboxIRI=''
+aboxFileName=''
+aboxFileExtension=''
+instanceLabelCreationOption=''
+
+def getTBoxIRI():
+    return tboxIRI
+
+def setTBoxIRI(iri):
+    global tboxIRI
+    tboxIRI = iri
+
+def getABoxIRI():
+    return aboxIRI
+
+def setABoxIRI(iri):
+    global aboxIRI
+    aboxIRI=iri
+
+def getABoxFileName():
+    return aboxFileName
+
+def setABoxFileName(fileName):
+    global aboxFileName
+    aboxFileName = fileName
+
+def getInstanceLabelCreationOption():
+    return instanceLabelCreationOption
+
+def setInstanceLabelCreationOption(labelCreationOption):
+    global instanceLabelCreationOption
+    instanceLabelCreationOption = labelCreationOption
+
+def readInstanceLabelCreationOption():
+    global instanceLabelCreationOption
+    instanceLabelCreationOption = config.get('InstanceParameter', 'create.label.using.instance.name')
+    return instanceLabelCreationOption
+
+def getABoxFileExtension():
+    return aboxFileExtension
+
+def setABoxFileExtension(fileExtension):
+    global aboxFileExtension
+    aboxFileExtension = fileExtension
+
+def readABoxFileExtension():
+    global aboxFileExtension
+    aboxFileExtension = config.get('FileSection', 'kb.abox.file.extension')
+    return aboxFileExtension
+
+
+if __name__ == '__main__':
+    """Shows the default values available in the property file"""
+    print(readInstanceLabelCreationOption())
+    print(readABoxFileExtension())
+    """Sets new values to update the ones read from the property file"""
+    setTBoxIRI("http://a/test/tbox/iri")
+    setABoxIRI("http://a/test/abox/iri")
+    setABoxFileName("a-test-a-box-file-name")
+    setInstanceLabelCreationOption("no")
+    setABoxFileExtension("a-test-a-box-file-extension")
+    """Shows the new values set via setter functions above"""
+    print(getTBoxIRI())
+    print(getABoxIRI())
+    print(getABoxFileName())
+    print(getInstanceLabelCreationOption())
+    print(getABoxFileExtension())
```

### Comparing `entityrdfizer-1.0.6/entityrdfizer/tboxgenerator/csv2tbox.py` & `entityrdfizer-1.0.7/entityrdfizer/tboxgenerator/csv2tbox.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from entityrdfizer.javagateway.gateway import jpsBaseLibGW
-from py4j.java_gateway import Py4JJavaError, Py4JError
-import textwrap
-import glob
-import os
-
-# create the separate JVM view
-jpsBaseLibGW_view = jpsBaseLibGW.createModuleView()
-# import required Java packages into the created JVM view
-jpsBaseLibGW.importPackages(jpsBaseLibGW_view,'uk.ac.cam.cares.jps.base.converter.*')
-
-def run_tbox_generator(
-    csvFileOrDirPath,
-    outDir):
-
-    if os.path.isfile(csvFileOrDirPath):
-        if outDir is None: outDir = os.path.dirname(csvFileOrDirPath)
-        os.makedirs(outDir, exist_ok=True)
-        outDir =os.path.abspath(outDir)
-
-        csv2tbox(csvFileOrDirPath, outDir)
-    elif os.path.isdir(csvFileOrDirPath):
-        if outDir is None: outDir = csvFileOrDirPath
-        os.makedirs(outDir, exist_ok=True)
-
-        csv_files = glob.glob(os.path.join(csvFileOrDirPath, "*.csv"))
-        for csv_file in csv_files:
-            csv2tbox(csv_file, outDir)
-    else:
-        print(f"File or directory {csvFileOrDirPath} does not exists")
-
-def csv2tbox(csvFile, outDir):
-    print(f"Converting tbox {csvFile} into rdf format.")
-    outFile = os.path.join(outDir,os.path.basename(csvFile)+'.owl')
-    TBoxGenerator = jpsBaseLibGW_view.TBoxGeneration()
-    try:
-        # the file name is added to the outDir, as the java code expects output file path
-        TBoxGenerator.generateTBox(csvFile, outFile)
-    except (Py4JJavaError, Py4JError) as e:
-        print(textwrap.dedent("""
-            Error: Tbox generation failed. Add 'redirect_stderr' parameter to the launch
-                   gateway method to see a more detailed error log."""))
-        raise e(f"Tbox generation failed with the following error {e.java_exception}. ")
+from entityrdfizer.javagateway.gateway import jpsBaseLibGW
+from py4j.java_gateway import Py4JJavaError, Py4JError
+import textwrap
+import glob
+import os
+
+# create the separate JVM view
+jpsBaseLibGW_view = jpsBaseLibGW.createModuleView()
+# import required Java packages into the created JVM view
+jpsBaseLibGW.importPackages(jpsBaseLibGW_view,'uk.ac.cam.cares.jps.base.converter.*')
+
+def run_tbox_generator(
+    csvFileOrDirPath,
+    outDir):
+
+    if os.path.isfile(csvFileOrDirPath):
+        if outDir is None: outDir = os.path.dirname(csvFileOrDirPath)
+        os.makedirs(outDir, exist_ok=True)
+        outDir =os.path.abspath(outDir)
+
+        csv2tbox(csvFileOrDirPath, outDir)
+    elif os.path.isdir(csvFileOrDirPath):
+        if outDir is None: outDir = csvFileOrDirPath
+        os.makedirs(outDir, exist_ok=True)
+
+        csv_files = glob.glob(os.path.join(csvFileOrDirPath, "*.csv"))
+        for csv_file in csv_files:
+            csv2tbox(csv_file, outDir)
+    else:
+        print(f"File or directory {csvFileOrDirPath} does not exists")
+
+def csv2tbox(csvFile, outDir):
+    print(f"Converting tbox {csvFile} into rdf format.")
+    outFile = os.path.join(outDir,os.path.basename(csvFile)+'.owl')
+    TBoxGenerator = jpsBaseLibGW_view.TBoxGeneration()
+    try:
+        # the file name is added to the outDir, as the java code expects output file path
+        TBoxGenerator.generateTBox(csvFile, outFile)
+    except (Py4JJavaError, Py4JError) as e:
+        print(textwrap.dedent("""
+            Error: Tbox generation failed. Add 'redirect_stderr' parameter to the launch
+                   gateway method to see a more detailed error log."""))
+        raise e(f"Tbox generation failed with the following error {e.java_exception}. ")
     print(f"Conversion complete. Tbox created at {outFile}")
```

### Comparing `entityrdfizer-1.0.6/entityrdfizer.egg-info/SOURCES.txt` & `entityrdfizer-1.0.7/entityrdfizer.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,12 +13,13 @@
 entityrdfizer.egg-info/top_level.txt
 entityrdfizer/aboxgenerator/ABoxGeneration.py
 entityrdfizer/aboxgenerator/ABoxTemplateCSVFileToRDF.py
 entityrdfizer/aboxgenerator/ABoxTemplateCSVFilesToRDF.py
 entityrdfizer/aboxgenerator/PropertyReader.py
 entityrdfizer/aboxgenerator/__init__.py
 entityrdfizer/aboxgenerator/csv2abox.py
+entityrdfizer/aboxgenerator/tboxtools.py
 entityrdfizer/conf/EntityRDFizer.properties
 entityrdfizer/javagateway/__init__.py
 entityrdfizer/javagateway/gateway.py
 entityrdfizer/tboxgenerator/__init__.py
 entityrdfizer/tboxgenerator/csv2tbox.py
```

### Comparing `entityrdfizer-1.0.6/setup.py` & `entityrdfizer-1.0.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='entityrdfizer', # Required
-    version='1.0.6', # Required
-    # This should be your name or the name of the organization which owns the
-    # project.
-    author='Feroz Farazi', # Optional
-    license='MIT',
-    long_description=open('README.md').read(), # Optional
-    long_description_content_type="text/markdown",
-    packages=find_packages(exclude=("tests")),
-    url="https://github.com/cambridge-cares/TheWorldAvatar/tree/develop/EntityRDFizer",
-    python_requires='>=3.5, <4',
-    include_package_data=True,
-    install_requires= ['rdflib>=4.2, <6.0', 'docopt', 'py4jps>=1.0.6'],
-    entry_points={  # Optional
-        'console_scripts': [
-            'csv2rdf=entityrdfizer.driver:main',
-        ],
-    }
-)
+from setuptools import setup, find_packages
+
+setup(
+    name='entityrdfizer', # Required
+    version='1.0.7', # Required
+    # This should be your name or the name of the organization which owns the
+    # project.
+    author='Feroz Farazi', # Optional
+    license='MIT',
+    description='Converts instances from a CSV file into RDF.',
+    long_description=open('README.md').read(), # Optional
+    long_description_content_type="text/markdown",
+    packages=find_packages(exclude=("tests")),
+    url="https://github.com/cambridge-cares/TheWorldAvatar/tree/develop/EntityRDFizer",
+    python_requires='>=3.5, <4',
+    include_package_data=True,
+    install_requires= ['rdflib>=4.2, <6.0', 'docopt', 'py4jps>=1.0.6'],
+    entry_points={  # Optional
+        'console_scripts': [
+            'csv2rdf=entityrdfizer.driver:main',
+        ],
+    }
+)
```

