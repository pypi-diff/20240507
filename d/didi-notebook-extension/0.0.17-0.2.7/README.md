# Comparing `tmp/didi_notebook_extension-0.0.17.tar.gz` & `tmp/didi_notebook_extension-0.2.7.tar.gz`

## Comparing `didi_notebook_extension-0.0.17.tar` & `didi_notebook_extension-0.2.7.tar`

### file list

```diff
@@ -1,43 +1,46 @@
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/.copier-answers.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/CHANGELOG.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/RELEASE.md
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/Untitled.ipynb
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/Untitled1.ipynb
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/Untitled2.ipynb
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/babel.config.js
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/jest.config.js
--rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/tsconfig.test.json
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/untitled.py
--rw-r--r--   0        0        0   388697 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/yarn.lock
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/.virtual_documents/Untitled2.ipynb
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/didi_notebook_extension/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/didi_notebook_extension/_version.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/didi_notebook_extension/labextension/package.json
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/didi_notebook_extension/labextension/static/728.9916fbef502e316a159a.js
--rw-r--r--   0        0        0    10378 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/didi_notebook_extension/labextension/static/958.bd36d1031c08063aa2e9.js
--rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/didi_notebook_extension/labextension/static/remoteEntry.8939b006cb56785ffe74.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/didi_notebook_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/didi_notebook_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/src/api.ts
--rw-r--r--   0        0        0     6371 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/src/index.ts
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/src/__tests__/didi_notebook_extension.spec.ts
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/style/index.js
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/ui-tests/yarn.lock
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/ui-tests/tests/didi_extension.spec.ts
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/LICENSE
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/README.md
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/pyproject.toml
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 didi_notebook_extension-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/.copier-answers.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/CHANGELOG.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/RELEASE.md
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/Untitled.ipynb
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/Untitled1.ipynb
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/Untitled2.ipynb
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/babel.config.js
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/jest.config.js
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/tsconfig.test.json
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/untitled.py
+-rw-r--r--   0        0        0   376404 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/yarn.lock
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/.virtual_documents/Untitled.ipynb
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/.virtual_documents/Untitled1.ipynb
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/.virtual_documents/Untitled2.ipynb
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/.virtual_documents/Untitled6.ipynb
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/didi_notebook_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/didi_notebook_extension/_version.py
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/didi_notebook_extension/labextension/package.json
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/didi_notebook_extension/labextension/static/728.adf73d00115832453a58.js
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/didi_notebook_extension/labextension/static/958.eb0e437e53b6a86814b4.js
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/didi_notebook_extension/labextension/static/remoteEntry.669ff8394f95a035c486.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/didi_notebook_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/didi_notebook_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/src/api.ts
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/src/index.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/src/__tests__/didi_notebook_extension.spec.ts
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/style/index.js
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/ui-tests/tests/didi_extension.spec.ts
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/README.md
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 didi_notebook_extension-0.2.7/PKG-INFO
```

### Comparing `didi_notebook_extension-0.0.17/.copier-answers.yml` & `didi_notebook_extension-0.2.7/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `didi_notebook_extension-0.0.17/RELEASE.md` & `didi_notebook_extension-0.2.7/RELEASE.md`

 * *Files identical despite different names*

### Comparing `didi_notebook_extension-0.0.17/Untitled.ipynb` & `didi_notebook_extension-0.2.7/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `didi_notebook_extension-0.0.17/jest.config.js` & `didi_notebook_extension-0.2.7/jest.config.js`

 * *Files identical despite different names*

### Comparing `didi_notebook_extension-0.0.17/package.json` & `didi_notebook_extension-0.2.7/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'dependencies'": "{delete: ['@jupyterlab/docmanager']}", "'version'": "'0.2.7'"}*

```diff
@@ -4,15 +4,14 @@
         "name": "dongmeiqi"
     },
     "bugs": {
         "url": "https://github.com/yobi-maggie/didi-notebook-extension/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^4.0.0",
-        "@jupyterlab/docmanager": "^4.1.8",
         "@jupyterlab/mainmenu": "^4.1.6"
     },
     "description": "A JupyterLab extension.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
         "@types/jest": "^29.2.0",
@@ -188,9 +187,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.0.17"
+    "version": "0.2.7"
 }
```

### Comparing `didi_notebook_extension-0.0.17/tsconfig.json` & `didi_notebook_extension-0.2.7/tsconfig.json`

 * *Files identical despite different names*

### Comparing `didi_notebook_extension-0.0.17/yarn.lock` & `didi_notebook_extension-0.2.7/yarn.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1615,15 +1615,15 @@
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
   checksum: 19dc88d09fc750563347001e83c6194bbb2a25c874bd919d2d81809e1f98d6330222ddbd284aa9758a09eeb41fd153ec7c2cf810b2ee51452c25963d7f5833d5
   languageName: node
   linkType: hard
 
-"@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.2.0, @codemirror/state@npm:^6.4.0, @codemirror/state@npm:^6.4.1":
+"@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.2.0, @codemirror/state@npm:^6.4.0":
   version: 6.4.1
   resolution: "@codemirror/state@npm:6.4.1"
   checksum: b81b55574091349eed4d32fc0eadb0c9688f1f7c98b681318f59138ee0f527cb4c4a97831b70547c0640f02f3127647838ae6730782de4a3dd2cc58836125d01
   languageName: node
   linkType: hard
 
 "@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.17.0, @codemirror/view@npm:^6.23.0, @codemirror/view@npm:^6.9.6":
@@ -2065,15 +2065,15 @@
   dependencies:
     "@jridgewell/resolve-uri": ^3.1.0
     "@jridgewell/sourcemap-codec": ^1.4.14
   checksum: 9d3c40d225e139987b50c48988f8717a54a8c994d8a948ee42e1412e08988761d0754d7d10b803061cc3aebf35f92a5dbbab493bd0e1a9ef9e89a2130e83ba34
   languageName: node
   linkType: hard
 
-"@jupyter/react-components@npm:^0.15.2, @jupyter/react-components@npm:^0.15.3":
+"@jupyter/react-components@npm:^0.15.2":
   version: 0.15.3
   resolution: "@jupyter/react-components@npm:0.15.3"
   dependencies:
     "@jupyter/web-components": ^0.15.3
     "@microsoft/fast-react-wrapper": ^0.3.22
     react: ">=17.0.0 <19.0.0"
   checksum: 1a6b256314259c6465c4b6d958575710536b82234a7bf0fba3e889a07e1f19ff8ab321450be354359876f92c45dbcc9d21a840237ff4a619806d9de696f55496
@@ -2102,28 +2102,14 @@
     "@lumino/signaling": ^1.10.0 || ^2.0.0
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   checksum: a239b1dd57cfc9ba36c06ac5032a1b6388849ae01a1d0db0d45094f71fdadf4d473b4bf8becbef0cfcdc85cae505361fbec0822b02da5aa48e06b66f742dd7a0
   languageName: node
   linkType: hard
 
-"@jupyter/ydoc@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@jupyter/ydoc@npm:2.0.1"
-  dependencies:
-    "@jupyterlab/nbformat": ^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0
-    "@lumino/coreutils": ^1.11.0 || ^2.0.0
-    "@lumino/disposable": ^1.10.0 || ^2.0.0
-    "@lumino/signaling": ^1.10.0 || ^2.0.0
-    y-protocols: ^1.0.5
-    yjs: ^13.5.40
-  checksum: f5f29e1ff3327ebc1cf326f53634e03c4c7bf7733d235087fe26975c16eebd404f23c2f3ba88b6e04b1927846be7162b09b8b8719a4b29e51d0299c745018cbb
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/application@npm:^4.0.0, @jupyterlab/application@npm:^4.1.6":
   version: 4.1.6
   resolution: "@jupyterlab/application@npm:4.1.6"
   dependencies:
     "@fortawesome/fontawesome-free": ^5.12.0
     "@jupyterlab/apputils": ^4.2.6
     "@jupyterlab/coreutils": ^6.1.6
@@ -2173,43 +2159,14 @@
     "@types/react": ^18.0.26
     react: ^18.2.0
     sanitize-html: ~2.7.3
   checksum: 2ca507223fb1ca3a527ce6c544c6fc1433a0eef9a41db54031f1b159a3ef29f4908e7408c22ce0cbf6e8a2e46999ab3f9175e06df54412dd6f583a5bdf11fb6a
   languageName: node
   linkType: hard
 
-"@jupyterlab/apputils@npm:^4.3.0":
-  version: 4.3.0
-  resolution: "@jupyterlab/apputils@npm:4.3.0"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.2.0
-    "@jupyterlab/observables": ^5.2.0
-    "@jupyterlab/rendermime-interfaces": ^3.10.0
-    "@jupyterlab/services": ^7.2.0
-    "@jupyterlab/settingregistry": ^4.2.0
-    "@jupyterlab/statedb": ^4.2.0
-    "@jupyterlab/statusbar": ^4.2.0
-    "@jupyterlab/translation": ^4.2.0
-    "@jupyterlab/ui-components": ^4.2.0
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.3.0
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/domutils": ^2.0.1
-    "@lumino/messaging": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.2
-    "@types/react": ^18.0.26
-    react: ^18.2.0
-    sanitize-html: ~2.12.1
-  checksum: 96f4f9055c464fb6f0e2545d21623b9500936da44cd7bafa9c1154164f6fc1846a518bc637ef46d6a082d208d12acf737d8aa679ce5546427ac04f068cf10cd5
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/attachments@npm:^4.1.6":
   version: 4.1.6
   resolution: "@jupyterlab/attachments@npm:4.1.6"
   dependencies:
     "@jupyterlab/nbformat": ^4.1.6
     "@jupyterlab/observables": ^5.1.6
     "@jupyterlab/rendermime": ^4.1.6
@@ -2317,38 +2274,14 @@
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
   checksum: 0c34e3f30e20aa590ac8308b00b1dc89a51b0b214cd0d548311b5b7392ae072db42e7823963ca0faf7761eadf5c4b62a1b25e467e44c93a0ccb9ac5ad645d1c3
   languageName: node
   linkType: hard
 
