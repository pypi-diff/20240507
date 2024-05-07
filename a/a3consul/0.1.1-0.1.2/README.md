# Comparing `tmp/a3consul-0.1.1.tar.gz` & `tmp/a3consul-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a3consul-0.1.1.tar", last modified: Tue Apr 23 03:33:39 2024, max compression
+gzip compressed data, was "a3consul-0.1.2.tar", last modified: Tue May  7 03:30:15 2024, max compression
```

## Comparing `a3consul-0.1.1.tar` & `a3consul-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-23 03:33:39.502809 a3consul-0.1.1/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)    11357 2024-02-08 11:23:49.000000 a3consul-0.1.1/LICENSE
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       66 2024-04-18 08:54:48.000000 a3consul-0.1.1/MANIFEST.in
--rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1253 2024-04-23 03:33:39.502809 a3consul-0.1.1/PKG-INFO
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      131 2024-04-18 08:56:18.000000 a3consul-0.1.1/README.md
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-23 03:33:39.502809 a3consul-0.1.1/a3consul/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       47 2024-04-23 02:44:40.000000 a3consul-0.1.1/a3consul/__init__.py
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-23 03:33:39.502809 a3consul-0.1.1/a3consul/scene_cases/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       24 2024-03-21 02:01:29.000000 a3consul-0.1.1/a3consul/scene_cases/__init__.py
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-23 03:33:39.502809 a3consul-0.1.1/a3consul/scene_cases/watch_nodes/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      169 2024-03-29 06:18:34.000000 a3consul-0.1.1/a3consul/scene_cases/watch_nodes/__init__.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1190 2024-04-18 10:41:58.000000 a3consul-0.1.1/a3consul/scene_cases/watch_nodes/abstract_node_change_service.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      720 2024-04-18 10:26:46.000000 a3consul-0.1.1/a3consul/scene_cases/watch_nodes/cmds.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     2524 2024-04-23 03:28:26.000000 a3consul-0.1.1/a3consul/scene_cases/watch_nodes/node_thread.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      463 2024-04-23 03:28:26.000000 a3consul-0.1.1/a3consul/utils.py
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-23 03:33:39.502809 a3consul-0.1.1/a3consul.egg-info/
--rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1253 2024-04-23 03:33:39.000000 a3consul-0.1.1/a3consul.egg-info/PKG-INFO
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      509 2024-04-23 03:33:39.000000 a3consul-0.1.1/a3consul.egg-info/SOURCES.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-04-23 03:33:39.000000 a3consul-0.1.1/a3consul.egg-info/dependency_links.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-04-23 03:33:39.000000 a3consul-0.1.1/a3consul.egg-info/not-zip-safe
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       29 2024-04-23 03:33:39.000000 a3consul-0.1.1/a3consul.egg-info/requires.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        9 2024-04-23 03:33:39.000000 a3consul-0.1.1/a3consul.egg-info/top_level.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1144 2024-04-23 03:33:39.502809 a3consul-0.1.1/setup.cfg
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       39 2024-02-08 11:23:49.000000 a3consul-0.1.1/setup.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-05-07 03:30:15.041015 a3consul-0.1.2/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)    11357 2024-02-08 11:23:49.000000 a3consul-0.1.2/LICENSE
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       66 2024-04-18 08:54:48.000000 a3consul-0.1.2/MANIFEST.in
+-rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1253 2024-05-07 03:30:15.041015 a3consul-0.1.2/PKG-INFO
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      131 2024-04-18 08:56:18.000000 a3consul-0.1.2/README.md
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-05-07 03:30:15.037015 a3consul-0.1.2/a3consul/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       47 2024-05-07 03:27:41.000000 a3consul-0.1.2/a3consul/__init__.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-05-07 03:30:15.037015 a3consul-0.1.2/a3consul/scene_cases/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       24 2024-03-21 02:01:29.000000 a3consul-0.1.2/a3consul/scene_cases/__init__.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-05-07 03:30:15.041015 a3consul-0.1.2/a3consul/scene_cases/watch_nodes/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      169 2024-03-29 06:18:34.000000 a3consul-0.1.2/a3consul/scene_cases/watch_nodes/__init__.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1190 2024-04-18 10:41:58.000000 a3consul-0.1.2/a3consul/scene_cases/watch_nodes/abstract_node_change_service.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      720 2024-04-18 10:26:46.000000 a3consul-0.1.2/a3consul/scene_cases/watch_nodes/cmds.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     2878 2024-05-07 03:17:41.000000 a3consul-0.1.2/a3consul/scene_cases/watch_nodes/node_thread.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      463 2024-04-23 03:28:26.000000 a3consul-0.1.2/a3consul/utils.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-05-07 03:30:15.041015 a3consul-0.1.2/a3consul.egg-info/
+-rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1253 2024-05-07 03:30:15.000000 a3consul-0.1.2/a3consul.egg-info/PKG-INFO
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      509 2024-05-07 03:30:15.000000 a3consul-0.1.2/a3consul.egg-info/SOURCES.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-05-07 03:30:15.000000 a3consul-0.1.2/a3consul.egg-info/dependency_links.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-05-07 03:30:15.000000 a3consul-0.1.2/a3consul.egg-info/not-zip-safe
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       29 2024-05-07 03:30:15.000000 a3consul-0.1.2/a3consul.egg-info/requires.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        9 2024-05-07 03:30:15.000000 a3consul-0.1.2/a3consul.egg-info/top_level.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1144 2024-05-07 03:30:15.041015 a3consul-0.1.2/setup.cfg
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       39 2024-02-08 11:23:49.000000 a3consul-0.1.2/setup.py
```

### Comparing `a3consul-0.1.1/LICENSE` & `a3consul-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `a3consul-0.1.1/PKG-INFO` & `a3consul-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a3consul
-Version: 0.1.1
+Version: 0.1.2
 Summary: It is just a thin wrapper of py-consul.
 Home-page: https://github.com/three-kinds/a3consul
 Author: three-kinds
 Author-email: 3179158552@qq.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/three-kinds/a3consul
 Project-URL: Source, https://github.com/three-kinds/a3consul
```

