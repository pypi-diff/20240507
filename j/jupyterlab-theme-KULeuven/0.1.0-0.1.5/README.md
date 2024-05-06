# Comparing `tmp/jupyterlab-theme-KULeuven-0.1.0.tar.gz` & `tmp/jupyterlab_theme_kuleuven-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab-theme-KULeuven-0.1.0.tar", last modified: Fri Jan  6 00:14:25 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab-theme-KULeuven-0.1.0.tar` & `jupyterlab_theme_kuleuven-0.1.5.tar`

### file list

```diff
@@ -1,39 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:14:25.472067 jupyterlab-theme-KULeuven-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-01-06 00:14:25.472067 jupyterlab-theme-KULeuven-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:14:25.468067 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:14:25.468067 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-01-06 00:14:25.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:14:25.468067 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-06 00:14:25.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/labextension/static/568.76c1fbcde852f79afa9b.js
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-01-06 00:14:25.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/labextension/static/remoteEntry.72b7047cc46956997303.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-06 00:14:24.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-06 00:14:25.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:14:25.468067 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/labextension/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:14:25.468067 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/labextension/themes/jupyterlab-theme-KULeuven/
--rw-r--r--   0 runner    (1001) docker     (123)    20023 2023-01-06 00:14:25.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/labextension/themes/jupyterlab-theme-KULeuven/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 00:14:25.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/labextension/themes/jupyterlab-theme-KULeuven/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:14:25.468067 jupyterlab-theme-KULeuven-0.1.0/jupyterlab_theme_KULeuven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-01-06 00:14:25.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab_theme_KULeuven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-01-06 00:14:25.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab_theme_KULeuven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 00:14:25.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab_theme_KULeuven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 00:13:58.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab_theme_KULeuven.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-06 00:14:25.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab_theme_KULeuven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-06 00:14:25.000000 jupyterlab-theme-KULeuven-0.1.0/jupyterlab_theme_KULeuven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 00:14:25.472067 jupyterlab-theme-KULeuven-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:14:25.468067 jupyterlab-theme-KULeuven-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:14:25.472067 jupyterlab-theme-KULeuven-0.1.0/style/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/style/KULeuven.svg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/style/KULeuven2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/style/variables.css
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-01-06 00:12:29.000000 jupyterlab-theme-KULeuven-0.1.0/tsconfig.json
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/.eslintignore
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/.eslintrc.js
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/.prettierrc
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/.yarnrc.yml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/MANIFEST.in
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/install.json
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/tsconfig.json
+-rw-r--r--   0        0        0   374897 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/yarn.lock
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/_version.py
+-rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/labextension/package.json
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/labextension/schemas/jupyterlab-theme-KULeuven/package.json.orig
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/labextension/schemas/jupyterlab-theme-KULeuven/slides.json
+-rw-r--r--   0        0        0    26379 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/labextension/static/502.b9cb77141db3d362c4d0.js
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/labextension/static/509.c346d8921a4fcdf636d7.js
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/labextension/static/remoteEntry.e309524faa90a70a07f7.js
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    22083 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/labextension/themes/jupyterlab-theme-KULeuven/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/labextension/themes/jupyterlab-theme-KULeuven/index.js
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/schema/slides.json
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/src/index.ts
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/style/KULeuven.svg
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/style/KULeuven2.svg
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/style/base.css
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/style/index.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/style/index.js
+-rw-r--r--   0        0        0    13740 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/style/variables.css
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/.github/README.md
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 jupyterlab_theme_kuleuven-0.1.5/PKG-INFO
```

