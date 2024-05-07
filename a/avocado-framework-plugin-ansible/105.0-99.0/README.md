# Comparing `tmp/avocado_framework_plugin_ansible-105.0.tar.gz` & `tmp/avocado-framework-plugin-ansible-99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avocado_framework_plugin_ansible-105.0.tar", last modified: Tue May  7 18:46:12 2024, max compression
+gzip compressed data, was "avocado-framework-plugin-ansible-99.0.tar", last modified: Thu Nov 10 19:13:31 2022, max compression
```

## Comparing `avocado_framework_plugin_ansible-105.0.tar` & `avocado-framework-plugin-ansible-99.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2024-05-07 18:46:12.759681 avocado_framework_plugin_ansible-105.0/
--rw-r--r--   0 cleber    (1000) cleber    (1000)       16 2024-05-03 14:13:15.000000 avocado_framework_plugin_ansible-105.0/MANIFEST.in
--rw-r--r--   0 cleber    (1000) cleber    (1000)      503 2024-05-07 18:46:12.759681 avocado_framework_plugin_ansible-105.0/PKG-INFO
--rw-r--r--   0 cleber    (1000) cleber    (1000)        6 2024-05-07 18:43:50.000000 avocado_framework_plugin_ansible-105.0/VERSION
-drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2024-05-07 18:46:12.758681 avocado_framework_plugin_ansible-105.0/avocado_ansible/
--rw-r--r--   0 cleber    (1000) cleber    (1000)     2249 2024-05-03 14:13:15.000000 avocado_framework_plugin_ansible-105.0/avocado_ansible/module.py
-drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2024-05-07 18:46:12.758681 avocado_framework_plugin_ansible-105.0/avocado_framework_plugin_ansible.egg-info/
--rw-r--r--   0 cleber    (1000) cleber    (1000)      503 2024-05-07 18:46:12.000000 avocado_framework_plugin_ansible-105.0/avocado_framework_plugin_ansible.egg-info/PKG-INFO
--rw-r--r--   0 cleber    (1000) cleber    (1000)      392 2024-05-07 18:46:12.000000 avocado_framework_plugin_ansible-105.0/avocado_framework_plugin_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 cleber    (1000) cleber    (1000)        1 2024-05-07 18:46:12.000000 avocado_framework_plugin_ansible-105.0/avocado_framework_plugin_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 cleber    (1000) cleber    (1000)      173 2024-05-07 18:46:12.000000 avocado_framework_plugin_ansible-105.0/avocado_framework_plugin_ansible.egg-info/entry_points.txt
--rw-r--r--   0 cleber    (1000) cleber    (1000)       53 2024-05-07 18:46:12.000000 avocado_framework_plugin_ansible-105.0/avocado_framework_plugin_ansible.egg-info/requires.txt
--rw-r--r--   0 cleber    (1000) cleber    (1000)       16 2024-05-07 18:46:12.000000 avocado_framework_plugin_ansible-105.0/avocado_framework_plugin_ansible.egg-info/top_level.txt
--rw-r--r--   0 cleber    (1000) cleber    (1000)       38 2024-05-07 18:46:12.759681 avocado_framework_plugin_ansible-105.0/setup.cfg
--rw-r--r--   0 cleber    (1000) cleber    (1000)     1809 2024-05-03 14:13:15.000000 avocado_framework_plugin_ansible-105.0/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:13:31.528361 avocado-framework-plugin-ansible-99.0/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       16 2022-11-04 17:27:10.000000 avocado-framework-plugin-ansible-99.0/MANIFEST.in
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      273 2022-11-10 19:13:31.527361 avocado-framework-plugin-ansible-99.0/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        5 2022-11-10 19:09:51.000000 avocado-framework-plugin-ansible-99.0/VERSION
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:13:31.527361 avocado-framework-plugin-ansible-99.0/avocado_ansible/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     2249 2022-11-04 17:27:10.000000 avocado-framework-plugin-ansible-99.0/avocado_ansible/module.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:13:31.527361 avocado-framework-plugin-ansible-99.0/avocado_framework_plugin_ansible.egg-info/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      273 2022-11-10 19:13:31.000000 avocado-framework-plugin-ansible-99.0/avocado_framework_plugin_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      392 2022-11-10 19:13:31.000000 avocado-framework-plugin-ansible-99.0/avocado_framework_plugin_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        1 2022-11-10 19:13:31.000000 avocado-framework-plugin-ansible-99.0/avocado_framework_plugin_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      173 2022-11-10 19:13:31.000000 avocado-framework-plugin-ansible-99.0/avocado_framework_plugin_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       37 2022-11-10 19:13:31.000000 avocado-framework-plugin-ansible-99.0/avocado_framework_plugin_ansible.egg-info/requires.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       16 2022-11-10 19:13:31.000000 avocado-framework-plugin-ansible-99.0/avocado_framework_plugin_ansible.egg-info/top_level.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       38 2022-11-10 19:13:31.528361 avocado-framework-plugin-ansible-99.0/setup.cfg
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1599 2022-11-04 17:27:10.000000 avocado-framework-plugin-ansible-99.0/setup.py
```

### Comparing `avocado_framework_plugin_ansible-105.0/avocado_ansible/module.py` & `avocado-framework-plugin-ansible-99.0/avocado_ansible/module.py`

 * *Files identical despite different names*

### Comparing `avocado_framework_plugin_ansible-105.0/setup.py` & `avocado-framework-plugin-ansible-99.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,29 +23,22 @@
 else:
     packages = find_namespace_packages(include=["avocado_ansible"])
 
 VERSION = open("VERSION", "r", encoding="utf-8").read().strip()
 
 setup(
     name="avocado-framework-plugin-ansible",
-    description="Adds to Avocado the ability to use ansible modules as dependencies for tests",
-    long_description="Adds to Avocado the ability to use ansible modules as dependencies for tests",
-    long_description_content_type="text/x-rst",
+    description="Adds to Avocado the ability to use ansible modules as dependecies for tests",
     version=VERSION,
     author="Avocado Developers",
     author_email="avocado-devel@redhat.com",
     url="http://avocado-framework.github.io/",
     packages=packages,
     include_package_data=True,
-    install_requires=[
-        f"avocado-framework=={VERSION}",
-        "cffi",
-        "pycparser",
-        "ansible-core",
-    ],
+    install_requires=[f"avocado-framework=={VERSION}", "ansible-core"],
     test_suite="tests",
     entry_points={
         "console_scripts": [
             "avocado-runner-ansible-module = avocado_ansible.module:main",
         ],
         "avocado.plugins.runnable.runner": [
             "ansible-module = avocado_ansible.module:AnsibleModuleRunner"
```

