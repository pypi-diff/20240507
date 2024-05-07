# Comparing `tmp/kgraphmemory-0.0.4.tar.gz` & `tmp/kgraphmemory-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgraphmemory-0.0.4.tar", last modified: Mon May  6 21:28:47 2024, max compression
+gzip compressed data, was "kgraphmemory-0.0.5.tar", last modified: Tue May  7 21:12:10 2024, max compression
```

## Comparing `kgraphmemory-0.0.4.tar` & `kgraphmemory-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:28:47.557629 kgraphmemory-0.0.4/
--rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-05-01 12:23:12.000000 kgraphmemory-0.0.4/LICENSE
--rw-r--r--   0 hadfield   (501) staff       (20)      784 2024-05-06 21:28:47.557435 kgraphmemory-0.0.4/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)       14 2024-05-01 12:23:12.000000 kgraphmemory-0.0.4/README.md
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:28:47.555881 kgraphmemory-0.0.4/kgraphmemory/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 12:28:09.000000 kgraphmemory-0.0.4/kgraphmemory/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:28:47.556712 kgraphmemory-0.0.4/kgraphmemory/entitymodel/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 16:38:02.000000 kgraphmemory-0.0.4/kgraphmemory/entitymodel/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)       30 2024-05-01 16:38:31.000000 kgraphmemory-0.0.4/kgraphmemory/entitymodel/entitymodel.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2844 2024-05-01 16:50:59.000000 kgraphmemory-0.0.4/kgraphmemory/entitymodel/spacy_en_core_web_model.py
--rw-r--r--   0 hadfield   (501) staff       (20)    13263 2024-05-05 23:20:01.000000 kgraphmemory-0.0.4/kgraphmemory/kginteraction_graph.py
--rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-05 01:39:33.000000 kgraphmemory-0.0.4/kgraphmemory/kgraph.py
--rw-r--r--   0 hadfield   (501) staff       (20)     3283 2024-05-05 19:08:16.000000 kgraphmemory-0.0.4/kgraphmemory/kgraph_memory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      402 2024-05-05 21:09:58.000000 kgraphmemory-0.0.4/kgraphmemory/kgresult_list.py
--rw-r--r--   0 hadfield   (501) staff       (20)      858 2024-05-05 20:50:12.000000 kgraphmemory-0.0.4/kgraphmemory/kgresult_match.py
--rw-r--r--   0 hadfield   (501) staff       (20)      293 2024-05-05 19:53:28.000000 kgraphmemory-0.0.4/kgraphmemory/kgstatus.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:28:47.556920 kgraphmemory-0.0.4/kgraphmemory/utils/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-05 02:58:49.000000 kgraphmemory-0.0.4/kgraphmemory/utils/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)      288 2024-05-05 03:06:01.000000 kgraphmemory-0.0.4/kgraphmemory/utils/uri_generator.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:28:47.556407 kgraphmemory-0.0.4/kgraphmemory.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      784 2024-05-06 21:28:47.000000 kgraphmemory-0.0.4/kgraphmemory.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)      659 2024-05-06 21:28:47.000000 kgraphmemory-0.0.4/kgraphmemory.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-06 21:28:47.000000 kgraphmemory-0.0.4/kgraphmemory.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-06 21:28:47.000000 kgraphmemory-0.0.4/kgraphmemory.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       13 2024-05-06 21:28:47.000000 kgraphmemory-0.0.4/kgraphmemory.egg-info/top_level.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-06 21:28:47.557664 kgraphmemory-0.0.4/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)     1024 2024-05-06 21:28:10.000000 kgraphmemory-0.0.4/setup.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:28:47.557125 kgraphmemory-0.0.4/test/
--rw-r--r--   0 hadfield   (501) staff       (20)      422 2024-05-04 22:59:09.000000 kgraphmemory-0.0.4/test/test_domain_objects.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2119 2024-05-04 23:04:55.000000 kgraphmemory-0.0.4/test/test_graph_collection.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:12:10.115046 kgraphmemory-0.0.5/
+-rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-05-01 12:23:12.000000 kgraphmemory-0.0.5/LICENSE
+-rw-r--r--   0 hadfield   (501) staff       (20)      784 2024-05-07 21:12:10.114847 kgraphmemory-0.0.5/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)       14 2024-05-01 12:23:12.000000 kgraphmemory-0.0.5/README.md
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:12:10.113329 kgraphmemory-0.0.5/kgraphmemory/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 12:28:09.000000 kgraphmemory-0.0.5/kgraphmemory/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:12:10.114148 kgraphmemory-0.0.5/kgraphmemory/entitymodel/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 16:38:02.000000 kgraphmemory-0.0.5/kgraphmemory/entitymodel/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       30 2024-05-01 16:38:31.000000 kgraphmemory-0.0.5/kgraphmemory/entitymodel/entitymodel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2844 2024-05-01 16:50:59.000000 kgraphmemory-0.0.5/kgraphmemory/entitymodel/spacy_en_core_web_model.py
+-rw-r--r--   0 hadfield   (501) staff       (20)    13810 2024-05-07 20:33:09.000000 kgraphmemory-0.0.5/kgraphmemory/kginteraction_graph.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-05 01:39:33.000000 kgraphmemory-0.0.5/kgraphmemory/kgraph.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     3283 2024-05-05 19:08:16.000000 kgraphmemory-0.0.5/kgraphmemory/kgraph_memory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      402 2024-05-05 21:09:58.000000 kgraphmemory-0.0.5/kgraphmemory/kgresult_list.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      858 2024-05-05 20:50:12.000000 kgraphmemory-0.0.5/kgraphmemory/kgresult_match.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      293 2024-05-05 19:53:28.000000 kgraphmemory-0.0.5/kgraphmemory/kgstatus.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:12:10.114341 kgraphmemory-0.0.5/kgraphmemory/utils/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-05 02:58:49.000000 kgraphmemory-0.0.5/kgraphmemory/utils/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      288 2024-05-05 03:06:01.000000 kgraphmemory-0.0.5/kgraphmemory/utils/uri_generator.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:12:10.113854 kgraphmemory-0.0.5/kgraphmemory.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      784 2024-05-07 21:12:10.000000 kgraphmemory-0.0.5/kgraphmemory.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)      659 2024-05-07 21:12:10.000000 kgraphmemory-0.0.5/kgraphmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-07 21:12:10.000000 kgraphmemory-0.0.5/kgraphmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-07 21:12:10.000000 kgraphmemory-0.0.5/kgraphmemory.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       13 2024-05-07 21:12:10.000000 kgraphmemory-0.0.5/kgraphmemory.egg-info/top_level.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-07 21:12:10.115082 kgraphmemory-0.0.5/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)     1024 2024-05-07 21:08:19.000000 kgraphmemory-0.0.5/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:12:10.114543 kgraphmemory-0.0.5/test/
+-rw-r--r--   0 hadfield   (501) staff       (20)      422 2024-05-04 22:59:09.000000 kgraphmemory-0.0.5/test/test_domain_objects.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2119 2024-05-04 23:04:55.000000 kgraphmemory-0.0.5/test/test_graph_collection.py
```

### Comparing `kgraphmemory-0.0.4/LICENSE` & `kgraphmemory-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kgraphmemory-0.0.4/PKG-INFO` & `kgraphmemory-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: kgraphmemory
-Version: 0.0.4
+Version: 0.0.5
 Summary: KGraph Memory
 Home-page: https://github.com/vital-ai/kgraphmemory
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vital-ai-vitalsigns>=0.1.4
-Requires-Dist: vital-ai-domain>=0.1.3
+Requires-Dist: vital-ai-vitalsigns>=0.1.9
+Requires-Dist: vital-ai-domain>=0.1.4
 Requires-Dist: six
 Requires-Dist: pyyaml
