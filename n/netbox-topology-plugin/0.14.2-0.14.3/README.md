# Comparing `tmp/netbox-topology-plugin-0.14.2.tar.gz` & `tmp/netbox_topology_plugin-0.14.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-topology-plugin-0.14.2.tar", last modified: Thu Mar  7 05:26:23 2024, max compression
+gzip compressed data, was "netbox_topology_plugin-0.14.3.tar", last modified: Tue May  7 16:04:39 2024, max compression
```

## Comparing `netbox-topology-plugin-0.14.2.tar` & `netbox_topology_plugin-0.14.3.tar`

### file list

```diff
@@ -1,209 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.813794 netbox-topology-plugin-0.14.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15619 2024-03-07 05:26:23.813794 netbox-topology-plugin-0.14.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13603 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.769795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.769795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/api/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.769795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.761795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.769795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)    81084 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   155758 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/button_utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.769795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/img/dead_node.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.773795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/jquery/
--rw-r--r--   0 runner    (1001) docker     (127)    89476 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/jquery/jquery-3.5.1.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.773795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/jquery-ui-1.12.1/
--rw-r--r--   0 runner    (1001) docker     (127)   253669 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/jquery-ui-1.12.1/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    17386 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.773795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/
--rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.773795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/css/
--rw-r--r--   0 runner    (1001) docker     (127)   109158 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/css/next.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.773795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/api.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.773795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.773795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/css/external-small.png
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/css/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    18199 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/css/main.css
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.773795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/img/
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/img/spinner.gif
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.777795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/api-filter.js
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/api-list.js
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/api-search.js
--rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/apidocs.js
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/yui-prettify.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.765795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.777795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/CHANGES.html
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/README.html
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.css
--rw-r--r--   0 runner    (1001) docker     (127)    17803 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.805794 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    25234 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.Iterable.html
--rw-r--r--   0 runner    (1001) docker     (127)    48619 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.Object.html
--rw-r--r--   0 runner    (1001) docker     (127)    35302 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.Observable.html
--rw-r--r--   0 runner    (1001) docker     (127)    45639 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Collection.html
--rw-r--r--   0 runner    (1001) docker     (127)    37901 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.CollectionRelation.html
--rw-r--r--   0 runner    (1001) docker     (127)    18661 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Convex.html
--rw-r--r--   0 runner    (1001) docker     (127)    43043 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Counter.html
--rw-r--r--   0 runner    (1001) docker     (127)    33264 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Dictionary.html
--rw-r--r--   0 runner    (1001) docker     (127)    53932 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Edge.html
--rw-r--r--   0 runner    (1001) docker     (127)    59726 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.EdgeSet.html
--rw-r--r--   0 runner    (1001) docker     (127)   119401 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.EdgeSetCollection.html
--rw-r--r--   0 runner    (1001) docker     (127)    18999 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Force.html
--rw-r--r--   0 runner    (1001) docker     (127)    63973 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableCollection.html
--rw-r--r--   0 runner    (1001) docker     (127)    36330 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableDictionary.html
--rw-r--r--   0 runner    (1001) docker     (127)    16431 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.ForceProcessor.html
--rw-r--r--   0 runner    (1001) docker     (127)    16439 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.NeXtForceProcessor.html
--rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.QuickProcessor.html
--rw-r--r--   0 runner    (1001) docker     (127)    55235 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.html
--rw-r--r--   0 runner    (1001) docker     (127)    35562 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableObject.html
--rw-r--r--   0 runner    (1001) docker     (127)    45256 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Query.html
--rw-r--r--   0 runner    (1001) docker     (127)    49392 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.SortedMap.html
--rw-r--r--   0 runner    (1001) docker     (127)    62409 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Vertex.html
--rw-r--r--   0 runner    (1001) docker     (127)    71085 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.VertexSet.html
--rw-r--r--   0 runner    (1001) docker     (127)    19005 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.BezierCurve.html
--rw-r--r--   0 runner    (1001) docker     (127)    32582 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Line.html
--rw-r--r--   0 runner    (1001) docker     (127)    16363 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Math.html
--rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Matrix.html
--rw-r--r--   0 runner    (1001) docker     (127)    35270 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Vector.html
--rw-r--r--   0 runner    (1001) docker     (127)    82638 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.BezierCurves.html
--rw-r--r--   0 runner    (1001) docker     (127)    78093 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Circle.html
--rw-r--r--   0 runner    (1001) docker     (127)    75391 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Component.html
--rw-r--r--   0 runner    (1001) docker     (127)    39045 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.DragManager.html
--rw-r--r--   0 runner    (1001) docker     (127)    78090 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Group.html
--rw-r--r--   0 runner    (1001) docker     (127)    79964 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Icon.html
--rw-r--r--   0 runner    (1001) docker     (127)    25185 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Icons.html
--rw-r--r--   0 runner    (1001) docker     (127)    78997 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Image.html
--rw-r--r--   0 runner    (1001) docker     (127)    78087 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Line.html
--rw-r--r--   0 runner    (1001) docker     (127)    47423 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.LinkSetTooltipContent.html
--rw-r--r--   0 runner    (1001) docker     (127)    47417 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.LinkTooltipContent.html
--rw-r--r--   0 runner    (1001) docker     (127)    47451 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.NodeTooltipContent.html
--rw-r--r--   0 runner    (1001) docker     (127)    78087 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Path.html
--rw-r--r--   0 runner    (1001) docker     (127)    79031 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Polygon.html
--rw-r--r--   0 runner    (1001) docker     (127)    78087 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Rect.html
--rw-r--r--   0 runner    (1001) docker     (127)    64159 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Stage.html
--rw-r--r--   0 runner    (1001) docker     (127)    78993 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Text.html
--rw-r--r--   0 runner    (1001) docker     (127)    96941 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractLink.html
--rw-r--r--   0 runner    (1001) docker     (127)   104702 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractNode.html
--rw-r--r--   0 runner    (1001) docker     (127)    17814 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Categories.html
--rw-r--r--   0 runner    (1001) docker     (127)    82659 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.CircleGroup.html
--rw-r--r--   0 runner    (1001) docker     (127)    21210 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Config.html
--rw-r--r--   0 runner    (1001) docker     (127)    37494 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.DefaultScene.html
--rw-r--r--   0 runner    (1001) docker     (127)    65840 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Event.html
--rw-r--r--   0 runner    (1001) docker     (127)    37371 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Graph.html
--rw-r--r--   0 runner    (1001) docker     (127)    81928 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupItem.html
--rw-r--r--   0 runner    (1001) docker     (127)    95877 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupsLayer.html
--rw-r--r--   0 runner    (1001) docker     (127)    86763 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Layer.html
--rw-r--r--   0 runner    (1001) docker     (127)    23428 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LayoutMixin.html
--rw-r--r--   0 runner    (1001) docker     (127)   123134 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Link.html
--rw-r--r--   0 runner    (1001) docker     (127)    45654 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkMixin.html
--rw-r--r--   0 runner    (1001) docker     (127)   131521 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkSet.html
--rw-r--r--   0 runner    (1001) docker     (127)    93323 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LinksLayer.html
--rw-r--r--   0 runner    (1001) docker     (127)   129258 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Node.html
--rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeMixin.html
--rw-r--r--   0 runner    (1001) docker     (127)   135707 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeSet.html
--rw-r--r--   0 runner    (1001) docker     (127)    96743 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.NodesLayer.html
--rw-r--r--   0 runner    (1001) docker     (127)    85369 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Path.html
--rw-r--r--   0 runner    (1001) docker     (127)    91173 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.PathLayer.html
--rw-r--r--   0 runner    (1001) docker     (127)    82662 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.PolygonGroup.html
--rw-r--r--   0 runner    (1001) docker     (127)    82658 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.RectGroup.html
--rw-r--r--   0 runner    (1001) docker     (127)    37180 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Scene.html
--rw-r--r--   0 runner    (1001) docker     (127)    23767 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.SceneMixin.html
--rw-r--r--   0 runner    (1001) docker     (127)    38916 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionNodeScene.html
--rw-r--r--   0 runner    (1001) docker     (127)    37480 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionScene.html
--rw-r--r--   0 runner    (1001) docker     (127)    43075 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.StageMixin.html
--rw-r--r--   0 runner    (1001) docker     (127)    66091 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Tooltip.html
--rw-r--r--   0 runner    (1001) docker     (127)    58522 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipManager.html
--rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipMixin.html
--rw-r--r--   0 runner    (1001) docker     (127)    16446 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipPolicy.html
--rw-r--r--   0 runner    (1001) docker     (127)    19201 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.USMapLayout.html
--rw-r--r--   0 runner    (1001) docker     (127)    37528 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.ZoomBySelection.html
--rw-r--r--   0 runner    (1001) docker     (127)   217923 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.html
--rw-r--r--   0 runner    (1001) docker     (127)    78089 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Triangle.html
--rw-r--r--   0 runner    (1001) docker     (127)    42047 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.html
--rw-r--r--   0 runner    (1001) docker     (127)    45721 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.AbstractComponent.html
--rw-r--r--   0 runner    (1001) docker     (127)    48292 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Application.html
--rw-r--r--   0 runner    (1001) docker     (127)    47377 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Component.html
--rw-r--r--   0 runner    (1001) docker     (127)    29569 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.CssClass.html
--rw-r--r--   0 runner    (1001) docker     (127)    29569 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.CssStyle.html
--rw-r--r--   0 runner    (1001) docker     (127)    53483 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.DOMComponent.html
--rw-r--r--   0 runner    (1001) docker     (127)    64459 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Popover.html
--rw-r--r--   0 runner    (1001) docker     (127)    62226 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Popup.html
--rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.PopupContainer.html
--rw-r--r--   0 runner    (1001) docker     (127)    33822 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.Env.html
--rw-r--r--   0 runner    (1001) docker     (127)    30512 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.Util.html
--rw-r--r--   0 runner    (1001) docker     (127)    53166 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Document.html
--rw-r--r--   0 runner    (1001) docker     (127)    66752 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Element.html
--rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Fragment.html
--rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Node.html
--rw-r--r--   0 runner    (1001) docker     (127)    16811 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Text.html
--rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.widget.ZIndexManager.html
--rw-r--r--   0 runner    (1001) docker     (127)   488048 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/data.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.805794 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/files/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/files/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.805794 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    20154 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.data.html
--rw-r--r--   0 runner    (1001) docker     (127)    16998 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.geometry.html
--rw-r--r--   0 runner    (1001) docker     (127)    24856 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.graphic.Topology.html
--rw-r--r--   0 runner    (1001) docker     (127)    19379 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.graphic.html
--rw-r--r--   0 runner    (1001) docker     (127)    16910 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.html
--rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.ui.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.809794 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    53944 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/CiscoSansExtraLight.otf
--rw-r--r--   0 runner    (1001) docker     (127)    52108 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/CiscoSansRegular.otf
--rw-r--r--   0 runner    (1001) docker     (127)    44036 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)    50305 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)    43832 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23556 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    44332 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)    48996 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)    44140 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    24084 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    26072 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.eot
--rw-r--r--   0 runner    (1001) docker     (127)   101322 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25900 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    25976 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.woff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.809794 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/js/
--rw-r--r--   0 runner    (1001) docker     (127)   554834 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/js/next.js
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.765795 netbox-topology-plugin-0.14.2/netbox_topology_plugin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.813794 netbox-topology-plugin-0.14.2/netbox_topology_plugin/templates/netbox_topology_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/templates/netbox_topology_plugin/site_topo_button.html
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/templates/netbox_topology_plugin/site_topo_button_3.x.html
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/templates/netbox_topology_plugin/site_topology.html
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/templates/netbox_topology_plugin/site_topology_3.x.html
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/templates/netbox_topology_plugin/topology.html
--rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/templates/netbox_topology_plugin/topology_3.x.html
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    22436 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:26:23.813794 netbox-topology-plugin-0.14.2/netbox_topology_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15619 2024-03-07 05:26:23.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16614 2024-03-07 05:26:23.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 05:26:23.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-07 05:26:23.000000 netbox-topology-plugin-0.14.2/netbox_topology_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-07 05:26:16.000000 netbox-topology-plugin-0.14.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 05:26:23.813794 netbox-topology-plugin-0.14.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.647892 netbox_topology_plugin-0.14.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15619 2024-05-07 16:04:39.647892 netbox_topology_plugin-0.14.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13603 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.607892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.607892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.607892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/constants/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/constants/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.611892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/migrations/0002_alter_savedtopology_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/migrations/0003_alter_savedtopology_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.603892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.611892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)    81084 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   155758 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/button_utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.611892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/img/dead_node.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.611892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/jquery/
+-rw-r--r--   0 runner    (1001) docker     (127)    89476 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/jquery/jquery-3.5.1.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.611892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/jquery-ui-1.12.1/
+-rw-r--r--   0 runner    (1001) docker     (127)   253669 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/jquery-ui-1.12.1/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17386 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.611892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.611892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   109158 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/css/next.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.611892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/api.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.615892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.615892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/css/external-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/css/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18199 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.615892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/img/spinner.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.615892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/api-filter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/api-list.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/api-search.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/apidocs.js
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/yui-prettify.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.603892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.615892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/CHANGES.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/README.html
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    17803 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.639892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25234 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.Iterable.html
+-rw-r--r--   0 runner    (1001) docker     (127)    48619 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.Object.html
+-rw-r--r--   0 runner    (1001) docker     (127)    35302 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.Observable.html
+-rw-r--r--   0 runner    (1001) docker     (127)    45639 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)    37901 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.CollectionRelation.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18661 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Convex.html
+-rw-r--r--   0 runner    (1001) docker     (127)    43043 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Counter.html
+-rw-r--r--   0 runner    (1001) docker     (127)    33264 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Dictionary.html
+-rw-r--r--   0 runner    (1001) docker     (127)    53932 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Edge.html
+-rw-r--r--   0 runner    (1001) docker     (127)    59726 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.EdgeSet.html
+-rw-r--r--   0 runner    (1001) docker     (127)   119401 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.EdgeSetCollection.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18999 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Force.html
+-rw-r--r--   0 runner    (1001) docker     (127)    63973 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableCollection.html
+-rw-r--r--   0 runner    (1001) docker     (127)    36330 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableDictionary.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16431 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.ForceProcessor.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16439 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.NeXtForceProcessor.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.QuickProcessor.html
+-rw-r--r--   0 runner    (1001) docker     (127)    55235 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.html
+-rw-r--r--   0 runner    (1001) docker     (127)    35562 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableObject.html
+-rw-r--r--   0 runner    (1001) docker     (127)    45256 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Query.html
+-rw-r--r--   0 runner    (1001) docker     (127)    49392 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.SortedMap.html
+-rw-r--r--   0 runner    (1001) docker     (127)    62409 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Vertex.html
+-rw-r--r--   0 runner    (1001) docker     (127)    71085 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.VertexSet.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19005 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.BezierCurve.html
+-rw-r--r--   0 runner    (1001) docker     (127)    32582 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Line.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16363 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Math.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Matrix.html
+-rw-r--r--   0 runner    (1001) docker     (127)    35270 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Vector.html
+-rw-r--r--   0 runner    (1001) docker     (127)    82638 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.BezierCurves.html
+-rw-r--r--   0 runner    (1001) docker     (127)    78093 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Circle.html
+-rw-r--r--   0 runner    (1001) docker     (127)    75391 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Component.html
+-rw-r--r--   0 runner    (1001) docker     (127)    39045 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.DragManager.html
+-rw-r--r--   0 runner    (1001) docker     (127)    78090 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Group.html
+-rw-r--r--   0 runner    (1001) docker     (127)    79964 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25185 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Icons.html
+-rw-r--r--   0 runner    (1001) docker     (127)    78997 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Image.html
+-rw-r--r--   0 runner    (1001) docker     (127)    78087 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Line.html
+-rw-r--r--   0 runner    (1001) docker     (127)    47423 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.LinkSetTooltipContent.html
+-rw-r--r--   0 runner    (1001) docker     (127)    47417 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.LinkTooltipContent.html
+-rw-r--r--   0 runner    (1001) docker     (127)    47451 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.NodeTooltipContent.html
+-rw-r--r--   0 runner    (1001) docker     (127)    78087 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Path.html
+-rw-r--r--   0 runner    (1001) docker     (127)    79031 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Polygon.html
+-rw-r--r--   0 runner    (1001) docker     (127)    78087 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Rect.html
+-rw-r--r--   0 runner    (1001) docker     (127)    64159 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Stage.html
+-rw-r--r--   0 runner    (1001) docker     (127)    78993 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Text.html
+-rw-r--r--   0 runner    (1001) docker     (127)    96941 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractLink.html
+-rw-r--r--   0 runner    (1001) docker     (127)   104702 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractNode.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17814 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Categories.html
+-rw-r--r--   0 runner    (1001) docker     (127)    82659 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.CircleGroup.html
+-rw-r--r--   0 runner    (1001) docker     (127)    21210 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Config.html
+-rw-r--r--   0 runner    (1001) docker     (127)    37494 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.DefaultScene.html
+-rw-r--r--   0 runner    (1001) docker     (127)    65840 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Event.html
+-rw-r--r--   0 runner    (1001) docker     (127)    37371 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Graph.html
+-rw-r--r--   0 runner    (1001) docker     (127)    81928 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupItem.html
+-rw-r--r--   0 runner    (1001) docker     (127)    95877 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupsLayer.html
+-rw-r--r--   0 runner    (1001) docker     (127)    86763 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Layer.html
+-rw-r--r--   0 runner    (1001) docker     (127)    23428 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LayoutMixin.html
+-rw-r--r--   0 runner    (1001) docker     (127)   123134 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Link.html
+-rw-r--r--   0 runner    (1001) docker     (127)    45654 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkMixin.html
+-rw-r--r--   0 runner    (1001) docker     (127)   131521 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkSet.html
+-rw-r--r--   0 runner    (1001) docker     (127)    93323 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LinksLayer.html
+-rw-r--r--   0 runner    (1001) docker     (127)   129258 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Node.html
+-rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeMixin.html
+-rw-r--r--   0 runner    (1001) docker     (127)   135707 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeSet.html
+-rw-r--r--   0 runner    (1001) docker     (127)    96743 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.NodesLayer.html
+-rw-r--r--   0 runner    (1001) docker     (127)    85369 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Path.html
+-rw-r--r--   0 runner    (1001) docker     (127)    91173 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.PathLayer.html
+-rw-r--r--   0 runner    (1001) docker     (127)    82662 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.PolygonGroup.html
+-rw-r--r--   0 runner    (1001) docker     (127)    82658 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.RectGroup.html
+-rw-r--r--   0 runner    (1001) docker     (127)    37180 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Scene.html
+-rw-r--r--   0 runner    (1001) docker     (127)    23767 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.SceneMixin.html
+-rw-r--r--   0 runner    (1001) docker     (127)    38916 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionNodeScene.html
+-rw-r--r--   0 runner    (1001) docker     (127)    37480 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionScene.html
+-rw-r--r--   0 runner    (1001) docker     (127)    43075 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.StageMixin.html
+-rw-r--r--   0 runner    (1001) docker     (127)    66091 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Tooltip.html
+-rw-r--r--   0 runner    (1001) docker     (127)    58522 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipManager.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipMixin.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16446 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipPolicy.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19201 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.USMapLayout.html
+-rw-r--r--   0 runner    (1001) docker     (127)    37528 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.ZoomBySelection.html
+-rw-r--r--   0 runner    (1001) docker     (127)   217923 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.html
+-rw-r--r--   0 runner    (1001) docker     (127)    78089 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Triangle.html
+-rw-r--r--   0 runner    (1001) docker     (127)    42047 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.html
+-rw-r--r--   0 runner    (1001) docker     (127)    45721 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.AbstractComponent.html
+-rw-r--r--   0 runner    (1001) docker     (127)    48292 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Application.html
+-rw-r--r--   0 runner    (1001) docker     (127)    47377 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Component.html
+-rw-r--r--   0 runner    (1001) docker     (127)    29569 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.CssClass.html
+-rw-r--r--   0 runner    (1001) docker     (127)    29569 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.CssStyle.html
+-rw-r--r--   0 runner    (1001) docker     (127)    53483 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.DOMComponent.html
+-rw-r--r--   0 runner    (1001) docker     (127)    64459 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Popover.html
+-rw-r--r--   0 runner    (1001) docker     (127)    62226 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Popup.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.PopupContainer.html
+-rw-r--r--   0 runner    (1001) docker     (127)    33822 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.Env.html
+-rw-r--r--   0 runner    (1001) docker     (127)    30512 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.Util.html
+-rw-r--r--   0 runner    (1001) docker     (127)    53166 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Document.html
+-rw-r--r--   0 runner    (1001) docker     (127)    66752 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Element.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Fragment.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Node.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16811 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Text.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.widget.ZIndexManager.html
+-rw-r--r--   0 runner    (1001) docker     (127)   488048 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/data.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.639892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/files/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.639892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20154 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.data.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16998 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.geometry.html
+-rw-r--r--   0 runner    (1001) docker     (127)    24856 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.graphic.Topology.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19379 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.graphic.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16910 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.ui.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.643892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    53944 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/CiscoSansExtraLight.otf
+-rw-r--r--   0 runner    (1001) docker     (127)    52108 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/CiscoSansRegular.otf
+-rw-r--r--   0 runner    (1001) docker     (127)    44036 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    50305 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    43832 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23556 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    44332 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    48996 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    44140 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    24084 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    26072 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   101322 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25900 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    25976 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.woff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.643892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   554834 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/js/next.js
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.603892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.647892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/templates/netbox_topology_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/templates/netbox_topology_plugin/site_topo_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/templates/netbox_topology_plugin/site_topology.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/templates/netbox_topology_plugin/topology.html
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.647892 netbox_topology_plugin-0.14.3/netbox_topology_plugin/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/utils/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/utils/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/utils/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13749 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/utils/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:04:39.647892 netbox_topology_plugin-0.14.3/netbox_topology_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15619 2024-05-07 16:04:39.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16891 2024-05-07 16:04:39.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:04:39.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 16:04:39.000000 netbox_topology_plugin-0.14.3/netbox_topology_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-07 16:04:32.000000 netbox_topology_plugin-0.14.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:04:39.647892 netbox_topology_plugin-0.14.3/setup.cfg
```

### Comparing `netbox-topology-plugin-0.14.2/LICENSE` & `netbox_topology_plugin-0.14.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/PKG-INFO` & `netbox_topology_plugin-0.14.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-topology-plugin
-Version: 0.14.2
+Version: 0.14.3
 Summary: Netbox Topology Plugin, fork of netbox-topology-plugin.  Powered by NextUI
 Author-email: Daniel Sheppard <dans@dansheps.com>, Igor Korotchenkov <iDebugAll@gmail.com>
 Maintainer-email: Daniel Sheppard <dans@dansheps.com>
 License: MIT License
         
         Copyright (c) 2024 Daniel Sheppard
         Copyright (c) 2020 Igor Korotchenkov