### Comparing `a3consul-0.1.1/a3consul/scene_cases/watch_nodes/abstract_node_change_service.py` & `a3consul-0.1.2/a3consul/scene_cases/watch_nodes/abstract_node_change_service.py`

 * *Files identical despite different names*

### Comparing `a3consul-0.1.1/a3consul/scene_cases/watch_nodes/cmds.py` & `a3consul-0.1.2/a3consul/scene_cases/watch_nodes/cmds.py`

 * *Files identical despite different names*

### Comparing `a3consul-0.1.1/a3consul/scene_cases/watch_nodes/node_thread.py` & `a3consul-0.1.2/a3consul/scene_cases/watch_nodes/node_thread.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,24 @@
         # 配置为守护线程
         super().__init__(daemon=True, *args, **kwargs)
 
     def get_node_id(self) -> str:
         self._client = Consul(**self._conf['init'])
         self._session_id = self._client.session.create(**self._conf['session'], behavior='delete')
 
-        nodes_path = f'{self._nodes_path}{uuid.uuid4().hex}'
+        node_name = uuid.uuid4().hex
+        _node_conf = self._conf.get('node') or dict()
+        prefix = _node_conf.get('prefix') or None
+        if prefix is not None:
+            node_name = f'{prefix}-{node_name}'
+        max_length = _node_conf.get('max_length') or None
+        if max_length is not None:
+            node_name = node_name[:max_length]
+
+        nodes_path = f'{self._nodes_path}{node_name}'
         node_id = nodes_path.rsplit('/', 2)[-1]
 
         self._client.kv.put(key=nodes_path, value='', acquire=self._session_id)
         self.logger.info(f'[{self._topic}]获得节点id: {node_id}')
         return node_id
 
     def _renew_session(self, timeout_seconds: float) -> bool:
```

### Comparing `a3consul-0.1.1/a3consul.egg-info/PKG-INFO` & `a3consul-0.1.2/a3consul.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a3consul
-Version: 0.1.1
+Version: 0.1.2
 Summary: It is just a thin wrapper of py-consul.
 Home-page: https://github.com/three-kinds/a3consul
 Author: three-kinds
 Author-email: 3179158552@qq.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/three-kinds/a3consul
 Project-URL: Source, https://github.com/three-kinds/a3consul
```

### Comparing `a3consul-0.1.1/setup.cfg` & `a3consul-0.1.2/setup.cfg`

 * *Files identical despite different names*