### Comparing `jupyterlab-theme-KULeuven-0.1.0/LICENSE` & `jupyterlab_theme_kuleuven-0.1.5/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Jan Genoe
+Copyright (c) 2023, Jan Genoe
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `jupyterlab-theme-KULeuven-0.1.0/PKG-INFO` & `jupyterlab_theme_kuleuven-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyterlab-theme-KULeuven
-Version: 0.1.0
-Summary: A Jupyterlab theme for the KULeuven
-Home-page: https://github.com/KULeuven-Diepenbeek/jupyterlab-theme-KULeuven
-Author: Jan Genoe
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
+Version: 0.1.5
+Dynamic: Keywords
+Summary: A theme for KULeuven jupyterlab-deck slides
+Project-URL: Homepage, https://github.com/KULeuven-Diepenbeek/jupyterlab-theme-KULeuven
+Project-URL: Bug Tracker, https://github.com/KULeuven-Diepenbeek/jupyterlab-theme-KULeuven/issues
+Project-URL: Repository, https://github.com/KULeuven-Diepenbeek/jupyterlab-theme-KULeuven.git
+Author-email: Jan Genoe <jan.genoe@kuleuven.be>
+License: BSD-3-Clause License
+License-File: LICENSE
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Themes
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # jupyterlab-theme-KULeuven
 
-[![Github Actions Status](https://github.com/KULeuven-Diepenbeek/jupyterlab-theme-KULeuven/workflows/Build/badge.svg)](https://github.com/KULeuven-Diepenbeek/jupyterlab-theme-KULeuven/actions/workflows/build.yml)
-A theme for KULeuven jupyterlab-deck slides
+
+A jupyterlab theme for KULeuven.
+It provides also styles jupyterlab-deck slides, but it should also work without jupyterlab-deck.
 
 ## Requirements
 
-- JupyterLab >= 3.0
-- jupyterlab-deck
+- JupyterLab >= 4.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
 pip install jupyterlab-theme-KULeuven
```