-"@jupyterlab/codeeditor@npm:^4.2.0":
-  version: 4.2.0
-  resolution: "@jupyterlab/codeeditor@npm:4.2.0"
-  dependencies:
-    "@codemirror/state": ^6.4.1
-    "@jupyter/ydoc": ^2.0.1
-    "@jupyterlab/apputils": ^4.3.0
-    "@jupyterlab/coreutils": ^6.2.0
-    "@jupyterlab/nbformat": ^4.2.0
-    "@jupyterlab/observables": ^5.2.0
-    "@jupyterlab/statusbar": ^4.2.0
-    "@jupyterlab/translation": ^4.2.0
-    "@jupyterlab/ui-components": ^4.2.0
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/dragdrop": ^2.1.4
-    "@lumino/messaging": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.2
-    react: ^18.2.0
-  checksum: a6e2b1cf7e46ae86154b20bd4a3c29c7c4bb0feb7b0cf6461470db99f2d6f4df13084f861fad7de9409a040191f075dcb3f148328eff419a2494cd84326749b2
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/codemirror@npm:^4.1.6":
   version: 4.1.6
   resolution: "@jupyterlab/codemirror@npm:4.1.6"
   dependencies:
     "@codemirror/autocomplete": ^6.5.1
     "@codemirror/commands": ^6.2.3
     "@codemirror/lang-cpp": ^6.0.2
@@ -2397,28 +2330,14 @@
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
   checksum: f351f327f9c7ab14ac291e4ca85a8f4289dd315e9f2e68fc6acb52efab6c47fde158f65a83ba780c382665459995bad68c7b1f9c4ffef6b9038ac81252a3f07a
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:^6.2.0":
-  version: 6.2.0
-  resolution: "@jupyterlab/coreutils@npm:6.2.0"
-  dependencies:
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/signaling": ^2.1.2
-    minimist: ~1.2.0
-    path-browserify: ^1.0.0
-    url-parse: ~1.5.4
-  checksum: 1975f19f567b63484055b0d1d10757b2bf66274814083e50702bb6017af22341cc3f5924d0ec7da408feacd652120b476aaaf50286a5401f798f257e899aed91
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/docmanager@npm:^4.1.6":
   version: 4.1.6
   resolution: "@jupyterlab/docmanager@npm:4.1.6"
   dependencies:
     "@jupyterlab/apputils": ^4.2.6
     "@jupyterlab/coreutils": ^6.1.6
     "@jupyterlab/docregistry": ^4.1.6
@@ -2434,39 +2353,14 @@
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
   checksum: 890a8f86fc3d96d896e86ed64ef3c713152d781c941eea99d1b2d021bf5d1844f2d0a52d8cb077b1e8a1d31f13a6253c118cbe70440e10df20a490ab2595bab2
   languageName: node
   linkType: hard
 
-"@jupyterlab/docmanager@npm:^4.1.8":
-  version: 4.2.0
-  resolution: "@jupyterlab/docmanager@npm:4.2.0"
-  dependencies:
-    "@jupyterlab/apputils": ^4.3.0
-    "@jupyterlab/coreutils": ^6.2.0
-    "@jupyterlab/docregistry": ^4.2.0
-    "@jupyterlab/services": ^7.2.0
-    "@jupyterlab/statedb": ^4.2.0
-    "@jupyterlab/statusbar": ^4.2.0
-    "@jupyterlab/translation": ^4.2.0
-    "@jupyterlab/ui-components": ^4.2.0
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/messaging": ^2.0.1
-    "@lumino/polling": ^2.1.2
-    "@lumino/properties": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.2
-    react: ^18.2.0
-  checksum: 63e461bf75ce4b12ada41cf727b11f956c62312b2e017fdaf9979ba16a86cb5078e7eed4f508e122afc3718d1ee18548c8ec6a1bb50f4a95a2217a77a8e0b1c3
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/docregistry@npm:^4.1.6":
   version: 4.1.6
   resolution: "@jupyterlab/docregistry@npm:4.1.6"
   dependencies:
     "@jupyter/ydoc": ^1.1.1
     "@jupyterlab/apputils": ^4.2.6
     "@jupyterlab/codeeditor": ^4.1.6
@@ -2485,40 +2379,14 @@
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
   checksum: 0b7db803cd0013e1b65f0294b5bec2f6d4047cd7b191080ade3d67ff78d1d5a2d0e3a7016532dd316899b291bbc0b07561a958b2dd750dbcf3fc34927552c0d8
   languageName: node
   linkType: hard
 
-"@jupyterlab/docregistry@npm:^4.2.0":
-  version: 4.2.0
-  resolution: "@jupyterlab/docregistry@npm:4.2.0"
-  dependencies:
-    "@jupyter/ydoc": ^2.0.1
-    "@jupyterlab/apputils": ^4.3.0
-    "@jupyterlab/codeeditor": ^4.2.0
-    "@jupyterlab/coreutils": ^6.2.0
-    "@jupyterlab/observables": ^5.2.0
-    "@jupyterlab/rendermime": ^4.2.0
-    "@jupyterlab/rendermime-interfaces": ^3.10.0
-    "@jupyterlab/services": ^7.2.0
-    "@jupyterlab/translation": ^4.2.0
-    "@jupyterlab/ui-components": ^4.2.0
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/messaging": ^2.0.1
-    "@lumino/properties": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.2
-    react: ^18.2.0
-  checksum: ef616ca11a07a5a2d8865d909499662e8c37b19e9487081682c47808becb5d87fe09a4d1c0175ea8afd3c96a255a437b8d762e990c81d71cf9cc13cf99fe3c3b
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/documentsearch@npm:^4.1.6":
   version: 4.1.6
   resolution: "@jupyterlab/documentsearch@npm:4.1.6"
   dependencies:
     "@jupyterlab/apputils": ^4.2.6
     "@jupyterlab/translation": ^4.1.6
     "@jupyterlab/ui-components": ^4.1.6
@@ -2605,23 +2473,14 @@
   resolution: "@jupyterlab/nbformat@npm:4.1.6"
   dependencies:
     "@lumino/coreutils": ^2.1.2
   checksum: 4ef43fdaaecec06732528753c5316adaa883c77ae86d129fb5d1f0542124acc0e7bb5692aae799463722b8c47ce8934356572c040d682e0ce41548eca3ca421b
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^4.2.0":
-  version: 4.2.0
-  resolution: "@jupyterlab/nbformat@npm:4.2.0"
-  dependencies:
-    "@lumino/coreutils": ^2.1.2
-  checksum: adecadcb63de48f09aeb54eebfed8b77ab322c478fd903001e09780a01e7cf68f93716a2598631d4426d8ad9d3dc6349e8892db12575f74c8daea33f63b9c111
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/notebook@npm:^4.1.6":
   version: 4.1.6
   resolution: "@jupyterlab/notebook@npm:4.1.6"
   dependencies:
     "@jupyter/ydoc": ^1.1.1
     "@jupyterlab/apputils": ^4.2.6
     "@jupyterlab/cells": ^4.1.6
@@ -2664,27 +2523,14 @@
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
   checksum: 930e53ca38dd08232ec46585acf8d49ebbef9628a792619fbf51a1da13f3249da24a7a8b24c34a2c7ce3fa50145a4e647b65e19275ea5ce92946a2ad805faa82
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:^5.2.0":
-  version: 5.2.0
-  resolution: "@jupyterlab/observables@npm:5.2.0"
-  dependencies:
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/messaging": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-  checksum: 98460d55d8ac559c79be87fe5e105cc200556e87276daed739fd89e8393c74ba9b03f67c8ecf7a02e8d8ee1fd8a60031ced6c1b7884ab5f10c8bdb876f150c5f
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/outputarea@npm:^4.1.6":
   version: 4.1.6
   resolution: "@jupyterlab/outputarea@npm:4.1.6"
   dependencies:
     "@jupyterlab/apputils": ^4.2.6
     "@jupyterlab/nbformat": ^4.1.6
     "@jupyterlab/observables": ^5.1.6
@@ -2699,24 +2545,14 @@
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
   checksum: e45e0db75b1d4def07ff48323ac84ef1b7eedfd09cff24a9c669db8da9bc846fd8186eaa34a210e66fdab2c0b6a9be93e406e7e54456063fbe879bf2c2ffcbea
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime-interfaces@npm:^3.10.0":
-  version: 3.10.0
-  resolution: "@jupyterlab/rendermime-interfaces@npm:3.10.0"
-  dependencies:
-    "@lumino/coreutils": ^1.11.0 || ^2.1.2
-    "@lumino/widgets": ^1.37.2 || ^2.3.2
-  checksum: 08999b64a6896a4d58869ec00ca64a1b3931e01b438d471a0ad1404407f6231667f686b823a9cb482349f3d774693368320d2d4463c23fdd1de81cb4ddf34f20
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/rendermime-interfaces@npm:^3.9.6":
   version: 3.9.6
   resolution: "@jupyterlab/rendermime-interfaces@npm:3.9.6"
   dependencies:
     "@lumino/coreutils": ^1.11.0 || ^2.1.2
     "@lumino/widgets": ^1.37.2 || ^2.3.1
   checksum: 9dd08d4c71ece6e68e2972b4ce950153e2d38cc876208bb1f0e5d533daf50b062bd6aa1711c94934ea2a1f8445cf49dc6370cda80e1372b3fbede0d4534b0235