```

### Comparing `netbox-topology-plugin-0.14.2/README.md` & `netbox_topology_plugin-0.14.3/README.md`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/api/serializers.py` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/filters.py` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/migrations/0001_initial.py` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/migrations/0001_initial.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 from django.db import migrations, models
 import django.db.models.deletion
 
 
+def getusermodel():
+    try:
+        from users.models import NetBoxUser
+        return 'users.netboxuser'
+    except ImportError:
+        return 'users.user'
+
+
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
         ('users', '0010_update_jsonfield'),
     ]
@@ -15,11 +23,11 @@
             name='SavedTopology',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False)),
                 ('name', models.CharField(blank=True, max_length=100)),
                 ('topology', models.JSONField()),
                 ('layout_context', models.JSONField(blank=True, null=True)),
                 ('timestamp', models.DateTimeField()),
-                ('created_by', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='users.netboxuser')),
+                ('created_by', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=getusermodel())),
             ],
         ),
     ]
```

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/bootstrap.bundle.min.js` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/bootstrap.min.css` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/button_utils.js` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/button_utils.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/img/dead_node.png` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/img/dead_node.png`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/jquery/jquery-3.5.1.min.js` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/jquery/jquery-3.5.1.min.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/jquery-ui-1.12.1/jquery-ui.min.js` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/jquery-ui-1.12.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_app.js` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_app.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/LICENSE.txt` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/css/next.css` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/css/next.css`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/api.js` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/api.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/css/logo.png` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/css/logo.png`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/css/main.css` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/css/main.css`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/favicon.ico` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/img/spinner.gif` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/img/spinner.gif`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/api-filter.js` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/api-filter.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/api-list.js` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/api-list.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/api-search.js` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/api-search.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/apidocs.js` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/js/apidocs.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/CHANGES.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/CHANGES.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/COPYING` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/COPYING`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/README.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/README.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.css` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.css`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.js` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/assets/vendor/prettify/prettify-min.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.Iterable.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.Iterable.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.Object.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.Object.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.Observable.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.Observable.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Collection.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Collection.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.CollectionRelation.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.CollectionRelation.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Convex.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Convex.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Counter.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Counter.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Dictionary.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Dictionary.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Edge.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Edge.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.EdgeSet.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.EdgeSet.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.EdgeSetCollection.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.EdgeSetCollection.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Force.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Force.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableCollection.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableCollection.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableDictionary.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableDictionary.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.ForceProcessor.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.ForceProcessor.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.NeXtForceProcessor.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.NeXtForceProcessor.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.QuickProcessor.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.QuickProcessor.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableGraph.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableObject.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.ObservableObject.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Query.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Query.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.SortedMap.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.SortedMap.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Vertex.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.Vertex.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.VertexSet.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.data.VertexSet.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.BezierCurve.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.BezierCurve.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Line.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Line.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Math.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Math.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Matrix.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Matrix.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Vector.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.geometry.Vector.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.BezierCurves.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.BezierCurves.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Circle.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Circle.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Component.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Component.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.DragManager.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.DragManager.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Group.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Group.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Icon.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Icon.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Icons.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Icons.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Image.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Image.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Line.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Line.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.LinkSetTooltipContent.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.LinkSetTooltipContent.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.LinkTooltipContent.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.LinkTooltipContent.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.NodeTooltipContent.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.NodeTooltipContent.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Path.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Path.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Polygon.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Polygon.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Rect.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Rect.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Stage.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Stage.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Text.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Text.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractLink.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractLink.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractNode.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.AbstractNode.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Categories.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Categories.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.CircleGroup.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.CircleGroup.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Config.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Config.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.DefaultScene.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.DefaultScene.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Event.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Event.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Graph.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Graph.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupItem.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupItem.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupsLayer.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.GroupsLayer.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Layer.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Layer.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LayoutMixin.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LayoutMixin.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Link.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Link.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkMixin.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkMixin.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkSet.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LinkSet.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LinksLayer.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.LinksLayer.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Node.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Node.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeMixin.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeMixin.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeSet.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.NodeSet.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.NodesLayer.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.NodesLayer.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Path.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Path.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.PathLayer.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.PathLayer.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.PolygonGroup.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.PolygonGroup.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.RectGroup.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.RectGroup.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Scene.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Scene.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.SceneMixin.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.SceneMixin.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionNodeScene.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionNodeScene.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionScene.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.SelectionScene.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.StageMixin.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.StageMixin.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Tooltip.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.Tooltip.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipManager.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipManager.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipMixin.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipMixin.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipPolicy.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.TooltipPolicy.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.USMapLayout.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.USMapLayout.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.ZoomBySelection.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.ZoomBySelection.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Topology.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Triangle.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.graphic.Triangle.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.AbstractComponent.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.AbstractComponent.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Application.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Application.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Component.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Component.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.CssClass.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.CssClass.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.CssStyle.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.CssStyle.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.DOMComponent.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.DOMComponent.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Popover.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Popover.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Popup.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.Popup.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.PopupContainer.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.PopupContainer.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.Env.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.Env.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.Util.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.Util.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Document.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Document.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Element.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Element.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Fragment.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Fragment.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Node.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Node.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Text.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.ui.nx.dom.Text.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.widget.ZIndexManager.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/classes/nx.widget.ZIndexManager.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/data.json` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/data.json`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/index.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/index.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.data.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.data.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.geometry.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.geometry.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.graphic.Topology.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.graphic.Topology.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.graphic.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.graphic.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.ui.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/doc/modules/nx.ui.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/CiscoSansExtraLight.otf` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/CiscoSansExtraLight.otf`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/CiscoSansRegular.otf` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/CiscoSansRegular.otf`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.eot` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.eot`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.svg` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.ttf` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.ttf`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.woff` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansextralight-webfont.woff`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.eot` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.eot`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.svg` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.ttf` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.woff` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.woff`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.eot` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.eot`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.svg` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.ttf` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.ttf`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.woff` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.woff`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/js/next.js` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/static/netbox_topology_plugin/next_sources/js/next.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/template_content.py` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/template_content.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,16 +9,13 @@
 class SiteTopologyButtons(PluginTemplateExtension):
     """
     Extend the DCIM site template to include content from this plugin.
     """
     model = 'dcim.site'
 
     def buttons(self):
-        if NETBOX_CURRENT_VERSION >= version.parse("3.0"):
-            return self.render('netbox_topology_plugin/site_topo_button_3.x.html')
-        else:
-            return self.render('netbox_topology_plugin/site_topo_button.html')
+        return self.render('netbox_topology_plugin/site_topo_button.html')
 
 
 # PluginTemplateExtension subclasses must be packaged into an iterable named
 # template_extensions to be imported by NetBox.
 template_extensions = [SiteTopologyButtons]
```

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/templates/netbox_topology_plugin/site_topo_button.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/templates/netbox_topology_plugin/site_topo_button.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-<button type="button" class="btn btn-primary" data-toggle="modal" data-target="#topology_modal" data-obj="{{ object.name }}" title="Show site topology">
+<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#topology_modal" data-bs-obj="{{ object.name }}" title="Show site topology">
     <i class="fa fa-signal" aria-hidden="true"></i>
     Topology
 </button>
 
 <div class="modal fade" id="topology_modal" tabindex="-1" role="dialog">
     <div class="modal-dialog modal-lg" role="document">
         <div class="modal-content">
                 <div class="modal-header">