### Comparing `jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/labextension/static/remoteEntry.72b7047cc46956997303.js` & `jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/labextension/static/remoteEntry.e309524faa90a70a07f7.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,16 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, s, p, d, h, c, v = {
-            807: (e, r, t) => {
+    var e, r, t, n, o, a, i, u, l, f, s, p, d, c, h, v, m, g = {
+            7: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(568).then((() => () => t(568))),
-                        "./extension": () => t.e(568).then((() => () => t(568)))
+                        "./index": () => t.e(509).then((() => () => t(509))),
+                        "./extension": () => t.e(509).then((() => () => t(509))),
+                        "./style": () => t.e(502).then((() => () => t(502)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -20,105 +21,113 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
-        m = {};
+        b = {};
 
-    function g(e) {
-        var r = m[e];
+    function y(e) {
+        var r = b[e];
         if (void 0 !== r) return r.exports;
-        var t = m[e] = {
+        var t = b[e] = {
+            id: e,
             exports: {}
         };
-        return v[e](t, t.exports, g), t.exports
+        return g[e](t, t.exports, y), t.exports
     }
-    g.m = v, g.c = m, g.n = e => {
+    y.m = g, y.c = b, y.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return g.d(r, {
+        return y.d(r, {
             a: r
         }), r
-    }, g.d = (e, r) => {
-        for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
+    }, y.d = (e, r) => {
+        for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + ".76c1fbcde852f79afa9b.js?v=76c1fbcde852f79afa9b", g.g = function() {
+    }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
+        502: "b9cb77141db3d362c4d0",
+        509: "c346d8921a4fcdf636d7"
+    } [e] + ".js?v=" + {
+        502: "b9cb77141db3d362c4d0",
+        509: "c346d8921a4fcdf636d7"
+    } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab-theme-KULeuven:", g.l = (t, n, o, a) => {
+    }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab-theme-KULeuven:", y.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
                     var s = l[f];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
                         i = s;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, y.nc && i.setAttribute("nonce", y.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var p = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(d);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 d = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, g.r = e => {
+    }, y.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        g.S = {};
+        y.S = {};
         var e = {},
             r = {};
-        g.I = (t, n) => {
+        y.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                g.o(g.S, t) || (g.S[t] = {});
-                var a = g.S[t],
+                y.o(y.S, t) || (y.S[t] = {});
+                var a = y.S[t],
                     i = "jupyterlab-theme-KULeuven",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => g.e(568).then((() => () => g(568))),
+                        get: () => y.e(509).then((() => () => y(509))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-theme-KULeuven", "0.1.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-theme-KULeuven", "0.1.5"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        g.g.importScripts && (e = g.g.location + "");
-        var r = g.g.document;
+        y.g.importScripts && (e = y.g.location + "");
+        var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && (!e || !/^http(s?):/.test(e));) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), g.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), y.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -177,87 +186,93 @@
                 } else {
                     if (u <= n || s < p != o) return !1;
                     l = !1
                 } else "s" != p && "n" != p && (l = !1, u--)
             }
         }
         var d = [],
-            h = d.pop.bind(d);
+            c = d.pop.bind(d);
         for (i = 1; i < e.length; i++) {
-            var c = e[i];
-            d.push(1 == c ? h() | h() : 2 == c ? h() & h() : c ? a(c, r) : !h())
+            var h = e[i];
+            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
-        return !!h()
+        return !!c()
     }, i = (e, r) => {
-        var t = g.S[e];
-        if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = y.S[e];
+        if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
-    }, s = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
-        var a = g.I(r);
-        return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), d = {}, h = {
-        740: () => p("default", "@jupyterlab/apputils", [1, 3, 5, 2])
-    }, c = {
-        568: [740]
-    }, g.f.consumes = (e, r) => {
-        g.o(c, e) && c[e].forEach((e => {
-            if (g.o(d, e)) return r.push(d[e]);
-            var t = r => {
-                    d[e] = 0, g.m[e] = t => {
-                        delete g.c[e], t.exports = r()
+        return a(n, o) || s(l(e, t, o, n)), p(e[t][o])
+    }, s = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, p = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
+        var a = y.I(r);
+        return a && a.then ? a.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
+        923: () => d("default", "@jupyterlab/apputils", [1, 4, 3, 0])
+    }, v = {
+        509: [923]
+    }, m = {}, y.f.consumes = (e, r) => {
+        y.o(v, e) && v[e].forEach((e => {
+            if (y.o(c, e)) return r.push(c[e]);
+            if (!m[e]) {
+                var t = r => {
+                    c[e] = 0, y.m[e] = t => {
+                        delete y.c[e], t.exports = r()
                     }
-                },
-                n = r => {
-                    delete d[e], g.m[e] = t => {
-                        throw delete g.c[e], r
+                };
+                m[e] = !0;
+                var n = r => {
+                    delete c[e], y.m[e] = t => {
+                        throw delete y.c[e], r
                     }
                 };
-            try {
-                var o = h[e]();
-                o.then ? r.push(d[e] = o.then(t).catch(n)) : t(o)
-            } catch (e) {
-                n(e)
+                try {
+                    var o = h[e]();
+                    o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
+                } catch (e) {
+                    n(e)
+                }
             }
         }))
     }, (() => {
+        y.b = document.baseURI || self.location.href;
         var e = {
-            533: 0
+            505: 0
         };
-        g.f.j = (r, t) => {
-            var n = g.o(e, r) ? e[r] : void 0;
+        y.f.j = (r, t) => {
+            var n = y.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = g.p + g.u(r),
+                    var a = y.p + y.u(r),
                         i = new Error;
-                    g.l(a, (t => {
-                        if (g.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    y.l(a, (t => {
+                        if (y.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
                     l = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) g.o(i, n) && (g.m[n] = i[n]);
-                    u && u(g)
+                    for (n in i) y.o(i, n) && (y.m[n] = i[n]);
+                    u && u(y)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], g.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], y.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkjupyterlab_theme_KULeuven = self.webpackChunkjupyterlab_theme_KULeuven || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })();
-    var b = g(807);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyterlab-theme-KULeuven"] = b
+    })(), y.nc = void 0;
+    var w = y(7);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyterlab-theme-KULeuven"] = w
 })();
```

### Comparing `jupyterlab-theme-KULeuven-0.1.0/jupyterlab-theme-KULeuven/labextension/themes/jupyterlab-theme-KULeuven/index.css` & `jupyterlab_theme_kuleuven-0.1.5/jupyterlab-theme-KULeuven/labextension/themes/jupyterlab-theme-KULeuven/index.css`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+/*
+    See the JupyterLab Developer Guide for useful CSS Patterns:
+
+    https://jupyterlab.readthedocs.io/en/stable/developer/css.html
+*/
+
+.metadataform-Jupyter_KULeuven_slides-custom-field-content {
+  border: solid 1px;
+}
+
+#metadataform-Jupyter_KULeuven_slides-custom-field-elem {
+  display: flex;
+}
+
+.metadataform-Jupyter_KULeuven_slides-custom-field-add .jp-icon3 {
+  fill: var(--jp-success-color1);
+}
+
+.metadataform-Jupyter_KULeuven_slides-custom-field-item .jp-icon3 {
+  fill: var(--jp-error-color1);
+}
+
+#metadataform-Jupyter_KULeuven_slides-custom-field-add-input {
+  width: 100%;
+  box-sizing: border-box;
+}
+
+.metadata-form-Jupyter_KULeuven_slides-custom-checkbox.checked .jp-icon3 {
+  fill: var(--jp-success-color1);
+}
+
+.metadata-form-Jupyter_KULeuven_slides-custom-checkbox.unchecked .jp-icon3 {
+  fill: var(--jp-error-color1);
+}
+
 /* ----------------------------------------------------------------------------
 | Copyright (c) Jupyter Development Team.
 | Distributed under the terms of the Modified BSD License.
 |--------------------------------------------------------------------------- */
 
 /*
 The following CSS variables define the main, public API for styling JupyterLab.
@@ -380,15 +415,15 @@
   #jp-main-content-panel {
     width: 100vw !important;
     height: 100vh !important;
     border: 0 !important;
     padding: 0 !important;
     margin: 0 !important;
     top: 0 !important;
-    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='158.7' height='56.7' viewBox='0 0 158.7 56.7'%3E%3Cstyle type='text/css'%3E.st0%7Bfill:%2300407A;%7D .st1%7Bfill:%2354BCEB;%7D .st2%7Bfill:none;%7D .st3%7Bfill:%23FFFFFF;%7D%3C/style%3E%3Cpath class='st0' d='M5.7 5.7h153.1v51H5.7z'/%3E%3Cpath class='st1' d='M0 0v56.7h5.7v-51h153V0z'/%3E%3Cpath class='st2' d='M17 22.7h130.4v17H17z'/%3E%3Cpath class='st3' d='M17 22.7h5.1v5.9l4.5-5.9h6.2l-6 6.6 6.9 10.4h-6.3l-4.1-6.6-1.4 1.6v5H17v-17zM49.1 33.1c0 4.7-2.5 7-7.5 7s-7.5-2.3-7.5-7V22.7h5.1V32c0 1.7 0 3.9 2.5 3.9 2.4 0 2.4-2.2 2.4-3.9v-9.3h5.1v10.4zM56.5 22.7h5.1v12.6h7.2v4.4H56.5v-17zM70.3 22.7h13.5V27h-8.5v2.1H83v4h-7.7v2.1H84v4.4H70.3V22.7zM100.4 33.1c0 4.7-2.5 7-7.5 7s-7.5-2.3-7.5-7V22.7h5.1V32c0 1.7 0 3.9 2.5 3.9 2.4 0 2.4-2.2 2.4-3.9v-9.3h5.1v10.4zM111.7 39.7H106l-4.9-17h5.1l2.7 10.3 2.7-10.3h5.2l-5.1 17zM117.5 22.7H131V27h-8.5v2.1h7.7v4h-7.7v2.1h8.7v4.4h-13.7V22.7zM132.6 22.7h5.2l4.8 9.1v-9.1h4.8v17h-4.9l-5-9.3v9.3h-4.8v-17z'/%3E%3C/svg%3E"),
+    background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='158.7' height='56.7' viewBox='0 0 158.7 56.7'%3e%3cstyle type='text/css'%3e.st0%7bfill:%2300407A%3b%7d .st1%7bfill:%2354BCEB%3b%7d .st2%7bfill:none%3b%7d .st3%7bfill:white%3b%7d%3c/style%3e%3cpath class='st0' d='M5.7 5.7h153.1v51H5.7z'/%3e%3cpath class='st1' d='M0 0v56.7h5.7v-51h153V0z'/%3e%3cpath class='st2' d='M17 22.7h130.4v17H17z'/%3e%3cpath class='st3' d='M17 22.7h5.1v5.9l4.5-5.9h6.2l-6 6.6 6.9 10.4h-6.3l-4.1-6.6-1.4 1.6v5H17v-17zM49.1 33.1c0 4.7-2.5 7-7.5 7s-7.5-2.3-7.5-7V22.7h5.1V32c0 1.7 0 3.9 2.5 3.9 2.4 0 2.4-2.2 2.4-3.9v-9.3h5.1v10.4zM56.5 22.7h5.1v12.6h7.2v4.4H56.5v-17zM70.3 22.7h13.5V27h-8.5v2.1H83v4h-7.7v2.1H84v4.4H70.3V22.7zM100.4 33.1c0 4.7-2.5 7-7.5 7s-7.5-2.3-7.5-7V22.7h5.1V32c0 1.7 0 3.9 2.5 3.9 2.4 0 2.4-2.2 2.4-3.9v-9.3h5.1v10.4zM111.7 39.7H106l-4.9-17h5.1l2.7 10.3 2.7-10.3h5.2l-5.1 17zM117.5 22.7H131V27h-8.5v2.1h7.7v4h-7.7v2.1h8.7v4.4h-13.7V22.7zM132.6 22.7h5.2l4.8 9.1v-9.1h4.8v17h-4.9l-5-9.3v9.3h-4.8v-17z'/%3e%3c/svg%3e"),
       linear-gradient(#fff 91vh, var(--kuleuven-blue0) 91vh);
     background-position: right 11vw bottom 1.5vh, bottom;
     background-size: 15vh, 100%;
     background-repeat: no-repeat, no-repeat;
   }
   
 body[data-jp-deck-mode='presenting']
@@ -557,12 +592,19 @@
 
 /* Replace the default JupyterLab Logo */
 #jp-MainLogo > svg {
   visibility: hidden;
 }
 
 #jp-MainLogo {
-  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='27' height='28' viewBox='0 0 54.7 56.7'%3E%3Cstyle type='text/css'%3E.st0%7Bfill:%2300407A;%7D .st1%7Bfill:%2354BCEB;%7D .st2%7Bfill:none;%7D .st3%7Bfill:%23FFFFFF;%7D%3C/style%3E%3Cpath class='st0' d='M5.7 5.7h153.1v51H5.7z'/%3E%3Cpath class='st1' d='M0 0v56.7h5.7v-51h153V0z'/%3E%3Cpath class='st2' d='M17 22.7h130.4v17H17z'/%3E%3Cpath class='st3' d='M17 22.7h5.1v5.9l4.5-5.9h6.2l-6 6.6 6.9 10.4h-6.3l-4.1-6.6-1.4 1.6v5H17v-17zM49.1 33.1c0 4.7-2.5 7-7.5 7s-7.5-2.3-7.5-7V22.7h5.1V32c0 1.7 0 3.9 2.5 3.9 2.4 0 2.4-2.2 2.4-3.9v-9.3h5.1v10.4zM56.5 22.7h5.1v12.6h7.2v4.4H56.5v-17zM70.3 22.7h13.5V27h-8.5v2.1H83v4h-7.7v2.1H84v4.4H70.3V22.7zM100.4 33.1c0 4.7-2.5 7-7.5 7s-7.5-2.3-7.5-7V22.7h5.1V32c0 1.7 0 3.9 2.5 3.9 2.4 0 2.4-2.2 2.4-3.9v-9.3h5.1v10.4zM111.7 39.7H106l-4.9-17h5.1l2.7 10.3 2.7-10.3h5.2l-5.1 17zM117.5 22.7H131V27h-8.5v2.1h7.7v4h-7.7v2.1h8.7v4.4h-13.7V22.7zM132.6 22.7h5.2l4.8 9.1v-9.1h4.8v17h-4.9l-5-9.3v9.3h-4.8v-17z'/%3E%3C/svg%3E");
+  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='27' height='28' viewBox='0 0 54.7 56.7'%3e%3cstyle type='text/css'%3e.st0%7bfill:%2300407A%3b%7d .st1%7bfill:%2354BCEB%3b%7d .st2%7bfill:none%3b%7d .st3%7bfill:white%3b%7d%3c/style%3e%3cpath class='st0' d='M5.7 5.7h153.1v51H5.7z'/%3e%3cpath class='st1' d='M0 0v56.7h5.7v-51h153V0z'/%3e%3cpath class='st2' d='M17 22.7h130.4v17H17z'/%3e%3cpath class='st3' d='M17 22.7h5.1v5.9l4.5-5.9h6.2l-6 6.6 6.9 10.4h-6.3l-4.1-6.6-1.4 1.6v5H17v-17zM49.1 33.1c0 4.7-2.5 7-7.5 7s-7.5-2.3-7.5-7V22.7h5.1V32c0 1.7 0 3.9 2.5 3.9 2.4 0 2.4-2.2 2.4-3.9v-9.3h5.1v10.4zM56.5 22.7h5.1v12.6h7.2v4.4H56.5v-17zM70.3 22.7h13.5V27h-8.5v2.1H83v4h-7.7v2.1H84v4.4H70.3V22.7zM100.4 33.1c0 4.7-2.5 7-7.5 7s-7.5-2.3-7.5-7V22.7h5.1V32c0 1.7 0 3.9 2.5 3.9 2.4 0 2.4-2.2 2.4-3.9v-9.3h5.1v10.4zM111.7 39.7H106l-4.9-17h5.1l2.7 10.3 2.7-10.3h5.2l-5.1 17zM117.5 22.7H131V27h-8.5v2.1h7.7v4h-7.7v2.1h8.7v4.4h-13.7V22.7zM132.6 22.7h5.2l4.8 9.1v-9.1h4.8v17h-4.9l-5-9.3v9.3h-4.8v-17z'/%3e%3c/svg%3e");
   background-repeat: no-repeat;
   background-position: center;
 }
 
+.jp-ApplicationShell-header .jp-Toolbar-logo {
+  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='158.7' height='56.7' viewBox='0 0 158.7 56.7'%3e%3cstyle type='text/css'%3e.st0%7bfill:%2300407A%3b%7d .st1%7bfill:%2354BCEB%3b%7d .st2%7bfill:none%3b%7d .st3%7bfill:white%3b%7d%3c/style%3e%3cpath class='st0' d='M5.7 5.7h153.1v51H5.7z'/%3e%3cpath class='st1' d='M0 0v56.7h5.7v-51h153V0z'/%3e%3cpath class='st2' d='M17 22.7h130.4v17H17z'/%3e%3cpath class='st3' d='M17 22.7h5.1v5.9l4.5-5.9h6.2l-6 6.6 6.9 10.4h-6.3l-4.1-6.6-1.4 1.6v5H17v-17zM49.1 33.1c0 4.7-2.5 7-7.5 7s-7.5-2.3-7.5-7V22.7h5.1V32c0 1.7 0 3.9 2.5 3.9 2.4 0 2.4-2.2 2.4-3.9v-9.3h5.1v10.4zM56.5 22.7h5.1v12.6h7.2v4.4H56.5v-17zM70.3 22.7h13.5V27h-8.5v2.1H83v4h-7.7v2.1H84v4.4H70.3V22.7zM100.4 33.1c0 4.7-2.5 7-7.5 7s-7.5-2.3-7.5-7V22.7h5.1V32c0 1.7 0 3.9 2.5 3.9 2.4 0 2.4-2.2 2.4-3.9v-9.3h5.1v10.4zM111.7 39.7H106l-4.9-17h5.1l2.7 10.3 2.7-10.3h5.2l-5.1 17zM117.5 22.7H131V27h-8.5v2.1h7.7v4h-7.7v2.1h8.7v4.4h-13.7V22.7zM132.6 22.7h5.2l4.8 9.1v-9.1h4.8v17h-4.9l-5-9.3v9.3h-4.8v-17z'/%3e%3c/svg%3e");
+  background-size: contain;
+  background-repeat: no-repeat;
+  background-position: center;
+  max-width: 100%;
+}
```

### Comparing `jupyterlab-theme-KULeuven-0.1.0/style/KULeuven.svg` & `jupyterlab_theme_kuleuven-0.1.5/style/KULeuven.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab-theme-KULeuven-0.1.0/style/KULeuven2.svg` & `jupyterlab_theme_kuleuven-0.1.5/style/KULeuven2.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab-theme-KULeuven-0.1.0/style/index.css` & `jupyterlab_theme_kuleuven-0.1.5/style/index.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+@import url('base.css');
 @import './variables.css';
 
 /* Set the default typography for monospace elements */
 tt,
 code,
 kbd,
 samp,
@@ -196,7 +197,15 @@
 }
 
 #jp-MainLogo {
   background-image: url('./KULeuven2.svg');
   background-repeat: no-repeat;
   background-position: center;
 }
+
+.jp-ApplicationShell-header .jp-Toolbar-logo {
+  background-image: url('./KULeuven.svg');
+  background-size: contain;
+  background-repeat: no-repeat;
+  background-position: center;
+  max-width: 100%;
+}
```

### Comparing `jupyterlab-theme-KULeuven-0.1.0/style/variables.css` & `jupyterlab_theme_kuleuven-0.1.5/style/variables.css`

 * *Files identical despite different names*

### Comparing `jupyterlab-theme-KULeuven-0.1.0/tsconfig.json` & `jupyterlab_theme_kuleuven-0.1.5/tsconfig.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9802631578947368%*

 * *Differences: {"'compilerOptions'": "{'target': 'ES2018', delete: ['types']}"}*

```diff
@@ -13,14 +13,13 @@
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2017",
-        "types": []
+        "target": "ES2018"
     },
     "include": [
         "src/*"
     ]
 }
```

