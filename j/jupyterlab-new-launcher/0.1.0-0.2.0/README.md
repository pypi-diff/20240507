# Comparing `tmp/jupyterlab_new_launcher-0.1.0.tar.gz` & `tmp/jupyterlab_new_launcher-0.2.0.tar.gz`

## Comparing `jupyterlab_new_launcher-0.1.0.tar` & `jupyterlab_new_launcher-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,60 @@
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/.copier-answers.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/babel.config.js
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/jest.config.js
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/junit.xml
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/setup.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/tsconfig.test.json
--rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/yarn.lock
--rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/docs/images/dialog.png
--rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/docs/images/launcher.png
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/_version.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/package.json
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
--rw-r--r--   0        0        0    19391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/static/21.09cd58745a7785ee864d.js
--rw-r--r--   0        0        0     8382 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/static/728.379a3ceb37c59a35119c.js
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/static/remoteEntry.3bf9447fc2344a3f202a.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/schema/plugin.json
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/src/commands.ts
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/src/database.ts
--rw-r--r--   0        0        0     8874 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/src/dialogs.tsx
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/src/icons.ts
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/src/index.ts
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/src/item.ts
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/src/launcher.tsx
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/src/svg.d.ts
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/src/types.ts
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/src/__tests__/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/src/components/card.tsx
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/src/components/section.tsx
--rw-r--r--   0        0        0    11163 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/src/components/table.tsx
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/style/index.js
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/style/icons/md/LICENSE
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/style/icons/md/file.svg
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/style/icons/md/star.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/LICENSE
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/README.md
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/.copier-answers.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/babel.config.js
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jest.config.js
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/junit.xml
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/setup.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/tsconfig.test.json
+-rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/yarn.lock
+-rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/docs/images/dialog.png
+-rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/docs/images/launcher.png
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/_version.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/package.json
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
+-rw-r--r--   0        0        0    21040 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/21.b553ea2f251b3240c2ae.js
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/728.ea49658c85c6542563e2.js
+-rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/remoteEntry.097f22d9f5ab72ff351d.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/schema/plugin.json
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/commands.ts
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/database.ts
+-rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/dialogs.tsx
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/icons.ts
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/index.ts
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/item.ts
+-rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/launcher.tsx
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/svg.d.ts
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/types.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/__tests__/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/components/card.tsx
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/components/section.tsx
+-rw-r--r--   0        0        0    11435 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/components/table.tsx
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/style/index.js
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/style/icons/md/LICENSE
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/style/icons/md/file.svg
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/style/icons/md/star.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0    26996 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
+-rw-r--r--   0        0        0    27431 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
+-rw-r--r--   0        0        0    33351 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/README.md
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/PKG-INFO
```

### Comparing `jupyterlab_new_launcher-0.1.0/.copier-answers.yml` & `jupyterlab_new_launcher-0.2.0/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/RELEASE.md` & `jupyterlab_new_launcher-0.2.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/jest.config.js` & `jupyterlab_new_launcher-0.2.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/package.json` & `jupyterlab_new_launcher-0.2.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.0'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_new_launcher-0.1.0/tsconfig.json` & `jupyterlab_new_launcher-0.2.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/yarn.lock` & `jupyterlab_new_launcher-0.2.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/docs/images/dialog.png` & `jupyterlab_new_launcher-0.2.0/docs/images/dialog.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/docs/images/launcher.png` & `jupyterlab_new_launcher-0.2.0/docs/images/launcher.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/__init__.py` & `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/package.json` & `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.097f22d9f5ab72ff351d.js'}}",*

 * * "'version'": "'0.2.0'"}*