-                    <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
-                    <h2 class="modal-title" style="text-align: center;"><a href={% url 'plugins:netbox_topology_plugin:topology' %}?site_id={{ object.id }}>{{ object.name }} Topology</a></h2>
+                    <button type="button" class="btn btn-sm btn-danger" data-bs-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
+                    <h2 class="modal-title" style="text-align: center;width:100%;"><a href={% url 'plugins:netbox_topology_plugin:topology' %}?site_id={{ object.id }}>{{ object.name }} Topology</a></h2>
                 </div>
         <iframe src="{% url 'plugins:netbox_topology_plugin:site_topology' %}?site_id={{ object.id }}" style="height: 75vh; width: 100%;"></iframe>
         </div>
     </div>
-</div>
+</div>
```

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/templates/netbox_topology_plugin/site_topology.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/templates/netbox_topology_plugin/site_topology.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,55 @@
+{% extends 'base/base.html' %}
 {% load static %}
 
-<!DOCTYPE html>
-
-<html>
-    <head>
-        <meta charset="utf-8">
+{% block head %}
         <link rel="stylesheet"href="{% static 'netbox_topology_plugin/next_sources/css/next.css' %}">
-        <link rel="stylesheet"href="{% static 'netbox_topology_plugin/bootstrap.min.css' %}">
-        <link rel="stylesheet"href="{% static 'font-awesome-4.7.0/css/font-awesome.min.css' %}">
         <script src="{% static 'netbox_topology_plugin/next_sources/js/next.js' %}"></script>
         <script src="{% static 'netbox_topology_plugin/button_utils.js' %}"></script>
-    </head>
-    <body>
+
+{% endblock %} 
+
+{% block layout %}
+
         <div class="container-sm ml-4 my-sm-3" id="nx-ui-topology">
-            <div class="row">
-              <div class="col-xs-4">
-                <div class="btn-group">
-                    <button class="btn btn-outline-secondary btn-sm " onclick='horizontal()'>Horizontal Layout</button>
-                    <button class="btn btn-outline-secondary btn-sm" onclick="vertical()">Vertical Layout</button>
-                </div>
+            <div class="control-group">
+              <div class="btn-group">
+                  <button class="btn btn-primary btn-sm " onclick='horizontal()'>Horizontal Layout</button>
+                  <button class="btn btn-primary btn-sm" onclick="vertical()">Vertical Layout</button>
               </div>
-              <div class="col-xs-4 ml-2">
-                <input class="btn btn-outline-secondary btn-sm" type="button" id="showHideUndonnectedButton" value="" onclick="return showHideUndonnectedButtonOnClick(this);" />
-              </div>
-              <div class="col-xs-4 ml-2">
-                <input class="btn btn-outline-secondary btn-sm" type="button" id="showHidePassiveDevicesButton" value="" onclick="return showHidePassiveDevicesButtonOnClick(this);" />
-              </div>
-              <div class="col-xs-4 ml-2">
-                <div class="dropdown">
-                    <button class="btn btn-outline-secondary btn-sm dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
-                      Select Layers
-                    </button>
-                    <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
-                        <h6 class="dropdown-header">Device Roles</h6>
-                        <div class="dropdown-divider"></div>
-                        {% for device_role_slug, device_role_name, is_visible in device_roles %}
+              <input class="btn btn-primary btn-sm" type="button" id="showHideUndonnectedButton" value="" onclick="return showHideUndonnectedButtonOnClick(this);" />
+              <input class="btn btn-primary btn-sm" type="button" id="showHidePassiveDevicesButton" value="" onclick="return showHidePassiveDevicesButtonOnClick(this);" />
+              <div class="dropdown btn-group">
+                  <button class="btn btn-primary btn-sm dropdown-toggle" type="button" id="dropdownMenuButton" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
+                    Select Layers
+                  </button>
+                  <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
+                      <h6 class="dropdown-header">Device Roles</h6>
+                      <div class="dropdown-divider"></div>
+                      {% for device_role_slug, device_role_name, is_visible in device_roles %}
+                          <div class="checkbox ml-1 my-1">
+                              <label>
+                                  <input onchange="layerSelectorOnChange(this)" type="checkbox" value="{{ device_role_slug }}" {{ is_visible|yesno:"checked," }}>{{ device_role_name }}
+                              </label>
+                          </div>
+                      {% endfor %}
+                      <div class="dropdown-divider"></div>
+                      {% if device_tags %}
+                        <h6 class="dropdown-header">Device Tags</h6>
+                        {% for tag, is_visible in device_tags %}
                             <div class="checkbox ml-1 my-1">
                                 <label>
-                                    <input onchange="layerSelectorOnChange(this)" type="checkbox" value="{{ device_role_slug }}" {{ is_visible|yesno:"checked," }}>{{ device_role_name }}
+                                   <input onchange="layerSelectorByTagOnChange(this)" type="checkbox" value="{{ tag }}"  {{ is_visible|yesno:"checked," }}>{{ tag }}
                                 </label>
                             </div>
                         {% endfor %}
-                        <div class="dropdown-divider"></div>
-                        {% if device_tags %}
-                          <h6 class="dropdown-header">Device Tags</h6>
-                          {% for tag, is_visible in device_tags %}
-                              <div class="checkbox ml-1 my-1">
-                                  <label>
-                                      <input onchange="layerSelectorByTagOnChange(this)" type="checkbox" value="{{ tag }}" {{ is_visible|yesno:"checked," }}>{{ tag }}
-                                  </label>
-                              </div>
-                          {% endfor %}
-                        {% endif %}
-                        <div class="dropdown-divider"></div>
-                    </div>
+                      {% endif %}
+                      <div class="dropdown-divider"></div>
                   </div>
-              </div>
+                </div>
             </div>
         </div>
         
         <script type="text/javascript">
             var displayUnconnected = {{ display_unconnected|yesno:"true,false" }};
             var displayPassiveDevices = {{ display_passive_devices|yesno:"true,false" }};
             var displayLogicalMultiCableLinks = {{ display_logical_multicable_links|yesno:"true,false" }};
@@ -70,13 +60,9 @@
             console.log(topologyData);
         </script>
         <script type="text/javascript">
             showHideUndonnectedButtonInitial();
             showHidePassiveDevicesButtonInitial();
         </script>
         <script src="{% static 'netbox_topology_plugin/next_app.js' %}"></script>
-        <script src="{% static 'jquery/jquery-3.4.1.min.js' %}"></script>
-        <script src="{% static 'jquery/jquery-3.5.1.min.js' %}"></script>
-        <script src="{% static 'jquery-ui-1.12.1/jquery-ui.min.js' %}"></script>
-        <script src="{% static 'netbox_topology_plugin/bootstrap.bundle.min.js' %}"></script>
-    </body>
-</html>
+
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
-{% load static %}
+{% extends 'base/base.html' %} {% load static %} {% block head %}
+{% endblock %} {% block layout %}
 Horizontal Layout Vertical Layout
-[Unknown INPUT type]
-[Unknown INPUT type]
+[Unknown INPUT type][Unknown INPUT type]
 Select Layers
 ** DDeevviiccee RRoolleess **
 {% for device_role_slug, device_role_name, is_visible in device_roles %}
 { is_visible|yesno:"checked," }}>{{ device_role_name }}
 {% endfor %}
 {% if device_tags %}
 ** DDeevviiccee TTaaggss **
 {% for tag, is_visible in device_tags %}
 { is_visible|yesno:"checked," }}>{{ tag }}
 {% endfor %} {% endif %}
+{% endblock %}
```

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin/templates/netbox_topology_plugin/topology.html` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin/templates/netbox_topology_plugin/topology.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,115 +1,140 @@
-{% extends 'base.html' %}
+{% extends 'base/layout.html' %}
 {% load buttons %}
 {% load static %}
+{% load plugins %}
+{% load helpers %}
 
 {% block header %}
 <script src="{% static 'netbox_topology_plugin/next_sources/js/next.js' %}"></script>
 <link rel="stylesheet"href="{% static 'netbox_topology_plugin/next_sources/css/next.css' %}">
 <script src="{% static 'netbox_topology_plugin/button_utils.js' %}"></script>
 {% endblock %}
 
 {% block content %}
 
-<h2>Topology Viewer</h2>
-
-<div class="col-md-3 pull-right right-side-panel noprint" style="z-index: 2;">
-    {% include 'inc/search_panel.html' %}
-    {% block sidebar %}{% endblock %}
-    <div class="panel panel-default">
-        <div class="panel-heading">
-            <span class="mdi mdi-magnify" aria-hidden="true"></span>
-            <strong>Load Saved View</strong>
-        </div>
-        <div class="panel-body">
-            <form action="." method="get" class="form">
-                {% for field in load_saved_filter_form.visible_fields %}
-                    <div class="form-group">
-                            {{ field.label_tag }}
-                            {{ field }}
-                    </div>
-                {% endfor %}
-                <div class="text-right noprint">
-                    <button type="submit" class="btn btn-primary">
-                        <span class="mdi mdi-application-import" aria-hidden="true"></span> Apply
-                    </button>
-                    <a href="." class="btn btn-default">
-                        <span class="mdi mdi-close-thick" aria-hidden="true"></span> Clear
-                    </a>
-                </div>
-            </form>
-        </div>
+<div class="title-container px-3 pb-3">
+    <div id="content-title">
+        <h1 class="h2 w-100">Topology Viewer</h1>
     </div>
 </div>
-<div>
-    <div class="btn-group">
-        <button class="btn btn-primary " onclick='horizontal()'>Horizontal Layout</button>
-        <button class="btn btn-primary" onclick="vertical()">Vertical Layout</button>
-    </div>
-    <input class="btn btn-primary" type="button" id="showHideUndonnectedButton" value="" onclick="return showHideUndonnectedButtonOnClick(this);" />
-    <input class="btn btn-primary" type="button" id="showHidePassiveDevicesButton" value="" onclick="return showHidePassiveDevicesButtonOnClick(this);" />
-    <div class="btn-group">
-        <div class="dropdown">
-            <button class="btn btn-primary dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
-                Select Layers
-            </button>
-            <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
-                <h6 class="dropdown-header">Device Roles</h6>
-                <div class="dropdown-divider"></div>
-                {% for device_role_slug, device_role_name, is_visible in device_roles %}
-                    <div class="checkbox ml-1 my-1">
-                        <label>
-                            <input onchange="layerSelectorOnChange(this)" type="checkbox" value="{{ device_role_slug }}" {{ is_visible|yesno:"checked," }}>{{ device_role_name }}
-                        </label>
+
+<ul class="nav nav-tabs px-3">
+
+      <li class="nav-item" role="presentation">
+        <button class="nav-link active" id="topology-tab" data-bs-toggle="tab" data-bs-target="#topology" type="button" role="tab" aria-controls="topology" aria-selected="true">
+          Topology
+        </button>
+      </li>
+
+        <li class="nav-item" role="presentation">
+          <button class="nav-link" id="filters-form-tab" data-bs-toggle="tab" data-bs-target="#filters-form" type="button" role="tab" aria-controls="filters-form" aria-selected="false">
+            Filters
+          </button>
+        </li>
+
+
+</ul>
+
+<div class="tab-content">
+    <div class="tab-pane active" id="topology" role="tabpanel" aria-labelledby="topology-tab">
+
+        <div>
+
+            <div class="btn-group">
+                <button class="btn btn-primary " onclick='horizontal()'>Horizontal Layout</button>
+                <button class="btn btn-primary" onclick="vertical()">Vertical Layout</button>
+            </div>
+
+            <input class="btn btn-primary" type="button" id="showHideUndonnectedButton" value="" onclick="return showHideUndonnectedButtonOnClick(this);" />
+            <input class="btn btn-primary" type="button" id="showHidePassiveDevicesButton" value="" onclick="return showHidePassiveDevicesButtonOnClick(this);" />
+
+            <div class="btn-group">
+                <div class="dropdown">
+                    <button class="btn btn-primary dropdown-toggle" type="button" id="dropdownMenuButton" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
+                        Select Layers
+                    </button>
+                    <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
+                        <h6 class="dropdown-header">Device Roles</h6>
+                        <div class="dropdown-divider"></div>
+
+                        {% for device_role_slug, device_role_name, is_visible in device_roles %}
+                            <div class="checkbox ml-1 my-1">
+                                <label>
+                                    <input onchange="layerSelectorOnChange(this)" type="checkbox" value="{{ device_role_slug }}" {{ is_visible|yesno:"checked," }}>{{ device_role_name }}
+                                </label>
+                            </div>
+                        {% endfor %}
+
+                        <div class="dropdown-divider"></div>
+                        {% if device_tags %}
+                            <h6 class="dropdown-header">Device Tags</h6>
+                            {% for tag, is_visible in device_tags %}
+                                <div class="checkbox ml-1 my-1">
+                                    <label>
+                                        <input onchange="layerSelectorByTagOnChange(this)" type="checkbox" value="{{ tag }}" {{ is_visible|yesno:"checked," }}>{{ tag }}
+                                    </label>
+                                </div>
+                            {% endfor %}
+                        {% endif %}
+                        <div class="dropdown-divider"></div>
                     </div>
-                {% endfor %}
-                <div class="dropdown-divider"></div>
-                {% if device_tags %}
-                    <h6 class="dropdown-header">Device Tags</h6>
-                    {% for tag, is_visible in device_tags %}
-                        <div class="checkbox ml-1 my-1">
-                            <label>
-                                <input onchange="layerSelectorByTagOnChange(this)" type="checkbox" value="{{ tag }}" {{ is_visible|yesno:"checked," }}>{{ tag }}
-                            </label>
-                        </div>
-                    {% endfor %}
-                {% endif %}
-                <div class="dropdown-divider"></div>
+                </div>
             </div>
-        </div>
-    </div>
-    <div class="btn-group">
-        <div class="dropdown">
-            <button class="btn btn-primary dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
-                Save Current View
-            </button>
-            <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
-                <h6 class="dropdown-header">Saved View Name:</h6>
-                <div style="margin-bottom: 5px; margin-left: 2px; margin-right: 2px;">
-                    <input type="text" id="topoSaveName" name="topoSaveName"></input>
+            <div class="btn-group">
+                <div class="dropdown">
+                    <button class="btn btn-primary dropdown-toggle" type="button" id="dropdownMenuButton" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
+                        Save Current View
+                    </button>
+                    <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
+                        <h6 class="dropdown-header">Saved View Name:</h6>
+                        <div style="margin-bottom: 5px; margin-left: 2px; margin-right: 2px;">
+                            <input type="text" id="topoSaveName" name="topoSaveName"></input>
+                        </div>
+                        <div style="margin-left: 2px; margin-right: 2px;">
+                            <label class="control-label col-sm-6 pull-left" for="saveTopologyView" id="saveResult" style="margin-top: 7px; margin-left:4px;"></label>
+                            <input class="btn btn-primary pull-right" type="button" id="saveTopologyView" value="Submit"  onclick="return saveView(topoSaveURI, netbox_csrf_token);" />
+                        </div>
+                    </div>
                 </div>
-                <div style="margin-left: 2px; margin-right: 2px;">
-                    <label class="control-label col-sm-6 pull-left" for="saveTopologyView" id="saveResult" style="margin-top: 7px; margin-left:4px;"></label>
-                    <input class="btn btn-primary pull-right" type="button" id="saveTopologyView" value="Submit" onclick="return saveView(topoSaveURI, netbox_csrf_token);" />
+            </div>
+            <div class="btn-group">
+                <button class="btn btn-primary dropdown-toggle" type="button" id="dropdownMenuButton" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
+                    Load Saved View
+                </button>
+                <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
+                    <form action="." method="get" class="form">
+                        <select name='saved_topology_id' class="form-select" id='id_saved_topology'>
+                                <option value selected>----------</option>
+                        {% for saved_topo in load_saved %}
+                                <option value="{{ saved_topo.id }}" >{{ saved_topo.name }}</option>
+                        {% endfor %}
+                        </select>
+                        <button type="submit" class="btn btn-primary">
+                            <span class="mdi mdi-application-import" aria-hidden="true"></span> Apply
+                        </button>
+                    </form>
                 </div>
             </div>
         </div>
-    </div>
-</div>
-<div class="row noprint" style="z-index: 1;">
-    <div class="col-lg-3" style="z-index: 1;">
-        <div class="pull-left noprint">
-            <div id="nx-ui-topology" class="container">
+        <div class="row noprint" style="z-index: 1;">
+            <div class="col-lg-3" style="z-index: 1;">
+                <div class="pull-left noprint">
+                    <div id="nx-ui-topology" class="container">
 
+                    </div>
+                </div>
             </div>
         </div>
     </div>
+    <div class="tab-pane" id="filters-form" role="tabpanel" aria-labelledby="filters-form-tab">
+        {% include 'inc/filter_list.html' %}
+    </div>
 </div>
 
-
 {% endblock %}
 
 {% block javascript %}
 
 
 <script type="text/javascript">
     var displayUnconnected = {{ display_unconnected|yesno:"true,false" }};
@@ -117,21 +142,23 @@
     var displayLogicalMultiCableLinks = {{ display_logical_multicable_links|yesno:"true,false" }};
     var undisplayedRoles = {{ undisplayed_roles|safe }};
     var undisplayedDeviceTags = {{ undisplayed_device_tags|safe }};
     var topologyData = {{ source_data|safe }};
     var topologySavedData = {{ source_data|safe }};
     var initialLayout = '{{ initial_layout|safe }}';
     var requestGET = {{ requestGET|safe }};
+    var netbox_csrf_token = '{{ csrf_token }}'
     var topoSaveURI = '{% url 'plugins-api:netbox_topology_plugin-api:savedtopology-list' %}';
     console.log(topologyData);
 </script>
 <script src="{% static 'netbox_topology_plugin/next_app.js' %}"></script>
+<script src="{% static 'netbox_topology_plugin/jquery/jquery-3.4.1.min.js' %}"></script>
+<script src="{% static 'netbox_topology_plugin/jquery/jquery-3.5.1.min.js' %}"></script>
+
 
 <script type="text/javascript">
     showHideUndonnectedButtonInitial();
     showHidePassiveDevicesButtonInitial();
 </script>
 
 {% endblock %}
 
-
-
```