@@ -2739,34 +2575,14 @@
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     lodash.escape: ^4.0.1
   checksum: f79430851e97c4a26938bdbd3d834a0beba2860630f5f8bcccda433a2b3c52d26b180e89d016ec7cd0fce28cbc71dc825307b8b37ca63951775965cb091381ab
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime@npm:^4.2.0":
-  version: 4.2.0
-  resolution: "@jupyterlab/rendermime@npm:4.2.0"
-  dependencies:
-    "@jupyterlab/apputils": ^4.3.0
-    "@jupyterlab/coreutils": ^6.2.0
-    "@jupyterlab/nbformat": ^4.2.0
-    "@jupyterlab/observables": ^5.2.0
-    "@jupyterlab/rendermime-interfaces": ^3.10.0
-    "@jupyterlab/services": ^7.2.0
-    "@jupyterlab/translation": ^4.2.0
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/messaging": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.2
-    lodash.escape: ^4.0.1
-  checksum: 296eba0721a2900cb960fbdb99e98f82999e982f4332f6be8af7ccbb7055b9bcb1517a2b24e5c3b6759c722d5f06f9a68d6a61c8cb59c40855b7852a45aca2bd
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/services@npm:^7.1.6":
   version: 7.1.6
   resolution: "@jupyterlab/services@npm:7.1.6"
   dependencies:
     "@jupyter/ydoc": ^1.1.1
     "@jupyterlab/coreutils": ^6.1.6
     "@jupyterlab/nbformat": ^4.1.6
@@ -2778,33 +2594,14 @@
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     ws: ^8.11.0
   checksum: ad47d3c9b211be4be3aad2714f3028e66ad381a6367a57f347644c693f055ee9c7655d15630a637d9181b42e89c2b8183675abc561c3959820a6bc03d3f2af12
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^7.2.0":
-  version: 7.2.0
-  resolution: "@jupyterlab/services@npm:7.2.0"
-  dependencies:
-    "@jupyter/ydoc": ^2.0.1
-    "@jupyterlab/coreutils": ^6.2.0
-    "@jupyterlab/nbformat": ^4.2.0
-    "@jupyterlab/settingregistry": ^4.2.0
-    "@jupyterlab/statedb": ^4.2.0
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/polling": ^2.1.2
-    "@lumino/properties": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    ws: ^8.11.0
-  checksum: edc93389913d792841b615cd0a317e16c77621cd5cb35e67c40f7a58bcf0e31c77718ae7abcf643621ba86ce78c795d6008a9413d84ecad2b42e39bd52db1447
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/settingregistry@npm:^4.1.6":
   version: 4.1.6
   resolution: "@jupyterlab/settingregistry@npm:4.1.6"
   dependencies:
     "@jupyterlab/nbformat": ^4.1.6
     "@jupyterlab/statedb": ^4.1.6
     "@lumino/commands": ^2.2.0
@@ -2816,59 +2613,27 @@
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
   checksum: 93c1a4921a30243f2bd2c9591319e749e2f5cb5884f6962241857640afb6b67600cdba44fb308a23bffacc7defa3c6fc3d2ad15be52ff5946f0a8fd873b5fddd
   languageName: node
   linkType: hard
 
-"@jupyterlab/settingregistry@npm:^4.2.0":
-  version: 4.2.0
-  resolution: "@jupyterlab/settingregistry@npm:4.2.0"
-  dependencies:
-    "@jupyterlab/nbformat": ^4.2.0
-    "@jupyterlab/statedb": ^4.2.0
-    "@lumino/commands": ^2.3.0
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/signaling": ^2.1.2
-    "@rjsf/utils": ^5.13.4
-    ajv: ^8.12.0
-    json5: ^2.2.3
-  peerDependencies:
-    react: ">=16"
-  checksum: fc60490e9e977e38b14b27a9e3896b47a28930a76a84888dd86180105b9ab6d1e68544f1184bdba72b4c5aa003cb13f10c8e5ca60685827fe6f893302483a109
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/statedb@npm:^4.1.6":
   version: 4.1.6
   resolution: "@jupyterlab/statedb@npm:4.1.6"
   dependencies:
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
   checksum: 4aba49eeead6ac6306ec2d8146543230db9296e7bf088380290eb4b89698b66573c00ba630890b821047b584fc59716b64ba06a013d4698551adeaf20b034301
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:^4.2.0":
-  version: 4.2.0
-  resolution: "@jupyterlab/statedb@npm:4.2.0"
-  dependencies:
-    "@lumino/commands": ^2.3.0
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/properties": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-  checksum: 69620478aa7bf452d7440b9433b6411edef537cd7d9f72f87f70bd6fc0c8fc50003d02ab8d9d4b0746383f98cb7035b093ce5e596e6560e3c35c5a0fe434dce4
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/statusbar@npm:^4.1.6":
   version: 4.1.6
   resolution: "@jupyterlab/statusbar@npm:4.1.6"
   dependencies:
     "@jupyterlab/ui-components": ^4.1.6
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
@@ -2877,30 +2642,14 @@
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
   checksum: ad8a7f366b8a3b3f1f6a4993a0b890192f5de99f0fe3b29aecb7a6474d568203798bee63b77012d4cfdc793b7b376ec8bd64b3c5e67cb26511b13801e7a75f77
   languageName: node
   linkType: hard
 
-"@jupyterlab/statusbar@npm:^4.2.0":
-  version: 4.2.0
-  resolution: "@jupyterlab/statusbar@npm:4.2.0"
-  dependencies:
-    "@jupyterlab/ui-components": ^4.2.0
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/messaging": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.2
-    react: ^18.2.0
-  checksum: 1ab4bfab3d6b37f0ff93ffd8b747b90ec7e532c554c8203716931923bcd97c61ad1b34c07b9973517022f022879014b57614a27f7417996697a5c97cad814c3b
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/testing@npm:^4.1.6":
   version: 4.1.6
   resolution: "@jupyterlab/testing@npm:4.1.6"
   dependencies:
     "@babel/core": ^7.10.2
     "@babel/preset-env": ^7.10.2
     "@jupyterlab/coreutils": ^6.1.6
@@ -2966,27 +2715,14 @@
     "@jupyterlab/services": ^7.1.6
     "@jupyterlab/statedb": ^4.1.6
     "@lumino/coreutils": ^2.1.2
   checksum: 6de45e310d7ac83f2ed2e3e0c372ba71d087e597891d9e9a7ff791f6fc7fc3804d0d18dad5b152757c5a2b583d564ed7f4361561fa993be303e415a47e8b2fa6
   languageName: node
   linkType: hard
 
-"@jupyterlab/translation@npm:^4.2.0":
-  version: 4.2.0
-  resolution: "@jupyterlab/translation@npm:4.2.0"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.2.0
-    "@jupyterlab/rendermime-interfaces": ^3.10.0
-    "@jupyterlab/services": ^7.2.0
-    "@jupyterlab/statedb": ^4.2.0
-    "@lumino/coreutils": ^2.1.2
-  checksum: 0b2d4d3827946bf5b12db5e98356d15dc7721279bb791a46f2927b20b49b597fd717b0d24b84ae4c7b96540f99a0eed82ba0609c186675daf80b343df9792a21
-  languageName: node
-  linkType: hard
-
 "@jupyterlab/ui-components@npm:^4.1.6":
   version: 4.1.6
   resolution: "@jupyterlab/ui-components@npm:4.1.6"
   dependencies:
     "@jupyter/react-components": ^0.15.2
     "@jupyter/web-components": ^0.15.2
     "@jupyterlab/coreutils": ^6.1.6
@@ -3010,45 +2746,14 @@
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
   checksum: f555138b2345aac6ee5c580b517fd563b55b8a6b33f132de362d559a514bbbec970bd690970676173872674f802a5dd9de7ac75b897a0a2b09d7428dddc3c04d
   languageName: node
   linkType: hard
 
-"@jupyterlab/ui-components@npm:^4.2.0":
-  version: 4.2.0
-  resolution: "@jupyterlab/ui-components@npm:4.2.0"
-  dependencies:
-    "@jupyter/react-components": ^0.15.3
-    "@jupyter/web-components": ^0.15.3
-    "@jupyterlab/coreutils": ^6.2.0
-    "@jupyterlab/observables": ^5.2.0
-    "@jupyterlab/rendermime-interfaces": ^3.10.0
-    "@jupyterlab/translation": ^4.2.0
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.3.0
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/messaging": ^2.0.1
-    "@lumino/polling": ^2.1.2
-    "@lumino/properties": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.2
-    "@rjsf/core": ^5.13.4
-    "@rjsf/utils": ^5.13.4
-    react: ^18.2.0
-    react-dom: ^18.2.0
-    typestyle: ^2.0.4
-  peerDependencies:
-    react: ^18.2.0
-  checksum: 9352c9d5d4df2671999a79bcc0434c50731bc78e89b5d94cfcf1e91f55fb14dbe4670576f49b8c53f9c7bb3995e72455c9062ad6953411c188c8bb85edee0a00
-  languageName: node
-  linkType: hard
-
 "@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2, @lezer/common@npm:^1.1.0, @lezer/common@npm:^1.2.0, @lezer/common@npm:^1.2.1":
   version: 1.2.1
   resolution: "@lezer/common@npm:1.2.1"
   checksum: 0bd092e293a509ce334f4aaf9a4d4a25528f743cd9d7e7948c697e34ac703b805b288b62ad01563488fb206fc34ff05084f7fc5d864be775924b3d0d53ea5dd2
   languageName: node
   linkType: hard
 
@@ -3327,15 +3032,15 @@
   resolution: "@lumino/virtualdom@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
   checksum: cf59b6f15b430e13e9e657b7a0619b9056cd9ea7b2a87f407391d071c501b77403c302b6a66dca510382045e75b2e3fe551630bb391f1c6b33678057d4bec164
   languageName: node
   linkType: hard
 
-"@lumino/widgets@npm:^1.37.2 || ^2.3.1, @lumino/widgets@npm:^1.37.2 || ^2.3.2, @lumino/widgets@npm:^2.3.1, @lumino/widgets@npm:^2.3.2":
+"@lumino/widgets@npm:^1.37.2 || ^2.3.1, @lumino/widgets@npm:^2.3.1, @lumino/widgets@npm:^2.3.2":
   version: 2.3.2
   resolution: "@lumino/widgets@npm:2.3.2"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
@@ -5199,15 +4904,14 @@
 
 "didi-notebook-extension@workspace:.":
   version: 0.0.0-use.local
   resolution: "didi-notebook-extension@workspace:."
   dependencies:
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/builder": ^4.0.0
-    "@jupyterlab/docmanager": ^4.1.8
     "@jupyterlab/mainmenu": ^4.1.6
     "@jupyterlab/testutils": ^4.0.0
     "@types/jest": ^29.2.0
     "@types/json-schema": ^7.0.11
     "@types/react": ^18.0.26
     "@types/react-addons-linked-state-mixin": ^0.14.22
     "@typescript-eslint/eslint-plugin": ^6.1.0