```diff
@@ -108,15 +108,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/nebari-dev/jupyterlab-new-launcher",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.3bf9447fc2344a3f202a.js",
+            "load": "static/remoteEntry.097f22d9f5ab72ff351d.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/launcher-extension",
             "@jupyterlab/apputils-extension:sessionDialogs"
         ],
         "extension": true,
@@ -200,9 +200,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig` & `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.0'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/static/21.09cd58745a7785ee864d.js` & `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/21.b553ea2f251b3240c2ae.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,92 +1,92 @@
 "use strict";
 (self.webpackChunkjupyterlab_new_launcher = self.webpackChunkjupyterlab_new_launcher || []).push([
     [21], {
-        21: (e, t, a) => {
-            a.r(t), a.d(t, {
-                default: () => R
+        21: (e, t, s) => {
+            s.r(t), s.d(t, {
+                default: () => M
             });
-            var s = a(465),
-                n = a(638),
-                r = a(221),
-                o = a(595),
-                l = a(618),
-                i = a(714),
-                c = a(664),
-                d = a(53),
-                m = a(345);
+            var a = s(626),
+                n = s(923),
+                r = s(670),
+                o = s(260),
+                l = s(825),
+                i = s(265),
+                c = s(527),
+                d = s(53),
+                m = s(345);
             const u = new c.LabIcon({
                     name: "jupyterlab-new-launcher:star",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">\n  <path class="jp-icon3 jp-star-filled" fill="rgb(97,97,97)" d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z" />\n  <path class="jp-icon3 jp-star-border" fill="rgb(97,97,97)" d="M22 9.24l-7.19-.62L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21 12 17.27 18.18 21l-1.63-7.03L22 9.24zM12 15.4l-3.76 2.27 1-4.28-3.32-2.88 4.38-.38L12 6.1l1.71 4.04 4.38.38-3.32 2.88 1 4.28L12 15.4z" />\n</svg>\n'
                 }),
                 h = new c.LabIcon({
                     name: "jupyterlab-new-launcher:file",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">\n  <path class="jp-icon3" fill="rgb(97,97,97)" d="M13.81 22H6C4.89 22 4 21.11 4 20V4C4 2.9 4.89 2 6 2H14L20 8V13.09C19.67 13.04 19.34 13 19 13S18.33 13.04 18 13.09V9H13V4H6V20H13.09C13.21 20.72 13.46 21.39 13.81 22M23 18H20V15H18V18H15V20H18V23H20V20H23V18Z" />\n</svg>'
                 });
-            var p = a(602);
+            var p = s(602);
             class g {
                 constructor(e) {
                     var t;
                     this._options = e, this._refreshLastUsed = new p.Signal(this), this._refreshClock = null, this._lastUsed = null;
                     const {
-                        item: a,
-                        commands: s,
+                        item: s,
+                        commands: a,
                         lastUsedDatabase: n,
                         favoritesDatabase: r,
                         cwd: o
                     } = e, l = {
-                        ...a.args,
+                        ...s.args,
                         cwd: o
                     };
-                    this.command = a.command, this.args = l, this.category = a.category, this.rank = a.rank, this.kernelIconUrl = a.kernelIconUrl, this.metadata = a.metadata, this.iconClass = s.iconClass(a.command, l), this.icon = s.icon(a.command, l), this.caption = s.caption(a.command, l), this.label = s.label(a.command, l), this.lastUsed = n.get(a), this.starred = null !== (t = r.get(a)) && void 0 !== t && t
+                    this.command = s.command, this.args = l, this.category = s.category, this.rank = s.rank, this.kernelIconUrl = s.kernelIconUrl, this.metadata = s.metadata, this.iconClass = a.iconClass(s.command, l), this.icon = a.icon(s.command, l), this.caption = a.caption(s.command, l), this.label = a.label(s.command, l), this.lastUsed = n.get(s), this.starred = null !== (t = r.get(s)) && void 0 !== t && t
                 }
                 get lastUsed() {
                     return this._lastUsed
                 }
                 set lastUsed(e) {
                     this._lastUsed = e, this._setRefreshClock()
                 }
                 get refreshLastUsed() {
                     return this._refreshLastUsed
                 }
                 async execute() {
                     const {
                         item: e,
                         commands: t,
-                        lastUsedDatabase: a
+                        lastUsedDatabase: s
                     } = this._options;
-                    await t.execute(e.command, this.args), await a.recordAsUsedNow(e), this.lastUsed = a.get(e), this._refreshLastUsed.emit()
+                    await t.execute(e.command, this.args), await s.recordAsUsedNow(e), this.lastUsed = s.get(e), this._refreshLastUsed.emit()
                 }
                 async markAsUsed() {
                     const {
                         item: e,
                         lastUsedDatabase: t
                     } = this._options;
                     await t.recordAsUsedNow(e), this.lastUsed = t.get(e), this._refreshLastUsed.emit()
                 }
                 toggleStar() {
                     const {
                         item: e,
                         favoritesDatabase: t
-                    } = this._options, a = !t.get(e);
-                    return this.starred = a, t.set(e, a)
+                    } = this._options, s = !t.get(e);
+                    return this.starred = s, t.set(e, s)
                 }
                 _setRefreshClock() {
                     const e = this._lastUsed;
                     if (null !== this._refreshClock && (window.clearTimeout(this._refreshClock), this._refreshClock = null), !e) return;
                     const t = Date.now() - e.getTime(),
-                        a = t < 6e4 ? 1e4 : t < 36e5 ? 6e4 : 36e5;
+                        s = t < 6e4 ? 1e4 : t < 36e5 ? 6e4 : 36e5;
                     this._refreshClock = window.setTimeout((() => {
                         this._refreshLastUsed.emit(), this._setRefreshClock()
-                    }), a)
+                    }), s)
                 }
             }
-            var v = a(597),
-                _ = a(262);
-            const f = "jupyterlab-new-launcher:plugin";
+            var f = s(702),
+                _ = s(262);
+            const v = "jupyterlab-new-launcher:plugin";
             var b;
             ! function(e) {
                 e.create = "launcher:create", e.moveColumn = "new-launcher:table-move-column", e.toggleColumn = "new-launcher:table-toggle-column"
             }(b || (b = {}));
             const w = new _.Token("jupyterlab-new-launcher:ILauncherDatabase", "Databases for new launcher."),
                 C = "jp-starIconButton",
                 y = "jp-TableKernelItem";
@@ -106,199 +106,200 @@
                         return "Base?";
                     case "conda_is_currently_running":
                         return "Running?"
                 }
                 return e[0].toUpperCase() + e.substring(1)
             }
 
-            function D(e) {
-                var t, a, s, n;
+            function L(e) {
+                var t, s, a, n;
                 const {
                     trans: r
                 } = e;
                 let o, l;
-                if (e.showSearchBox) {
-                    const [e, t] = m.useState("");
-                    o = e, l = t
-                } else o = e.query;
-                const [, i] = m.useReducer((e => e + 1), 0), d = new Set;
-                for (const a of e.items) {
-                    const e = null === (t = a.metadata) || void 0 === t ? void 0 : t.kernel;
+                const [i, d] = m.useState("");
+                e.showSearchBox ? (o = i, l = d) : o = e.query;
+                const [, h] = m.useReducer((e => e + 1), 0), p = new Set;
+                for (const s of e.items) {
+                    const e = null === (t = s.metadata) || void 0 === t ? void 0 : t.kernel;
                     if (e)
-                        for (const t of Object.keys(e)) d.add(t)
+                        for (const t of Object.keys(e)) p.add(t)
                 }
-                const h = [...d].map((e => ({
-                        id: e,
-                        label: k(e),
-                        renderCell: t => {
-                            var a;
-                            const s = null === (a = t.metadata) || void 0 === a ? void 0 : a.kernel;
-                            if (!s) return "-";
-                            const n = s[e];
-                            return "string" == typeof n ? n : JSON.stringify(n)
-                        },
-                        sort: (t, a) => {
-                            var s, n;
-                            const r = null === (s = t.metadata) || void 0 === s ? void 0 : s.kernel,
-                                o = null === (n = a.metadata) || void 0 === n ? void 0 : n.kernel,
-                                l = r ? r[e] : void 0,
-                                i = o ? o[e] : void 0;
-                            return l === i ? 0 : l ? i ? "string" == typeof l && "string" == typeof i ? l.localeCompare(i) : l > i ? 1 : -1 : -1 : 1
-                        }
-                    }))),
-                    p = [{
-                        id: "icon",
-                        label: r.__("Icon"),
-                        renderCell: t => m.createElement("div", {
+                const g = [...p].map((e => ({
+                    id: e,
+                    label: k(e),
+                    renderCell: t => {
+                        var s;
+                        const a = null === (s = t.metadata) || void 0 === s ? void 0 : s.kernel;
+                        if (!a) return "-";
+                        const n = a[e];
+                        return "string" == typeof n ? n : JSON.stringify(n)
+                    },
+                    sort: (t, s) => {
+                        var a, n;
+                        const r = null === (a = t.metadata) || void 0 === a ? void 0 : a.kernel,
+                            o = null === (n = s.metadata) || void 0 === n ? void 0 : n.kernel,
+                            l = r ? r[e] : void 0,
+                            i = o ? o[e] : void 0;
+                        return l === i ? 0 : l ? i ? "string" == typeof l && "string" == typeof i ? l.localeCompare(i) : l > i ? 1 : -1 : -1 : 1
+                    }
+                })));
+                e.showWidgetType && g.push({
+                    id: "widget-type",
+                    label: r.__("Type"),
+                    renderCell: e => e.command.split(":")[0],
+                    sort: (e, t) => e.command.localeCompare(t.command)
+                });
+                const _ = [{
+                        id: "kernel",
+                        label: r.__("Kernel"),
+                        renderCell: t => m.createElement(m.Fragment, null, m.createElement("span", {
                             className: "jp-LauncherCard-icon",
                             onClick: () => e.onClick(t)
                         }, t.kernelIconUrl ? m.createElement("img", {
                             src: t.kernelIconUrl,
                             className: "jp-Launcher-kernelIcon",
                             alt: t.label
                         }) : m.createElement("div", {
                             className: "jp-LauncherCard-noKernelIcon"
-                        }, t.label[0].toUpperCase())),
-                        sort: (e, t) => e.command.localeCompare(t.command)
-                    }, {
-                        id: "kernel",
-                        label: r.__("Kernel"),
-                        renderCell: t => m.createElement("span", {
+                        }, t.label[0].toUpperCase())), m.createElement("span", {
                             className: y,
-                            onClick: a => {
-                                e.onClick(t), a.stopPropagation()
+                            onClick: s => {
+                                e.onClick(t), s.stopPropagation()
                             },
                             onKeyDown: e => {
                                 "Enter" === e.key && t.execute()
                             },
                             tabIndex: 0
-                        }, t.label),
+                        }, t.label)),
                         sort: (e, t) => e.label.localeCompare(t.label)
-                    }, ...h, {
+                    }, ...g, {
                         id: "last-used",
                         label: r.__("Last Used"),
                         renderCell: e => m.createElement(c.UseSignal, {
                             signal: e.refreshLastUsed
                         }, (() => e.lastUsed ? m.createElement("span", {
-                            title: v.Time.format(e.lastUsed)
-                        }, v.Time.formatHuman(e.lastUsed)) : r.__("Never"))),
+                            title: f.Time.format(e.lastUsed)
+                        }, f.Time.formatHuman(e.lastUsed)) : r.__("Never"))),
                         sort: (e, t) => e.lastUsed === t.lastUsed ? 0 : e.lastUsed ? t.lastUsed && e.lastUsed > t.lastUsed ? 1 : -1 : 1
                     }, {
                         id: "star",
                         label: "",
                         renderCell: e => {
                             const t = e.starred,
-                                a = t ? r.__("Click to add this kernel to favourites") : r.__("Click to remove the kernel from favourites");
+                                s = t ? r.__("Click to add this kernel to favourites") : r.__("Click to remove the kernel from favourites");
                             return m.createElement("button", {
                                 className: t ? `${C} jp-mod-starred` : C,
-                                title: a,
+                                title: s,
                                 onClick: t => {
-                                    e.toggleStar(), i(), t.stopPropagation()
+                                    e.toggleStar(), h(), t.stopPropagation()
                                 }
                             }, m.createElement(u.react, {
                                 className: "jp-starIcon"
                             }))
                         },
                         sort: (e, t) => Number(e.starred) - Number(t.starred)
                     }],
-                    g = null !== (a = e.hideColumns) && void 0 !== a ? a : [],
-                    _ = p.filter((e => !g.includes(e.id))),
-                    [f, w] = m.useState(null !== (s = e.settings.composite.hiddenColumns) && void 0 !== s ? s : {}),
-                    D = _.map((e => e.id)),
-                    [L, I] = m.useState(null !== (n = e.settings.composite.columnOrder) && void 0 !== n ? n : D),
-                    U = c.Table,
-                    E = () => {
-                        var t, a;
-                        const s = null !== (t = e.settings.composite.hiddenColumns) && void 0 !== t ? t : {};
-                        f !== s && w(s);
-                        const n = null !== (a = e.settings.composite.columnOrder) && void 0 !== a ? a : D;
-                        L !== n && I(n)
+                    v = null !== (s = e.hideColumns) && void 0 !== s ? s : [],
+                    w = _.filter((e => !v.includes(e.id))),
+                    [L, D] = m.useState(null !== (a = e.settings.composite.hiddenColumns) && void 0 !== a ? a : {}),
+                    S = w.map((e => e.id)),
+                    [E, I] = m.useState(null !== (n = e.settings.composite.columnOrder) && void 0 !== n ? n : S),
+                    N = c.Table,
+                    U = () => {
+                        var t, s;
+                        const a = null !== (t = e.settings.composite.hiddenColumns) && void 0 !== t ? t : {};
+                        L !== a && D(a);
+                        const n = null !== (s = e.settings.composite.columnOrder) && void 0 !== s ? s : S;
+                        E !== n && I(n)
                     };
-                return m.useEffect((() => (e.settings.changed.connect(E), () => {
-                    e.settings.changed.disconnect(E)
+                return m.useEffect((() => (e.settings.changed.connect(U), () => {
+                    e.settings.changed.disconnect(U)
                 }))), m.createElement("div", {
                     className: "jp-NewLauncher-table"
                 }, e.showSearchBox ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
                 }, m.createElement(c.FilterBox, {
-                    placeholder: r.__("Filter"),
+                    placeholder: r.__("Filter kernels"),
                     updateFilter: (e, t) => {
                         l(null != t ? t : "")
                     },
                     initialQuery: "",
                     useFuzzyFilter: !1
                 })) : null, m.createElement("div", {
                     className: "jp-NewLauncher-table-scroller",
                     onContextMenu: t => {
-                        var a;
+                        var s;
                         t.preventDefault();
-                        const s = new c.MenuSvg({
+                        const a = new c.MenuSvg({
                                 commands: e.commands
                             }),
                             n = new c.MenuSvg({
                                 commands: e.commands
                             });
-                        for (const e of _) n.addItem({
+                        for (const e of w) n.addItem({
                             command: b.toggleColumn,
                             args: {
                                 id: e.id,
                                 label: e.label
                             }
                         });
-                        n.title.label = r.__("Visible Columns"), s.addItem({
+                        n.title.label = r.__("Visible Columns"), a.addItem({
                             type: "submenu",
                             submenu: n
                         });
-                        const o = null === (a = t.target.closest("th[data-id]")) || void 0 === a ? void 0 : a.dataset.id;
-                        o && (s.addItem({
+                        const o = null === (s = t.target.closest("th[data-id]")) || void 0 === s ? void 0 : s.dataset.id;
+                        o && (a.addItem({
                             command: b.moveColumn,
                             args: {
                                 direction: "left",
-                                order: L,
+                                order: E,
                                 id: o
                             }
-                        }), s.addItem({
+                        }), a.addItem({
                             command: b.moveColumn,
                             args: {
                                 direction: "right",
-                                order: L,
+                                order: E,
                                 id: o
                             }
-                        })), s.open(t.clientX, t.clientY)
+                        })), a.open(t.clientX, t.clientY)
                     }
-                }, m.createElement(U, {
+                }, m.createElement(N, {
                     rows: e.items.filter((e => -1 !== e.label.toLowerCase().indexOf(o.toLowerCase()))).map((e => ({
                         data: e,
                         key: e.command + JSON.stringify(e.args)
                     }))),
                     blankIndicator: () => m.createElement("div", null, r.__("No entries")),
                     sortKey: "kernel",
                     onRowClick: e => {
                         const t = e.target,
-                            a = t.closest("tr");
-                        if (!a) return;
-                        const s = t.closest("td"),
-                            n = null == s ? void 0 : s.querySelector(`.${C}`);
+                            s = t.closest("tr");
+                        if (!s) return;
+                        const a = t.closest("td"),
+                            n = null == a ? void 0 : a.querySelector(`.${C}`);
                         if (n) return n.click();
-                        a.querySelector(`.${y}`).click()
+                        s.querySelector(`.${y}`).click()
                     },
-                    columns: _.filter((e => !f[e.id])).map((e => {
+                    columns: w.filter((e => "hidden" !== L[e.id])).map((e => {
                         var t;
                         return {
                             ...e,
-                            rank: null !== (t = L.indexOf(e.id)) && void 0 !== t ? t : 10
+                            rank: null !== (t = E.indexOf(e.id)) && void 0 !== t ? t : 10
                         }
                     })).sort(((e, t) => e.rank - t.rank))
                 })))
             }
 
-            function L(e) {
-                const [t, a] = m.useState(e.open);
+            function D(e) {
+                const [t, s] = m.useState(e.open);
                 return m.createElement("details", {
-                    onToggle: e => a(e.currentTarget.open),
+                    onToggle: t => {
+                        s(t.currentTarget.open), e.onToggled && e.onToggled(t.currentTarget.open)
+                    },
                     className: (0, c.classes)(e.className, "jp-CollapsibleSection"),
                     open: t
                 }, m.createElement("summary", null, m.createElement("div", {
                     className: "jp-CollapsibleSection-CollapserIconWrapper",
                     "aria-hidden": "true"
                 }, m.createElement(c.caretRightIcon.react, {
                     className: "jp-CollapsibleSection-CollapserIcon"
@@ -308,15 +309,15 @@
                 }), m.createElement("h3", {
                     className: "jp-CollapsibleSection-Title"
                 }, e.title)), m.createElement("div", {
                     className: "jp-Launcher-CardGroup jp-Launcher-cardContainer"
                 }, e.children))
             }
 
-            function I(e) {
+            function S(e) {
                 const {
                     item: t
                 } = e;
                 return m.createElement("div", {
                     onClick: () => t.execute(),
                     className: "jp-Launcher-TypeCard jp-LauncherCard",
                     title: t.caption,
@@ -327,100 +328,133 @@
                     icon: t.icon,
                     iconClass: (0, c.classes)(t.iconClass, "jp-Icon-cover")
                 })), m.createElement("div", {
                     className: "jp-LauncherCard-label"
                 }, m.createElement("p", null, t.label)))
             }
 
-            function U(e) {
+            function E(e) {
                 var t;
                 const {
-                    trans: a,
-                    cwd: s,
+                    trans: s,
+                    cwd: a,
                     typeItems: n,
-                    otherItems: r
-                } = e, [o, l] = m.useState(""), i = new Set;
-                for (const a of e.notebookItems) {
-                    const e = null === (t = a.metadata) || void 0 === t ? void 0 : t.kernel;
+                    otherItems: r,
+                    favouritesChanged: o
+                } = e, [l, i] = m.useState(""), [, d] = m.useReducer((e => e + 1), 0), [p, g] = m.useState(e.settings.composite.starredSection), [f, _] = m.useState(e.settings.composite.searchAllSections), v = () => {
+                    const t = e.settings.composite.starredSection;
+                    p !== t && g(t);
+                    const s = e.settings.composite.searchAllSections;
+                    f !== s && _(s)
+                };
+                if (m.useEffect((() => (e.settings.changed.connect(v), () => {
+                        e.settings.changed.disconnect(v)
+                    }))), o) {
+                    const e = () => {
+                        p && d()
+                    };
+                    m.useEffect((() => (o.connect(e), () => {
+                        o.disconnect(e)
+                    })))
+                }
+                const b = new Set;
+                for (const s of e.notebookItems) {
+                    const e = null === (t = s.metadata) || void 0 === t ? void 0 : t.kernel;
                     if (e)
-                        for (const t of Object.keys(e)) i.add(t)
+                        for (const t of Object.keys(e)) b.add(t)
                 }
+                const w = [...e.notebookItems, ...e.consoleItems].filter((e => e.starred)),
+                    C = e.settings.composite.collapsedSections;
                 return m.createElement("div", {
                     className: "jp-LauncherBody"
                 }, m.createElement("div", {
                     className: "jp-NewLauncher-TopBar"
                 }, m.createElement("div", {
                     className: "jp-Launcher-cwd"
-                }, m.createElement("h3", null, a.__("Current folder:"), " ", m.createElement("code", null, s || "/"))), m.createElement("div", {
+                }, m.createElement("h3", null, s.__("Current folder:"), " ", m.createElement("code", null, a || "/"))), m.createElement("div", {
                     className: "jp-NewLauncher-OtherItems"
-                }, r.map((e => m.createElement(I, {
+                }, r.map((e => m.createElement(S, {
                     item: e,
-                    trans: a
-                }))))), m.createElement("div", {
+                    trans: s
+                }))))), f ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
                 }, m.createElement(c.FilterBox, {
-                    placeholder: a.__("Filter"),
+                    placeholder: s.__("Filter"),
                     updateFilter: (e, t) => {
-                        l(null != t ? t : "")
+                        i(null != t ? t : "")
                     },
                     initialQuery: "",
                     useFuzzyFilter: !1
-                })), m.createElement(L, {
+                })) : null, m.createElement(D, {
                     className: "jp-Launcher-openByType",
-                    title: a.__("Create Empty"),
+                    title: s.__("Create Empty"),
                     icon: h,
-                    open: !0
-                }, n.filter((e => !o || -1 !== e.label.toLowerCase().indexOf(o.toLowerCase()))).map((e => m.createElement(I, {
+                    open: "collapsed" !== C["create-empty"]
+                }, n.filter((e => !l || -1 !== e.label.toLowerCase().indexOf(l.toLowerCase()))).map((e => m.createElement(S, {
                     item: e,
-                    trans: a
-                })))), m.createElement(L, {
+                    trans: s
+                })))), p ? m.createElement(D, {
                     className: "jp-Launcher-openByKernel",
-                    title: a.__("Launch Notebook"),
+                    title: s.__("Starred"),
+                    icon: u,
+                    open: "collapsed" !== C.starred
+                }, w.length > 0 ? m.createElement(L, {
+                    items: w,
+                    commands: e.commands,
+                    showSearchBox: !f,
+                    showWidgetType: !0,
+                    query: l,
+                    settings: e.settings,
+                    trans: s,
+                    onClick: e => e.execute()
+                }) : "No starred items") : null, m.createElement(D, {
+                    className: "jp-Launcher-openByKernel jp-Launcher-launchNotebook",
+                    title: s.__("Launch Notebook"),
                     icon: c.notebookIcon,
-                    open: !0
-                }, m.createElement(D, {
+                    open: "collapsed" !== C["launch-notebook"]
+                }, m.createElement(L, {
                     items: e.notebookItems,
                     commands: e.commands,
-                    showSearchBox: !1,
-                    query: o,
+                    showSearchBox: !f,
+                    query: l,
                     settings: e.settings,
-                    trans: a,
+                    trans: s,
                     onClick: e => e.execute()
-                })), m.createElement(L, {
-                    className: "jp-Launcher-openByKernel",
-                    title: a.__("Launch Console"),
+                })), m.createElement(D, {
+                    className: "jp-Launcher-openByKernel jp-Launcher-launchConsole",
+                    title: s.__("Launch Console"),
                     icon: c.consoleIcon,
-                    open: !1
-                }, m.createElement(D, {
+                    open: "collapsed" !== C["launch-console"]
+                }, m.createElement(L, {
                     items: e.consoleItems,
                     commands: e.commands,
-                    showSearchBox: !1,
-                    query: o,
+                    showSearchBox: !f,
+                    query: l,
                     settings: e.settings,
-                    trans: a,
+                    trans: s,
                     onClick: e => e.execute()
                 })))
             }
-            class E extends o.Launcher {
+            class I extends o.Launcher {
                 constructor(e) {
                     super(e), this.renderCommand = e => new g({
                         item: e,
                         cwd: this.cwd,
                         commands: this.commands,
                         lastUsedDatabase: this._lastUsedDatabase,
                         favoritesDatabase: this._favoritesDatabase
                     }), this.renderKernelCommand = e => this.renderCommand(e), this.commands = e.commands, this.trans = this.translator.load("jupyterlab-new-launcher"), this._lastUsedDatabase = e.lastUsedDatabase, this._favoritesDatabase = e.favoritesDatabase, this._settings = e.settings
                 }
                 render() {
                     if (!this.model) return null;
                     const e = this.trans,
                         t = [...this.model.items()],
-                        a = e.__("Notebook"),
-                        s = e.__("Console"),
-                        n = [a, s],
+                        s = e.__("Notebook"),
+                        a = e.__("Console"),
+                        n = [s, a],
                         r = ["inspector:open"],
                         o = t.filter((e => r.includes(e.command))).map(this.renderCommand),
                         l = t.filter((e => !(e.category && n.includes(e.category) || r.includes(e.command)))),
                         i = {
                             "terminal:create-new": 3,
                             "fileeditor:create-new": 6,
                             "fileeditor:create-new-markdown-file": 5
@@ -429,54 +463,55 @@
                     const c = [{
                             command: "notebook:create-new",
                             rank: 1
                         }, {
                             command: "console:create",
                             rank: 4
                         }, ...l].sort(((e, t) => {
-                            var a, s;
-                            return (null !== (a = null == e ? void 0 : e.rank) && void 0 !== a ? a : 0) - (null !== (s = null == t ? void 0 : t.rank) && void 0 !== s ? s : 0)
+                            var s, a;
+                            return (null !== (s = null == e ? void 0 : e.rank) && void 0 !== s ? s : 0) - (null !== (a = null == t ? void 0 : t.rank) && void 0 !== a ? a : 0)
                         })),
-                        d = t.filter((e => e.category && e.category === a)).map(this.renderKernelCommand),
-                        u = t.filter((e => e.category && e.category === s)).map(this.renderKernelCommand),
+                        d = t.filter((e => e.category && e.category === s)).map(this.renderKernelCommand),
+                        u = t.filter((e => e.category && e.category === a)).map(this.renderKernelCommand),
                         h = c.map(this.renderCommand);
-                    return m.createElement(U, {
+                    return m.createElement(E, {
                         trans: this.trans,
                         cwd: this.cwd,
                         commands: this.commands,
                         typeItems: h,
                         notebookItems: d,
                         consoleItems: u,
                         otherItems: o,
-                        settings: this._settings
+                        settings: this._settings,
+                        favouritesChanged: this._favoritesDatabase.changed
                     })
                 }
             }
-            class S extends n.SessionContextDialogs {
+            class N extends n.SessionContextDialogs {
                 constructor(e) {
                     var t;
                     super(e), this.options = e;
-                    const a = null !== (t = e.translator) && void 0 !== t ? t : i.nullTranslator;
-                    this.trans = a.load("jupyterlab")
+                    const s = null !== (t = e.translator) && void 0 !== t ? t : i.nullTranslator;
+                    this.trans = s.load("jupyterlab")
                 }
                 async selectKernel(e) {
                     const t = this.trans;
                     if (e.isDisposed) return Promise.resolve();
-                    let a = t.__("Cancel");
-                    e.hasNoKernel && (a = e.kernelDisplayName);
-                    const s = [n.Dialog.cancelButton({
-                            label: a
+                    let s = t.__("Cancel");
+                    e.hasNoKernel && (s = e.kernelDisplayName);
+                    const a = [n.Dialog.cancelButton({
+                            label: s
                         }), n.Dialog.okButton({
                             label: t.__("Select"),
                             ariaLabel: t.__("Select Kernel"),
                             className: "jp-KernelSelector-SelectButton"
                         })],
                         r = e.kernelPreference.autoStartDefault,
                         o = "boolean" == typeof r,
-                        l = await this.options.settingRegistry.load(f),
+                        l = await this.options.settingRegistry.load(v),
                         i = new n.Dialog({
                             title: t.__("Select Kernel"),
                             body: new j({
                                 data: {
                                     specs: e.specsManager.specs,
                                     sessions: e.sessionManager.running(),
                                     preference: e.kernelPreference
@@ -486,15 +521,15 @@
                                 lastUsedDatabase: this.options.database.lastUsed,
                                 settings: l,
                                 trans: t,
                                 acceptDialog: () => {
                                     i.resolve(1)
                                 }
                             }),
-                            buttons: s,
+                            buttons: a,
                             checkbox: o ? {
                                 label: t.__("Always start the preferred kernel"),
                                 caption: t.__("Remember my choice and always start the preferred kernel"),
                                 checked: r
                             } : null
                         });
                     i.node.classList.add("jp-KernelSelector-Dialog");
@@ -505,63 +540,72 @@
                         autoStartDefault: c.isChecked
                     });
                     const d = c.value;
                     if (null === d && !e.hasNoKernel) return e.shutdown();
                     d && await e.changeKernel(d)
                 }
             }
-            const N = {
+            const U = {
                 id: "jupyterlab-new-launcher:dialogs",
                 description: "Session dialogs for redesigned JupyterLab launcher",
                 provides: n.ISessionContextDialogs,
                 autoStart: !0,
                 requires: [i.ITranslator, w, l.ISettingRegistry],
-                activate: (e, t, a, s) => new S({
+                activate: (e, t, s, a) => new N({
                     translator: t,
-                    database: a,
+                    database: s,
                     commands: e.commands,
-                    settingRegistry: s
+                    settingRegistry: a
                 })
             };
             class j extends n.ReactWidget {
                 constructor(e) {
                     super(), this.options = e, this.renderKernelCommand = e => new g({
                         item: e,
                         cwd: "",
                         commands: this.commands,
                         lastUsedDatabase: this._lastUsedDatabase,
                         favoritesDatabase: this._favoritesDatabase
                     }), this._selection = null, this.commands = e.commands, this._lastUsedDatabase = e.lastUsedDatabase, this._favoritesDatabase = e.favoritesDatabase, this._settings = e.settings, this.trans = e.trans
                 }
+                onBeforeAttach(e) {
+                    super.onBeforeAttach(e), this.node.style.minWidth = "", this.node.style.minHeight = ""
+                }
+                onAfterAttach(e) {
+                    super.onAfterAttach(e), requestAnimationFrame((() => {
+                        const e = this.node.getBoundingClientRect();
+                        this.node.style.minWidth = e.width + "px", this.node.style.minHeight = e.height + "px"
+                    }))
+                }
                 render() {
                     var e;
                     const t = [],
-                        a = this.options.data.specs.kernelspecs;
-                    for (const e of Object.values(a)) {
+                        s = this.options.data.specs.kernelspecs;
+                    for (const e of Object.values(s)) {
                         if (!e) continue;
-                        const a = e.resources["logo-svg"] || e.resources["logo-64x64"];
+                        const s = e.resources["logo-svg"] || e.resources["logo-64x64"];
                         t.push({
                             command: "notebook:create-new",
                             args: {
                                 isLauncher: !0,
                                 kernelName: e.name
                             },
-                            kernelIconUrl: a,
+                            kernelIconUrl: s,
                             metadata: {
                                 kernel: _.JSONExt.deepCopy(e.metadata || {})
                             }
                         })
                     }
-                    const s = [];
+                    const a = [];
                     for (const t of this.options.data.sessions) {
                         const n = t.kernel;
                         if (!n) continue;
-                        const r = a[n.name],
+                        const r = s[n.name],
                             o = r.resources["logo-svg"] || r.resources["logo-64x64"];
-                        s.push({
+                        a.push({
                             command: "notebook:create-new",
                             args: {
                                 isLauncher: !0,
                                 kernelName: r.name
                             },
                             kernelIconUrl: o,
                             metadata: {
@@ -571,30 +615,30 @@
                                     "used by": t.name
                                 },
                                 model: n
                             }
                         })
                     }
                     const n = t.map(this.renderKernelCommand),
-                        r = s.map(this.renderKernelCommand);
+                        r = a.map(this.renderKernelCommand);
                     return m.createElement(m.Fragment, null, m.createElement("h3", {
                         className: "jp-KernelSelector-Section"
-                    }, this.trans.__("Start a new kernel")), m.createElement(D, {
+                    }, this.trans.__("Start a new kernel")), m.createElement(L, {
                         trans: this.trans,
                         commands: this.commands,
                         items: n,
                         settings: this._settings,
                         query: "",
                         showSearchBox: !0,
                         onClick: e => {
                             this._selection = e, this.options.acceptDialog()
                         }
                     }), r.length > 0 ? m.createElement(m.Fragment, null, m.createElement("h3", {
                         className: "jp-KernelSelector-Section"
-                    }, this.trans.__("Connect to a running kernel")), m.createElement(D, {
+                    }, this.trans.__("Connect to a running kernel")), m.createElement(L, {
                         trans: this.trans,
                         commands: this.commands,
                         items: r,
                         settings: this._settings,
                         query: "",
                         showSearchBox: !1,
                         onClick: e => {
@@ -606,30 +650,30 @@
                 getValue() {
                     var e;
                     return this._selection ? (null === (e = this._selection.metadata) || void 0 === e ? void 0 : e.model) ? this._selection.metadata.model : {
                         name: this._selection.args.kernelName
                     } : null
                 }
             }
-            var x = a(750);
+            var x = s(101);
             class B {
                 constructor(e) {
                     this._updateDB = async () => {
                         const e = await this._fetch();
                         this._db = e
                     }, this._db = null, this._stateDB = e.stateDB;
                     const t = new _.PromiseDelegate;
                     this.ready = t.promise, this._updateDB().then((() => t.resolve())), window.setInterval(this._updateDB, e.fetchInterval)
                 }
                 _get(e) {
                     return this._db ? this._db[this._itemKey(e)] : (console.error("Database is not ready!"), null)
                 }
                 async _set(e, t) {
-                    const a = await this._fetch();
-                    this._db = a, a[this._itemKey(e)] = t, await this._stateDB.save(this._stateDBKey, a)
+                    const s = await this._fetch();
+                    this._db = s, s[this._itemKey(e)] = t, await this._stateDB.save(this._stateDBKey, s)
                 }
                 async _fetch() {
                     let e = await this._stateDB.fetch(this._stateDBKey);
                     return void 0 === e && (e = await this._stateDB.fetch(this._stateDBKey)), void 0 === e ? {} : e
                 }
             }
             class K extends B {
@@ -645,120 +689,123 @@
                     const t = super._get(e);
                     return t ? new Date(t) : null
                 }
                 async recordAsUsedNow(e) {
                     this._set(e, (new Date).toUTCString())
                 }
             }
-            class M extends K {
+            class A extends K {
                 constructor() {
-                    super(...arguments), this._stateDBKey = "new-launcher:favorites"
+                    super(...arguments), this._stateDBKey = "new-launcher:favorites", this._changed = new p.Signal(this)
                 }
                 get(e) {
                     var t;
                     return null !== (t = super._get(e)) && void 0 !== t ? t : null
                 }
                 async set(e, t) {
-                    this._set(e, t)
+                    this._set(e, t), this._changed.emit()
+                }
+                get changed() {
+                    return this._changed
                 }
             }
-            const O = {
+            const R = {
                     id: "jupyterlab-new-launcher:database",
                     description: "A redesigned JupyterLab launcher databases",
                     provides: w,
                     autoStart: !0,
                     requires: [x.IStateDB],
                     activate: (e, t) => {
-                        const a = {
+                        const s = {
                             stateDB: t,
                             fetchInterval: 1e4
                         };
                         return {
-                            lastUsed: new T(a),
-                            favorites: new M(a)
+                            lastUsed: new T(s),
+                            favorites: new A(s)
                         }
                     }
                 },
-                R = [{
-                    id: f,
+                M = [{
+                    id: v,
                     description: "A redesigned JupyterLab launcher",
                     provides: o.ILauncher,
                     autoStart: !0,
                     requires: [i.ITranslator, l.ISettingRegistry, w],
-                    optional: [s.ILabShell, n.ICommandPalette, r.IDefaultFileBrowser],
-                    activate: function(e, t, a, s, r, l, i) {
+                    optional: [a.ILabShell, n.ICommandPalette, r.IDefaultFileBrowser],
+                    activate: function(e, t, s, a, r, l, i) {
                         const {
                             commands: m,
                             shell: u
                         } = e, h = t.load("jupyterlab-new-launcher"), p = new o.LauncherModel;
-                        return a.load(f).then((t => {
-                            ! function(e, t, a) {
+                        return s.load(v).then((t => {
+                            ! function(e, t, s) {
                                 e.commands.addCommand(b.toggleColumn, {
                                     label: e => {
                                         if (e.label) return e.label;
                                         if (e.id) {
                                             const t = e.id;
                                             return t[0].toLocaleUpperCase() + t.substring(1)
                                         }
                                         return t.__("Toggle given column")
                                     },
                                     execute: async e => {
                                         var t;
-                                        const s = e.id;
-                                        if (!s) return console.error("Column ID missing");
-                                        const n = null !== (t = a.user.hiddenColumns) && void 0 !== t ? t : {};
-                                        n[s] ? n[s] = !1 : n[s] = !0, await a.set("hiddenColumns", n)
+                                        const a = e.id;
+                                        if (!a) return console.error("Column ID missing");
+                                        const n = null !== (t = s.user.hiddenColumns) && void 0 !== t ? t : {};
+                                        "visible" !== n[a] && n[a] ? n[a] = "visible" : n[a] = "hidden", await s.set("hiddenColumns", n)
                                     },
                                     isToggleable: !0,
                                     isToggled: e => {
                                         var t;
-                                        const s = e.id;
-                                        return s ? !(null !== (t = a.user.hiddenColumns) && void 0 !== t ? t : {})[s] : (console.error("Column ID missing for checking if toggled"), !1)
+                                        const a = e.id;
+                                        return a ? "hidden" !== (null !== (t = s.user.hiddenColumns) && void 0 !== t ? t : {})[a] : (console.error("Column ID missing for checking if toggled"), !1)
                                     }
                                 }), e.commands.addCommand(b.moveColumn, {
                                     label: e => "left" === e.direction ? t.__("Move Column Left") : "right" === e.direction ? t.__("Move Column Right") : t.__("Move column left or right"),
                                     execute: async e => {
                                         const t = e.order,
-                                            s = e.id,
-                                            n = t.indexOf(s),
+                                            a = e.id,
+                                            n = t.indexOf(a),
                                             r = n + ("left" === e.direction ? -1 : 1);
                                         if (r < 0 || r >= t.length) return void console.log("Cannot move the column any further");
                                         const o = t[r];
-                                        t[r] = s, t[n] = o, await a.set("columnOrder", t)
+                                        t[r] = a, t[n] = o, await s.set("columnOrder", t)
                                     }
                                 })
                             }(e, h, t)
                         })), m.addCommand(b.create, {
                             label: h.__("New Launcher"),
                             icon: e => e.toolbar ? c.addIcon : void 0,
                             execute: async e => {
                                 var o, l;
                                 const g = null !== (l = null !== (o = e.cwd) && void 0 !== o ? o : null == i ? void 0 : i.model.path) && void 0 !== l ? l : "",
-                                    v = "launcher-" + F.id++,
-                                    _ = await a.load(f);
-                                await Promise.all([s.lastUsed.ready, s.favorites.ready]);
-                                const b = new E({
+                                    f = "launcher-" + O.id++,
+                                    _ = await s.load(v);
+                                await Promise.all([a.lastUsed.ready, a.favorites.ready]);
+                                const b = new I({
                                     model: p,
                                     cwd: g,
                                     callback: e => {
                                         (0, d.find)(u.widgets("main"), (t => t === e)) && (u.add(e, "main", {
-                                            ref: v
+                                            ref: f
                                         }), b.dispose())
                                     },
                                     commands: m,
                                     translator: t,
-                                    lastUsedDatabase: s.lastUsed,
-                                    favoritesDatabase: s.favorites,
+                                    lastUsedDatabase: a.lastUsed,
+                                    favoritesDatabase: a.favorites,
                                     settings: _
                                 });
                                 b.model = p, b.title.icon = c.launcherIcon, b.title.label = h.__("Launcher");
                                 const w = new n.MainAreaWidget({
                                     content: b
                                 });
-                                if (w.title.closable = !!Array.from(u.widgets("main")).length, w.id = v, u.add(w, "main", {
+                                if (w.title.closable = !!Array.from(u.widgets("main")).length, w.id = f, u.add(w, "main", {
                                         activate: e.activate,
                                         ref: e.ref
                                     }), r && r.layoutModified.connect((() => {
                                         w.title.closable = Array.from(r.widgets("main")).length > 1
                                     }), w), i) {
                                     const e = e => {
                                         b.cwd = e.path
@@ -773,22 +820,22 @@
                             r.layoutModified.connect((() => {
                                 r.isEmpty("main") && m.execute(b.create)
                             }))
                         })), l && l.addItem({
                             command: b.create,
                             category: h.__("Launcher")
                         }), r && (r.addButtonEnabled = !0, r.addRequested.connect(((e, t) => {
-                            var a;
-                            const s = (null === (a = t.currentTitle) || void 0 === a ? void 0 : a.owner.id) || t.titles[t.titles.length - 1].owner.id;
+                            var s;
+                            const a = (null === (s = t.currentTitle) || void 0 === s ? void 0 : s.owner.id) || t.titles[t.titles.length - 1].owner.id;
                             return m.execute(b.create, {
-                                ref: s
+                                ref: a
                             })
                         }))), p
                     }
-                }, N, O];
-            var F;
+                }, U, R];
+            var O;
             ! function(e) {
                 e.id = 0
-            }(F || (F = {}))
+            }(O || (O = {}))
         }
     }
 ]);
```