#### html2text {}

```diff
@@ -1,17 +1,13 @@
-{% extends 'base.html' %} {% load buttons %} {% load static %} {% block header
-%}
+{% extends 'base/layout.html' %} {% load buttons %} {% load static %} {% load
+plugins %} {% load helpers %} {% block header %}
 {% endblock %} {% block content %}
-********** TTooppoollooggyy VViieewweerr **********
-{% include 'inc/search_panel.html' %} {% block sidebar %}{% endblock %}
-LLooaadd SSaavveedd VViieeww
-{% for field in load_saved_filter_form.visible_fields %}
-{{ field.label_tag }} {{ field }}
-{% endfor %}
-Apply _C_l_e_a_r
+************ TTooppoollooggyy VViieewweerr ************
+    * Topology
+    * Filters
 Horizontal Layout Vertical Layout
 [Unknown INPUT type][Unknown INPUT type]
 Select Layers
 ** DDeevviiccee RRoolleess **
 {% for device_role_slug, device_role_name, is_visible in device_roles %}
 { is_visible|yesno:"checked," }}>{{ device_role_name }}
 {% endfor %}
@@ -20,9 +16,15 @@
 {% for tag, is_visible in device_tags %}
 { is_visible|yesno:"checked," }}>{{ tag }}
 {% endfor %} {% endif %}
 Save Current View
 ** SSaavveedd VViieeww NNaammee:: **
 [topoSaveName        ]
 [Unknown INPUT type]
+Load Saved View
+{% for saved_topo in load_saved %}
+{{ saved_topo.name }}
+{% endfor %}
+Apply
+{% include 'inc/filter_list.html' %}
 {% endblock %} {% block javascript %}
 {% endblock %}
```

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin.egg-info/PKG-INFO` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-topology-plugin
-Version: 0.14.2
+Version: 0.14.3
 Summary: Netbox Topology Plugin, fork of netbox-topology-plugin.  Powered by NextUI
 Author-email: Daniel Sheppard <dans@dansheps.com>, Igor Korotchenkov <iDebugAll@gmail.com>
 Maintainer-email: Daniel Sheppard <dans@dansheps.com>
 License: MIT License
         
         Copyright (c) 2024 Daniel Sheppard
         Copyright (c) 2020 Igor Korotchenkov
```