-Requires-Dist: vital-ai-haley-kg>=0.1.3
+Requires-Dist: vital-ai-haley-kg>=0.1.4
 Requires-Dist: rdflib==7.0.0
 Requires-Dist: SPARQLWrapper==2.0.0
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 Requires-Dist: transformers==4.40.1
 
 # kgraphmemory
```

### Comparing `kgraphmemory-0.0.4/kgraphmemory/entitymodel/spacy_en_core_web_model.py` & `kgraphmemory-0.0.5/kgraphmemory/entitymodel/spacy_en_core_web_model.py`

 * *Files identical despite different names*

### Comparing `kgraphmemory-0.0.4/kgraphmemory/kginteraction_graph.py` & `kgraphmemory-0.0.5/kgraphmemory/kginteraction_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,20 @@
     def search_entities(self, entity_type: str) -> KGResultList:
         interaction_uri = str(self._interaction.URI)
         result_list = KGResultList()
         print('InteractionURI: ' + interaction_uri)
         nodes = self.graph.get_nodes_outgoing(interaction_uri)
         entities = [node for node in nodes if isinstance(node, KGEntity)]
         # TODO push filter into search
-        results = self.graph.search(entity_type, 1000)
+        print('Searching entities...')
+        results = self.graph.search(entity_type, 'http://vital.ai/ontology/haley-ai-kg#KGEntity', 1000)
+        print('Searching entities...done.')
         for r in results:
             go = r.graph_object