### Comparing `jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/static/728.379a3ceb37c59a35119c.js` & `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/728.ea49658c85c6542563e2.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
             t.d(e, {
                 A: () => p
             });
             var r = t(601),
                 a = t.n(r),
                 o = t(314),
                 i = t.n(o)()(a());
-            i.push([n.id, ".jp-Launcher-CardGroup {\n  justify-content: center;\n}\n\n.jp-CollapsibleSection {\n  --jp-animation-depth: 10px;\n  --jp-animation-time: 150ms;\n  --jp-title-height: 24px;\n\n  padding: var(--jp-animation-depth);\n  padding-left: 0;\n  padding-right: 0;\n}\n\n.jp-Launcher-cwd > h3 {\n  font-size: var(--jp-ui-font-size1);\n  margin: 0;\n}\n\n.jp-NewLauncher-OtherItems .jp-LauncherCard-label {\n  display: none;\n}\n\n.jp-NewLauncher-OtherItems .jp-Launcher-TypeCard {\n  width: unset;\n  min-height: unset;\n  flex-direction: row;\n  margin: 0;\n  box-shadow: none;\n  border-color: var(--jp-border-color0);\n}\n\n.jp-NewLauncher-OtherItems .jp-LauncherCard-icon {\n  height: 24px;\n}\n\n.jp-NewLauncher-OtherItems .jp-Launcher-TypeCard > .jp-LauncherCard-icon svg {\n  width: 16px;\n  height: 16px;\n}\n\n.jp-NewLauncher-TopBar {\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n  padding: 8px 0;\n}\n\n.jp-Launcher-searchBox input {\n  box-shadow: none;\n  border: var(--jp-border-width) solid var(--jp-border-color1);\n}\n\n.jp-CollapsibleSection > summary {\n  cursor: pointer;\n  transition: margin var(--jp-animation-time) ease-out;\n  list-style: none;\n  display: inline-block; /* contain the clickable area */\n  padding-right: 12px; /* but extend it a little */\n  min-width: 185px;\n}\n\n.jp-CollapsibleSection > summary:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.jp-CollapsibleSection[open] > summary {\n  margin-bottom: var(--jp-animation-depth);\n}\n\n.jp-CollapsibleSection-CollapserIcon > svg {\n  transition: transform var(--jp-animation-time) ease-out;\n  width: var(--jp-title-height);\n  height: var(--jp-title-height);\n}\n\n.jp-CollapsibleSection[open] .jp-CollapsibleSection-CollapserIcon > svg {\n  transform: rotate(90deg);\n}\n\n.jp-CollapsibleSection-CollapserIconWrapper {\n  display: inline-block;\n}\n\n.jp-CollapsibleSection-CategoryIcon > svg {\n  width: 24px;\n  height: 24px;\n  margin-left: 4px;\n  margin-right: 8px;\n}\n\n.jp-CollapsibleSection-Title {\n  display: inline-block;\n  line-height: var(--jp-title-height);\n  vertical-align: top;\n  margin: 0;\n  user-select: none;\n  font-weight: normal;\n}\n\n.jp-LauncherBody {\n  padding: 0 24px;\n  height: 100%;\n  overflow-y: auto;\n}\n\n.jp-NewLauncher-table {\n  --jp-icon-size: 16px;\n\n  display: flex;\n  flex-direction: column;\n  overflow: hidden;\n}\n\n.jp-NewLauncher-table .jp-sortable-table {\n  border: var(--jp-border-width) solid var(--jp-border-color2);\n  border-top: 0;\n}\n\n.jp-NewLauncher-table .jp-Launcher-kernelIcon {\n  width: var(--jp-icon-size);\n  height: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-LauncherCard-noKernelIcon {\n  font-size: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-LauncherCard-icon {\n  height: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table th[data-id='icon'],\n.jp-NewLauncher-table th[data-id='star'] {\n  width: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-starIcon {\n  width: var(--jp-icon-size);\n  height: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table-scroller {\n  overflow: auto;\n  margin-top: 4px;\n}\n\n.jp-starIconButton {\n  --jp-transition-transform: rotate(72deg);\n\n  border: 0;\n  margin: 0;\n  padding: 0 6px;\n  background: transparent;\n  cursor: pointer;\n}\n\n.jp-starIcon .jp-star-filled {\n  opacity: 0;\n}\n\n.jp-starIcon .jp-star-filled,\n.jp-starIcon .jp-star-border {\n  transition-property: opacity, transform;\n  transition-duration: 0.2s;\n  transition-timing-function: ease-out;\n  transform-origin: center;\n}\n\n.jp-starIconButton.jp-mod-starred .jp-star-filled {\n  opacity: 1;\n  transform: var(--jp-transition-transform);\n}\n\n.jp-starIconButton.jp-mod-starred .jp-star-border {\n  opacity: 0;\n  transform: var(--jp-transition-transform);\n}\n\n.jp-KernelSelector-Dialog > .jp-Dialog-content {\n  max-height: 80%;\n  max-width: unset;\n}\n\n.jp-KernelSelector-Dialog > .jp-Dialog-content > .jp-Dialog-header {\n  display: none;\n}\n\n.jp-KernelSelector-SelectButton {\n  display: none;\n}\n\n.jp-KernelSelector-Dialog .jp-NewLauncher-table {\n  margin-bottom: 8px;\n}\n\n.jp-KernelSelector-Section {\n  margin: 0;\n  margin-bottom: 4px;\n}\n\n/* Styles for scenario where full row is clickable  */\n\n.jp-NewLauncher-table tr {\n  cursor: pointer;\n}\n\n.jp-Launcher-TypeCard {\n  user-select: none;\n}\n\n.jp-Launcher-TypeCard > .jp-LauncherCard-icon svg {\n  align-items: center;\n  display: flex;\n  height: 52px;\n  width: 52px;\n}\n", ""]);
+            i.push([n.id, ".jp-Launcher-CardGroup {\n  justify-content: center;\n}\n\n.jp-CollapsibleSection {\n  --jp-animation-depth: 10px;\n  --jp-animation-time: 150ms;\n  --jp-title-height: 24px;\n\n  padding: var(--jp-animation-depth);\n  padding-left: 0;\n  padding-right: 0;\n}\n\n.jp-Launcher-cwd > h3 {\n  font-size: var(--jp-ui-font-size1);\n  margin: 0;\n}\n\n.jp-NewLauncher-OtherItems .jp-LauncherCard-label {\n  display: none;\n}\n\n.jp-NewLauncher-OtherItems .jp-Launcher-TypeCard {\n  width: unset;\n  min-height: unset;\n  flex-direction: row;\n  margin: 0;\n  box-shadow: none;\n  border-color: var(--jp-border-color0);\n}\n\n.jp-NewLauncher-OtherItems .jp-LauncherCard-icon {\n  height: 24px;\n}\n\n.jp-NewLauncher-OtherItems .jp-Launcher-TypeCard > .jp-LauncherCard-icon svg {\n  width: 24px;\n  height: 16px;\n}\n\n.jp-NewLauncher-TopBar {\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n  padding: 8px 0;\n}\n\n.jp-Launcher-searchBox input {\n  /* (no longer needed in lab 4.2+) */\n  box-shadow: none;\n}\n\n.jp-Launcher-searchBox input,\n.jp-Launcher-searchBox jp-search::part(root) {\n  border: var(--jp-border-width) solid var(--jp-border-color1);\n}\n\n.jp-Launcher-searchBox .jp-FilterBox {\n  width: 100%;\n}\n\n.jp-CollapsibleSection > summary {\n  cursor: pointer;\n  transition: margin var(--jp-animation-time) ease-out;\n  list-style: none;\n  display: inline-block; /* contain the clickable area */\n  padding-right: 12px; /* but extend it a little */\n  min-width: 185px;\n}\n\n.jp-CollapsibleSection > summary:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.jp-CollapsibleSection[open] > summary {\n  margin-bottom: var(--jp-animation-depth);\n}\n\n.jp-CollapsibleSection-CollapserIcon > svg {\n  transition: transform var(--jp-animation-time) ease-out;\n  width: var(--jp-title-height);\n  height: var(--jp-title-height);\n}\n\n.jp-CollapsibleSection[open] .jp-CollapsibleSection-CollapserIcon > svg {\n  transform: rotate(90deg);\n}\n\n.jp-CollapsibleSection-CollapserIconWrapper {\n  display: inline-block;\n}\n\n.jp-CollapsibleSection-CategoryIcon > svg {\n  width: 24px;\n  height: 24px;\n  margin-left: 4px;\n  margin-right: 8px;\n}\n\n.jp-CollapsibleSection-Title {\n  display: inline-block;\n  line-height: var(--jp-title-height);\n  vertical-align: top;\n  margin: 0;\n  user-select: none;\n  font-weight: normal;\n}\n\n.jp-LauncherBody {\n  padding: 0 24px;\n  height: 100%;\n  overflow-y: auto;\n}\n\n.jp-NewLauncher-table {\n  --jp-icon-size: 16px;\n\n  display: flex;\n  flex-direction: column;\n  overflow: hidden;\n}\n\n.jp-NewLauncher-table .jp-sortable-table {\n  border: var(--jp-border-width) solid var(--jp-border-color2);\n  border-top: 0;\n}\n\n.jp-NewLauncher-table .jp-Launcher-kernelIcon {\n  width: var(--jp-icon-size);\n  height: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-LauncherCard-noKernelIcon {\n  font-size: var(--jp-icon-size);\n  line-height: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-LauncherCard-icon {\n  height: var(--jp-icon-size);\n  width: var(--jp-icon-size);\n  display: inline-block;\n}\n\n.jp-TableKernelItem {\n  display: inline-block;\n  line-height: var(--jp-icon-size);\n  vertical-align: top;\n  padding-left: 4px;\n}\n\n.jp-NewLauncher-table th[data-id='icon'],\n.jp-NewLauncher-table th[data-id='star'] {\n  width: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-starIcon {\n  width: var(--jp-icon-size);\n  height: var(--jp-icon-size);\n}\n\n.jp-starIconButton:hover > .jp-starIcon {\n  border-radius: 50%;\n  box-shadow: 0 0 0 2px var(--jp-layout-color3);\n  background: var(--jp-layout-color1);\n}\n\n.jp-NewLauncher-table-scroller {\n  overflow: auto;\n  margin-top: 4px;\n}\n\n.jp-starIconButton {\n  --jp-transition-transform: rotate(72deg);\n\n  border: 0;\n  margin: 0;\n  padding: 0 6px;\n  background: transparent;\n  cursor: pointer;\n}\n\n.jp-starIcon .jp-star-filled {\n  opacity: 0;\n}\n\n.jp-starIcon .jp-star-filled,\n.jp-starIcon .jp-star-border {\n  transition-property: opacity, transform;\n  transition-duration: 0.2s;\n  transition-timing-function: ease-out;\n  transform-origin: center;\n}\n\n.jp-starIconButton.jp-mod-starred .jp-star-filled {\n  opacity: 1;\n  transform: var(--jp-transition-transform);\n}\n\n.jp-starIconButton.jp-mod-starred .jp-star-border {\n  opacity: 0;\n  transform: var(--jp-transition-transform);\n}\n\n.jp-KernelSelector-Dialog > .jp-Dialog-content {\n  max-height: 80%;\n  max-width: unset;\n}\n\n.jp-KernelSelector-Dialog > .jp-Dialog-content > .jp-Dialog-header {\n  display: none;\n}\n\n.jp-KernelSelector-SelectButton {\n  display: none;\n}\n\n.jp-KernelSelector-Dialog .jp-NewLauncher-table {\n  margin-bottom: 8px;\n}\n\n.jp-KernelSelector-Section {\n  margin: 0;\n  margin-bottom: 4px;\n}\n\n/* Styles for scenario where full row is clickable  */\n\n.jp-NewLauncher-table tr {\n  cursor: pointer;\n}\n\n.jp-Launcher-TypeCard {\n  user-select: none;\n}\n\n.jp-Launcher-TypeCard > .jp-LauncherCard-icon svg {\n  align-items: center;\n  display: flex;\n  height: 52px;\n  width: 52px;\n}\n", ""]);
             const p = i
         },
         314: n => {
             n.exports = function(n) {
                 var e = [];
                 return e.toString = function() {
                     return this.map((function(e) {
@@ -27,17 +27,17 @@
                     ]);
                     var i = {};
                     if (r)
                         for (var p = 0; p < this.length; p++) {
                             var c = this[p][0];
                             null != c && (i[c] = !0)
                         }
-                    for (var s = 0; s < n.length; s++) {
-                        var l = [].concat(n[s]);
-                        r && i[l[0]] || (void 0 !== o && (void 0 === l[5] || (l[1] = "@layer".concat(l[5].length > 0 ? " ".concat(l[5]) : "", " {").concat(l[1], "}")), l[5] = o), t && (l[2] ? (l[1] = "@media ".concat(l[2], " {").concat(l[1], "}"), l[2] = t) : l[2] = t), a && (l[4] ? (l[1] = "@supports (".concat(l[4], ") {").concat(l[1], "}"), l[4] = a) : l[4] = "".concat(a)), e.push(l))
+                    for (var l = 0; l < n.length; l++) {
+                        var s = [].concat(n[l]);
+                        r && i[s[0]] || (void 0 !== o && (void 0 === s[5] || (s[1] = "@layer".concat(s[5].length > 0 ? " ".concat(s[5]) : "", " {").concat(s[1], "}")), s[5] = o), t && (s[2] ? (s[1] = "@media ".concat(s[2], " {").concat(s[1], "}"), s[2] = t) : s[2] = t), a && (s[4] ? (s[1] = "@supports (".concat(s[4], ") {").concat(s[1], "}"), s[4] = a) : s[4] = "".concat(a)), e.push(s))
                     }
                 }, e
             }
         },
         601: n => {
             n.exports = function(n) {
                 return n[1]
@@ -53,18 +53,18 @@
                         break
                     } return t
             }
 
             function r(n, r) {
                 for (var o = {}, i = [], p = 0; p < n.length; p++) {
                     var c = n[p],
-                        s = r.base ? c[0] + r.base : c[0],
-                        l = o[s] || 0,
-                        u = "".concat(s, " ").concat(l);
-                    o[s] = l + 1;
+                        l = r.base ? c[0] + r.base : c[0],
+                        s = o[l] || 0,
+                        u = "".concat(l, " ").concat(s);
+                    o[l] = s + 1;
                     var d = t(u),
                         h = {
                             css: c[1],
                             media: c[2],
                             sourceMap: c[3],
                             supports: c[4],
                             layer: c[5]
@@ -97,17 +97,17 @@
                 var o = r(n = n || [], a = a || {});
                 return function(n) {
                     n = n || [];
                     for (var i = 0; i < o.length; i++) {
                         var p = t(o[i]);
                         e[p].references--
                     }
-                    for (var c = r(n, a), s = 0; s < o.length; s++) {
-                        var l = t(o[s]);
-                        0 === e[l].references && (e[l].updater(), e.splice(l, 1))
+                    for (var c = r(n, a), l = 0; l < o.length; l++) {
+                        var s = t(o[l]);
+                        0 === e[s].references && (e[s].updater(), e.splice(s, 1))
                     }
                     o = c
                 }
             }
         },
         659: n => {
             var e = {};
@@ -136,15 +136,15 @@
         },
         56: (n, e, t) => {
             n.exports = function(n) {
                 var e = t.nc;
                 e && n.setAttribute("nonce", e)
             }
         },
-        825: n => {
+        206: n => {
             n.exports = function(n) {
                 if ("undefined" == typeof document) return {
                     update: function() {},
                     remove: function() {}
                 };
                 var e = n.insertStyleElement(n);
                 return {
@@ -176,23 +176,23 @@
                 }
             }
         },
         728: (n, e, t) => {
             t.r(e);
             var r = t(72),
                 a = t.n(r),
-                o = t(825),
+                o = t(206),
                 i = t.n(o),
                 p = t(659),
                 c = t.n(p),
-                s = t(56),
-                l = t.n(s),
+                l = t(56),
+                s = t.n(l),
                 u = t(540),
                 d = t.n(u),
                 h = t(113),
                 j = t.n(h),
                 f = t(475),
                 m = {};
-            m.styleTagTransform = j(), m.setAttributes = l(), m.insert = c().bind(null, "head"), m.domAPI = i(), m.insertStyleElement = d(), a()(f.A, m), f.A && f.A.locals && f.A.locals
+            m.styleTagTransform = j(), m.setAttributes = s(), m.insert = c().bind(null, "head"), m.domAPI = i(), m.insertStyleElement = d(), a()(f.A, m), f.A && f.A.locals && f.A.locals
         }
     }
 ]);
```

### Comparing `jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/static/remoteEntry.3bf9447fc2344a3f202a.js` & `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/remoteEntry.097f22d9f5ab72ff351d.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -43,19 +43,19 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        21: "09cd58745a7785ee864d",
-        728: "379a3ceb37c59a35119c"
+        21: "b553ea2f251b3240c2ae",
+        728: "ea49658c85c6542563e2"
     } [e] + ".js?v=" + {
-        21: "09cd58745a7785ee864d",
-        728: "379a3ceb37c59a35119c"
+        21: "b553ea2f251b3240c2ae",
+        728: "ea49658c85c6542563e2"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -106,15 +106,15 @@
                     var a = o[e] = o[e] || {},
                         u = a[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
                         get: () => m.e(21).then((() => () => m(21))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-new-launcher", "0.1.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-new-launcher", "0.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -209,28 +209,28 @@
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, a) {
         var o = m.I(r);
         return o && o.then ? o.then(e.bind(e, r, m.S[r], t, n, a)) : e(r, m.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
         53: () => p("default", "@lumino/algorithm", [1, 2, 0, 0]),
-        221: () => p("default", "@jupyterlab/filebrowser", [1, 4, 1, 6]),
+        101: () => p("default", "@jupyterlab/statedb", [1, 4, 2, 0]),
+        260: () => p("default", "@jupyterlab/launcher", [1, 4, 2, 0]),
         262: () => p("default", "@lumino/coreutils", [1, 2, 0, 0]),
+        265: () => p("default", "@jupyterlab/translation", [1, 4, 2, 0]),
         345: () => p("default", "react", [1, 18, 2, 0]),
-        465: () => p("default", "@jupyterlab/application", [1, 4, 1, 6]),
-        595: () => p("default", "@jupyterlab/launcher", [1, 4, 1, 6]),
-        597: () => p("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
+        527: () => p("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
         602: () => p("default", "@lumino/signaling", [1, 2, 0, 0]),
-        618: () => p("default", "@jupyterlab/settingregistry", [1, 4, 1, 6]),
-        638: () => p("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
-        664: () => p("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
-        714: () => p("default", "@jupyterlab/translation", [1, 4, 1, 6]),
-        750: () => p("default", "@jupyterlab/statedb", [1, 4, 1, 6])
+        626: () => p("default", "@jupyterlab/application", [1, 4, 2, 0]),
+        670: () => p("default", "@jupyterlab/filebrowser", [1, 4, 2, 0]),
+        702: () => p("default", "@jupyterlab/coreutils", [1, 6, 2, 0]),
+        825: () => p("default", "@jupyterlab/settingregistry", [1, 4, 2, 0]),
+        923: () => p("default", "@jupyterlab/apputils", [1, 4, 3, 0])
     }, v = {
-        21: [53, 221, 262, 345, 465, 595, 597, 602, 618, 638, 664, 714, 750]
+        21: [53, 101, 260, 262, 265, 345, 527, 602, 626, 670, 702, 825, 923]
     }, b = {}, m.f.consumes = (e, r) => {
         m.o(v, e) && v[e].forEach((e => {
             if (m.o(c, e)) return r.push(c[e]);
             if (!b[e]) {
                 var t = r => {
                     c[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
```

### Comparing `jupyterlab_new_launcher-0.1.0/jupyterlab_new_launcher/labextension/static/third-party-licenses.json` & `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/src/commands.ts` & `jupyterlab_new_launcher-0.2.0/src/commands.ts`

 * *Files 9% similar despite different names*

```diff
@@ -25,33 +25,33 @@
       if (!id) {
         return console.error('Column ID missing');
       }
       const columns =
         (settings.user.hiddenColumns as
           | ISettingsLayout['hiddenColumns']
           | undefined) ?? {};
-      if (columns[id]) {
-        columns[id] = false;
+      if (columns[id] === 'visible' || !columns[id]) {
+        columns[id] = 'hidden';
       } else {
-        columns[id] = true;
+        columns[id] = 'visible';
       }
       await settings.set('hiddenColumns', columns);
     },
     isToggleable: true,
     isToggled: args => {
       const id = args.id as string | undefined;
       if (!id) {
         console.error('Column ID missing for checking if toggled');
         return false;
       }
       const columns =
         (settings.user.hiddenColumns as
           | ISettingsLayout['hiddenColumns']
           | undefined) ?? {};
-      return !columns[id];
+      return columns[id] !== 'hidden';
     }
   });
   app.commands.addCommand(CommandIDs.moveColumn, {
     label: args => {
       if (args.direction === 'left') {
         return trans.__('Move Column Left');
       } else if (args.direction === 'right') {
```

### Comparing `jupyterlab_new_launcher-0.1.0/src/database.ts` & `jupyterlab_new_launcher-0.2.0/src/database.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import { IStateDB } from '@jupyterlab/statedb';
 import { ReadonlyPartialJSONValue, PromiseDelegate } from '@lumino/coreutils';
+import { Signal } from '@lumino/signaling';
 import { ILauncher } from '@jupyterlab/launcher';
 import {
   ILastUsedDatabase,
   IFavoritesDatabase,
   ILauncherDatabase
 } from './types';
 import {
@@ -90,15 +91,22 @@
 
   get(item: ILauncher.IItemOptions) {
     return super._get(item) ?? null;
   }
 
   async set(item: ILauncher.IItemOptions, isFavourite: boolean) {
     this._set(item, isFavourite);
+    this._changed.emit();
   }
+
+  get changed() {
+    return this._changed;
+  }
+
+  private _changed = new Signal<FavoritesDatabase, void>(this);
 }
 
 /**
  * Initialization data for the jupyterlab-new-launcher extension.
  */
 export const databasePlugin: JupyterFrontEndPlugin<ILauncherDatabase> = {
   id: 'jupyterlab-new-launcher:database',
```

### Comparing `jupyterlab_new_launcher-0.1.0/src/dialogs.tsx` & `jupyterlab_new_launcher-0.2.0/src/dialogs.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 import type { CommandRegistry } from '@lumino/commands';
+import type { Message } from '@lumino/messaging';
 import {
   SessionContextDialogs,
   ISessionContextDialogs,
   ISessionContext,
   SessionContext,
   Dialog,
   ReactWidget
@@ -175,14 +176,31 @@
       cwd: '',
       commands: this.commands,
       lastUsedDatabase: this._lastUsedDatabase,
       favoritesDatabase: this._favoritesDatabase
     });
   };
 
+  onBeforeAttach(msg: Message) {
+    super.onBeforeAttach(msg);
+    this.node.style.minWidth = '';
+    this.node.style.minHeight = '';
+  }
+
+  onAfterAttach(msg: Message) {
+    super.onAfterAttach(msg);
+    requestAnimationFrame(() => {
+      // Set minimum dimensions so that when user starts typing to filter
+      // the kernels the dialog does not start jumping around.
+      const bbox = this.node.getBoundingClientRect();
+      this.node.style.minWidth = bbox.width + 'px';
+      this.node.style.minHeight = bbox.height + 'px';
+    });
+  }
+
   /**
    * Render the launcher to virtual DOM nodes.
    */
   protected render(): React.ReactElement<any> | null {
     const items: ILauncher.IItemOptions[] = [];
     const specs = this.options.data.specs!.kernelspecs!;
```

### Comparing `jupyterlab_new_launcher-0.1.0/src/index.ts` & `jupyterlab_new_launcher-0.2.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/src/item.ts` & `jupyterlab_new_launcher-0.2.0/src/item.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/src/types.ts` & `jupyterlab_new_launcher-0.2.0/src/types.ts`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,19 @@
 export namespace CommandIDs {
   export const create = 'launcher:create';
   export const moveColumn = 'new-launcher:table-move-column';
   export const toggleColumn = 'new-launcher:table-toggle-column';
 }
 
 export interface ISettingsLayout {
-  hiddenColumns: Record<string, boolean>;
+  hiddenColumns: Record<string, 'visible' | 'hidden'>;
   columnOrder: string[];
+  starredSection: boolean;
+  collapsedSections: Record<string, 'collapsed' | 'expanded'>;
+  searchAllSections: boolean;
 }
 
 export interface IItem extends ILauncher.IItemOptions {
   label: string;
   caption: string;
   icon: VirtualElement.IRenderer | undefined;
   iconClass: string;
@@ -43,14 +46,15 @@
   recordAsUsedNow(item: ILauncher.IItemOptions): Promise<void>;
 }
 
 export interface IFavoritesDatabase {
   ready: Promise<void>;
   get(item: ILauncher.IItemOptions): boolean | null;
   set(item: ILauncher.IItemOptions, isFavourite: boolean): Promise<void>;
+  changed: ISignal<IFavoritesDatabase, void>;
 }
 
 /**
  * Databases for new launcher.
  */
 export const ILauncherDatabase = new Token<ILauncherDatabase>(
   'jupyterlab-new-launcher:ILauncherDatabase',
```

### Comparing `jupyterlab_new_launcher-0.1.0/src/components/card.tsx` & `jupyterlab_new_launcher-0.2.0/src/components/card.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/src/components/section.tsx` & `jupyterlab_new_launcher-0.2.0/src/components/section.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,25 @@
 
 export function CollapsibleSection(
   props: React.PropsWithChildren<{
     title: string;
     className: string;
     icon: LabIcon;
     open: boolean;
+    onToggled?: (open: boolean) => void;
   }>
 ) {
   const [open, setOpen] = React.useState<boolean>(props.open);
 
-  const handleToggle = (event: { currentTarget: { open: boolean } }) =>
+  const handleToggle = (event: { currentTarget: { open: boolean } }) => {
     setOpen(event.currentTarget.open);
+    if (props.onToggled) {
+      props.onToggled(event.currentTarget.open);
+    }
+  };
 
   return (
     <details
       onToggle={handleToggle}
       className={classes(props.className, 'jp-CollapsibleSection')}
       open={open}
     >
```

### Comparing `jupyterlab_new_launcher-0.1.0/src/components/table.tsx` & `jupyterlab_new_launcher-0.2.0/src/components/table.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 const KERNEL_ITEM_CLASS = 'jp-TableKernelItem';
 
 function columnLabelFromKey(key: string): string {
   if (key.length === 0) {
     return '(empty)';
   }
   switch (key) {
-    // Added by nb_conda_kernels <= 2.5.0
+    // Added by nb_conda_kernels
     case 'conda_env_name':
       return 'Environment';
     case 'conda_env_path':
       return 'Environment path';
-    // Will be added once https://github.com/anaconda/nb_conda_kernels/pull/262/ is released
+    // Added by nb_conda_kernels >= 2.5.1
     case 'conda_language':
       return 'Language';
     case 'conda_raw_kernel_name':
       return 'Kernel';
     case 'conda_is_base_environment':
       return 'Base?';
     case 'conda_is_currently_running':
@@ -46,20 +46,22 @@
   items: IKernelItem[];
   commands: CommandRegistry;
   settings: ISettingRegistry.ISettings;
   showSearchBox: boolean;
   query: string;
   onClick: (item: IKernelItem) => void;
   hideColumns?: string[];
+  showWidgetType?: boolean;
 }) {
   const { trans } = props;
   let query: string;
   let updateQuery: (value: string) => void;
+  // Note: state cannot be defined in conditionals, or React will error out when toggling it.
+  const [_query, _updateQuery] = React.useState<string>('');
   if (props.showSearchBox) {
-    const [_query, _updateQuery] = React.useState<string>('');
     query = _query;
     updateQuery = _updateQuery;
   } else {
     query = props.query;
   }
 
   // Hoisted to avoid "Rendered fewer hooks than expected" error on toggling the Star column
@@ -117,59 +119,65 @@
           }
           return aValue > bValue ? 1 : -1;
         }
       };
     }
   );
 
-  const availableColumns: Table.IColumn<IKernelItem>[] = [
-    {
-      id: 'icon',
-      label: trans.__('Icon'),
-      renderCell: (row: IKernelItem) => (
-        <div
-          className="jp-LauncherCard-icon"
-          onClick={() => props.onClick(row)}
-        >
-          {row.kernelIconUrl ? (
-            <img
-              src={row.kernelIconUrl}
-              className="jp-Launcher-kernelIcon"
-              alt={row.label}
-            />
-          ) : (
-            <div className="jp-LauncherCard-noKernelIcon">
-              {row.label[0].toUpperCase()}
-            </div>
-          )}
-        </div>
-      ),
+  if (props.showWidgetType) {
+    extraColumns.push({
+      id: 'widget-type',
+      label: trans.__('Type'),
+      renderCell: (row: IKernelItem) => {
+        return row.command.split(':')[0];
+      },
       sort: (a: IKernelItem, b: IKernelItem) =>
         a.command.localeCompare(b.command)
-    },
+    });
+  }
+
+  const availableColumns: Table.IColumn<IKernelItem>[] = [
     {
       id: 'kernel',
       label: trans.__('Kernel'),
       renderCell: (row: IKernelItem) => (
-        <span
-          className={KERNEL_ITEM_CLASS}
-          onClick={event => {
-            props.onClick(row);
-            event.stopPropagation();
-          }}
-          onKeyDown={event => {
-            // TODO memoize func defs for perf
-            if (event.key === 'Enter') {
-              row.execute();
-            }
-          }}
-          tabIndex={0}
-        >
-          {row.label}
-        </span>
+        <>
+          <span
+            className="jp-LauncherCard-icon"
+            onClick={() => props.onClick(row)}
+          >
+            {row.kernelIconUrl ? (
+              <img
+                src={row.kernelIconUrl}
+                className="jp-Launcher-kernelIcon"
+                alt={row.label}
+              />
+            ) : (
+              <div className="jp-LauncherCard-noKernelIcon">
+                {row.label[0].toUpperCase()}
+              </div>
+            )}
+          </span>
+          <span
+            className={KERNEL_ITEM_CLASS}
+            onClick={event => {
+              props.onClick(row);
+              event.stopPropagation();
+            }}
+            onKeyDown={event => {
+              // TODO memoize func defs for perf
+              if (event.key === 'Enter') {
+                row.execute();
+              }
+            }}
+            tabIndex={0}
+          >
+            {row.label}
+          </span>
+        </>
       ),
       sort: (a: IKernelItem, b: IKernelItem) => a.label.localeCompare(b.label)
     },
     ...extraColumns,
     {
       id: 'last-used',
       label: trans.__('Last Used'),
@@ -274,15 +282,15 @@
   });
 
   return (
     <div className="jp-NewLauncher-table">
       {props.showSearchBox ? (
         <div className="jp-Launcher-searchBox">
           <FilterBox
-            placeholder={trans.__('Filter')}
+            placeholder={trans.__('Filter kernels')}
             updateFilter={(_, query) => {
               updateQuery(query ?? '');
             }}
             initialQuery={''}
             useFuzzyFilter={false}
           />
         </div>
@@ -347,15 +355,15 @@
             if (starButton) {
               return (starButton as HTMLElement).click();
             }
             const element = row.querySelector(`.${KERNEL_ITEM_CLASS}`)!;
             (element as HTMLElement).click();
           }}
           columns={columns
-            .filter(column => !hiddenColumns[column.id])
+            .filter(column => hiddenColumns[column.id] !== 'hidden')
             .map(column => {
               return {
                 ...column,
                 rank: columnOrder.indexOf(column.id) ?? 10
               };
             })
             .sort((a, b) => {
```

### Comparing `jupyterlab_new_launcher-0.1.0/style/base.css` & `jupyterlab_new_launcher-0.2.0/style/base.css`

 * *Files 4% similar despite different names*

```diff
@@ -31,30 +31,39 @@
 }
 
 .jp-NewLauncher-OtherItems .jp-LauncherCard-icon {
   height: 24px;
 }
 
 .jp-NewLauncher-OtherItems .jp-Launcher-TypeCard > .jp-LauncherCard-icon svg {
-  width: 16px;
+  width: 24px;
   height: 16px;
 }
 
 .jp-NewLauncher-TopBar {
   display: flex;
   justify-content: space-between;
   align-items: center;
   padding: 8px 0;
 }
 
 .jp-Launcher-searchBox input {
+  /* (no longer needed in lab 4.2+) */
   box-shadow: none;
+}
+
+.jp-Launcher-searchBox input,
+.jp-Launcher-searchBox jp-search::part(root) {
   border: var(--jp-border-width) solid var(--jp-border-color1);
 }
 
+.jp-Launcher-searchBox .jp-FilterBox {
+  width: 100%;
+}
+
 .jp-CollapsibleSection > summary {
   cursor: pointer;
   transition: margin var(--jp-animation-time) ease-out;
   list-style: none;
   display: inline-block; /* contain the clickable area */
   padding-right: 12px; /* but extend it a little */
   min-width: 185px;
@@ -120,30 +129,46 @@
 .jp-NewLauncher-table .jp-Launcher-kernelIcon {
   width: var(--jp-icon-size);
   height: var(--jp-icon-size);
 }
 
 .jp-NewLauncher-table .jp-LauncherCard-noKernelIcon {
   font-size: var(--jp-icon-size);
+  line-height: var(--jp-icon-size);
 }
 
 .jp-NewLauncher-table .jp-LauncherCard-icon {
   height: var(--jp-icon-size);
+  width: var(--jp-icon-size);
+  display: inline-block;
+}
+
+.jp-TableKernelItem {
+  display: inline-block;
+  line-height: var(--jp-icon-size);
+  vertical-align: top;
+  padding-left: 4px;
 }
 
 .jp-NewLauncher-table th[data-id='icon'],
 .jp-NewLauncher-table th[data-id='star'] {
   width: var(--jp-icon-size);
 }
 
 .jp-NewLauncher-table .jp-starIcon {
   width: var(--jp-icon-size);
   height: var(--jp-icon-size);
 }
 
+.jp-starIconButton:hover > .jp-starIcon {
+  border-radius: 50%;
+  box-shadow: 0 0 0 2px var(--jp-layout-color3);
+  background: var(--jp-layout-color1);
+}
+
 .jp-NewLauncher-table-scroller {
   overflow: auto;
   margin-top: 4px;
 }
 
 .jp-starIconButton {
   --jp-transition-transform: rotate(72deg);
```

### Comparing `jupyterlab_new_launcher-0.1.0/style/icons/md/LICENSE` & `jupyterlab_new_launcher-0.2.0/style/icons/md/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/ui-tests/README.md` & `jupyterlab_new_launcher-0.2.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/ui-tests/yarn.lock` & `jupyterlab_new_launcher-0.2.0/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/.gitignore` & `jupyterlab_new_launcher-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/LICENSE` & `jupyterlab_new_launcher-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/README.md` & `jupyterlab_new_launcher-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/pyproject.toml` & `jupyterlab_new_launcher-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.1.0/PKG-INFO` & `jupyterlab_new_launcher-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-new-launcher
-Version: 0.1.0
+Version: 0.2.0
 Dynamic: Keywords
 Summary: A redesigned JupyterLab launcher
 Project-URL: Homepage, https://github.com/nebari-dev/jupyterlab-new-launcher
 Project-URL: Bug Tracker, https://github.com/nebari-dev/jupyterlab-new-launcher/issues
 Project-URL: Repository, https://github.com/nebari-dev/jupyterlab-new-launcher.git
 Author-email: Nebari development team <internal-it@quansight.com>
 License: BSD 3-Clause License
```