### Comparing `netbox-topology-plugin-0.14.2/netbox_topology_plugin.egg-info/SOURCES.txt` & `netbox_topology_plugin-0.14.3/netbox_topology_plugin.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,26 +4,32 @@
 pyproject.toml
 netbox_topology_plugin/__init__.py
 netbox_topology_plugin/admin.py
 netbox_topology_plugin/filters.py
 netbox_topology_plugin/forms.py
 netbox_topology_plugin/models.py
 netbox_topology_plugin/navigation.py
+netbox_topology_plugin/settings.py
 netbox_topology_plugin/template_content.py
 netbox_topology_plugin/urls.py
 netbox_topology_plugin/views.py
 netbox_topology_plugin.egg-info/PKG-INFO
 netbox_topology_plugin.egg-info/SOURCES.txt
 netbox_topology_plugin.egg-info/dependency_links.txt
 netbox_topology_plugin.egg-info/top_level.txt
 netbox_topology_plugin/api/__init__.py
 netbox_topology_plugin/api/serializers.py
 netbox_topology_plugin/api/urls.py
 netbox_topology_plugin/api/views.py
+netbox_topology_plugin/constants/__init__.py
+netbox_topology_plugin/constants/icons.py
+netbox_topology_plugin/constants/interfaces.py
 netbox_topology_plugin/migrations/0001_initial.py
