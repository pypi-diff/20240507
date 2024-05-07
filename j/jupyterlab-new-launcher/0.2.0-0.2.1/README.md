# Comparing `tmp/jupyterlab_new_launcher-0.2.0.tar.gz` & `tmp/jupyterlab_new_launcher-0.2.1.tar.gz`

## Comparing `jupyterlab_new_launcher-0.2.0.tar` & `jupyterlab_new_launcher-0.2.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/.copier-answers.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/babel.config.js
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jest.config.js
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/junit.xml
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/setup.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/tsconfig.test.json
--rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/yarn.lock
--rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/docs/images/dialog.png
--rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/docs/images/launcher.png
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/_version.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/package.json
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
--rw-r--r--   0        0        0    21040 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/21.b553ea2f251b3240c2ae.js
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/728.ea49658c85c6542563e2.js
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/remoteEntry.097f22d9f5ab72ff351d.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/schema/plugin.json
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/commands.ts
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/database.ts
--rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/dialogs.tsx
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/icons.ts
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/index.ts
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/item.ts
--rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/launcher.tsx
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/svg.d.ts
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/types.ts
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/__tests__/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/components/card.tsx
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/components/section.tsx
--rw-r--r--   0        0        0    11435 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/src/components/table.tsx
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/style/index.js
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/style/icons/md/LICENSE
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/style/icons/md/file.svg
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/style/icons/md/star.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0    26996 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
--rw-r--r--   0        0        0    27431 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
--rw-r--r--   0        0        0    33351 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/LICENSE
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/README.md
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/.copier-answers.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/babel.config.js
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jest.config.js
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/junit.xml
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/setup.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/tsconfig.test.json
+-rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/yarn.lock
+-rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/docs/images/dialog.png
+-rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/docs/images/launcher.png
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/_version.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/package.json
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
+-rw-r--r--   0        0        0    21502 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/21.6aebeef0c48d440fad32.js
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/728.ea49658c85c6542563e2.js
+-rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/remoteEntry.9b81d6d816ee65d81ed3.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/schema/plugin.json
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/commands.ts
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/database.ts
+-rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/dialogs.tsx
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/icons.ts
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/index.ts
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/item.ts
+-rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/launcher.tsx
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/svg.d.ts
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/types.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/__tests__/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/components/card.tsx
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/components/section.tsx
+-rw-r--r--   0        0        0    11435 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/components/table.tsx
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/style/index.js
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/style/icons/md/LICENSE
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/style/icons/md/file.svg
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/style/icons/md/star.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0    26996 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
+-rw-r--r--   0        0        0    27431 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
+-rw-r--r--   0        0        0    33351 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/README.md
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/PKG-INFO
```

### Comparing `jupyterlab_new_launcher-0.2.0/.copier-answers.yml` & `jupyterlab_new_launcher-0.2.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/RELEASE.md` & `jupyterlab_new_launcher-0.2.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/jest.config.js` & `jupyterlab_new_launcher-0.2.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/package.json` & `jupyterlab_new_launcher-0.2.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `jupyterlab_new_launcher-0.2.0/tsconfig.json` & `jupyterlab_new_launcher-0.2.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/yarn.lock` & `jupyterlab_new_launcher-0.2.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/docs/images/dialog.png` & `jupyterlab_new_launcher-0.2.1/docs/images/dialog.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/docs/images/launcher.png` & `jupyterlab_new_launcher-0.2.1/docs/images/launcher.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/__init__.py` & `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/package.json` & `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.9b81d6d816ee65d81ed3.js'}}",*

 * * "'version'": "'0.2.1'"}*

```diff
@@ -108,15 +108,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/nebari-dev/jupyterlab-new-launcher",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.097f22d9f5ab72ff351d.js",
+            "load": "static/remoteEntry.9b81d6d816ee65d81ed3.js",
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
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig` & `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/21.b553ea2f251b3240c2ae.js` & `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/21.6aebeef0c48d440fad32.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,97 +1,106 @@
 "use strict";
 (self.webpackChunkjupyterlab_new_launcher = self.webpackChunkjupyterlab_new_launcher || []).push([
     [21], {
-        21: (e, t, s) => {
-            s.r(t), s.d(t, {
-                default: () => M
+        21: (e, t, a) => {
+            a.r(t), a.d(t, {
+                default: () => O
             });
-            var a = s(626),
-                n = s(923),
-                r = s(670),
-                o = s(260),
-                l = s(825),
-                i = s(265),
-                c = s(527),
-                d = s(53),
-                m = s(345);
+            var n = a(626),
+                s = a(923),
+                o = a(670),
+                r = a(260),
+                l = a(825),
+                i = a(265),
+                c = a(527),
+                d = a(53),
+                m = a(345);
             const u = new c.LabIcon({
                     name: "jupyterlab-new-launcher:star",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">\n  <path class="jp-icon3 jp-star-filled" fill="rgb(97,97,97)" d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z" />\n  <path class="jp-icon3 jp-star-border" fill="rgb(97,97,97)" d="M22 9.24l-7.19-.62L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21 12 17.27 18.18 21l-1.63-7.03L22 9.24zM12 15.4l-3.76 2.27 1-4.28-3.32-2.88 4.38-.38L12 6.1l1.71 4.04 4.38.38-3.32 2.88 1 4.28L12 15.4z" />\n</svg>\n'
                 }),
                 h = new c.LabIcon({
                     name: "jupyterlab-new-launcher:file",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">\n  <path class="jp-icon3" fill="rgb(97,97,97)" d="M13.81 22H6C4.89 22 4 21.11 4 20V4C4 2.9 4.89 2 6 2H14L20 8V13.09C19.67 13.04 19.34 13 19 13S18.33 13.04 18 13.09V9H13V4H6V20H13.09C13.21 20.72 13.46 21.39 13.81 22M23 18H20V15H18V18H15V20H18V23H20V20H23V18Z" />\n</svg>'
                 });
-            var p = s(602);
+            var p = a(602);
             class g {
                 constructor(e) {
-                    var t;
+                    var t, a, n, s;
                     this._options = e, this._refreshLastUsed = new p.Signal(this), this._refreshClock = null, this._lastUsed = null;
                     const {
-                        item: s,
-                        commands: a,
-                        lastUsedDatabase: n,
-                        favoritesDatabase: r,
-                        cwd: o
-                    } = e, l = {
-                        ...s.args,
-                        cwd: o
+                        item: o,
+                        commands: r,
+                        lastUsedDatabase: l,
+                        favoritesDatabase: i,
+                        cwd: c
+                    } = e, d = {
+                        ...o.args,
+                        cwd: c
                     };
-                    this.command = s.command, this.args = l, this.category = s.category, this.rank = s.rank, this.kernelIconUrl = s.kernelIconUrl, this.metadata = s.metadata, this.iconClass = a.iconClass(s.command, l), this.icon = a.icon(s.command, l), this.caption = a.caption(s.command, l), this.label = a.label(s.command, l), this.lastUsed = n.get(s), this.starred = null !== (t = r.get(s)) && void 0 !== t && t
+                    this.command = o.command, this.args = d, this.category = o.category, this.rank = o.rank, this.kernelIconUrl = o.kernelIconUrl, this.metadata = null !== (t = o.metadata) && void 0 !== t ? t : {}, this.iconClass = r.iconClass(o.command, d), this.icon = r.icon(o.command, d), this.caption = r.caption(o.command, d), this.label = r.label(o.command, d), this.lastUsed = l.get(o), this.starred = null !== (a = i.get(o)) && void 0 !== a && a;
+                    const m = (null !== (n = this.metadata.conda_env_name) && void 0 !== n ? n : "").match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
+                    if (m && this.metadata) {
+                        const e = m.groups;
+                        this.label = null !== (s = this.metadata.conda_language) && void 0 !== s ? s : e.environment, this.metadata = {
+                            ...this.metadata,
+                            conda_env_name: e.environment,
+                            Namespace: e.namespace
+                        }
+                    }
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
-                        lastUsedDatabase: s
+                        lastUsedDatabase: a
                     } = this._options;
-                    await t.execute(e.command, this.args), await s.recordAsUsedNow(e), this.lastUsed = s.get(e), this._refreshLastUsed.emit()
+                    await t.execute(e.command, this.args), await a.recordAsUsedNow(e), this.lastUsed = a.get(e), this._refreshLastUsed.emit()
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
-                    } = this._options, s = !t.get(e);
-                    return this.starred = s, t.set(e, s)
+                    } = this._options, a = !t.get(e);
+                    return this.starred = a, t.set(e, a)
                 }
                 _setRefreshClock() {
                     const e = this._lastUsed;
                     if (null !== this._refreshClock && (window.clearTimeout(this._refreshClock), this._refreshClock = null), !e) return;
                     const t = Date.now() - e.getTime(),
-                        s = t < 6e4 ? 1e4 : t < 36e5 ? 6e4 : 36e5;
+                        a = t < 6e4 ? 1e4 : t < 36e5 ? 6e4 : 36e5;
                     this._refreshClock = window.setTimeout((() => {
                         this._refreshLastUsed.emit(), this._setRefreshClock()
-                    }), s)
+                    }), a)
                 }
             }
-            var f = s(702),
-                _ = s(262);
-            const v = "jupyterlab-new-launcher:plugin";
+            var v = a(702),
+                f = a(262);
+            const _ = "jupyterlab-new-launcher:plugin";
             var b;
             ! function(e) {
                 e.create = "launcher:create", e.moveColumn = "new-launcher:table-move-column", e.toggleColumn = "new-launcher:table-toggle-column"
             }(b || (b = {}));
-            const w = new _.Token("jupyterlab-new-launcher:ILauncherDatabase", "Databases for new launcher."),
+            const w = new f.Token("jupyterlab-new-launcher:ILauncherDatabase", "Databases for new launcher."),
                 C = "jp-starIconButton",
                 y = "jp-TableKernelItem";
 
             function k(e) {
                 if (0 === e.length) return "(empty)";
                 switch (e) {
                     case "conda_env_name":
@@ -107,198 +116,198 @@
                     case "conda_is_currently_running":
                         return "Running?"
                 }
                 return e[0].toUpperCase() + e.substring(1)
             }
 
             function L(e) {
-                var t, s, a, n;
+                var t, a, n, s;
                 const {
-                    trans: r
+                    trans: o
                 } = e;
-                let o, l;
+                let r, l;
                 const [i, d] = m.useState("");
-                e.showSearchBox ? (o = i, l = d) : o = e.query;
+                e.showSearchBox ? (r = i, l = d) : r = e.query;
                 const [, h] = m.useReducer((e => e + 1), 0), p = new Set;
-                for (const s of e.items) {
-                    const e = null === (t = s.metadata) || void 0 === t ? void 0 : t.kernel;
+                for (const a of e.items) {
+                    const e = null === (t = a.metadata) || void 0 === t ? void 0 : t.kernel;
                     if (e)
                         for (const t of Object.keys(e)) p.add(t)
                 }
                 const g = [...p].map((e => ({
                     id: e,
                     label: k(e),
                     renderCell: t => {
-                        var s;
-                        const a = null === (s = t.metadata) || void 0 === s ? void 0 : s.kernel;
-                        if (!a) return "-";
-                        const n = a[e];
-                        return "string" == typeof n ? n : JSON.stringify(n)
+                        var a;
+                        const n = null === (a = t.metadata) || void 0 === a ? void 0 : a.kernel;
+                        if (!n) return "-";
+                        const s = n[e];
+                        return "string" == typeof s ? s : JSON.stringify(s)
                     },
-                    sort: (t, s) => {
-                        var a, n;
-                        const r = null === (a = t.metadata) || void 0 === a ? void 0 : a.kernel,
-                            o = null === (n = s.metadata) || void 0 === n ? void 0 : n.kernel,
-                            l = r ? r[e] : void 0,
-                            i = o ? o[e] : void 0;
+                    sort: (t, a) => {
+                        var n, s;
+                        const o = null === (n = t.metadata) || void 0 === n ? void 0 : n.kernel,
+                            r = null === (s = a.metadata) || void 0 === s ? void 0 : s.kernel,
+                            l = o ? o[e] : void 0,
+                            i = r ? r[e] : void 0;
                         return l === i ? 0 : l ? i ? "string" == typeof l && "string" == typeof i ? l.localeCompare(i) : l > i ? 1 : -1 : -1 : 1
                     }
                 })));
                 e.showWidgetType && g.push({
                     id: "widget-type",
-                    label: r.__("Type"),
+                    label: o.__("Type"),
                     renderCell: e => e.command.split(":")[0],
                     sort: (e, t) => e.command.localeCompare(t.command)
                 });
-                const _ = [{
+                const f = [{
                         id: "kernel",
-                        label: r.__("Kernel"),
+                        label: o.__("Kernel"),
                         renderCell: t => m.createElement(m.Fragment, null, m.createElement("span", {
                             className: "jp-LauncherCard-icon",
                             onClick: () => e.onClick(t)
                         }, t.kernelIconUrl ? m.createElement("img", {
                             src: t.kernelIconUrl,
                             className: "jp-Launcher-kernelIcon",
                             alt: t.label
                         }) : m.createElement("div", {
                             className: "jp-LauncherCard-noKernelIcon"
                         }, t.label[0].toUpperCase())), m.createElement("span", {
                             className: y,
-                            onClick: s => {
-                                e.onClick(t), s.stopPropagation()
+                            onClick: a => {
+                                e.onClick(t), a.stopPropagation()
                             },
                             onKeyDown: e => {
                                 "Enter" === e.key && t.execute()
                             },
                             tabIndex: 0
                         }, t.label)),
                         sort: (e, t) => e.label.localeCompare(t.label)
                     }, ...g, {
                         id: "last-used",
-                        label: r.__("Last Used"),
+                        label: o.__("Last Used"),
                         renderCell: e => m.createElement(c.UseSignal, {
                             signal: e.refreshLastUsed
                         }, (() => e.lastUsed ? m.createElement("span", {
-                            title: f.Time.format(e.lastUsed)
-                        }, f.Time.formatHuman(e.lastUsed)) : r.__("Never"))),
+                            title: v.Time.format(e.lastUsed)
+                        }, v.Time.formatHuman(e.lastUsed)) : o.__("Never"))),
                         sort: (e, t) => e.lastUsed === t.lastUsed ? 0 : e.lastUsed ? t.lastUsed && e.lastUsed > t.lastUsed ? 1 : -1 : 1
                     }, {
                         id: "star",
                         label: "",
                         renderCell: e => {
                             const t = e.starred,
-                                s = t ? r.__("Click to add this kernel to favourites") : r.__("Click to remove the kernel from favourites");
+                                a = t ? o.__("Click to add this kernel to favourites") : o.__("Click to remove the kernel from favourites");
                             return m.createElement("button", {
                                 className: t ? `${C} jp-mod-starred` : C,
-                                title: s,
+                                title: a,
                                 onClick: t => {
                                     e.toggleStar(), h(), t.stopPropagation()
                                 }
                             }, m.createElement(u.react, {
                                 className: "jp-starIcon"
                             }))
                         },
                         sort: (e, t) => Number(e.starred) - Number(t.starred)
                     }],
-                    v = null !== (s = e.hideColumns) && void 0 !== s ? s : [],
-                    w = _.filter((e => !v.includes(e.id))),
-                    [L, D] = m.useState(null !== (a = e.settings.composite.hiddenColumns) && void 0 !== a ? a : {}),
+                    _ = null !== (a = e.hideColumns) && void 0 !== a ? a : [],
+                    w = f.filter((e => !_.includes(e.id))),
+                    [L, D] = m.useState(null !== (n = e.settings.composite.hiddenColumns) && void 0 !== n ? n : {}),
                     S = w.map((e => e.id)),
-                    [E, I] = m.useState(null !== (n = e.settings.composite.columnOrder) && void 0 !== n ? n : S),
+                    [E, I] = m.useState(null !== (s = e.settings.composite.columnOrder) && void 0 !== s ? s : S),
                     N = c.Table,
                     U = () => {
-                        var t, s;
-                        const a = null !== (t = e.settings.composite.hiddenColumns) && void 0 !== t ? t : {};
-                        L !== a && D(a);
-                        const n = null !== (s = e.settings.composite.columnOrder) && void 0 !== s ? s : S;
-                        E !== n && I(n)
+                        var t, a;
+                        const n = null !== (t = e.settings.composite.hiddenColumns) && void 0 !== t ? t : {};
+                        L !== n && D(n);
+                        const s = null !== (a = e.settings.composite.columnOrder) && void 0 !== a ? a : S;
+                        E !== s && I(s)
                     };
                 return m.useEffect((() => (e.settings.changed.connect(U), () => {
                     e.settings.changed.disconnect(U)
                 }))), m.createElement("div", {
                     className: "jp-NewLauncher-table"
                 }, e.showSearchBox ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
                 }, m.createElement(c.FilterBox, {
-                    placeholder: r.__("Filter kernels"),
+                    placeholder: o.__("Filter kernels"),
                     updateFilter: (e, t) => {
                         l(null != t ? t : "")
                     },
                     initialQuery: "",
                     useFuzzyFilter: !1
                 })) : null, m.createElement("div", {
                     className: "jp-NewLauncher-table-scroller",
                     onContextMenu: t => {
-                        var s;
+                        var a;
                         t.preventDefault();
-                        const a = new c.MenuSvg({
+                        const n = new c.MenuSvg({
                                 commands: e.commands
                             }),
-                            n = new c.MenuSvg({
+                            s = new c.MenuSvg({
                                 commands: e.commands
                             });
-                        for (const e of w) n.addItem({
+                        for (const e of w) s.addItem({
                             command: b.toggleColumn,
                             args: {
                                 id: e.id,
                                 label: e.label
                             }
                         });
-                        n.title.label = r.__("Visible Columns"), a.addItem({
+                        s.title.label = o.__("Visible Columns"), n.addItem({
                             type: "submenu",
-                            submenu: n
+                            submenu: s
                         });
-                        const o = null === (s = t.target.closest("th[data-id]")) || void 0 === s ? void 0 : s.dataset.id;
-                        o && (a.addItem({
+                        const r = null === (a = t.target.closest("th[data-id]")) || void 0 === a ? void 0 : a.dataset.id;
+                        r && (n.addItem({
                             command: b.moveColumn,
                             args: {
                                 direction: "left",
                                 order: E,
-                                id: o
+                                id: r
                             }
-                        }), a.addItem({
+                        }), n.addItem({
                             command: b.moveColumn,
                             args: {
                                 direction: "right",
                                 order: E,
-                                id: o
+                                id: r
                             }
-                        })), a.open(t.clientX, t.clientY)
+                        })), n.open(t.clientX, t.clientY)
                     }
                 }, m.createElement(N, {
-                    rows: e.items.filter((e => -1 !== e.label.toLowerCase().indexOf(o.toLowerCase()))).map((e => ({
+                    rows: e.items.filter((e => -1 !== e.label.toLowerCase().indexOf(r.toLowerCase()))).map((e => ({
                         data: e,
                         key: e.command + JSON.stringify(e.args)
                     }))),
-                    blankIndicator: () => m.createElement("div", null, r.__("No entries")),
+                    blankIndicator: () => m.createElement("div", null, o.__("No entries")),
                     sortKey: "kernel",
                     onRowClick: e => {
                         const t = e.target,
-                            s = t.closest("tr");
-                        if (!s) return;
-                        const a = t.closest("td"),
-                            n = null == a ? void 0 : a.querySelector(`.${C}`);
-                        if (n) return n.click();
-                        s.querySelector(`.${y}`).click()
+                            a = t.closest("tr");
+                        if (!a) return;
+                        const n = t.closest("td"),
+                            s = null == n ? void 0 : n.querySelector(`.${C}`);
+                        if (s) return s.click();
+                        a.querySelector(`.${y}`).click()
                     },
                     columns: w.filter((e => "hidden" !== L[e.id])).map((e => {
                         var t;
                         return {
                             ...e,
                             rank: null !== (t = E.indexOf(e.id)) && void 0 !== t ? t : 10
                         }
                     })).sort(((e, t) => e.rank - t.rank))
                 })))
             }
 
             function D(e) {
-                const [t, s] = m.useState(e.open);
+                const [t, a] = m.useState(e.open);
                 return m.createElement("details", {
                     onToggle: t => {
-                        s(t.currentTarget.open), e.onToggled && e.onToggled(t.currentTarget.open)
+                        a(t.currentTarget.open), e.onToggled && e.onToggled(t.currentTarget.open)
                     },
                     className: (0, c.classes)(e.className, "jp-CollapsibleSection"),
                     open: t
                 }, m.createElement("summary", null, m.createElement("div", {
                     className: "jp-CollapsibleSection-CollapserIconWrapper",
                     "aria-hidden": "true"
                 }, m.createElement(c.caretRightIcon.react, {
@@ -331,237 +340,238 @@
                     className: "jp-LauncherCard-label"
                 }, m.createElement("p", null, t.label)))
             }
 
             function E(e) {
                 var t;
                 const {
-                    trans: s,
-                    cwd: a,
-                    typeItems: n,
-                    otherItems: r,
-                    favouritesChanged: o
-                } = e, [l, i] = m.useState(""), [, d] = m.useReducer((e => e + 1), 0), [p, g] = m.useState(e.settings.composite.starredSection), [f, _] = m.useState(e.settings.composite.searchAllSections), v = () => {
+                    trans: a,
+                    cwd: n,
+                    typeItems: s,
+                    otherItems: o,
+                    favouritesChanged: r
+                } = e, [l, i] = m.useState(""), [, d] = m.useReducer((e => e + 1), 0), [p, g] = m.useState(e.settings.composite.starredSection), [v, f] = m.useState(e.settings.composite.searchAllSections), _ = () => {
                     const t = e.settings.composite.starredSection;
                     p !== t && g(t);
-                    const s = e.settings.composite.searchAllSections;
-                    f !== s && _(s)
+                    const a = e.settings.composite.searchAllSections;
+                    v !== a && f(a)
                 };
-                if (m.useEffect((() => (e.settings.changed.connect(v), () => {
-                        e.settings.changed.disconnect(v)
-                    }))), o) {
+                if (m.useEffect((() => (e.settings.changed.connect(_), () => {
+                        e.settings.changed.disconnect(_)
+                    }))), r) {
                     const e = () => {
                         p && d()
                     };
-                    m.useEffect((() => (o.connect(e), () => {
-                        o.disconnect(e)
+                    m.useEffect((() => (r.connect(e), () => {
+                        r.disconnect(e)
                     })))
                 }
                 const b = new Set;
-                for (const s of e.notebookItems) {
-                    const e = null === (t = s.metadata) || void 0 === t ? void 0 : t.kernel;
+                for (const a of e.notebookItems) {
+                    const e = null === (t = a.metadata) || void 0 === t ? void 0 : t.kernel;
                     if (e)
                         for (const t of Object.keys(e)) b.add(t)
                 }
                 const w = [...e.notebookItems, ...e.consoleItems].filter((e => e.starred)),
                     C = e.settings.composite.collapsedSections;
                 return m.createElement("div", {
                     className: "jp-LauncherBody"
                 }, m.createElement("div", {
                     className: "jp-NewLauncher-TopBar"
                 }, m.createElement("div", {
                     className: "jp-Launcher-cwd"
-                }, m.createElement("h3", null, s.__("Current folder:"), " ", m.createElement("code", null, a || "/"))), m.createElement("div", {
+                }, m.createElement("h3", null, a.__("Current folder:"), " ", m.createElement("code", null, n || "/"))), m.createElement("div", {
                     className: "jp-NewLauncher-OtherItems"
-                }, r.map((e => m.createElement(S, {
+                }, o.map((e => m.createElement(S, {
                     item: e,
-                    trans: s
-                }))))), f ? m.createElement("div", {
+                    trans: a
+                }))))), v ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
                 }, m.createElement(c.FilterBox, {
-                    placeholder: s.__("Filter"),
+                    placeholder: a.__("Filter"),
                     updateFilter: (e, t) => {
                         i(null != t ? t : "")
                     },
                     initialQuery: "",
                     useFuzzyFilter: !1
                 })) : null, m.createElement(D, {
                     className: "jp-Launcher-openByType",
-                    title: s.__("Create Empty"),
+                    title: a.__("Create Empty"),
                     icon: h,
                     open: "collapsed" !== C["create-empty"]
-                }, n.filter((e => !l || -1 !== e.label.toLowerCase().indexOf(l.toLowerCase()))).map((e => m.createElement(S, {
+                }, s.filter((e => !l || -1 !== e.label.toLowerCase().indexOf(l.toLowerCase()))).map((e => m.createElement(S, {
                     item: e,
-                    trans: s
+                    trans: a
                 })))), p ? m.createElement(D, {
                     className: "jp-Launcher-openByKernel",
-                    title: s.__("Starred"),
+                    title: a.__("Starred"),
                     icon: u,
                     open: "collapsed" !== C.starred
                 }, w.length > 0 ? m.createElement(L, {
                     items: w,
                     commands: e.commands,
-                    showSearchBox: !f,
+                    showSearchBox: !v,
                     showWidgetType: !0,
                     query: l,
                     settings: e.settings,
-                    trans: s,
+                    trans: a,
                     onClick: e => e.execute()
                 }) : "No starred items") : null, m.createElement(D, {
                     className: "jp-Launcher-openByKernel jp-Launcher-launchNotebook",
-                    title: s.__("Launch Notebook"),
+                    title: a.__("Launch Notebook"),
                     icon: c.notebookIcon,
                     open: "collapsed" !== C["launch-notebook"]
                 }, m.createElement(L, {
                     items: e.notebookItems,
                     commands: e.commands,
-                    showSearchBox: !f,
+                    showSearchBox: !v,
                     query: l,
                     settings: e.settings,
-                    trans: s,
+                    trans: a,
                     onClick: e => e.execute()
                 })), m.createElement(D, {
                     className: "jp-Launcher-openByKernel jp-Launcher-launchConsole",
-                    title: s.__("Launch Console"),
+                    title: a.__("Launch Console"),
                     icon: c.consoleIcon,
                     open: "collapsed" !== C["launch-console"]
                 }, m.createElement(L, {
                     items: e.consoleItems,
                     commands: e.commands,
-                    showSearchBox: !f,
+                    showSearchBox: !v,
                     query: l,
                     settings: e.settings,
-                    trans: s,
+                    trans: a,
                     onClick: e => e.execute()
                 })))
             }
-            class I extends o.Launcher {
+            const I = "server-proxy:open";
+            class N extends r.Launcher {
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
-                        s = e.__("Notebook"),
-                        a = e.__("Console"),
-                        n = [s, a],
-                        r = ["inspector:open"],
-                        o = t.filter((e => r.includes(e.command))).map(this.renderCommand),
-                        l = t.filter((e => !(e.category && n.includes(e.category) || r.includes(e.command)))),
+                        a = e.__("Notebook"),
+                        n = e.__("Console"),
+                        s = [a, n],
+                        o = this._settings.composite.utilityCommands,
+                        r = t.filter((e => o.includes(e.command))).map(this.renderCommand),
+                        l = t.filter((e => (!e.category || !s.includes(e.category)) && !o.includes(e.command) || e.command === I)),
                         i = {
                             "terminal:create-new": 3,
                             "fileeditor:create-new": 6,
                             "fileeditor:create-new-markdown-file": 5
                         };
                     for (const e of l) e.command in i && (e.rank = i[e.command]);
                     const c = [{
                             command: "notebook:create-new",
                             rank: 1
                         }, {
                             command: "console:create",
                             rank: 4
                         }, ...l].sort(((e, t) => {
-                            var s, a;
-                            return (null !== (s = null == e ? void 0 : e.rank) && void 0 !== s ? s : 0) - (null !== (a = null == t ? void 0 : t.rank) && void 0 !== a ? a : 0)
+                            var a, n;
+                            return (null !== (a = null == e ? void 0 : e.rank) && void 0 !== a ? a : 0) - (null !== (n = null == t ? void 0 : t.rank) && void 0 !== n ? n : 0)
                         })),
-                        d = t.filter((e => e.category && e.category === s)).map(this.renderKernelCommand),
-                        u = t.filter((e => e.category && e.category === a)).map(this.renderKernelCommand),
+                        d = t.filter((e => e.category && e.category === a && e.command !== I)).map(this.renderKernelCommand),
+                        u = t.filter((e => e.category && e.category === n && e.command !== I)).map(this.renderKernelCommand),
                         h = c.map(this.renderCommand);
                     return m.createElement(E, {
                         trans: this.trans,
                         cwd: this.cwd,
                         commands: this.commands,
                         typeItems: h,
                         notebookItems: d,
                         consoleItems: u,
-                        otherItems: o,
+                        otherItems: r,
                         settings: this._settings,
                         favouritesChanged: this._favoritesDatabase.changed
                     })
                 }
             }
-            class N extends n.SessionContextDialogs {
+            class U extends s.SessionContextDialogs {
                 constructor(e) {
                     var t;
                     super(e), this.options = e;
-                    const s = null !== (t = e.translator) && void 0 !== t ? t : i.nullTranslator;
-                    this.trans = s.load("jupyterlab")
+                    const a = null !== (t = e.translator) && void 0 !== t ? t : i.nullTranslator;
+                    this.trans = a.load("jupyterlab")
                 }
                 async selectKernel(e) {
                     const t = this.trans;
                     if (e.isDisposed) return Promise.resolve();
-                    let s = t.__("Cancel");
-                    e.hasNoKernel && (s = e.kernelDisplayName);
-                    const a = [n.Dialog.cancelButton({
-                            label: s
-                        }), n.Dialog.okButton({
+                    let a = t.__("Cancel");
+                    e.hasNoKernel && (a = e.kernelDisplayName);
+                    const n = [s.Dialog.cancelButton({
+                            label: a
+                        }), s.Dialog.okButton({
                             label: t.__("Select"),
                             ariaLabel: t.__("Select Kernel"),
                             className: "jp-KernelSelector-SelectButton"
                         })],
-                        r = e.kernelPreference.autoStartDefault,
-                        o = "boolean" == typeof r,
-                        l = await this.options.settingRegistry.load(v),
-                        i = new n.Dialog({
+                        o = e.kernelPreference.autoStartDefault,
+                        r = "boolean" == typeof o,
+                        l = await this.options.settingRegistry.load(_),
+                        i = new s.Dialog({
                             title: t.__("Select Kernel"),
-                            body: new j({
+                            body: new x({
                                 data: {
                                     specs: e.specsManager.specs,
                                     sessions: e.sessionManager.running(),
                                     preference: e.kernelPreference
                                 },
                                 commands: this.options.commands,
                                 favoritesDatabase: this.options.database.favorites,
                                 lastUsedDatabase: this.options.database.lastUsed,
                                 settings: l,
                                 trans: t,
                                 acceptDialog: () => {
                                     i.resolve(1)
                                 }
                             }),
-                            buttons: a,
-                            checkbox: o ? {
+                            buttons: n,
+                            checkbox: r ? {
                                 label: t.__("Always start the preferred kernel"),
                                 caption: t.__("Remember my choice and always start the preferred kernel"),
-                                checked: r
+                                checked: o
                             } : null
                         });
                     i.node.classList.add("jp-KernelSelector-Dialog");
                     const c = await i.launch();
                     if (e.isDisposed || !c.button.accept) return;
-                    o && null !== c.isChecked && (e.kernelPreference = {
+                    r && null !== c.isChecked && (e.kernelPreference = {
                         ...e.kernelPreference,
                         autoStartDefault: c.isChecked
                     });
                     const d = c.value;
                     if (null === d && !e.hasNoKernel) return e.shutdown();
                     d && await e.changeKernel(d)
                 }
             }
-            const U = {
+            const j = {
                 id: "jupyterlab-new-launcher:dialogs",
                 description: "Session dialogs for redesigned JupyterLab launcher",
-                provides: n.ISessionContextDialogs,
+                provides: s.ISessionContextDialogs,
                 autoStart: !0,
                 requires: [i.ITranslator, w, l.ISettingRegistry],
-                activate: (e, t, s, a) => new N({
+                activate: (e, t, a, n) => new U({
                     translator: t,
-                    database: s,
+                    database: a,
                     commands: e.commands,
-                    settingRegistry: a
+                    settingRegistry: n
                 })
             };
-            class j extends n.ReactWidget {
+            class x extends s.ReactWidget {
                 constructor(e) {
                     super(), this.options = e, this.renderKernelCommand = e => new g({
                         item: e,
                         cwd: "",
                         commands: this.commands,
                         lastUsedDatabase: this._lastUsedDatabase,
                         favoritesDatabase: this._favoritesDatabase
@@ -575,73 +585,73 @@
                         const e = this.node.getBoundingClientRect();
                         this.node.style.minWidth = e.width + "px", this.node.style.minHeight = e.height + "px"
                     }))
                 }
                 render() {
                     var e;
                     const t = [],
-                        s = this.options.data.specs.kernelspecs;
-                    for (const e of Object.values(s)) {
+                        a = this.options.data.specs.kernelspecs;
+                    for (const e of Object.values(a)) {
                         if (!e) continue;
-                        const s = e.resources["logo-svg"] || e.resources["logo-64x64"];
+                        const a = e.resources["logo-svg"] || e.resources["logo-64x64"];
                         t.push({
                             command: "notebook:create-new",
                             args: {
                                 isLauncher: !0,
                                 kernelName: e.name
                             },
-                            kernelIconUrl: s,
+                            kernelIconUrl: a,
                             metadata: {
-                                kernel: _.JSONExt.deepCopy(e.metadata || {})
+                                kernel: f.JSONExt.deepCopy(e.metadata || {})
                             }
                         })
                     }
-                    const a = [];
+                    const n = [];
                     for (const t of this.options.data.sessions) {
-                        const n = t.kernel;
-                        if (!n) continue;
-                        const r = s[n.name],
-                            o = r.resources["logo-svg"] || r.resources["logo-64x64"];
-                        a.push({
+                        const s = t.kernel;
+                        if (!s) continue;
+                        const o = a[s.name],
+                            r = o.resources["logo-svg"] || o.resources["logo-64x64"];
+                        n.push({
                             command: "notebook:create-new",
                             args: {
                                 isLauncher: !0,
-                                kernelName: r.name
+                                kernelName: o.name
                             },
-                            kernelIconUrl: o,
+                            kernelIconUrl: r,
                             metadata: {
                                 kernel: {
-                                    ..._.JSONExt.deepCopy(r.metadata || {}),
-                                    state: null !== (e = n.execution_state) && void 0 !== e ? e : "running",
+                                    ...f.JSONExt.deepCopy(o.metadata || {}),
+                                    state: null !== (e = s.execution_state) && void 0 !== e ? e : "running",
                                     "used by": t.name
                                 },
-                                model: n
+                                model: s
                             }
                         })
                     }
-                    const n = t.map(this.renderKernelCommand),
-                        r = a.map(this.renderKernelCommand);
+                    const s = t.map(this.renderKernelCommand),
+                        o = n.map(this.renderKernelCommand);
                     return m.createElement(m.Fragment, null, m.createElement("h3", {
                         className: "jp-KernelSelector-Section"
                     }, this.trans.__("Start a new kernel")), m.createElement(L, {
                         trans: this.trans,
                         commands: this.commands,
-                        items: n,
+                        items: s,
                         settings: this._settings,
                         query: "",
                         showSearchBox: !0,
                         onClick: e => {
                             this._selection = e, this.options.acceptDialog()
                         }
-                    }), r.length > 0 ? m.createElement(m.Fragment, null, m.createElement("h3", {
+                    }), o.length > 0 ? m.createElement(m.Fragment, null, m.createElement("h3", {
                         className: "jp-KernelSelector-Section"
                     }, this.trans.__("Connect to a running kernel")), m.createElement(L, {
                         trans: this.trans,
                         commands: this.commands,
-                        items: r,
+                        items: o,
                         settings: this._settings,
                         query: "",
                         showSearchBox: !1,
                         onClick: e => {
                             this._selection = e, this.options.acceptDialog()
                         },
                         hideColumns: ["last-used", "star"]
@@ -650,192 +660,192 @@
                 getValue() {
                     var e;
                     return this._selection ? (null === (e = this._selection.metadata) || void 0 === e ? void 0 : e.model) ? this._selection.metadata.model : {
                         name: this._selection.args.kernelName
                     } : null
                 }
             }
-            var x = s(101);
-            class B {
+            var B = a(101);
+            class K {
                 constructor(e) {
                     this._updateDB = async () => {
                         const e = await this._fetch();
                         this._db = e
                     }, this._db = null, this._stateDB = e.stateDB;
-                    const t = new _.PromiseDelegate;
+                    const t = new f.PromiseDelegate;
                     this.ready = t.promise, this._updateDB().then((() => t.resolve())), window.setInterval(this._updateDB, e.fetchInterval)
                 }
                 _get(e) {
                     return this._db ? this._db[this._itemKey(e)] : (console.error("Database is not ready!"), null)
                 }
                 async _set(e, t) {
-                    const s = await this._fetch();
-                    this._db = s, s[this._itemKey(e)] = t, await this._stateDB.save(this._stateDBKey, s)
+                    const a = await this._fetch();
+                    this._db = a, a[this._itemKey(e)] = t, await this._stateDB.save(this._stateDBKey, a)
                 }
                 async _fetch() {
                     let e = await this._stateDB.fetch(this._stateDBKey);
                     return void 0 === e && (e = await this._stateDB.fetch(this._stateDBKey)), void 0 === e ? {} : e
                 }
             }
-            class K extends B {
+            class T extends K {
                 _itemKey(e) {
                     return e.command + "_" + JSON.stringify(e.args)
                 }
             }
-            class T extends K {
+            class A extends T {
                 constructor() {
                     super(...arguments), this._stateDBKey = "new-launcher:last-used"
                 }
                 get(e) {
                     const t = super._get(e);
                     return t ? new Date(t) : null
                 }
                 async recordAsUsedNow(e) {
                     this._set(e, (new Date).toUTCString())
                 }
             }
-            class A extends K {
+            class R extends T {
                 constructor() {
                     super(...arguments), this._stateDBKey = "new-launcher:favorites", this._changed = new p.Signal(this)
                 }
                 get(e) {
                     var t;
                     return null !== (t = super._get(e)) && void 0 !== t ? t : null
                 }
                 async set(e, t) {
                     this._set(e, t), this._changed.emit()
                 }
                 get changed() {
                     return this._changed
                 }
             }
-            const R = {
+            const M = {
                     id: "jupyterlab-new-launcher:database",
                     description: "A redesigned JupyterLab launcher databases",
                     provides: w,
                     autoStart: !0,
-                    requires: [x.IStateDB],
+                    requires: [B.IStateDB],
                     activate: (e, t) => {
-                        const s = {
+                        const a = {
                             stateDB: t,
                             fetchInterval: 1e4
                         };
                         return {
-                            lastUsed: new T(s),
-                            favorites: new A(s)
+                            lastUsed: new A(a),
+                            favorites: new R(a)
                         }
                     }
                 },
-                M = [{
-                    id: v,
+                O = [{
+                    id: _,
                     description: "A redesigned JupyterLab launcher",
-                    provides: o.ILauncher,
+                    provides: r.ILauncher,
                     autoStart: !0,
                     requires: [i.ITranslator, l.ISettingRegistry, w],
-                    optional: [a.ILabShell, n.ICommandPalette, r.IDefaultFileBrowser],
-                    activate: function(e, t, s, a, r, l, i) {
+                    optional: [n.ILabShell, s.ICommandPalette, o.IDefaultFileBrowser],
+                    activate: function(e, t, a, n, o, l, i) {
                         const {
                             commands: m,
                             shell: u
-                        } = e, h = t.load("jupyterlab-new-launcher"), p = new o.LauncherModel;
-                        return s.load(v).then((t => {
-                            ! function(e, t, s) {
+                        } = e, h = t.load("jupyterlab-new-launcher"), p = new r.LauncherModel;
+                        return a.load(_).then((t => {
+                            ! function(e, t, a) {
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
-                                        const a = e.id;
-                                        if (!a) return console.error("Column ID missing");
-                                        const n = null !== (t = s.user.hiddenColumns) && void 0 !== t ? t : {};
-                                        "visible" !== n[a] && n[a] ? n[a] = "visible" : n[a] = "hidden", await s.set("hiddenColumns", n)
+                                        const n = e.id;
+                                        if (!n) return console.error("Column ID missing");
+                                        const s = null !== (t = a.user.hiddenColumns) && void 0 !== t ? t : {};
+                                        "visible" !== s[n] && s[n] ? s[n] = "visible" : s[n] = "hidden", await a.set("hiddenColumns", s)
                                     },
                                     isToggleable: !0,
                                     isToggled: e => {
                                         var t;
-                                        const a = e.id;
-                                        return a ? "hidden" !== (null !== (t = s.user.hiddenColumns) && void 0 !== t ? t : {})[a] : (console.error("Column ID missing for checking if toggled"), !1)
+                                        const n = e.id;
+                                        return n ? "hidden" !== (null !== (t = a.user.hiddenColumns) && void 0 !== t ? t : {})[n] : (console.error("Column ID missing for checking if toggled"), !1)
                                     }
                                 }), e.commands.addCommand(b.moveColumn, {
                                     label: e => "left" === e.direction ? t.__("Move Column Left") : "right" === e.direction ? t.__("Move Column Right") : t.__("Move column left or right"),
                                     execute: async e => {
                                         const t = e.order,
-                                            a = e.id,
-                                            n = t.indexOf(a),
-                                            r = n + ("left" === e.direction ? -1 : 1);
-                                        if (r < 0 || r >= t.length) return void console.log("Cannot move the column any further");
-                                        const o = t[r];
-                                        t[r] = a, t[n] = o, await s.set("columnOrder", t)
+                                            n = e.id,
+                                            s = t.indexOf(n),
+                                            o = s + ("left" === e.direction ? -1 : 1);
+                                        if (o < 0 || o >= t.length) return void console.log("Cannot move the column any further");
+                                        const r = t[o];
+                                        t[o] = n, t[s] = r, await a.set("columnOrder", t)
                                     }
                                 })
                             }(e, h, t)
                         })), m.addCommand(b.create, {
                             label: h.__("New Launcher"),
                             icon: e => e.toolbar ? c.addIcon : void 0,
                             execute: async e => {
-                                var o, l;
-                                const g = null !== (l = null !== (o = e.cwd) && void 0 !== o ? o : null == i ? void 0 : i.model.path) && void 0 !== l ? l : "",
-                                    f = "launcher-" + O.id++,
-                                    _ = await s.load(v);
-                                await Promise.all([a.lastUsed.ready, a.favorites.ready]);
-                                const b = new I({
+                                var r, l;
+                                const g = null !== (l = null !== (r = e.cwd) && void 0 !== r ? r : null == i ? void 0 : i.model.path) && void 0 !== l ? l : "",
+                                    v = "launcher-" + F.id++,
+                                    f = await a.load(_);
+                                await Promise.all([n.lastUsed.ready, n.favorites.ready]);
+                                const b = new N({
                                     model: p,
                                     cwd: g,
                                     callback: e => {
                                         (0, d.find)(u.widgets("main"), (t => t === e)) && (u.add(e, "main", {
-                                            ref: f
+                                            ref: v
                                         }), b.dispose())
                                     },
                                     commands: m,
                                     translator: t,
-                                    lastUsedDatabase: a.lastUsed,
-                                    favoritesDatabase: a.favorites,
-                                    settings: _
+                                    lastUsedDatabase: n.lastUsed,
+                                    favoritesDatabase: n.favorites,
+                                    settings: f
                                 });
                                 b.model = p, b.title.icon = c.launcherIcon, b.title.label = h.__("Launcher");
-                                const w = new n.MainAreaWidget({
+                                const w = new s.MainAreaWidget({
                                     content: b
                                 });
-                                if (w.title.closable = !!Array.from(u.widgets("main")).length, w.id = f, u.add(w, "main", {
+                                if (w.title.closable = !!Array.from(u.widgets("main")).length, w.id = v, u.add(w, "main", {
                                         activate: e.activate,
                                         ref: e.ref
-                                    }), r && r.layoutModified.connect((() => {
-                                        w.title.closable = Array.from(r.widgets("main")).length > 1
+                                    }), o && o.layoutModified.connect((() => {
+                                        w.title.closable = Array.from(o.widgets("main")).length > 1
                                     }), w), i) {
                                     const e = e => {
                                         b.cwd = e.path
                                     };
                                     i.model.pathChanged.connect(e), b.disposed.connect((() => {
                                         i.model.pathChanged.disconnect(e)
                                     }))
                                 }
                                 return w
                             }
-                        }), r && Promise.all([e.restored, null == i ? void 0 : i.model.restored]).then((() => {
-                            r.layoutModified.connect((() => {
-                                r.isEmpty("main") && m.execute(b.create)
+                        }), o && Promise.all([e.restored, null == i ? void 0 : i.model.restored]).then((() => {
+                            o.layoutModified.connect((() => {
+                                o.isEmpty("main") && m.execute(b.create)
                             }))
                         })), l && l.addItem({
                             command: b.create,
                             category: h.__("Launcher")
-                        }), r && (r.addButtonEnabled = !0, r.addRequested.connect(((e, t) => {
-                            var s;
-                            const a = (null === (s = t.currentTitle) || void 0 === s ? void 0 : s.owner.id) || t.titles[t.titles.length - 1].owner.id;
+                        }), o && (o.addButtonEnabled = !0, o.addRequested.connect(((e, t) => {
+                            var a;
+                            const n = (null === (a = t.currentTitle) || void 0 === a ? void 0 : a.owner.id) || t.titles[t.titles.length - 1].owner.id;
                             return m.execute(b.create, {
-                                ref: a
+                                ref: n
                             })
                         }))), p
                     }
-                }, U, R];
-            var O;
+                }, j, M];
+            var F;
             ! function(e) {
                 e.id = 0
-            }(O || (O = {}))
+            }(F || (F = {}))
         }
     }
 ]);
```

### Comparing `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/728.ea49658c85c6542563e2.js` & `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/728.ea49658c85c6542563e2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/remoteEntry.097f22d9f5ab72ff351d.js` & `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/remoteEntry.9b81d6d816ee65d81ed3.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -43,18 +43,18 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        21: "b553ea2f251b3240c2ae",
+        21: "6aebeef0c48d440fad32",
         728: "ea49658c85c6542563e2"
     } [e] + ".js?v=" + {
-        21: "b553ea2f251b3240c2ae",
+        21: "6aebeef0c48d440fad32",
         728: "ea49658c85c6542563e2"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -106,15 +106,15 @@
                     var a = o[e] = o[e] || {},
                         u = a[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
                         get: () => m.e(21).then((() => () => m(21))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-new-launcher", "0.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-new-launcher", "0.2.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_new_launcher-0.2.0/jupyterlab_new_launcher/labextension/static/third-party-licenses.json` & `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/src/commands.ts` & `jupyterlab_new_launcher-0.2.1/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/src/database.ts` & `jupyterlab_new_launcher-0.2.1/src/database.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/src/dialogs.tsx` & `jupyterlab_new_launcher-0.2.1/src/dialogs.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/src/index.ts` & `jupyterlab_new_launcher-0.2.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/src/item.ts` & `jupyterlab_new_launcher-0.2.1/src/item.ts`

 * *Files 18% similar despite different names*

```diff
@@ -36,22 +36,38 @@
     const args = { ...item.args, cwd };
     // base
     this.command = item.command;
     this.args = args;
     this.category = item.category;
     this.rank = item.rank;
     this.kernelIconUrl = item.kernelIconUrl;
-    this.metadata = item.metadata;
+    this.metadata = item.metadata ?? {};
     // custom
     this.iconClass = commands.iconClass(item.command, args);
     this.icon = commands.icon(item.command, args);
     this.caption = commands.caption(item.command, args);
     this.label = commands.label(item.command, args);
     this.lastUsed = lastUsedDatabase.get(item);
     this.starred = favoritesDatabase.get(item) ?? false;
+    // special handling for conda-store
+    // https://www.nebari.dev/docs/faq/#why-is-there-duplication-in-names-of-environments
+    const condaStoreMatch = (
+      (this.metadata['conda_env_name'] as string | undefined) ?? ''
+    ).match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
+    if (condaStoreMatch && this.metadata) {
+      const groups = condaStoreMatch.groups!;
+      this.label =
+        (this.metadata['conda_language'] as string | undefined) ??
+        groups.environment;
+      this.metadata = {
+        ...this.metadata,
+        conda_env_name: groups.environment,
+        Namespace: groups.namespace
+      };
+    }
   }
   get lastUsed(): Date | null {
     return this._lastUsed;
   }
   set lastUsed(value: Date | null) {
     this._lastUsed = value;
     this._setRefreshClock();
```

### Comparing `jupyterlab_new_launcher-0.2.0/src/launcher.tsx` & `jupyterlab_new_launcher-0.2.1/src/launcher.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -208,14 +208,16 @@
   export interface IOptions extends ILauncher.IOptions {
     lastUsedDatabase: ILastUsedDatabase;
     favoritesDatabase: IFavoritesDatabase;
     settings: ISettingRegistry.ISettings;
   }
 }
 
+const SERVER_PROXY_COMMAND = 'server-proxy:open';
+
 export class NewLauncher extends Launcher {
   constructor(options: NewLauncher.IOptions) {
     super(options);
     this.commands = options.commands;
     this.trans = this.translator.load('jupyterlab-new-launcher');
     this._lastUsedDatabase = options.lastUsedDatabase;
     this._favoritesDatabase = options.favoritesDatabase;
@@ -252,25 +254,27 @@
     const trans = this.trans;
     const items = [...this.model.items()];
 
     const notebookCategory = trans.__('Notebook');
     const consoleCategory = trans.__('Console');
     const kernelCategories = [notebookCategory, consoleCategory];
 
-    const otherCommands = ['inspector:open'];
+    const otherCommands = this._settings.composite
+      .utilityCommands as ISettingsLayout['utilityCommands'];
 
     const otherItems = items
       .filter(item => otherCommands.includes(item.command))
       .map(this.renderCommand);
 
     // TODO: maybe better to filter out everything from default lab and re-populate the kernel categories manually to get more metadata?
     const nonKernelItems = items.filter(
       item =>
-        (!item.category || !kernelCategories.includes(item.category)) &&
-        !otherCommands.includes(item.command)
+        ((!item.category || !kernelCategories.includes(item.category)) &&
+          !otherCommands.includes(item.command)) ||
+        item.command === SERVER_PROXY_COMMAND
     );
     const rankOverrides = {
       'terminal:create-new': 3, // TODO: replace with terminal which asks for environment choice?
       'fileeditor:create-new': 6,
       'fileeditor:create-new-markdown-file': 5
     };
     for (const item of nonKernelItems) {
@@ -287,19 +291,29 @@
         command: 'console:create',
         rank: 4
       },
       ...nonKernelItems
     ].sort((a, b) => (a?.rank ?? 0) - (b?.rank ?? 0));
 
     const notebookItems = items
-      .filter(item => item.category && item.category === notebookCategory)
+      .filter(
+        item =>
+          item.category &&
+          item.category === notebookCategory &&
+          item.command !== SERVER_PROXY_COMMAND
+      )
       .map(this.renderKernelCommand);
 
     const consoleItems = items
-      .filter(item => item.category && item.category === consoleCategory)
+      .filter(
+        item =>
+          item.category &&
+          item.category === consoleCategory &&
+          item.command !== SERVER_PROXY_COMMAND
+      )
       .map(this.renderKernelCommand);
 
     // TODO: only create items once or if changed; dispose of them too
     const typeItems: IItem[] = typeCommands.map(this.renderCommand);
 
     return (
       <LauncherBody
```

### Comparing `jupyterlab_new_launcher-0.2.0/src/types.ts` & `jupyterlab_new_launcher-0.2.1/src/types.ts`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 export interface ISettingsLayout {
   hiddenColumns: Record<string, 'visible' | 'hidden'>;
   columnOrder: string[];
   starredSection: boolean;
   collapsedSections: Record<string, 'collapsed' | 'expanded'>;
   searchAllSections: boolean;
+  utilityCommands: string[];
 }
 
 export interface IItem extends ILauncher.IItemOptions {
   label: string;
   caption: string;
   icon: VirtualElement.IRenderer | undefined;
   iconClass: string;
```

### Comparing `jupyterlab_new_launcher-0.2.0/src/components/card.tsx` & `jupyterlab_new_launcher-0.2.1/src/components/card.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/src/components/section.tsx` & `jupyterlab_new_launcher-0.2.1/src/components/section.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/src/components/table.tsx` & `jupyterlab_new_launcher-0.2.1/src/components/table.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/style/base.css` & `jupyterlab_new_launcher-0.2.1/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/style/icons/md/LICENSE` & `jupyterlab_new_launcher-0.2.1/style/icons/md/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/ui-tests/README.md` & `jupyterlab_new_launcher-0.2.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/ui-tests/yarn.lock` & `jupyterlab_new_launcher-0.2.1/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts` & `jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png` & `jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png` & `jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png` & `jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/.gitignore` & `jupyterlab_new_launcher-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/LICENSE` & `jupyterlab_new_launcher-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/README.md` & `jupyterlab_new_launcher-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/pyproject.toml` & `jupyterlab_new_launcher-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.0/PKG-INFO` & `jupyterlab_new_launcher-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-new-launcher
-Version: 0.2.0
+Version: 0.2.1
 Dynamic: Keywords
 Summary: A redesigned JupyterLab launcher
 Project-URL: Homepage, https://github.com/nebari-dev/jupyterlab-new-launcher
 Project-URL: Bug Tracker, https://github.com/nebari-dev/jupyterlab-new-launcher/issues
 Project-URL: Repository, https://github.com/nebari-dev/jupyterlab-new-launcher.git
 Author-email: Nebari development team <internal-it@quansight.com>
 License: BSD 3-Clause License
```