+            print(f"Entity Name: {go.name}")
             go_score = r.score
             if isinstance(go, KGEntity):
                 if go in entities:
                     match = KGResultMatch(go_score)
                     match.add_match("entity", go)
                     result_list.add_result(match)
         return result_list
@@ -60,14 +63,15 @@
         entity_result_list = self.search_entities(entity_type)
 
         if len(entity_result_list) > 0:
             entity_match = entity_result_list[0]
             entity = entity_match['entity']
             entity_uri = entity.URI
 
+            print('Searching entity frames...')
             frame_result_list = self.search_entity_frames(entity_uri, frame_type)
 
             if len(frame_result_list) > 0:
                 frame_match = frame_result_list[0]
                 frame = frame_match['frame']
 
                 result_match = KGResultMatch()
@@ -83,30 +87,33 @@
             self,
             entity_type: str,
             frame_type: str,
             slot_type: str) -> KGResultList:
 
         result_list = KGResultList()
 
+        print('Searching entities...')
         entity_result_list = self.search_entities(entity_type)
 
         if len(entity_result_list) > 0:
 
             for entity_match in entity_result_list:
                 # entity_match = entity_result_list[0]
                 entity = entity_match.matches['entity']
                 entity_uri = entity.URI
 
+                print('Searching entity frames...')
                 frame_result_list = self.search_entity_frames(entity_uri, frame_type)
 
                 if len(frame_result_list) > 0:
                     frame_match = frame_result_list[0]
                     frame = frame_match.matches['frame']
                     frame_uri = frame.URI
 
+                    print('Searching entity frame slots...')
                     slot_result_list = self.search_frame_slots(frame_uri, slot_type)
 
                     if len(slot_result_list) > 0:
                         slot_match = slot_result_list[0]
                         slot = slot_match.matches['slot']
                         slot_uri = slot.URI
 
@@ -135,15 +142,15 @@
         return result_list
 
     def search_relations(self, relation_type: str) -> KGResultList:
         result_list = KGResultList()
 
         relations = [edge for edge in self.graph if isinstance(edge, Edge_hasKGRelation)]
 
-        results = self.graph.search(relation_type, 1000)
+        results = self.graph.search(relation_type, None, 1000)
 
         for r in results:
             go = r.graph_object
             go_score = r.score
             if isinstance(go, Edge_hasKGRelation):
                 if go in relations:
                     match = KGResultMatch(go_score)
@@ -181,15 +188,15 @@
         result_list = KGResultList()
         in_edges = self.graph.get_edges_incoming(entity_uri)
         out_edges = self.graph.get_edges_outgoing(entity_uri)
         rel_out_edges = [edge for edge in out_edges if isinstance(edge, Edge_hasKGRelation)]
         rel_in_edges = [edge for edge in in_edges if isinstance(edge, Edge_hasKGRelation)]
         edges = rel_out_edges + rel_in_edges
         # TODO push filter into search
-        results = self.graph.search(relation_type, 1000)
+        results = self.graph.search(relation_type, None, 1000)
         for r in results:
             go = r.graph_object
             go_score = r.score
             if isinstance(go, Edge_hasKGRelation):
                 if go in edges:
                     match = KGResultMatch(go_score)
                     match.add_match("relation", go)
@@ -207,15 +214,15 @@
 
     def search_frames(self, frame_type: str) -> KGResultList:
         interaction_uri = self._interaction.URI
         result_list = KGResultList()
         nodes = self.graph.get_nodes_outgoing(interaction_uri)
         frames = [node for node in nodes if isinstance(node, KGFrame)]
         # TODO push filter into search