+netbox_topology_plugin/migrations/0002_alter_savedtopology_id.py
+netbox_topology_plugin/migrations/0003_alter_savedtopology_created_by.py
 netbox_topology_plugin/migrations/__init__.py
 netbox_topology_plugin/static/netbox_topology_plugin/bootstrap.bundle.min.js
 netbox_topology_plugin/static/netbox_topology_plugin/bootstrap.min.css
 netbox_topology_plugin/static/netbox_topology_plugin/button_utils.js
 netbox_topology_plugin/static/netbox_topology_plugin/next_app.js
 netbox_topology_plugin/static/netbox_topology_plugin/img/dead_node.png
 netbox_topology_plugin/static/netbox_topology_plugin/jquery/jquery-3.5.1.min.js
@@ -170,12 +176,14 @@
 netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/ciscosansregular-webfont.woff
 netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.eot
 netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.svg
 netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.ttf
 netbox_topology_plugin/static/netbox_topology_plugin/next_sources/fonts/next-font.woff
 netbox_topology_plugin/static/netbox_topology_plugin/next_sources/js/next.js
 netbox_topology_plugin/templates/netbox_topology_plugin/site_topo_button.html
-netbox_topology_plugin/templates/netbox_topology_plugin/site_topo_button_3.x.html
 netbox_topology_plugin/templates/netbox_topology_plugin/site_topology.html
-netbox_topology_plugin/templates/netbox_topology_plugin/site_topology_3.x.html
 netbox_topology_plugin/templates/netbox_topology_plugin/topology.html
-netbox_topology_plugin/templates/netbox_topology_plugin/topology_3.x.html
+netbox_topology_plugin/utils/__init__.py
+netbox_topology_plugin/utils/filtering.py
+netbox_topology_plugin/utils/icons.py
+netbox_topology_plugin/utils/interfaces.py
+netbox_topology_plugin/utils/topology.py
```

### Comparing `netbox-topology-plugin-0.14.2/pyproject.toml` & `netbox_topology_plugin-0.14.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 maintainers = [
     {name = "Daniel Sheppard", email = "dans@dansheps.com"},
 ]
 description = "Netbox Topology Plugin, fork of netbox-topology-plugin.  Powered by NextUI"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["netbox-plugin", "netbox-topology"]
-version = "0.14.2"
+version = "0.14.3"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = []
 
 [project.urls]
```

