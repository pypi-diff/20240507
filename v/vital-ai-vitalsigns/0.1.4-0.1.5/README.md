# Comparing `tmp/vital-ai-vitalsigns-0.1.4.tar.gz` & `tmp/vital-ai-vitalsigns-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-ai-vitalsigns-0.1.4.tar", last modified: Mon May  6 21:09:20 2024, max compression
+gzip compressed data, was "vital-ai-vitalsigns-0.1.5.tar", last modified: Tue May  7 13:55:58 2024, max compression
```

## Comparing `vital-ai-vitalsigns-0.1.4.tar` & `vital-ai-vitalsigns-0.1.5.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.520155 vital-ai-vitalsigns-0.1.4/
--rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.4/LICENSE
--rw-r--r--   0 hadfield   (501) staff       (20)      660 2024-05-06 21:09:20.519925 vital-ai-vitalsigns-0.1.4/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)       25 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.4/README.md
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-06 21:09:20.520201 vital-ai-vitalsigns-0.1.4/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)     1071 2024-05-06 21:09:03.000000 vital-ai-vitalsigns-0.1.4/setup.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.473860 vital-ai-vitalsigns-0.1.4/test/
--rw-r--r--   0 hadfield   (501) staff       (20)      489 2024-05-02 22:13:47.000000 vital-ai-vitalsigns-0.1.4/test/test_embedding_model.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2119 2024-05-04 19:54:30.000000 vital-ai-vitalsigns-0.1.4/test/test_graph_collection.py
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:51:38.000000 vital-ai-vitalsigns-0.1.4/test/test_package_discovery.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2749 2024-05-04 14:15:24.000000 vital-ai-vitalsigns-0.1.4/test/test_query_builder.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.474386 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.475627 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/collection/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:00:36.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/collection/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)    11465 2024-05-06 21:08:25.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/collection/graph_collection.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1030 2024-05-03 21:08:09.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/collection/rdf_collection_impl.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1640 2024-05-03 21:19:06.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/collection/vector_collection_impl.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.475868 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/embedding/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:22:30.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/embedding/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1172 2024-05-03 15:21:19.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/embedding/embedding_model.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.476573 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/impl/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 18:25:32.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/impl/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2310 2024-05-04 18:20:33.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/impl/vitalsigns_impl.py
--rw-r--r--   0 hadfield   (501) staff       (20)      269 2024-03-19 17:21:02.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/impl/vitalsigns_package.py
--rw-r--r--   0 hadfield   (501) staff       (20)     5515 2024-05-04 18:49:12.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/impl/vitalsigns_registry.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.479607 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/
--rw-r--r--   0 hadfield   (501) staff       (20)       47 2024-03-19 21:49:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/BaseDomainOntology.py
--rw-r--r--   0 hadfield   (501) staff       (20)     4988 2024-05-04 20:22:24.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/GraphObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1843 2024-05-04 18:11:27.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_Edge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      338 2024-03-17 20:11:18.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_Edge.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1690 2024-05-04 18:13:01.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      310 2024-03-17 20:11:39.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1868 2024-05-04 18:13:13.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_HyperEdge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      354 2024-03-17 20:11:44.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_HyperEdge.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1657 2024-05-04 18:13:26.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_HyperNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      298 2024-03-17 20:11:51.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_HyperNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1642 2024-05-04 18:11:50.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_Node.py
--rw-r--r--   0 hadfield   (501) staff       (20)      294 2024-03-17 20:11:57.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_Node.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.479843 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/classproperties/
--rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-03 23:34:11.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/classproperties/ClassProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-03 22:18:04.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/classproperties/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.480304 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/datatype/
--rw-r--r--   0 hadfield   (501) staff       (20)      241 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/datatype/GeoLocation.py
--rw-r--r--   0 hadfield   (501) staff       (20)       23 2024-05-03 17:43:23.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/datatype/Truth.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/datatype/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.483798 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/
--rw-r--r--   0 hadfield   (501) staff       (20)      492 2024-05-03 20:14:56.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/BooleanProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      603 2024-05-03 20:14:56.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/DateTimeProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      492 2024-05-03 20:22:03.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/DoubleProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      489 2024-05-03 20:22:09.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/FloatProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      552 2024-05-03 20:22:16.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/GeoLocationProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      897 2024-05-03 20:45:02.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/IProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      489 2024-05-03 20:22:27.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/IntegerProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      537 2024-05-03 20:22:27.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/LongProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      355 2024-05-03 20:22:44.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/MultiValueProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      314 2024-05-03 20:23:03.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/OtherProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      543 2024-05-03 20:26:30.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/StringProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      540 2024-05-03 20:26:30.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/TruthProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      537 2024-05-03 20:26:30.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/URIProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.484143 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/trait/
--rw-r--r--   0 hadfield   (501) staff       (20)      715 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/trait/PropertyTrait.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/trait/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.484857 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:00:23.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)      351 2024-05-03 22:16:06.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query/property_constraint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      293 2024-05-03 18:45:19.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query/result_element.py
--rw-r--r--   0 hadfield   (501) staff       (20)      522 2024-05-03 18:46:27.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query/result_list.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2456 2024-05-04 14:04:22.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query/vital_graph_query.py
--rw-r--r--   0 hadfield   (501) staff       (20)      565 2024-05-04 14:04:22.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query/vital_query.py
--rw-r--r--   0 hadfield   (501) staff       (20)      889 2024-05-04 14:12:47.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query/vital_select_query.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.485141 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query_impl/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:01:10.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query_impl/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:02:54.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query_impl/sparql_query_impl.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:03:29.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query_impl/weaviate_vector_query_impl.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.485325 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/utils/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-02 19:19:42.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/utils/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)       30 2024-05-02 19:20:23.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/utils/uri_generator.py
--rw-r--r--   0 hadfield   (501) staff       (20)      894 2024-05-04 18:08:26.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/vitalsigns.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.475148 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      660 2024-05-06 21:09:20.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)    14057 2024-05-06 21:09:20.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-06 21:09:20.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-06 21:09:20.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns.egg-info/entry_points.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       77 2024-05-06 21:09:20.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       45 2024-05-06 21:09:20.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns.egg-info/top_level.txt
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.485430 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.507067 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/
--rw-r--r--   0 hadfield   (501) staff       (20)     1476 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/AggregationResult.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/AggregationResult.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2083 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/DatabaseConnection.py
--rw-r--r--   0 hadfield   (501) staff       (20)      309 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/DatabaseConnection.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1551 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Dataset.py
--rw-r--r--   0 hadfield   (501) staff       (20)      186 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Dataset.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/DomainModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      360 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/DomainModel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/DomainOntology.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1273 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_SameAs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_SameAs.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1285 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasApp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasApp.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1288 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasOrganization.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasOrganization.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasSegment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasSegment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasSession.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasSession.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasTransaction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasTransaction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/GraphMatch.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/GraphMatch.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1664 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/RDFStatement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/RDFStatement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1381 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SparqlAskResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SparqlAskResponse.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SparqlBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SparqlBinding.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1531 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1414 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.py
--rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SqlResultRow.py
--rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SqlResultRow.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1382 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SqlUpdateResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SqlUpdateResponse.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1353 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/URIReference.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/URIReference.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_Category.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_Category.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_Event.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_Event.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1279 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1276 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_PathQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_PathQuery.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1483 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1358 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_Query.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_Query.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1282 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1277 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalApp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalApp.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1353 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalAuthKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalAuthKey.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalOrganization.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalOrganization.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalProvisioning.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalProvisioning.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1458 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalSegment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalSegment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1294 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1951 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      305 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2419 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      414 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1540 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1279 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceKey.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1435 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1342 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1291 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceRootKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceRootKey.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1923 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      294 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1555 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalSession.py
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalSession.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1482 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalTransaction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalTransaction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:09:20.519643 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_URIProp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasAggregationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasAppID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasBackwardCompVersion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasCatalogName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasConfigString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasConnectionError.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasConnectionState.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasDatabase.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasDateRetrieved.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasDbType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasDefaultPackageValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasDefaultSegmentName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasDomainOWL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasDomainOWLHash.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasEdgeDestination.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasEdgeSource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasEndpointType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasEndpointURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasGraphQueries.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasHyperEdgeDestination.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasHyperEdgeSource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasListIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasOntologyIRI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasOrganizationID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasPassword.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasPoolInitialSize.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasPoolMaxTotal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasPreferredImportVersions.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasProvenance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasQueryString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasRdfContext.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasRdfObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasRdfPredicate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasRdfSubject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasRepositoryName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasRootPath.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasSegmentID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasSelectQueries.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasSerializedJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasSerializedRDF.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasServerURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasSessionID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasSessionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasSourceName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasSourceUrl.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasTargetAppID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasTargetOrganizationID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasTimestamp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasTransactionID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasTransactionState.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasURIRef.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasUpdateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasUpdatedRowsCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasUpdatedTriplesCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasUriGenerationStrategy.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasUsername.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasVersionIRI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_hasVersionInfo.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_isActive.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_isPositiveResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_isPreferred.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_isPrimary.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_isReadOnly.py
--rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_types.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/Property_vitaltype.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/properties/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.048543 vital-ai-vitalsigns-0.1.5/
+-rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.5/LICENSE
+-rw-r--r--   0 hadfield   (501) staff       (20)      660 2024-05-07 13:55:58.048258 vital-ai-vitalsigns-0.1.5/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)       25 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.5/README.md
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-07 13:55:58.048587 vital-ai-vitalsigns-0.1.5/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)     1071 2024-05-07 12:37:34.000000 vital-ai-vitalsigns-0.1.5/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:57.998569 vital-ai-vitalsigns-0.1.5/test/
+-rw-r--r--   0 hadfield   (501) staff       (20)      489 2024-05-02 22:13:47.000000 vital-ai-vitalsigns-0.1.5/test/test_embedding_model.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2242 2024-05-07 12:57:33.000000 vital-ai-vitalsigns-0.1.5/test/test_graph_collection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:51:38.000000 vital-ai-vitalsigns-0.1.5/test/test_package_discovery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2749 2024-05-04 14:15:24.000000 vital-ai-vitalsigns-0.1.5/test/test_query_builder.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:57.998929 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.000317 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/collection/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:00:36.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/collection/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)    11460 2024-05-07 13:33:57.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/collection/graph_collection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1030 2024-05-03 21:08:09.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/collection/rdf_collection_impl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1640 2024-05-03 21:19:06.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/collection/vector_collection_impl.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.000658 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/embedding/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:22:30.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/embedding/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2486 2024-05-07 13:54:47.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/embedding/embedding_model.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.001450 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/impl/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 18:25:32.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/impl/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2401 2024-05-07 13:32:41.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/impl/vitalsigns_impl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      269 2024-03-19 17:21:02.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/impl/vitalsigns_package.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     5439 2024-05-07 13:01:47.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/impl/vitalsigns_registry.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.004626 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)       47 2024-03-19 21:49:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/BaseDomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     4987 2024-05-07 12:44:44.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/GraphObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1843 2024-05-04 18:11:27.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_Edge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      338 2024-03-17 20:11:18.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_Edge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1690 2024-05-04 18:13:01.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      310 2024-03-17 20:11:39.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1868 2024-05-04 18:13:13.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_HyperEdge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      354 2024-03-17 20:11:44.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_HyperEdge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1657 2024-05-04 18:13:26.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_HyperNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      298 2024-03-17 20:11:51.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_HyperNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1642 2024-05-04 18:11:50.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_Node.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      294 2024-03-17 20:11:57.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_Node.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.004946 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/classproperties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-03 23:34:11.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/classproperties/ClassProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-03 22:18:04.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/classproperties/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.005480 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/datatype/
+-rw-r--r--   0 hadfield   (501) staff       (20)      241 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/datatype/GeoLocation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       23 2024-05-03 17:43:23.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/datatype/Truth.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/datatype/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.008417 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      549 2024-05-07 13:21:09.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/BooleanProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      741 2024-05-07 13:24:30.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/DateTimeProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      683 2024-05-07 13:27:08.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/DoubleProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      680 2024-05-07 13:27:16.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/FloatProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      552 2024-05-03 20:22:16.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/GeoLocationProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      897 2024-05-03 20:45:02.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/IProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      676 2024-05-07 13:28:26.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/IntegerProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      724 2024-05-07 13:28:37.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/LongProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      355 2024-05-03 20:22:44.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/MultiValueProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      446 2024-05-07 13:31:15.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/OtherProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      675 2024-05-07 13:30:16.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/StringProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      540 2024-05-03 20:26:30.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/TruthProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      669 2024-05-07 13:30:29.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/URIProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.008723 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/trait/
+-rw-r--r--   0 hadfield   (501) staff       (20)      701 2024-05-07 13:02:48.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/trait/PropertyTrait.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/trait/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.010674 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:00:23.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      351 2024-05-03 22:16:06.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query/property_constraint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      293 2024-05-03 18:45:19.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query/result_element.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      522 2024-05-03 18:46:27.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query/result_list.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2456 2024-05-04 14:04:22.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query/vital_graph_query.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      565 2024-05-04 14:04:22.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query/vital_query.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      889 2024-05-04 14:12:47.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query/vital_select_query.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.011115 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query_impl/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:01:10.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query_impl/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:02:54.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query_impl/sparql_query_impl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:03:29.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query_impl/weaviate_vector_query_impl.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.011396 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/utils/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-02 19:19:42.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/utils/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       30 2024-05-02 19:20:23.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/utils/uri_generator.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      894 2024-05-04 18:08:26.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/vitalsigns.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:57.999733 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      660 2024-05-07 13:55:57.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)    14057 2024-05-07 13:55:57.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-07 13:55:57.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-07 13:55:57.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns.egg-info/entry_points.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       77 2024-05-07 13:55:57.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       45 2024-05-07 13:55:57.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns.egg-info/top_level.txt
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.011812 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.033104 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)     1476 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/AggregationResult.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/AggregationResult.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2083 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/DatabaseConnection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      309 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/DatabaseConnection.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1551 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Dataset.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      186 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Dataset.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/DomainModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      360 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/DomainModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/DomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1273 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_SameAs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_SameAs.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1285 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasApp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasApp.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1288 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasOrganization.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasOrganization.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasSegment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasSegment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasSession.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasSession.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasTransaction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasTransaction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/GraphMatch.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/GraphMatch.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1664 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/RDFStatement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/RDFStatement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1381 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SparqlAskResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SparqlAskResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SparqlBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SparqlBinding.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1531 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1414 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SqlResultRow.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SqlResultRow.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1382 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SqlUpdateResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SqlUpdateResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1353 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/URIReference.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/URIReference.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_Category.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_Category.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_Event.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_Event.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1279 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1276 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_PathQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_PathQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1483 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1358 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_Query.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_Query.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1282 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1277 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalApp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalApp.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1353 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalAuthKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalAuthKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalOrganization.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalOrganization.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalProvisioning.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalProvisioning.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1458 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalSegment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalSegment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1294 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1951 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      305 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2419 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      414 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1540 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1279 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1435 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1342 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1291 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceRootKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceRootKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1923 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      294 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1555 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalSession.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalSession.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1482 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalTransaction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalTransaction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 13:55:58.047791 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_URIProp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasAggregationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasAppID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasBackwardCompVersion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasCatalogName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasConfigString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasConnectionError.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasConnectionState.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasDatabase.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasDateRetrieved.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasDbType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasDefaultPackageValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasDefaultSegmentName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasDomainOWL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasDomainOWLHash.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasEdgeDestination.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasEdgeSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasEndpointType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasEndpointURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasGraphQueries.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasHyperEdgeDestination.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasHyperEdgeSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasListIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasOntologyIRI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasOrganizationID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasPassword.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasPoolInitialSize.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasPoolMaxTotal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasPreferredImportVersions.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasProvenance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasQueryString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasRdfContext.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasRdfObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasRdfPredicate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasRdfSubject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasRepositoryName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasRootPath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasSegmentID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasSelectQueries.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasSerializedJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasSerializedRDF.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasServerURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasSessionID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasSessionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasSourceName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasSourceUrl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasTargetAppID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasTargetOrganizationID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasTimestamp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasTransactionID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasTransactionState.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasURIRef.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasUpdateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasUpdatedRowsCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasUpdatedTriplesCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasUriGenerationStrategy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasUsername.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasVersionIRI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_hasVersionInfo.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_isActive.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_isPositiveResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_isPreferred.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_isPrimary.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_isReadOnly.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_types.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/Property_vitaltype.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/properties/__init__.py
```

### Comparing `vital-ai-vitalsigns-0.1.4/LICENSE` & `vital-ai-vitalsigns-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/PKG-INFO` & `vital-ai-vitalsigns-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vital-ai-vitalsigns
-Version: 0.1.4
+Version: 0.1.5
 Summary: VitalSigns knowledge graph bindings
 Home-page: https://github.com/vital-ai/vital-vitalsigns-python
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vital-ai-vitalsigns-0.1.4/setup.py` & `vital-ai-vitalsigns-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vital-ai-vitalsigns',
-    version='0.1.4',
+    version='0.1.5',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='VitalSigns knowledge graph bindings',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/vital-vitalsigns-python',
     packages=find_packages(exclude=["test"]),