-        results = self.graph.search(frame_type, 1000)
+        results = self.graph.search(frame_type, 'http://vital.ai/ontology/haley-ai-kg#KGFrame', 1000)
         for r in results:
             go = r.graph_object
             go_score = r.score
             if isinstance(go, KGFrame):
                 if go in frames:
                     match = KGResultMatch(go_score)
                     match.add_match("frame", go)
@@ -235,15 +242,15 @@
             self,
             entity_uri: str,
             frame_type: str) -> KGResultList:
         result_list = KGResultList()
         nodes = self.graph.get_nodes_outgoing(entity_uri)
         frames = [node for node in nodes if isinstance(node, KGFrame)]
         # TODO push filter into search
-        results = self.graph.search(frame_type, 1000)
+        results = self.graph.search(frame_type, 'http://vital.ai/ontology/haley-ai-kg#KGFrame', 1000)
         for r in results:
             go = r.graph_object
             go_score = r.score
             if isinstance(go, KGFrame):
                 if go in frames:
                     match = KGResultMatch(go_score)
                     match.add_match("frame", go)
@@ -263,15 +270,16 @@
             self,
             frame_uri: str,
             slot_type: str) -> KGResultList:
         result_list = KGResultList()
         nodes = self.graph.get_nodes_outgoing(str(frame_uri))
         slots = [node for node in nodes if isinstance(node, KGSlot)]
         # TODO push filter into search
-        results = self.graph.search(slot_type, 1000)
+        # Must account for all types of slots in filter
+        results = self.graph.search(slot_type, None, 1000)
         for r in results:
             go = r.graph_object
             go_score = r.score
             if isinstance(go, KGSlot):
                 if go in slots:
                     slot_name = go.name
```

### Comparing `kgraphmemory-0.0.4/kgraphmemory/kgraph_memory.py` & `kgraphmemory-0.0.5/kgraphmemory/kgraph_memory.py`

 * *Files identical despite different names*

### Comparing `kgraphmemory-0.0.4/kgraphmemory/kgresult_match.py` & `kgraphmemory-0.0.5/kgraphmemory/kgresult_match.py`

 * *Files identical despite different names*

### Comparing `kgraphmemory-0.0.4/kgraphmemory.egg-info/PKG-INFO` & `kgraphmemory-0.0.5/kgraphmemory.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: kgraphmemory
-Version: 0.0.4
+Version: 0.0.5
 Summary: KGraph Memory
 Home-page: https://github.com/vital-ai/kgraphmemory
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vital-ai-vitalsigns>=0.1.4
-Requires-Dist: vital-ai-domain>=0.1.3
+Requires-Dist: vital-ai-vitalsigns>=0.1.9
+Requires-Dist: vital-ai-domain>=0.1.4
 Requires-Dist: six
 Requires-Dist: pyyaml
-Requires-Dist: vital-ai-haley-kg>=0.1.3
+Requires-Dist: vital-ai-haley-kg>=0.1.4
 Requires-Dist: rdflib==7.0.0
 Requires-Dist: SPARQLWrapper==2.0.0
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 Requires-Dist: transformers==4.40.1
 
 # kgraphmemory
```

### Comparing `kgraphmemory-0.0.4/kgraphmemory.egg-info/SOURCES.txt` & `kgraphmemory-0.0.5/kgraphmemory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kgraphmemory-0.0.4/setup.py` & `kgraphmemory-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kgraphmemory',
-    version='0.0.4',
+    version='0.0.5',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='KGraph Memory',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/kgraphmemory',
     packages=find_packages(exclude=["test"]),
     license='Apache License 2.0',
     install_requires=[
-            'vital-ai-vitalsigns>=0.1.4',
-            'vital-ai-domain>=0.1.3',
+            'vital-ai-vitalsigns>=0.1.9',
+            'vital-ai-domain>=0.1.4',
             'six',
             'pyyaml',
-            'vital-ai-haley-kg>=0.1.3',
+            'vital-ai-haley-kg>=0.1.4',
             'rdflib==7.0.0',
             'SPARQLWrapper==2.0.0',
             'networkx',
             'matplotlib',
             # 'sentence-transformers==2.7.0'
             'transformers==4.40.1'
     ],
```

### Comparing `kgraphmemory-0.0.4/test/test_graph_collection.py` & `kgraphmemory-0.0.5/test/test_graph_collection.py`

 * *Files identical despite different names*