@@ -5264,26 +4968,15 @@
     domelementtype: ^2.0.1
     domhandler: ^4.2.0
     entities: ^2.0.0
   checksum: fbb0b01f87a8a2d18e6e5a388ad0f7ec4a5c05c06d219377da1abc7bb0f674d804f4a8a94e3f71ff15f6cb7dcfc75704a54b261db672b9b3ab03da6b758b0b22
   languageName: node
   linkType: hard
 
-"dom-serializer@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "dom-serializer@npm:2.0.0"
-  dependencies:
-    domelementtype: ^2.3.0
-    domhandler: ^5.0.2
-    entities: ^4.2.0
-  checksum: cd1810544fd8cdfbd51fa2c0c1128ec3a13ba92f14e61b7650b5de421b88205fd2e3f0cc6ace82f13334114addb90ed1c2f23074a51770a8e9c1273acbc7f3e6
-  languageName: node
-  linkType: hard
-
-"domelementtype@npm:^2.0.1, domelementtype@npm:^2.2.0, domelementtype@npm:^2.3.0":
+"domelementtype@npm:^2.0.1, domelementtype@npm:^2.2.0":
   version: 2.3.0
   resolution: "domelementtype@npm:2.3.0"
   checksum: ee837a318ff702622f383409d1f5b25dd1024b692ef64d3096ff702e26339f8e345820f29a68bcdcea8cfee3531776b3382651232fbeae95612d6f0a75efb4f6
   languageName: node
   linkType: hard
 
 "domexception@npm:^4.0.0":
@@ -5300,45 +4993,25 @@
   resolution: "domhandler@npm:4.3.1"
   dependencies:
     domelementtype: ^2.2.0
   checksum: 4c665ceed016e1911bf7d1dadc09dc888090b64dee7851cccd2fcf5442747ec39c647bb1cb8c8919f8bbdd0f0c625a6bafeeed4b2d656bbecdbae893f43ffaaa
   languageName: node
   linkType: hard
 
-"domhandler@npm:^5.0.2, domhandler@npm:^5.0.3":
-  version: 5.0.3
-  resolution: "domhandler@npm:5.0.3"
-  dependencies:
-    domelementtype: ^2.3.0
-  checksum: 0f58f4a6af63e6f3a4320aa446d28b5790a009018707bce2859dcb1d21144c7876482b5188395a188dfa974238c019e0a1e610d2fc269a12b2c192ea2b0b131c
-  languageName: node
-  linkType: hard
-
 "domutils@npm:^2.5.2":
   version: 2.8.0
   resolution: "domutils@npm:2.8.0"
   dependencies:
     dom-serializer: ^1.0.1
     domelementtype: ^2.2.0
     domhandler: ^4.2.0
   checksum: abf7434315283e9aadc2a24bac0e00eab07ae4313b40cc239f89d84d7315ebdfd2fb1b5bf750a96bc1b4403d7237c7b2ebf60459be394d625ead4ca89b934391
   languageName: node
   linkType: hard
 
-"domutils@npm:^3.0.1":
-  version: 3.1.0
-  resolution: "domutils@npm:3.1.0"
-  dependencies:
-    dom-serializer: ^2.0.0
-    domelementtype: ^2.3.0
-    domhandler: ^5.0.3
-  checksum: e5757456ddd173caa411cfc02c2bb64133c65546d2c4081381a3bafc8a57411a41eed70494551aa58030be9e58574fcc489828bebd673863d39924fb4878f416
-  languageName: node
-  linkType: hard
-
 "duplicate-package-checker-webpack-plugin@npm:^3.0.0":
   version: 3.0.0
   resolution: "duplicate-package-checker-webpack-plugin@npm:3.0.0"
   dependencies:
     chalk: ^2.3.0
     find-root: ^1.0.0
     lodash: ^4.17.4
@@ -5411,15 +5084,15 @@
 "entities@npm:^2.0.0":
   version: 2.2.0
   resolution: "entities@npm:2.2.0"
   checksum: 19010dacaf0912c895ea262b4f6128574f9ccf8d4b3b65c7e8334ad0079b3706376360e28d8843ff50a78aabcb8f08f0a32dbfacdc77e47ed77ca08b713669b3
   languageName: node
   linkType: hard
 
-"entities@npm:^4.2.0, entities@npm:^4.4.0":
+"entities@npm:^4.4.0":
   version: 4.5.0
   resolution: "entities@npm:4.5.0"
   checksum: 853f8ebd5b425d350bffa97dd6958143179a5938352ccae092c62d1267c4e392a039be1bae7d51b6e4ffad25f51f9617531fedf5237f15df302ccfb452cbf2d7
   languageName: node
   linkType: hard
 
 "env-paths@npm:^2.2.0":
@@ -6429,26 +6102,14 @@
     domhandler: ^4.0.0
     domutils: ^2.5.2
     entities: ^2.0.0
   checksum: 81a7b3d9c3bb9acb568a02fc9b1b81ffbfa55eae7f1c41ae0bf840006d1dbf54cb3aa245b2553e2c94db674840a9f0fdad7027c9a9d01a062065314039058c4e
   languageName: node
   linkType: hard
 
-"htmlparser2@npm:^8.0.0":
-  version: 8.0.2
-  resolution: "htmlparser2@npm:8.0.2"
-  dependencies:
-    domelementtype: ^2.3.0
-    domhandler: ^5.0.3
-    domutils: ^3.0.1
-    entities: ^4.4.0
-  checksum: 29167a0f9282f181da8a6d0311b76820c8a59bc9e3c87009e21968264c2987d2723d6fde5a964d4b7b6cba663fca96ffb373c06d8223a85f52a6089ced942700
-  languageName: node
-  linkType: hard
-
 "http-cache-semantics@npm:^4.1.1":
   version: 4.1.1
   resolution: "http-cache-semantics@npm:4.1.1"
   checksum: 83ac0bc60b17a3a36f9953e7be55e5c8f41acc61b22583060e8dedc9dd5e3607c823a88d0926f9150e571f90946835c7fe150732801010845c72cd8bbff1a236
   languageName: node
   linkType: hard
 
@@ -9175,28 +8836,14 @@
 "safer-buffer@npm:>= 2.1.2 < 3.0.0":
   version: 2.1.2
   resolution: "safer-buffer@npm:2.1.2"
   checksum: cab8f25ae6f1434abee8d80023d7e72b598cf1327164ddab31003c51215526801e40b66c5e65d658a0af1e9d6478cadcb4c745f4bd6751f97d8644786c0978b0
   languageName: node
   linkType: hard
 
-"sanitize-html@npm:~2.12.1":
-  version: 2.12.1
-  resolution: "sanitize-html@npm:2.12.1"
-  dependencies:
-    deepmerge: ^4.2.2
-    escape-string-regexp: ^4.0.0
-    htmlparser2: ^8.0.0
-    is-plain-object: ^5.0.0
-    parse-srcset: ^1.0.2
-    postcss: ^8.3.11
-  checksum: fb96ea7170d51b5af2607f5cfd84464c78fc6f47e339407f55783e781c6a0288a8d40bbf97ea6a8758924ba9b2d33dcc4846bb94caacacd90d7f2de10ed8541a
-  languageName: node
-  linkType: hard
-
 "sanitize-html@npm:~2.7.3":
   version: 2.7.3
   resolution: "sanitize-html@npm:2.7.3"
   dependencies:
     deepmerge: ^4.2.2
     escape-string-regexp: ^4.0.0
     htmlparser2: ^6.0.0
```

### Comparing `didi_notebook_extension-0.0.17/didi_notebook_extension/__init__.py` & `didi_notebook_extension-0.2.7/didi_notebook_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `didi_notebook_extension-0.0.17/didi_notebook_extension/labextension/package.json` & `didi_notebook_extension-0.2.7/didi_notebook_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9716435185185186%*

 * *Differences: {"'dependencies'": "{delete: ['@jupyterlab/docmanager']}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.669ff8394f95a035c486.js'}}",*

 * * "'version'": "'0.2.7'"}*

```diff
@@ -4,15 +4,14 @@
         "name": "dongmeiqi"
     },
     "bugs": {
         "url": "https://github.com/yobi-maggie/didi-notebook-extension/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^4.0.0",
-        "@jupyterlab/docmanager": "^4.1.8",
         "@jupyterlab/mainmenu": "^4.1.6"
     },
     "description": "A JupyterLab extension.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
         "@types/jest": "^29.2.0",
@@ -107,15 +106,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/yobi-maggie/didi-notebook-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.8939b006cb56785ffe74.js",
+            "load": "static/remoteEntry.669ff8394f95a035c486.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "didi_notebook_extension/labextension"
     },
     "keywords": [
         "jupyter",
@@ -193,9 +192,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.0.17"
+    "version": "0.2.7"
 }
```

### Comparing `didi_notebook_extension-0.0.17/didi_notebook_extension/labextension/static/728.9916fbef502e316a159a.js` & `didi_notebook_extension-0.2.7/didi_notebook_extension/labextension/static/728.adf73d00115832453a58.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
             t.d(e, {
                 A: () => p
             });
             var o = t(601),
                 a = t.n(o),
                 r = t(314),
                 i = t.n(r)()(a());