```

### Comparing `vital-ai-vitalsigns-0.1.4/test/test_graph_collection.py` & `vital-ai-vitalsigns-0.1.5/test/test_graph_collection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import logging
 from vital_ai_vitalsigns.collection.graph_collection import GraphCollection
 from vital_ai_vitalsigns.embedding.embedding_model import EmbeddingModel
 from vital_ai_vitalsigns.model.VITAL_Node import VITAL_Node
 from vital_ai_vitalsigns.vitalsigns import VitalSigns
 from vital_ai_vitalsigns_core.model.properties.Property_hasName import Property_hasName
 
 
 def main():
-    print('Hello World')
+    logging.basicConfig(level=logging.INFO)
+
+    logging.info('Hello World')
 
     embedder = EmbeddingModel()
 
     vs = VitalSigns()
     vs.put_embedding_model(embedder.get_model_id(), embedder)
 
     graph = GraphCollection()
@@ -49,35 +52,35 @@
 
     # query = 'pig'
     # query = 'apple'
     # query = 'noodles'
     # query = 'tea'
     query = 'frittata'
 
-    print('Search for: ' + query)
+    logging.info('Search for: ' + query)
 
     results = graph.search(query)
 
     if results is not None:
         re = results[0]
         obj = re.graph_object
         score = re.score