-            i.push([n.id, '/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n.hide-menu #jp-left-stack, \n.hide-menu #jp-right-stack,\n.hide-menu #jp-top-panel, \n.hide-menu .jp-SideBar,\n.hide-menu #jp-bottom-panel{\n    display: none !important;\n}\n.hide-menu #jp-main-dock-panel {\n    left: 0 !important;\n    width: 100% !important;\n}\n.hide-menu #jq-main-dock-panel #jp-main-dock-panel {\n    width: 100% !important;\n}\n.hide-menu #jp-main-vsplit-panel {\n    left: 0 !important;\n    width: 100% !important;\n}\n.hide-menu #jp-main-split-panel {\n    width: 100% !important;\n    left: 0 !important;\n}\n.hide-menu #jp-main-content-panel{\n    top: 0 !important;\n    left: 0 !important;\n    width: 100% !important;\n}\n.hide-menu .jp-NotebookPanel, .hide-menu .jp-Notebook {\n    width: 100% !important;\n}\n.hide-menu .jp-NotebookPanel  > .jp-NotebookPanel-toolbar,\n.hide-menu .lm-DockPanel  > .lm-DockPanel-tabBar\n {\n    width: 100% !important;\n}\n.from-studio .jp-KernelName, \n.from-studio .lm-DockPanel-tabBar,\n.from-studio .lm-TabBar \n.hide-menu.from-studio .jp-NotebookPanel  > .jp-NotebookPanel-toolbar,\n.hide-menu.from-studio .lm-DockPanel  > .lm-DockPanel-tabBar{\n    display: none !important;\n}\n.from-studio.hide-menu .jp-NotebookPanel, .from-studio.hide-menu .lm-DockPanel {\n    top: 0 !important;\n    border: none !important;\n}\n.from-studio .jp-Notebook-toolbarCellType .jp-Notebook-toolbarCellTypeDropdown option[value="raw"],\n.from-studio .jp-CommandToolbarButton .jp-ToolbarButtonComponent[data-command="docmanager:save"] {\n    display: none !important;\n}\n.from-studio .lm-Menu-item[data-command="notebook:create-console"], \n.from-studio .lm-Menu-item[data-command="inspector:open"],\n.from-studio .lm-Menu-item[data-command="logconsole:open"] {\n    display: none !important;\n}\n.from-studio .lm-TabBar .lm-TabBar-addButton {\n    display: none !important;\n}\n.from-studio {\n    background-color: #fff;\n}', ""]);
+            i.push([n.id, '/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n.hide-menu #jp-left-stack, \n.hide-menu #jp-right-stack,\n.hide-menu #jp-top-panel, \n.hide-menu .jp-SideBar,\n.hide-menu #jp-bottom-panel{\n    display: none !important;\n}\n.hide-menu #jp-main-dock-panel {\n    left: 0 !important;\n    width: 100% !important;\n}\n.hide-menu #jq-main-dock-panel #jp-main-dock-panel {\n    width: 100% !important;\n}\n.hide-menu #jp-main-vsplit-panel {\n    left: 0 !important;\n    width: 100% !important;\n}\n.hide-menu #jp-main-split-panel {\n    width: 100% !important;\n    left: 0 !important;\n}\n.hide-menu #jp-main-content-panel{\n    top: 0 !important;\n    left: 0 !important;\n    width: 100% !important;\n}\n.hide-menu .jp-NotebookPanel, .hide-menu .jp-Notebook {\n    width: 100% !important;\n}\n.hide-menu .jp-NotebookPanel  > .jp-NotebookPanel-toolbar,\n.hide-menu .lm-DockPanel  > .lm-DockPanel-tabBar\n {\n    width: 100% !important;\n}\n.from-studio .jp-KernelName, \n.from-studio .lm-DockPanel-tabBar,\n.from-studio .lm-TabBar \n.hide-menu.from-studio .jp-NotebookPanel  > .jp-NotebookPanel-toolbar,\n.hide-menu.from-studio .lm-DockPanel  > .lm-DockPanel-tabBar{\n    display: none !important;\n}\n.from-studio .jp-Notebook-toolbarCellType .jp-Notebook-toolbarCellTypeDropdown option[value="raw"],\n.from-studio .jp-CommandToolbarButton .jp-ToolbarButtonComponent[data-command="docmanager:save"] {\n    display: none !important;\n}\n.from-studio .lm-Menu-item[data-command="notebook:create-console"], \n.from-studio .lm-Menu-item[data-command="inspector:open"],\n.from-studio .lm-Menu-item[data-command="logconsole:open"] {\n    display: none !important;\n}\n.from-studio .lm-TabBar .lm-TabBar-addButton {\n    display: none !important;\n}\n.from-studio {\n    background-color: #fff;\n}', ""]);
             const p = i
         },
         314: n => {
             n.exports = function(n) {
                 var e = [];
                 return e.toString = function() {
                     return this.map((function(e) {
@@ -28,16 +28,16 @@
                     var i = {};
                     if (o)
                         for (var p = 0; p < this.length; p++) {
                             var s = this[p][0];
                             null != s && (i[s] = !0)
                         }
                     for (var l = 0; l < n.length; l++) {
-                        var u = [].concat(n[l]);
-                        o && i[u[0]] || (void 0 !== r && (void 0 === u[5] || (u[1] = "@layer".concat(u[5].length > 0 ? " ".concat(u[5]) : "", " {").concat(u[1], "}")), u[5] = r), t && (u[2] ? (u[1] = "@media ".concat(u[2], " {").concat(u[1], "}"), u[2] = t) : u[2] = t), a && (u[4] ? (u[1] = "@supports (".concat(u[4], ") {").concat(u[1], "}"), u[4] = a) : u[4] = "".concat(a)), e.push(u))
+                        var c = [].concat(n[l]);
+                        o && i[c[0]] || (void 0 !== r && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = r), t && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = t) : c[2] = t), a && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = a) : c[4] = "".concat(a)), e.push(c))
                     }
                 }, e
             }
         },
         601: n => {
             n.exports = function(n) {
                 return n[1]
@@ -54,35 +54,35 @@
                     } return t
             }
 
             function o(n, o) {
                 for (var r = {}, i = [], p = 0; p < n.length; p++) {
                     var s = n[p],
                         l = o.base ? s[0] + o.base : s[0],
-                        u = r[l] || 0,
-                        d = "".concat(l, " ").concat(u);
-                    r[l] = u + 1;
-                    var c = t(d),
+                        c = r[l] || 0,
+                        u = "".concat(l, " ").concat(c);
+                    r[l] = c + 1;
+                    var d = t(u),
                         m = {
                             css: s[1],
                             media: s[2],
                             sourceMap: s[3],
                             supports: s[4],
                             layer: s[5]
                         };
-                    if (-1 !== c) e[c].references++, e[c].updater(m);
+                    if (-1 !== d) e[d].references++, e[d].updater(m);
                     else {
                         var f = a(m, o);
                         o.byIndex = p, e.splice(p, 0, {
-                            identifier: d,
+                            identifier: u,
                             updater: f,
                             references: 1
                         })
                     }
-                    i.push(d)
+                    i.push(u)
                 }
                 return i
             }
 
             function a(n, e) {
                 var t = e.domAPI(e);
                 return t.update(n),
@@ -98,16 +98,16 @@
                 return function(n) {
                     n = n || [];
                     for (var i = 0; i < r.length; i++) {
                         var p = t(r[i]);
                         e[p].references--
                     }
                     for (var s = o(n, a), l = 0; l < r.length; l++) {
-                        var u = t(r[l]);
-                        0 === e[u].references && (e[u].updater(), e.splice(u, 1))
+                        var c = t(r[l]);
+                        0 === e[c].references && (e[c].updater(), e.splice(c, 1))
                     }
                     r = s
                 }
             }
         },
         659: n => {
             var e = {};
@@ -181,18 +181,18 @@
             var o = t(72),
                 a = t.n(o),
                 r = t(825),
                 i = t.n(r),
                 p = t(659),
                 s = t.n(p),
                 l = t(56),
-                u = t.n(l),
-                d = t(540),
-                c = t.n(d),
+                c = t.n(l),
+                u = t(540),
+                d = t.n(u),
                 m = t(113),
                 f = t.n(m),
                 h = t(475),
                 v = {};
-            v.styleTagTransform = f(), v.setAttributes = u(), v.insert = s().bind(null, "head"), v.domAPI = i(), v.insertStyleElement = c(), a()(h.A, v), h.A && h.A.locals && h.A.locals
+            v.styleTagTransform = f(), v.setAttributes = c(), v.insert = s().bind(null, "head"), v.domAPI = i(), v.insertStyleElement = d(), a()(h.A, v), h.A && h.A.locals && h.A.locals
         }
     }
 ]);