-        print('Top Result for: ' + query + ': ' + str(obj.name) + " (" + str(score) + ")")
-        print(obj.to_json())
-        print(obj.to_rdf())
+        logging.info('Top Result for: ' + query + ': ' + str(obj.name) + " (" + str(score) + ")")
+        logging.info(obj.to_json())
+        logging.info(obj.to_rdf())
     else:
-        print('No results')
+        logging.info('No results')
 
     # for r in results:
-    #    print(r)
+    #    logging.info(r)
 
     sparql_results = graph.sparql_query("SELECT ?s ?p ?o WHERE { ?s ?p ?o } ORDER BY ?s ?p")
 
     sparql_result_count = len(sparql_results)
-    print('Sparql Result Count: ' + str(sparql_result_count))
+    logging.info('Sparql Result Count: ' + str(sparql_result_count))
 
     for row in sparql_results:
-        print(f"Subject: {row['s']}, Property: {row['p']}, Object: {row['o']}")
+        logging.info(f"Subject: {row['s']}, Property: {row['p']}, Object: {row['o']}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `vital-ai-vitalsigns-0.1.4/test/test_query_builder.py` & `vital-ai-vitalsigns-0.1.5/test/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/collection/graph_collection.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/collection/graph_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         incoming_nodes = [self.get(node_uri) for node_uri in incoming_node_uris]
         return [node for node in incoming_nodes if node is not None]  # Filter out any None results
 
     def get_nodes_outgoing(self, uri):
         """
         Return the node objects that are the destination of an outgoing edge from the given URI.
         """
-        outgoing_node_uris = {str(item.edgeDestination) for item in self._data if
+        outgoing_node_uris = {item.edgeDestination for item in self._data if
                               isinstance(item, VITAL_Edge) and item.edgeSource == uri}
         outgoing_nodes = [self.get(node_uri) for node_uri in outgoing_node_uris]
         return [node for node in outgoing_nodes if node is not None]  # Filter out any None results
 
     def search(self, query: str, limit: int = 10):
 
         vs = VitalSigns()
```

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/collection/rdf_collection_impl.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/collection/rdf_collection_impl.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/collection/vector_collection_impl.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/collection/vector_collection_impl.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/impl/vitalsigns_impl.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/impl/vitalsigns_impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,17 @@
         if not trait_class:
             raise ValueError(f"No trait found with URI: {trait_uri}")
 
         class CombinedProperty(property_class, trait_class):
             def get_uri(self):
                 return super().get_uri()
 
+            def __hash__(self):
+                return hash((self.get_uri(), self.value))
+
         return CombinedProperty(value)
 
     @classmethod
     def get_trait_class_from_uri(cls, uri):
 
         vs = VitalSigns()
```

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/impl/vitalsigns_registry.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/impl/vitalsigns_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from importlib.metadata import entry_points
 import importlib
 import pkgutil
+import logging
 
 # these are not imported here to remove a circular dependency on start-up
 # from vital_ai_vitalsigns.model.VITAL_Edge import VITAL_Edge
 # from vital_ai_vitalsigns.model.VITAL_GraphContainerObject import VITAL_GraphContainerObject
 # from vital_ai_vitalsigns.model.VITAL_HyperEdge import VITAL_HyperEdge
 # from vital_ai_vitalsigns.model.VITAL_HyperNode import VITAL_HyperNode
 # from vital_ai_vitalsigns.model.VITAL_Node import VITAL_Node
@@ -21,14 +22,16 @@
 
     def build_registry(self):
         self.vitalsigns_packages = []
         self.vitalsigns_ontologies = []
 
         self.vitalsigns_classes = {}
 
+        logging.info('building vitalsigns class and property registry...')
+
         from vital_ai_vitalsigns.model.VITAL_Edge import VITAL_Edge
         from vital_ai_vitalsigns.model.VITAL_GraphContainerObject import VITAL_GraphContainerObject
         from vital_ai_vitalsigns.model.VITAL_HyperEdge import VITAL_HyperEdge
         from vital_ai_vitalsigns.model.VITAL_HyperNode import VITAL_HyperNode
         from vital_ai_vitalsigns.model.VITAL_Node import VITAL_Node
 
         self.vitalsigns_classes[VITAL_Node.get_class_uri()] = VITAL_Node
@@ -39,42 +42,41 @@
 
         self.vitalsigns_property_classes = {}
 
         for ep in entry_points().get('vitalsigns_packages', []):
             try:
                 module = importlib.import_module(ep.value)
                 self.vitalsigns_packages.append(module)
-                print('Discovered Module: ' + str(module))
+                logging.info('Discovered Module: ' + str(module))
             except ImportError as e:
-                print(f"Could not import {ep.value}: {e}")
+                logging.info(f"Could not import {ep.value}: {e}")
         for p in self.vitalsigns_packages:
             self.scan_vitalsigns_classes(p)
 
+        logging.info('completed build of vitalsigns class and property registry.')
+
     def _scan_module(self, module_name):
         try:
             module = importlib.import_module(module_name)
         except ImportError as e:
-            print(f"Error importing {module_name}: {e}")
+            logging.info(f"Error importing {module_name}: {e}")
             return
 
         for cls_name, cls in vars(module).items():
             if isinstance(cls, type):
                 if self.is_vitalsigns_ontology_class(cls):
-                    # print(f"Found VitalSigns Domain Ontology Class {cls_name} in {module.__name__}")
-                    print(f"Found VitalSigns Domain Ontology Class {cls_name} URI: {cls.OntologyURI}")
+                    logging.info(f"Found VitalSigns Domain Ontology Class {cls_name} URI: {cls.OntologyURI}")
                     self.vitalsigns_ontologies.append(cls)
                 if self.is_vitalsigns_class(cls):
-                    # print(f"Found VitalSigns Graph Class {cls_name} in {module.__name__}")
                     class_uri = cls.get_class_uri()
-                    print(f"Found VitalSigns Graph Class {cls_name} URI: {class_uri}")
+                    logging.info(f"Found VitalSigns Graph Class {cls_name} URI: {class_uri}")
                     self.vitalsigns_classes[class_uri] = cls
                 if self.is_vitalsigns_property_class(cls):
-                    # print(f"Found VitalSigns Property Class {cls_name} in {module.__name__}")
                     property_trait_uri = cls.get_uri()
-                    print(f"Found VitalSigns Property Class {cls_name} URI: {property_trait_uri}")
+                    logging.info(f"Found VitalSigns Property Class {cls_name} URI: {property_trait_uri}")
                     self.vitalsigns_property_classes[property_trait_uri] = cls
 
     def scan_vitalsigns_classes(self, package):
         for finder, name, is_pkg in pkgutil.walk_packages(package.__path__, package.__name__ + '.'):
             self._scan_module(name)
             if is_pkg:
                 self._scan_module(name)
@@ -123,8 +125,7 @@
         from vital_ai_vitalsigns.model.trait.PropertyTrait import PropertyTrait
 
         if cls is PropertyTrait:
             return False
         if issubclass(cls, PropertyTrait):
             return True
         return False
-
```

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/GraphObject.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/GraphObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from abc import ABC, abstractmethod
 import json
 import rdflib
 from rdflib import Graph, Literal, URIRef
-
 from vital_ai_vitalsigns.impl.vitalsigns_impl import VitalSignsImpl
 from vital_ai_vitalsigns.model.trait.PropertyTrait import PropertyTrait
 from vital_ai_vitalsigns.model.properties.BooleanProperty import BooleanProperty
 from vital_ai_vitalsigns.model.properties.LongProperty import LongProperty
 from vital_ai_vitalsigns.model.properties.StringProperty import StringProperty
 from vital_ai_vitalsigns.model.properties.URIProperty import URIProperty
```

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_Edge.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_Edge.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_HyperEdge.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_HyperEdge.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_HyperNode.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_HyperNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/VITAL_Node.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/VITAL_Node.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/DateTimeProperty.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/DateTimeProperty.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 from .IProperty import IProperty
 
 
 class DateTimeProperty(IProperty):
     def __init__(self, value: datetime):
         super().__init__(value)
 
+    def __bool__(self):
+        return self.value is not None
+
+    def __getattr__(self, attr):
+        return getattr(self.value, attr)
+
     def __str__(self):
         return self.value.strftime('%Y-%m-%d')
 
     def __eq__(self, other):
         if isinstance(other, datetime):
             return self.value == other
         elif isinstance(other, DateTimeProperty):
```

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/GeoLocationProperty.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/GeoLocationProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/IProperty.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/IProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/LongProperty.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/TruthProperty.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .IProperty import IProperty
 
 
-class LongProperty(IProperty):
-    def __init__(self, value: int):
+class TruthProperty(IProperty):
+    def __init__(self, value: str):
         super().__init__(value)
 
     def __str__(self):
         return str(self.value)
 
     def __eq__(self, other):
-        if isinstance(other, int):
+        if isinstance(other, str):
             return self.value == other
-        elif isinstance(other, LongProperty):
+        elif isinstance(other, TruthProperty):
             return self.value == other.value
         return NotImplemented
 
     def __rshift__(self, other):
         return self == other
 
     def to_json(self):
-        return {"value": self.value}
+        return {"value": self.value}
```

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/StringProperty.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/BooleanProperty.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from .IProperty import IProperty
 
 
-class StringProperty(IProperty):
-    def __init__(self, value: str):
+class BooleanProperty(IProperty):
+    def __init__(self, value: bool):
         super().__init__(value)
 
-    def __str__(self):
-        return str(self.value)
+    def __bool__(self):
+        return bool(self.value)
 
     def __eq__(self, other):
-        if isinstance(other, str):
+        if isinstance(other, bool):
             return self.value == other
-        elif isinstance(other, StringProperty):
+        elif isinstance(other, BooleanProperty):
             return self.value == other.value
         return NotImplemented
 
     def __rshift__(self, other):
         return self == other
 
     def to_json(self):
```

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/TruthProperty.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/URIProperty.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from .IProperty import IProperty
 
 
-class TruthProperty(IProperty):
+class URIProperty(IProperty):
     def __init__(self, value: str):
         super().__init__(value)
 
+    def __bool__(self):
+        return bool(self.value)
+
+    def __getattr__(self, attr):
+        return getattr(self.value, attr)
+
     def __str__(self):
         return str(self.value)
 
     def __eq__(self, other):
         if isinstance(other, str):
             return self.value == other
-        elif isinstance(other, TruthProperty):
+        elif isinstance(other, URIProperty):
             return self.value == other.value
         return NotImplemented
 
     def __rshift__(self, other):
         return self == other
 
     def to_json(self):
         return {"value": self.value}
+
```

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/properties/URIProperty.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/properties/DoubleProperty.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from .IProperty import IProperty
 
 
-class URIProperty(IProperty):
-    def __init__(self, value: str):
+class DoubleProperty(IProperty):
+    def __init__(self, value: float):
         super().__init__(value)
 
-    def __str__(self):
-        return str(self.value)
+    def __bool__(self):
+        return bool(self.value)
+
+    def __getattr__(self, attr):
+        return getattr(self.value, attr)
+
+    def __float__(self):
+        return float(self.value)
 
     def __eq__(self, other):
-        if isinstance(other, str):
+        if isinstance(other, float):
             return self.value == other
-        elif isinstance(other, URIProperty):
+        elif isinstance(other, DoubleProperty):
             return self.value == other.value
         return NotImplemented
 
     def __rshift__(self, other):
         return self == other
 
     def to_json(self):
```

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/model/trait/PropertyTrait.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/model/trait/PropertyTrait.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     @classmethod
     def get_uri(cls) -> str:
         """Returns the full URI combining namespace and local name."""
         return f"{cls.namespace}{cls.local_name}"
 
     @classmethod
     def get_short_name(cls) -> str:
-        """Transforms the local name into a short name by removing 'has' or 'is' prefixes and lowercasing the initial letter."""
+        """Transforms the local name into a short name by removing prefixes and lowercasing the initial letter."""
         name = cls.local_name
         if name.startswith("has"):
             name = name[3:]
         elif name.startswith("is"):
             name = name[2:]
 
         # Lowercase the first letter and return
```

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query/result_list.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query/result_list.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query/vital_graph_query.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query/vital_graph_query.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query/vital_query.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query/vital_query.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/query/vital_select_query.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/query/vital_select_query.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns/vitalsigns.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns/vitalsigns.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns.egg-info/PKG-INFO` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vital-ai-vitalsigns
-Version: 0.1.4
+Version: 0.1.5
 Summary: VitalSigns knowledge graph bindings
 Home-page: https://github.com/vital-ai/vital-vitalsigns-python
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns.egg-info/SOURCES.txt` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/AggregationResult.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/AggregationResult.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/DatabaseConnection.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/DatabaseConnection.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Dataset.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Dataset.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/DomainModel.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/DomainModel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_SameAs.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_SameAs.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasApp.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasApp.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasOrganization.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasOrganization.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasSegment.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasSegment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasSession.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasSession.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/Edge_hasTransaction.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/Edge_hasTransaction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/GraphMatch.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/GraphMatch.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/RDFStatement.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/RDFStatement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SparqlAskResponse.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SparqlAskResponse.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SparqlBinding.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SparqlBinding.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SqlResultRow.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SqlResultRow.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/SqlUpdateResponse.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/SqlUpdateResponse.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/URIReference.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/URIReference.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_Category.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_Category.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_Event.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_Event.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_PathQuery.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_PathQuery.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_Query.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_Query.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalApp.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalApp.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalAuthKey.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalAuthKey.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalOrganization.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalOrganization.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalProvisioning.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalProvisioning.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalSegment.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalSegment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceConfig.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceKey.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceKey.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceRootKey.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceRootKey.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalSession.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalSession.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.4/vital_ai_vitalsigns_core/model/VitalTransaction.py` & `vital-ai-vitalsigns-0.1.5/vital_ai_vitalsigns_core/model/VitalTransaction.py`

 * *Files identical despite different names*