```

### Comparing `didi_notebook_extension-0.0.17/didi_notebook_extension/labextension/static/958.bd36d1031c08063aa2e9.js` & `didi_notebook_extension-0.2.7/didi_notebook_extension/labextension/static/958.eb0e437e53b6a86814b4.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,305 +1,274 @@
 "use strict";
 (self.webpackChunkdidi_notebook_extension = self.webpackChunkdidi_notebook_extension || []).push([
     [958], {
-        958: (e, o, n) => {
-            n.r(o), n.d(o, {
+        958: (e, n, o) => {
+            o.r(n), o.d(n, {
                 default: () => T
             });
-            var t = n(626),
-                i = n(923),
-                a = n(72),
-                d = n.n(a),
-                s = n(825),
-                r = n.n(s),
-                l = n(659),
-                c = n.n(l),
-                u = n(56),
-                p = n.n(u),
-                m = n(540),
-                f = n.n(m),
-                h = n(113),
-                b = n.n(h),
-                g = n(646),
-                v = {};
-            v.styleTagTransform = b(), v.setAttributes = p(), v.insert = c().bind(null, "head"), v.domAPI = r(), v.insertStyleElement = f(), d()(g.A, v), g.A && g.A.locals && g.A.locals;
-            var k = n(670),
-                w = n(291);
+            var t = o(371),
+                i = o(440),
+                a = o(72),
+                r = o.n(a),
+                d = o(825),
+                s = o.n(d),
+                l = o(659),
+                c = o.n(l),
+                u = o(56),
+                p = o.n(u),
+                m = o(540),
+                f = o.n(m),
+                h = o(113),
+                b = o.n(h),
+                v = o(646),
+                g = {};
+            g.styleTagTransform = b(), g.setAttributes = p(), g.insert = c().bind(null, "head"), g.domAPI = s(), g.insertStyleElement = f(), r()(v.A, g), v.A && v.A.locals && v.A.locals;
+            var k = o(215),
+                y = o(943),
+                w = o(506);
             let x = "online"; - 1 !== location.hostname.indexOf("notebook-test.bigdata.xiaojukeji.com") ? x = "test" : -1 !== location.hostname.indexOf("didiglobal.com") && (x = "global");
-            const y = "global" !== x ? "2101066" : "2824";
-            var j = n(899);
-            const {
-                MainAreaWidget: C
-            } = n(923), {
-                Widget: L
-            } = n(256), T = {
-                id: "didi-notebook-extension:plugin",
-                description: "A JupyterLab extension.",
-                autoStart: !0,
-                requires: [k.IFileBrowserFactory, k.IDefaultFileBrowser, i.IWindowResolver, j.IDocumentManager, i.ICommandPalette, w.INotebookTracker],
-                optional: [t.ILabShell],
-                activate: async (e, o, n, t, i, a, d, s) => {
-                    const r = new URLSearchParams(window.location.search),
-                        l = r.get("from"),
-                        c = r.get("saveId"),
-                        u = r.get("hideMenu") || !1;
-                    console.log("-----didi-notebook-extension url query----", r);
-                    const p = new L;
-                    if (p.id = "didi-notebook-extension-plugin-window", p.title.label = "didi-notebook-extension Window", p.title.closable = !0, "studio" === l) {
-                        if (console.log("-----didi-notebook-extension----check from studio------"), document.body.classList.add("from-studio"), !await (async () => {
-                                console.log("----------didi-notebook-extensio checkLogin-----------");
-                                try {
-                                    let e = (await fetch("/api/isLogin", {
-                                        method: "GET"
-                                    })).body;
-                                    if (console.log("----------didi-notebook-extensio checkLogin success data-----------", e), 10001 === (null == e ? void 0 : e.code)) {
-                                        let o = "mis.diditaxi.com.cn";
-                                        "global" === x && (o = "mis-auth.didiglobal.com"), console.log("----------didi-notebook-extensio checkLogin failed data-----------", e);
-                                        const n = encodeURIComponent(location.href);
-                                        window.location.href = `//${o}/auth/sso/login?app_id=${y}&jumpto=${n}&callback_index=2`
-                                    } else if (0 === e.code || 1e4 === e.code || 14001 === e.code) return e;
-                                    return !0
-                                } catch (e) {
-                                    return console.error("Failed to check login status:", e), !0
-                                }
-                            })()) return void console.log("-----didi-notebook-extension----check login failed------");
-                        console.log("-----didi-notebook-extension----check login success------"), console.log("------from studio  window------", window), p.node.addEventListener("message", (o => {
-                            console.log("---------didi-notebook-extension content node 收到数据啦啦啦啦啦啦---------", o.data), "studio-debug-mode-save" === (o.data || {}).event && e.commands.execute("docmanager:save")
-                        }), !1), window.addEventListener("message", (async o => {
-                            var n, t;
-                            console.log("--------didi-notebook-extension window 收到数据啦啦啦啦啦啦---------", o.data);
-                            const a = o.data || {};
-                            if ("studio-debug-mode-save" === a.event) {
-                                console.log("--------didi-notebook-extension window docmanager:save 保存文件啦---------"), e.commands.execute("docmanager:save");
-                                try {
-                                    const e = null == s ? void 0 : s.currentWidget;
-                                    console.log("--------didi-notebook-extension windowcontextForWidget 保存文件啦---------");
-                                    const o = i.contextForWidget(e);
-                                    await (null == o ? void 0 : o.save()), console.log("--------didi-notebook-extension windowcontextForWidget context", o)
-                                } catch (e) {
-                                    console.log("--------didi-notebook-extension window 手动保存文件失败啦-----", e)
-                                }
-                                console.log("--------didi-notebook-extension windowcontextForWidget 保存成功啦---------"), window.parent.postMessage({
-                                    event: "notebook-extension-file-save",
-                                    id: (null == a ? void 0 : a.id) || c,
-                                    status: !0
-                                }, "*")
-                            } else if ("studio-quit-debug-mode" === a.event) {
-                                console.log("--------didi-notebook-extension window 手动停止kernel啦---------");
-                                try {
-                                    null === (t = null === (n = e.serviceManager) || void 0 === n ? void 0 : n.sessions) || void 0 === t || t.dispose(), console.log("--------------didi-notebook-extension Kernel terminated successfully.------------")
-                                } catch (e) {
-                                    console.error("--------------didi-notebook-extensionFailed to terminate kernel:", e)
-                                }
-                            }
-                        }), !1);
-                        const n = new C({
-                            content: p
-                        });
-                        s && (null == s || s.add(n, "main")), o.createFileBrowser("cur-file").model.fileChanged.connect(((e, o) => {
-                            "save" === o.type && (console.log("---didi-notebook-extension-----File saved-------", e, o), window.parent.postMessage({
-                                event: "notebook-extension-file-save",
-                                id: c,
-                                status: !0
+            const j = "global" !== x ? "280" : "2824",
+                {
+                    MainAreaWidget: C
+                } = o(440),
+                {
+                    Widget: L
+                } = o(256),
+                T = {
+                    id: "didi-notebook-extension:plugin",
+                    description: "A JupyterLab extension.",
+                    autoStart: !0,
+                    requires: [k.IMainMenu, y.IFileBrowserFactory, i.ICommandPalette, w.INotebookTracker],
+                    optional: [t.ILabShell],
+                    activate: async (e, n, o, t, i, a) => {
+                        const r = new URLSearchParams(window.location.search),
+                            d = r.get("from"),
+                            s = r.get("hideMenu") || !1;
+                        console.log("-----didi-notebook-extension url query----", r);
+                        const l = new L;
+                        if (l.id = "didi-notebook-extension-plugin-window", l.title.label = "didi-notebook-extension Window", l.title.closable = !0, "studio" === d) {
+                            if (console.log("-----didi-notebook-extension----check from studio------"), document.body.classList.add("from-studio"), !await (async () => {
+                                    console.log("----------didi-notebook-extensio checkLogin-----------");
+                                    try {
+                                        let e = (await fetch("/api/isLogin", {
+                                            method: "GET"
+                                        })).body;
+                                        if (console.log("----------didi-notebook-extensio checkLogin success data-----------", e), 10001 === (null == e ? void 0 : e.code)) {
+                                            let n = "mis.diditaxi.com.cn";
+                                            "global" === x && (n = "mis-auth.didiglobal.com"), console.log("----------didi-notebook-extensio checkLogin failed data-----------", e);
+                                            const o = encodeURIComponent(location.href);
+                                            window.location.href = `//${n}/auth/sso/login?app_id=${j}&jumpto=${o}&callback_index=2`
+                                        } else if (0 === e.code || 1e4 === e.code || 14001 === e.code) return e;
+                                        return !0
+                                    } catch (e) {
+                                        return console.error("Failed to check login status:", e), !0
+                                    }
+                                })()) return void console.log("-----didi-notebook-extension----check login failed------");
+                            console.log("-----didi-notebook-extension----check login success------"), console.log("------from studio  window------", window), l.node.addEventListener("message", (n => {
+                                console.log("---------didi-notebook-extension 收到数据啦啦啦啦啦啦---------", n.data), "studio-debug-mode-save" === (n.data || {}).event && e.commands.execute("docmanager:save")
+                            }));
+                            const n = new C({
+                                content: l
+                            });
+                            a && (null == a || a.add(n, "main"))
+                        }
+                        "true" !== s && !1 === s || (document.body.classList.add("hide-menu"), a && (a.leftCollapsed && a.expandLeft(), a.rightCollapsed && a.expandRight(), a.activeChanged.connect(((e, n) => {
+                            e.leftCollapsed && e.expandLeft(), e.rightCollapsed && e.expandRight()
+                        })))), o.createFileBrowser("cur-file").model.fileChanged.connect(((e, n) => {
+                            "save" === n.type && (console.log("---didi-notebook-extension-----File saved-------"), window.parent.postMessage({
+                                event: "studio-debug-mode-save",
+                                key: "save"
                             }, "*"))
-                        }))
+                        })), console.log("JupyterLab extension didinotebooktest is activated! log", d, s), console.log("JupyterLab extension didi-notebook-extension is activated!", window, e)
                     }
-                    "true" !== u && !1 === u || (document.body.classList.add("hide-menu"), s && (s.leftCollapsed && s.expandLeft(), s.rightCollapsed && s.expandRight(), s.activeChanged.connect(((e, o) => {
-                        e.leftCollapsed && e.expandLeft(), e.rightCollapsed && e.expandRight()
-                    })))), console.log("JupyterLab extension didinotebooktest is activated! log", l, u), console.log("JupyterLab extension didi-notebook-extension is activated!", window, e, document.getElementsByClassName("moon")), window.parent.postMessage({
-                        event: "notebook-extension-status",
-                        status: "loaded",
-                        id: c
-                    }, "*")
                 }
-            }
         },
-        475: (e, o, n) => {
-            n.d(o, {
-                A: () => s
+        475: (e, n, o) => {
+            o.d(n, {
+                A: () => d
             });
-            var t = n(601),
-                i = n.n(t),
-                a = n(314),
-                d = n.n(a)()(i());
-            d.push([e.id, '/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n.hide-menu #jp-left-stack, \n.hide-menu #jp-right-stack,\n.hide-menu #jp-top-panel, \n.hide-menu .jp-SideBar,\n.hide-menu #jp-bottom-panel{\n    display: none !important;\n}\n.hide-menu #jp-main-dock-panel {\n    left: 0 !important;\n    width: 100% !important;\n}\n.hide-menu #jq-main-dock-panel #jp-main-dock-panel {\n    width: 100% !important;\n}\n.hide-menu #jp-main-vsplit-panel {\n    left: 0 !important;\n    width: 100% !important;\n}\n.hide-menu #jp-main-split-panel {\n    width: 100% !important;\n    left: 0 !important;\n}\n.hide-menu #jp-main-content-panel{\n    top: 0 !important;\n    left: 0 !important;\n    width: 100% !important;\n}\n.hide-menu .jp-NotebookPanel, .hide-menu .jp-Notebook {\n    width: 100% !important;\n}\n.hide-menu .jp-NotebookPanel  > .jp-NotebookPanel-toolbar,\n.hide-menu .lm-DockPanel  > .lm-DockPanel-tabBar\n {\n    width: 100% !important;\n}\n.from-studio .jp-KernelName, \n.from-studio .lm-DockPanel-tabBar,\n.from-studio .lm-TabBar \n.hide-menu.from-studio .jp-NotebookPanel  > .jp-NotebookPanel-toolbar,\n.hide-menu.from-studio .lm-DockPanel  > .lm-DockPanel-tabBar{\n    display: none !important;\n}\n.from-studio.hide-menu .jp-NotebookPanel, .from-studio.hide-menu .lm-DockPanel {\n    top: 0 !important;\n    border: none !important;\n}\n.from-studio .jp-Notebook-toolbarCellType .jp-Notebook-toolbarCellTypeDropdown option[value="raw"],\n.from-studio .jp-CommandToolbarButton .jp-ToolbarButtonComponent[data-command="docmanager:save"] {\n    display: none !important;\n}\n.from-studio .lm-Menu-item[data-command="notebook:create-console"], \n.from-studio .lm-Menu-item[data-command="inspector:open"],\n.from-studio .lm-Menu-item[data-command="logconsole:open"] {\n    display: none !important;\n}\n.from-studio .lm-TabBar .lm-TabBar-addButton {\n    display: none !important;\n}\n.from-studio {\n    background-color: #fff;\n}', ""]);
-            const s = d
+            var t = o(601),
+                i = o.n(t),
+                a = o(314),
+                r = o.n(a)()(i());
+            r.push([e.id, '/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n.hide-menu #jp-left-stack, \n.hide-menu #jp-right-stack,\n.hide-menu #jp-top-panel, \n.hide-menu .jp-SideBar,\n.hide-menu #jp-bottom-panel{\n    display: none !important;\n}\n.hide-menu #jp-main-dock-panel {\n    left: 0 !important;\n    width: 100% !important;\n}\n.hide-menu #jq-main-dock-panel #jp-main-dock-panel {\n    width: 100% !important;\n}\n.hide-menu #jp-main-vsplit-panel {\n    left: 0 !important;\n    width: 100% !important;\n}\n.hide-menu #jp-main-split-panel {\n    width: 100% !important;\n    left: 0 !important;\n}\n.hide-menu #jp-main-content-panel{\n    top: 0 !important;\n    left: 0 !important;\n    width: 100% !important;\n}\n.hide-menu .jp-NotebookPanel, .hide-menu .jp-Notebook {\n    width: 100% !important;\n}\n.hide-menu .jp-NotebookPanel  > .jp-NotebookPanel-toolbar,\n.hide-menu .lm-DockPanel  > .lm-DockPanel-tabBar\n {\n    width: 100% !important;\n}\n.from-studio .jp-KernelName, \n.from-studio .lm-DockPanel-tabBar,\n.from-studio .lm-TabBar \n.hide-menu.from-studio .jp-NotebookPanel  > .jp-NotebookPanel-toolbar,\n.hide-menu.from-studio .lm-DockPanel  > .lm-DockPanel-tabBar{\n    display: none !important;\n}\n.from-studio .jp-Notebook-toolbarCellType .jp-Notebook-toolbarCellTypeDropdown option[value="raw"],\n.from-studio .jp-CommandToolbarButton .jp-ToolbarButtonComponent[data-command="docmanager:save"] {\n    display: none !important;\n}\n.from-studio .lm-Menu-item[data-command="notebook:create-console"], \n.from-studio .lm-Menu-item[data-command="inspector:open"],\n.from-studio .lm-Menu-item[data-command="logconsole:open"] {\n    display: none !important;\n}\n.from-studio .lm-TabBar .lm-TabBar-addButton {\n    display: none !important;\n}\n.from-studio {\n    background-color: #fff;\n}', ""]);
+            const d = r
         },
-        646: (e, o, n) => {
-            n.d(o, {
+        646: (e, n, o) => {
+            o.d(n, {
                 A: () => l
             });
-            var t = n(601),
-                i = n.n(t),
-                a = n(314),
-                d = n.n(a),
-                s = n(475),
-                r = d()(i());
-            r.i(s.A), r.push([e.id, "\n", ""]);
-            const l = r
+            var t = o(601),
+                i = o.n(t),
+                a = o(314),
+                r = o.n(a),
+                d = o(475),
+                s = r()(i());
+            s.i(d.A), s.push([e.id, "\n", ""]);
+            const l = s
         },
         314: e => {
             e.exports = function(e) {
-                var o = [];
-                return o.toString = function() {
-                    return this.map((function(o) {
-                        var n = "",
-                            t = void 0 !== o[5];
-                        return o[4] && (n += "@supports (".concat(o[4], ") {")), o[2] && (n += "@media ".concat(o[2], " {")), t && (n += "@layer".concat(o[5].length > 0 ? " ".concat(o[5]) : "", " {")), n += e(o), t && (n += "}"), o[2] && (n += "}"), o[4] && (n += "}"), n
+                var n = [];
+                return n.toString = function() {
+                    return this.map((function(n) {
+                        var o = "",
+                            t = void 0 !== n[5];
+                        return n[4] && (o += "@supports (".concat(n[4], ") {")), n[2] && (o += "@media ".concat(n[2], " {")), t && (o += "@layer".concat(n[5].length > 0 ? " ".concat(n[5]) : "", " {")), o += e(n), t && (o += "}"), n[2] && (o += "}"), n[4] && (o += "}"), o
                     })).join("")
-                }, o.i = function(e, n, t, i, a) {
+                }, n.i = function(e, o, t, i, a) {
                     "string" == typeof e && (e = [
                         [null, e, void 0]
                     ]);
-                    var d = {};
+                    var r = {};
                     if (t)
-                        for (var s = 0; s < this.length; s++) {
-                            var r = this[s][0];
-                            null != r && (d[r] = !0)
+                        for (var d = 0; d < this.length; d++) {
+                            var s = this[d][0];
+                            null != s && (r[s] = !0)
                         }
                     for (var l = 0; l < e.length; l++) {
                         var c = [].concat(e[l]);
-                        t && d[c[0]] || (void 0 !== a && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = a), n && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = n) : c[2] = n), i && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = i) : c[4] = "".concat(i)), o.push(c))
+                        t && r[c[0]] || (void 0 !== a && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = a), o && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = o) : c[2] = o), i && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = i) : c[4] = "".concat(i)), n.push(c))
                     }
-                }, o
+                }, n
             }
         },
         601: e => {
             e.exports = function(e) {
                 return e[1]
             }
         },
         72: e => {
-            var o = [];
+            var n = [];
 
-            function n(e) {
-                for (var n = -1, t = 0; t < o.length; t++)
-                    if (o[t].identifier === e) {
-                        n = t;
+            function o(e) {
+                for (var o = -1, t = 0; t < n.length; t++)
+                    if (n[t].identifier === e) {
+                        o = t;
                         break
-                    } return n
+                    } return o
             }
 
             function t(e, t) {
-                for (var a = {}, d = [], s = 0; s < e.length; s++) {
-                    var r = e[s],
-                        l = t.base ? r[0] + t.base : r[0],
+                for (var a = {}, r = [], d = 0; d < e.length; d++) {
+                    var s = e[d],
+                        l = t.base ? s[0] + t.base : s[0],
                         c = a[l] || 0,
                         u = "".concat(l, " ").concat(c);
                     a[l] = c + 1;
-                    var p = n(u),
+                    var p = o(u),
                         m = {
-                            css: r[1],
-                            media: r[2],
-                            sourceMap: r[3],
-                            supports: r[4],
-                            layer: r[5]
+                            css: s[1],
+                            media: s[2],
+                            sourceMap: s[3],
+                            supports: s[4],
+                            layer: s[5]
                         };
-                    if (-1 !== p) o[p].references++, o[p].updater(m);
+                    if (-1 !== p) n[p].references++, n[p].updater(m);
                     else {
                         var f = i(m, t);
-                        t.byIndex = s, o.splice(s, 0, {
+                        t.byIndex = d, n.splice(d, 0, {
                             identifier: u,
                             updater: f,
                             references: 1
                         })
                     }
-                    d.push(u)
+                    r.push(u)
                 }
-                return d
+                return r
             }
 
-            function i(e, o) {
-                var n = o.domAPI(o);
-                return n.update(e),
-                    function(o) {
-                        if (o) {
-                            if (o.css === e.css && o.media === e.media && o.sourceMap === e.sourceMap && o.supports === e.supports && o.layer === e.layer) return;
-                            n.update(e = o)
-                        } else n.remove()
+            function i(e, n) {
+                var o = n.domAPI(n);
+                return o.update(e),
+                    function(n) {
+                        if (n) {
+                            if (n.css === e.css && n.media === e.media && n.sourceMap === e.sourceMap && n.supports === e.supports && n.layer === e.layer) return;
+                            o.update(e = n)
+                        } else o.remove()
                     }
             }
             e.exports = function(e, i) {
                 var a = t(e = e || [], i = i || {});
                 return function(e) {
                     e = e || [];
-                    for (var d = 0; d < a.length; d++) {
-                        var s = n(a[d]);
-                        o[s].references--
+                    for (var r = 0; r < a.length; r++) {
+                        var d = o(a[r]);
+                        n[d].references--
                     }
-                    for (var r = t(e, i), l = 0; l < a.length; l++) {
-                        var c = n(a[l]);
-                        0 === o[c].references && (o[c].updater(), o.splice(c, 1))
+                    for (var s = t(e, i), l = 0; l < a.length; l++) {
+                        var c = o(a[l]);
+                        0 === n[c].references && (n[c].updater(), n.splice(c, 1))
                     }
-                    a = r
+                    a = s
                 }
             }
         },
         659: e => {
-            var o = {};
-            e.exports = function(e, n) {
+            var n = {};
+            e.exports = function(e, o) {
                 var t = function(e) {
-                    if (void 0 === o[e]) {
-                        var n = document.querySelector(e);
-                        if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
-                            n = n.contentDocument.head
+                    if (void 0 === n[e]) {
+                        var o = document.querySelector(e);
+                        if (window.HTMLIFrameElement && o instanceof window.HTMLIFrameElement) try {
+                            o = o.contentDocument.head
                         } catch (e) {
-                            n = null
+                            o = null
                         }
-                        o[e] = n
+                        n[e] = o
                     }
-                    return o[e]
+                    return n[e]
                 }(e);
                 if (!t) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                t.appendChild(n)
+                t.appendChild(o)
             }
         },
         540: e => {
             e.exports = function(e) {
-                var o = document.createElement("style");
-                return e.setAttributes(o, e.attributes), e.insert(o, e.options), o
+                var n = document.createElement("style");
+                return e.setAttributes(n, e.attributes), e.insert(n, e.options), n
             }
         },
-        56: (e, o, n) => {
+        56: (e, n, o) => {
             e.exports = function(e) {
-                var o = n.nc;
-                o && e.setAttribute("nonce", o)
+                var n = o.nc;
+                n && e.setAttribute("nonce", n)
             }
         },
         825: e => {
             e.exports = function(e) {
                 if ("undefined" == typeof document) return {
                     update: function() {},
                     remove: function() {}
                 };
-                var o = e.insertStyleElement(e);
+                var n = e.insertStyleElement(e);
                 return {
-                    update: function(n) {
-                        ! function(e, o, n) {
+                    update: function(o) {
+                        ! function(e, n, o) {
                             var t = "";
-                            n.supports && (t += "@supports (".concat(n.supports, ") {")), n.media && (t += "@media ".concat(n.media, " {"));
-                            var i = void 0 !== n.layer;
-                            i && (t += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), t += n.css, i && (t += "}"), n.media && (t += "}"), n.supports && (t += "}");
-                            var a = n.sourceMap;
-                            a && "undefined" != typeof btoa && (t += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a)))), " */")), o.styleTagTransform(t, e, o.options)
-                        }(o, e, n)
+                            o.supports && (t += "@supports (".concat(o.supports, ") {")), o.media && (t += "@media ".concat(o.media, " {"));
+                            var i = void 0 !== o.layer;
+                            i && (t += "@layer".concat(o.layer.length > 0 ? " ".concat(o.layer) : "", " {")), t += o.css, i && (t += "}"), o.media && (t += "}"), o.supports && (t += "}");
+                            var a = o.sourceMap;
+                            a && "undefined" != typeof btoa && (t += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a)))), " */")), n.styleTagTransform(t, e, n.options)
+                        }(n, e, o)
                     },
                     remove: function() {
                         ! function(e) {
                             if (null === e.parentNode) return !1;
                             e.parentNode.removeChild(e)
-                        }(o)
+                        }(n)
                     }
                 }
             }
         },
         113: e => {
-            e.exports = function(e, o) {
-                if (o.styleSheet) o.styleSheet.cssText = e;
+            e.exports = function(e, n) {
+                if (n.styleSheet) n.styleSheet.cssText = e;
                 else {
-                    for (; o.firstChild;) o.removeChild(o.firstChild);
-                    o.appendChild(document.createTextNode(e))
+                    for (; n.firstChild;) n.removeChild(n.firstChild);
+                    n.appendChild(document.createTextNode(e))
                 }
             }
         }
     }
 ]);
```

### Comparing `didi_notebook_extension-0.0.17/didi_notebook_extension/labextension/static/remoteEntry.8939b006cb56785ffe74.js` & `didi_notebook_extension-0.2.7/didi_notebook_extension/labextension/static/remoteEntry.669ff8394f95a035c486.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, o, i, a, u, l, d, s, f, p, c, h, v, b, g = {
-            212: (e, r, t) => {
+            798: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(958).then((() => () => t(958))),
                         "./extension": () => t.e(958).then((() => () => t(958))),
                         "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -43,19 +43,19 @@
         }), r
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
-        728: "9916fbef502e316a159a",
-        958: "bd36d1031c08063aa2e9"
+        728: "adf73d00115832453a58",
+        958: "eb0e437e53b6a86814b4"
     } [e] + ".js?v=" + {
-        728: "9916fbef502e316a159a",
-        958: "bd36d1031c08063aa2e9"
+        728: "adf73d00115832453a58",
+        958: "eb0e437e53b6a86814b4"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -106,15 +106,15 @@
                     var o = i[e] = i[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : a > u.from)) && (o[r] = {
                         get: () => y.e(958).then((() => () => y(958))),
                         from: a,
                         eager: !1
                     })
-                })("didi-notebook-extension", "0.0.17"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("didi-notebook-extension", "0.2.7"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -208,22 +208,22 @@
         return i(n, o) || s(l(e, t, o, n)), f(e[t][o])
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, f = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
         var i = y.I(r);
         return i && i.then ? i.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
     })(((e, r, t, n) => (a(e, t), d(r, 0, t, n)))), c = {}, h = {
+        215: () => p("default", "@jupyterlab/mainmenu", [1, 4, 1, 8]),
         256: () => p("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
-        291: () => p("default", "@jupyterlab/notebook", [1, 4, 2, 0]),
-        626: () => p("default", "@jupyterlab/application", [1, 4, 2, 0]),
-        670: () => p("default", "@jupyterlab/filebrowser", [1, 4, 2, 0]),
-        899: () => p("default", "@jupyterlab/docmanager", [1, 4, 2, 0]),
-        923: () => p("default", "@jupyterlab/apputils", [1, 4, 3, 0])
+        371: () => p("default", "@jupyterlab/application", [1, 4, 1, 8]),
+        440: () => p("default", "@jupyterlab/apputils", [1, 4, 2, 8]),
+        506: () => p("default", "@jupyterlab/notebook", [1, 4, 1, 8]),
+        943: () => p("default", "@jupyterlab/filebrowser", [1, 4, 1, 8])
     }, v = {
-        958: [256, 291, 626, 670, 899, 923]
+        958: [215, 256, 371, 440, 506, 943]
     }, b = {}, y.f.consumes = (e, r) => {
         y.o(v, e) && v[e].forEach((e => {
             if (y.o(c, e)) return r.push(c[e]);
             if (!b[e]) {
                 var t = r => {
                     c[e] = 0, y.m[e] = t => {
                         delete y.c[e], t.exports = r()
@@ -273,10 +273,10 @@
                     u && u(y)
                 }
                 for (r && r(t); l < i.length; l++) o = i[l], y.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkdidi_notebook_extension = self.webpackChunkdidi_notebook_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), y.nc = void 0;
-    var w = y(212);
+    var w = y(798);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["didi-notebook-extension"] = w
 })();
```

### Comparing `didi_notebook_extension-0.0.17/didi_notebook_extension/labextension/static/third-party-licenses.json` & `didi_notebook_extension-0.2.7/didi_notebook_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `didi_notebook_extension-0.0.17/src/api.ts` & `didi_notebook_extension-0.2.7/src/api.ts`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 if (
     location.hostname.indexOf('notebook-test.bigdata.xiaojukeji.com') !== -1
 ) {
     env = 'test';
 } else if (location.hostname.indexOf('didiglobal.com') !== -1) {
     env = 'global';
 }
-const ssoAppId = env !== 'global' ? '2101066' : '2824';
+const ssoAppId = env !== 'global' ? '280' : '2824';
 // 在你的扩展中
 export const checkLogin = async () => {
     console.log('----------didi-notebook-extensio checkLogin-----------');
 try {
     const response = await fetch(
         '/api/isLogin',
         // 'http://notebook-test.bigdata.xiaojukeji.com/api/isLogin',
```

### Comparing `didi_notebook_extension-0.0.17/style/base.css` & `didi_notebook_extension-0.2.7/style/base.css`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,14 @@
 .from-studio .jp-KernelName, 
 .from-studio .lm-DockPanel-tabBar,
 .from-studio .lm-TabBar 
 .hide-menu.from-studio .jp-NotebookPanel  > .jp-NotebookPanel-toolbar,
 .hide-menu.from-studio .lm-DockPanel  > .lm-DockPanel-tabBar{
     display: none !important;
 }
-.from-studio.hide-menu .jp-NotebookPanel, .from-studio.hide-menu .lm-DockPanel {
-    top: 0 !important;
-    border: none !important;
-}
 .from-studio .jp-Notebook-toolbarCellType .jp-Notebook-toolbarCellTypeDropdown option[value="raw"],
 .from-studio .jp-CommandToolbarButton .jp-ToolbarButtonComponent[data-command="docmanager:save"] {
     display: none !important;
 }
 .from-studio .lm-Menu-item[data-command="notebook:create-console"], 
 .from-studio .lm-Menu-item[data-command="inspector:open"],
 .from-studio .lm-Menu-item[data-command="logconsole:open"] {
```

### Comparing `didi_notebook_extension-0.0.17/ui-tests/README.md` & `didi_notebook_extension-0.2.7/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `didi_notebook_extension-0.0.17/ui-tests/tests/didi_extension.spec.ts` & `didi_notebook_extension-0.2.7/ui-tests/tests/didi_extension.spec.ts`

 * *Files identical despite different names*

### Comparing `didi_notebook_extension-0.0.17/.gitignore` & `didi_notebook_extension-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `didi_notebook_extension-0.0.17/LICENSE` & `didi_notebook_extension-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `didi_notebook_extension-0.0.17/README.md` & `didi_notebook_extension-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `didi_notebook_extension-0.0.17/pyproject.toml` & `didi_notebook_extension-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `didi_notebook_extension-0.0.17/PKG-INFO` & `didi_notebook_extension-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: didi_notebook_extension
-Version: 0.0.17
+Version: 0.2.7
 Dynamic: Keywords
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/yobi-maggie/didi-notebook-extension
 Project-URL: Bug Tracker, https://github.com/yobi-maggie/didi-notebook-extension/issues
 Project-URL: Repository, https://github.com/yobi-maggie/didi-notebook-extension.git
 Author-email: dongmeiqi <dongmeiqi@didiglobal.com>
 License: BSD 3-Clause License
```

