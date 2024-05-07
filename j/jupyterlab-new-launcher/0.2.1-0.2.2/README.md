# Comparing `tmp/jupyterlab_new_launcher-0.2.1.tar.gz` & `tmp/jupyterlab_new_launcher-0.2.2.tar.gz`

## Comparing `jupyterlab_new_launcher-0.2.1.tar` & `jupyterlab_new_launcher-0.2.2.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/.copier-answers.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/babel.config.js
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jest.config.js
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/junit.xml
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/setup.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/tsconfig.test.json
--rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/yarn.lock
--rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/docs/images/dialog.png
--rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/docs/images/launcher.png
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/_version.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/package.json
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
--rw-r--r--   0        0        0    21502 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/21.6aebeef0c48d440fad32.js
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/728.ea49658c85c6542563e2.js
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/remoteEntry.9b81d6d816ee65d81ed3.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/schema/plugin.json
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/commands.ts
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/database.ts
--rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/dialogs.tsx
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/icons.ts
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/index.ts
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/item.ts
--rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/launcher.tsx
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/svg.d.ts
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/types.ts
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/__tests__/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/components/card.tsx
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/components/section.tsx
--rw-r--r--   0        0        0    11435 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/src/components/table.tsx
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/style/index.js
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/style/icons/md/LICENSE
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/style/icons/md/file.svg
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/style/icons/md/star.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/yarn.lock
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0    26996 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
--rw-r--r--   0        0        0    27431 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
--rw-r--r--   0        0        0    33351 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/LICENSE
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/README.md
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/.copier-answers.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/babel.config.js
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/jest.config.js
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/junit.xml
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/setup.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/tsconfig.test.json
+-rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/yarn.lock
+-rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/docs/images/dialog.png
+-rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/docs/images/launcher.png
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/_version.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/package.json
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
+-rw-r--r--   0        0        0    24925 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/static/239.eba35c75272592009997.js
+-rw-r--r--   0        0        0     9025 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/static/728.fa379db84cb7d3fbc55e.js
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/static/remoteEntry.2e1e8df64ea6f9bac940.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/schema/plugin.json
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/src/commands.ts
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/src/database.ts
+-rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/src/dialogs.tsx
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/src/icons.ts
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/src/index.ts
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/src/item.ts
+-rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/src/launcher.tsx
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/src/svg.d.ts
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/src/types.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/src/__tests__/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/src/components/card.tsx
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/src/components/section.tsx
+-rw-r--r--   0        0        0    11435 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/src/components/table.tsx
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/style/index.js
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/style/icons/code-server.svg
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/style/icons/md/LICENSE
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/style/icons/md/file.svg
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/style/icons/md/star.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0    26996 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
+-rw-r--r--   0        0        0    27431 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
+-rw-r--r--   0        0        0    33351 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/README.md
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.2/PKG-INFO
```

### Comparing `jupyterlab_new_launcher-0.2.1/.copier-answers.yml` & `jupyterlab_new_launcher-0.2.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/RELEASE.md` & `jupyterlab_new_launcher-0.2.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/jest.config.js` & `jupyterlab_new_launcher-0.2.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/package.json` & `jupyterlab_new_launcher-0.2.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_new_launcher-0.2.1/tsconfig.json` & `jupyterlab_new_launcher-0.2.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/yarn.lock` & `jupyterlab_new_launcher-0.2.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/docs/images/dialog.png` & `jupyterlab_new_launcher-0.2.2/docs/images/dialog.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/docs/images/launcher.png` & `jupyterlab_new_launcher-0.2.2/docs/images/launcher.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/__init__.py` & `jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/package.json` & `jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.2e1e8df64ea6f9bac940.js'}}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -108,15 +108,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/nebari-dev/jupyterlab-new-launcher",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9b81d6d816ee65d81ed3.js",
+            "load": "static/remoteEntry.2e1e8df64ea6f9bac940.js",
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
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig` & `jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json` & `jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/21.6aebeef0c48d440fad32.js` & `jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/static/239.eba35c75272592009997.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,110 +1,119 @@
 "use strict";
 (self.webpackChunkjupyterlab_new_launcher = self.webpackChunkjupyterlab_new_launcher || []).push([
-    [21], {
-        21: (e, t, a) => {
-            a.r(t), a.d(t, {
-                default: () => O
+    [239], {
+        239: (e, t, n) => {
+            n.r(t), n.d(t, {
+                default: () => F
             });
-            var n = a(626),
-                s = a(923),
-                o = a(670),
-                r = a(260),
-                l = a(825),
-                i = a(265),
-                c = a(527),
-                d = a(53),
-                m = a(345);
-            const u = new c.LabIcon({
+            var a = n(626),
+                s = n(923),
+                o = n(670),
+                r = n(260),
+                l = n(825),
+                c = n(265),
+                i = n(527),
+                d = n(53),
+                m = n(345);
+            const u = new i.LabIcon({
                     name: "jupyterlab-new-launcher:star",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">\n  <path class="jp-icon3 jp-star-filled" fill="rgb(97,97,97)" d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z" />\n  <path class="jp-icon3 jp-star-border" fill="rgb(97,97,97)" d="M22 9.24l-7.19-.62L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21 12 17.27 18.18 21l-1.63-7.03L22 9.24zM12 15.4l-3.76 2.27 1-4.28-3.32-2.88 4.38-.38L12 6.1l1.71 4.04 4.38.38-3.32 2.88 1 4.28L12 15.4z" />\n</svg>\n'
                 }),
-                h = new c.LabIcon({
+                h = new i.LabIcon({
                     name: "jupyterlab-new-launcher:file",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">\n  <path class="jp-icon3" fill="rgb(97,97,97)" d="M13.81 22H6C4.89 22 4 21.11 4 20V4C4 2.9 4.89 2 6 2H14L20 8V13.09C19.67 13.04 19.34 13 19 13S18.33 13.04 18 13.09V9H13V4H6V20H13.09C13.21 20.72 13.46 21.39 13.81 22M23 18H20V15H18V18H15V20H18V23H20V20H23V18Z" />\n</svg>'
+                }),
+                p = new i.LabIcon({
+                    name: "jupyterlab-new-launcher:code-server",
+                    svgstr: '<svg width="64" viewBox="0 0 2250 2250" version="1.1" xmlns="http://www.w3.org/2000/svg" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;">\n<g class="jp-icon0" fill="#000" style="fill-rule:nonzero;">\n  <path d="M1991.66,1034.72c-38.493,0 -64.144,-22.57 -64.144,-68.897l-0,-266.084c-0,-169.867 -69.982,-263.709 -250.762,-263.709l-83.976,0l-0,179.368l25.661,0c71.144,0 104.967,39.201 104.967,109.285l0,235.201c0,102.156 30.324,143.733 96.806,165.114c-66.482,20.196 -96.806,62.958 -96.806,165.114l0,174.621c0,48.7 0,96.216 -12.829,144.917c-12.829,45.141 -33.823,87.903 -62.98,124.726c-16.329,21.386 -34.991,39.202 -55.981,55.835l-0,23.755l83.971,-0c180.781,-0 250.763,-93.843 250.763,-263.709l-0,-266.084c-0,-47.516 24.485,-68.897 64.144,-68.897l47.822,-0l-0,-179.37l-46.656,-0l0,-1.186Z"/>\n  <path d="M1420.16,706.904l-258.923,0c-5.833,0 -10.495,-4.752 -10.495,-10.691l-0,-20.192c-0,-5.941 4.662,-10.692 10.495,-10.692l260.089,0c5.83,0 10.495,4.751 10.495,10.692l0,20.192c0,5.939 -5.833,10.691 -11.661,10.691Z" />\n  <path d="M1464.48,963.474l-188.942,0c-5.833,0 -10.501,-4.754 -10.501,-10.693l0,-20.192c0,-5.938 4.668,-10.691 10.501,-10.691l188.942,-0c5.833,-0 10.495,4.753 10.495,10.691l-0,20.192c-0,4.754 -4.662,10.693 -10.495,10.693Z"/>\n  <path d="M1539.12,835.188l-377.885,0c-5.833,0 -10.495,-4.75 -10.495,-10.689l-0,-20.196c-0,-5.939 4.662,-10.69 10.495,-10.69l376.719,0c5.833,0 10.499,4.751 10.499,10.69l-0,20.196c-0,4.75 -3.5,10.689 -9.333,10.689Z"/>\n  <path d="M861.493,765.074c25.658,0 51.319,2.376 75.811,8.316l0,-48.705c0,-68.897 34.989,-109.285 104.971,-109.285l25.658,0l-0,-179.368l-83.977,0c-180.781,0 -250.758,93.842 -250.758,263.709l0,87.901c40.819,-14.252 83.977,-22.568 128.295,-22.568Z"/>\n  <path d="M1618.44,1411.25c-18.662,-150.861 -132.962,-276.776 -279.919,-305.285c-40.818,-8.314 -81.642,-9.504 -121.295,-2.376c-1.166,-0 -1.166,-1.189 -2.332,-1.189c-64.148,-136.605 -201.772,-226.884 -351.063,-226.884c-149.289,-0 -285.747,87.905 -351.062,224.51c-1.166,-0 -1.166,1.188 -2.332,1.188c-41.987,-4.753 -83.975,-2.379 -125.963,8.314c-144.623,35.634 -254.257,159.175 -274.085,308.847c-2.332,15.441 -3.499,30.883 -3.499,45.141c0,45.136 30.325,86.713 74.645,92.652c54.817,8.317 102.636,-34.448 101.469,-89.089c0,-8.317 0,-17.821 1.167,-26.134c9.331,-76.025 66.48,-140.168 141.123,-157.99c23.328,-5.939 46.654,-7.124 68.814,-3.559c71.146,9.502 141.124,-27.324 171.449,-91.467c22.162,-47.516 57.151,-89.094 103.804,-111.664c51.314,-24.946 109.633,-28.506 163.286,-9.499c55.979,20.192 97.966,62.954 123.627,116.409c26.824,52.27 39.653,89.093 96.805,96.221c23.325,3.559 88.639,2.374 113.132,1.185c47.82,0 95.64,16.631 129.463,51.079c22.156,23.757 38.485,53.455 45.486,86.715c10.495,53.455 -2.334,106.908 -33.825,147.296c-22.162,28.509 -52.485,49.89 -86.308,59.394c-16.329,4.754 -32.657,5.939 -48.986,5.939l-257.757,0c-51.314,0 -92.138,-41.573 -92.138,-93.842l0,-348.049c0,-14.251 -11.661,-26.13 -25.658,-26.13l-36.156,0c-71.148,1.185 -128.295,81.964 -128.295,167.488l-0,312.415c-0,92.652 73.476,167.488 164.451,167.488c0,0 404.714,-1.19 410.544,-1.19c93.304,-9.503 179.614,-58.204 237.927,-133.04c58.319,-72.46 85.142,-167.492 73.481,-264.894Z"/>\n</g></svg>'
                 });
-            var p = a(602);
-            class g {
+            var g = n(602);
+            class v {
                 constructor(e) {
-                    var t, a, n, s;
-                    this._options = e, this._refreshLastUsed = new p.Signal(this), this._refreshClock = null, this._lastUsed = null;
+                    var t, n, a, s, o;
+                    this._options = e, this._refreshLastUsed = new g.Signal(this), this._refreshClock = null, this._lastUsed = null;
                     const {
-                        item: o,
-                        commands: r,
-                        lastUsedDatabase: l,
+                        item: r,
+                        commands: l,
+                        lastUsedDatabase: c,
                         favoritesDatabase: i,
-                        cwd: c
-                    } = e, d = {
-                        ...o.args,
-                        cwd: c
+                        cwd: d
+                    } = e, m = {
+                        ...r.args,
+                        cwd: d
                     };
-                    this.command = o.command, this.args = d, this.category = o.category, this.rank = o.rank, this.kernelIconUrl = o.kernelIconUrl, this.metadata = null !== (t = o.metadata) && void 0 !== t ? t : {}, this.iconClass = r.iconClass(o.command, d), this.icon = r.icon(o.command, d), this.caption = r.caption(o.command, d), this.label = r.label(o.command, d), this.lastUsed = l.get(o), this.starred = null !== (a = i.get(o)) && void 0 !== a && a;
-                    const m = (null !== (n = this.metadata.conda_env_name) && void 0 !== n ? n : "").match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
-                    if (m && this.metadata) {
-                        const e = m.groups;
-                        this.label = null !== (s = this.metadata.conda_language) && void 0 !== s ? s : e.environment, this.metadata = {
+                    this.command = r.command, this.args = m, this.category = r.category, this.rank = r.rank, this.kernelIconUrl = r.kernelIconUrl, this.metadata = null !== (t = r.metadata) && void 0 !== t ? t : {}, this.iconClass = l.iconClass(r.command, m), this.icon = l.icon(r.command, m), this.caption = l.caption(r.command, m), this.label = l.label(r.command, m), this.lastUsed = c.get(r), this.starred = null !== (n = i.get(r)) && void 0 !== n && n;
+                    const u = this.metadata.kernel,
+                        h = (null !== (a = u.conda_env_name) && void 0 !== a ? a : "").match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
+                    if (h && this.metadata) {
+                        const e = h.groups;
+                        this.label = null !== (s = u.conda_language) && void 0 !== s ? s : e.environment, this.metadata = {
                             ...this.metadata,
-                            conda_env_name: e.environment,
-                            Namespace: e.namespace
+                            kernel: {
+                                ...u,
+                                conda_env_name: e.environment,
+                                Namespace: e.namespace
+                            }
                         }
                     }
+                    "server-proxy:open" === this.command && (null === (o = this.kernelIconUrl) || void 0 === o ? void 0 : o.endsWith("/vscode")) && (this.icon = p)
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
+                        lastUsedDatabase: n
                     } = this._options;
-                    await t.execute(e.command, this.args), await a.recordAsUsedNow(e), this.lastUsed = a.get(e), this._refreshLastUsed.emit()
+                    await t.execute(e.command, this.args), await n.recordAsUsedNow(e), this.lastUsed = n.get(e), this._refreshLastUsed.emit()
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
+                    } = this._options, n = !t.get(e);
+                    return this.starred = n, t.set(e, n)
                 }
                 _setRefreshClock() {
                     const e = this._lastUsed;
                     if (null !== this._refreshClock && (window.clearTimeout(this._refreshClock), this._refreshClock = null), !e) return;
                     const t = Date.now() - e.getTime(),
-                        a = t < 6e4 ? 1e4 : t < 36e5 ? 6e4 : 36e5;
+                        n = t < 6e4 ? 1e4 : t < 36e5 ? 6e4 : 36e5;
                     this._refreshClock = window.setTimeout((() => {
                         this._refreshLastUsed.emit(), this._setRefreshClock()
-                    }), a)
+                    }), n)
                 }
             }
-            var v = a(702),
-                f = a(262);
-            const _ = "jupyterlab-new-launcher:plugin";
-            var b;
+            var f = n(702),
+                _ = n(262);
+            const b = "jupyterlab-new-launcher:plugin";
+            var w;
             ! function(e) {
                 e.create = "launcher:create", e.moveColumn = "new-launcher:table-move-column", e.toggleColumn = "new-launcher:table-toggle-column"
-            }(b || (b = {}));
-            const w = new f.Token("jupyterlab-new-launcher:ILauncherDatabase", "Databases for new launcher."),
+            }(w || (w = {}));
+            const y = new _.Token("jupyterlab-new-launcher:ILauncherDatabase", "Databases for new launcher."),
                 C = "jp-starIconButton",
-                y = "jp-TableKernelItem";
+                k = "jp-TableKernelItem";
 
-            function k(e) {
+            function L(e) {
                 if (0 === e.length) return "(empty)";
                 switch (e) {
                     case "conda_env_name":
                         return "Environment";
                     case "conda_env_path":
                         return "Environment path";
                     case "conda_language":
@@ -115,379 +124,379 @@
                         return "Base?";
                     case "conda_is_currently_running":
                         return "Running?"
                 }
                 return e[0].toUpperCase() + e.substring(1)
             }
 
-            function L(e) {
-                var t, a, n, s;
+            function D(e) {
+                var t, n, a, s;
                 const {
                     trans: o
                 } = e;
                 let r, l;
-                const [i, d] = m.useState("");
-                e.showSearchBox ? (r = i, l = d) : r = e.query;
+                const [c, d] = m.useState("");
+                e.showSearchBox ? (r = c, l = d) : r = e.query;
                 const [, h] = m.useReducer((e => e + 1), 0), p = new Set;
-                for (const a of e.items) {
-                    const e = null === (t = a.metadata) || void 0 === t ? void 0 : t.kernel;
+                for (const n of e.items) {
+                    const e = null === (t = n.metadata) || void 0 === t ? void 0 : t.kernel;
                     if (e)
                         for (const t of Object.keys(e)) p.add(t)
                 }
                 const g = [...p].map((e => ({
                     id: e,
-                    label: k(e),
+                    label: L(e),
                     renderCell: t => {
-                        var a;
-                        const n = null === (a = t.metadata) || void 0 === a ? void 0 : a.kernel;
-                        if (!n) return "-";
-                        const s = n[e];
+                        var n;
+                        const a = null === (n = t.metadata) || void 0 === n ? void 0 : n.kernel;
+                        if (!a) return "-";
+                        const s = a[e];
                         return "string" == typeof s ? s : JSON.stringify(s)
                     },
-                    sort: (t, a) => {
-                        var n, s;
-                        const o = null === (n = t.metadata) || void 0 === n ? void 0 : n.kernel,
-                            r = null === (s = a.metadata) || void 0 === s ? void 0 : s.kernel,
+                    sort: (t, n) => {
+                        var a, s;
+                        const o = null === (a = t.metadata) || void 0 === a ? void 0 : a.kernel,
+                            r = null === (s = n.metadata) || void 0 === s ? void 0 : s.kernel,
                             l = o ? o[e] : void 0,
-                            i = r ? r[e] : void 0;
-                        return l === i ? 0 : l ? i ? "string" == typeof l && "string" == typeof i ? l.localeCompare(i) : l > i ? 1 : -1 : -1 : 1
+                            c = r ? r[e] : void 0;
+                        return l === c ? 0 : l ? c ? "string" == typeof l && "string" == typeof c ? l.localeCompare(c) : l > c ? 1 : -1 : -1 : 1
                     }
                 })));
                 e.showWidgetType && g.push({
                     id: "widget-type",
                     label: o.__("Type"),
                     renderCell: e => e.command.split(":")[0],
                     sort: (e, t) => e.command.localeCompare(t.command)
                 });
-                const f = [{
+                const v = [{
                         id: "kernel",
                         label: o.__("Kernel"),
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
-                            className: y,
-                            onClick: a => {
-                                e.onClick(t), a.stopPropagation()
+                            className: k,
+                            onClick: n => {
+                                e.onClick(t), n.stopPropagation()
                             },
                             onKeyDown: e => {
                                 "Enter" === e.key && t.execute()
                             },
                             tabIndex: 0
                         }, t.label)),
                         sort: (e, t) => e.label.localeCompare(t.label)
                     }, ...g, {
                         id: "last-used",
                         label: o.__("Last Used"),
-                        renderCell: e => m.createElement(c.UseSignal, {
+                        renderCell: e => m.createElement(i.UseSignal, {
                             signal: e.refreshLastUsed
                         }, (() => e.lastUsed ? m.createElement("span", {
-                            title: v.Time.format(e.lastUsed)
-                        }, v.Time.formatHuman(e.lastUsed)) : o.__("Never"))),
+                            title: f.Time.format(e.lastUsed)
+                        }, f.Time.formatHuman(e.lastUsed)) : o.__("Never"))),
                         sort: (e, t) => e.lastUsed === t.lastUsed ? 0 : e.lastUsed ? t.lastUsed && e.lastUsed > t.lastUsed ? 1 : -1 : 1
                     }, {
                         id: "star",
                         label: "",
                         renderCell: e => {
                             const t = e.starred,
-                                a = t ? o.__("Click to add this kernel to favourites") : o.__("Click to remove the kernel from favourites");
+                                n = t ? o.__("Click to add this kernel to favourites") : o.__("Click to remove the kernel from favourites");
                             return m.createElement("button", {
                                 className: t ? `${C} jp-mod-starred` : C,
-                                title: a,
+                                title: n,
                                 onClick: t => {
                                     e.toggleStar(), h(), t.stopPropagation()
                                 }
                             }, m.createElement(u.react, {
                                 className: "jp-starIcon"
                             }))
                         },
                         sort: (e, t) => Number(e.starred) - Number(t.starred)
                     }],
-                    _ = null !== (a = e.hideColumns) && void 0 !== a ? a : [],
-                    w = f.filter((e => !_.includes(e.id))),
-                    [L, D] = m.useState(null !== (n = e.settings.composite.hiddenColumns) && void 0 !== n ? n : {}),
-                    S = w.map((e => e.id)),
+                    _ = null !== (n = e.hideColumns) && void 0 !== n ? n : [],
+                    b = v.filter((e => !_.includes(e.id))),
+                    [y, D] = m.useState(null !== (a = e.settings.composite.hiddenColumns) && void 0 !== a ? a : {}),
+                    S = b.map((e => e.id)),
                     [E, I] = m.useState(null !== (s = e.settings.composite.columnOrder) && void 0 !== s ? s : S),
-                    N = c.Table,
-                    U = () => {
-                        var t, a;
-                        const n = null !== (t = e.settings.composite.hiddenColumns) && void 0 !== t ? t : {};
-                        L !== n && D(n);
-                        const s = null !== (a = e.settings.composite.columnOrder) && void 0 !== a ? a : S;
+                    j = i.Table,
+                    N = () => {
+                        var t, n;
+                        const a = null !== (t = e.settings.composite.hiddenColumns) && void 0 !== t ? t : {};
+                        y !== a && D(a);
+                        const s = null !== (n = e.settings.composite.columnOrder) && void 0 !== n ? n : S;
                         E !== s && I(s)
                     };
-                return m.useEffect((() => (e.settings.changed.connect(U), () => {
-                    e.settings.changed.disconnect(U)
+                return m.useEffect((() => (e.settings.changed.connect(N), () => {
+                    e.settings.changed.disconnect(N)
                 }))), m.createElement("div", {
                     className: "jp-NewLauncher-table"
                 }, e.showSearchBox ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
-                }, m.createElement(c.FilterBox, {
+                }, m.createElement(i.FilterBox, {
                     placeholder: o.__("Filter kernels"),
                     updateFilter: (e, t) => {
                         l(null != t ? t : "")
                     },
                     initialQuery: "",
                     useFuzzyFilter: !1
                 })) : null, m.createElement("div", {
                     className: "jp-NewLauncher-table-scroller",
                     onContextMenu: t => {
-                        var a;
+                        var n;
                         t.preventDefault();
-                        const n = new c.MenuSvg({
+                        const a = new i.MenuSvg({
                                 commands: e.commands
                             }),
-                            s = new c.MenuSvg({
+                            s = new i.MenuSvg({
                                 commands: e.commands
                             });
-                        for (const e of w) s.addItem({
-                            command: b.toggleColumn,
+                        for (const e of b) s.addItem({
+                            command: w.toggleColumn,
                             args: {
                                 id: e.id,
                                 label: e.label
                             }
                         });
-                        s.title.label = o.__("Visible Columns"), n.addItem({
+                        s.title.label = o.__("Visible Columns"), a.addItem({
                             type: "submenu",
                             submenu: s
                         });
-                        const r = null === (a = t.target.closest("th[data-id]")) || void 0 === a ? void 0 : a.dataset.id;
-                        r && (n.addItem({
-                            command: b.moveColumn,
+                        const r = null === (n = t.target.closest("th[data-id]")) || void 0 === n ? void 0 : n.dataset.id;
+                        r && (a.addItem({
+                            command: w.moveColumn,
                             args: {
                                 direction: "left",
                                 order: E,
                                 id: r
                             }
-                        }), n.addItem({
-                            command: b.moveColumn,
+                        }), a.addItem({
+                            command: w.moveColumn,
                             args: {
                                 direction: "right",
                                 order: E,
                                 id: r
                             }
-                        })), n.open(t.clientX, t.clientY)
+                        })), a.open(t.clientX, t.clientY)
                     }
-                }, m.createElement(N, {
+                }, m.createElement(j, {
                     rows: e.items.filter((e => -1 !== e.label.toLowerCase().indexOf(r.toLowerCase()))).map((e => ({
                         data: e,
                         key: e.command + JSON.stringify(e.args)
                     }))),
                     blankIndicator: () => m.createElement("div", null, o.__("No entries")),
                     sortKey: "kernel",
                     onRowClick: e => {
                         const t = e.target,
-                            a = t.closest("tr");
-                        if (!a) return;
-                        const n = t.closest("td"),
-                            s = null == n ? void 0 : n.querySelector(`.${C}`);
+                            n = t.closest("tr");
+                        if (!n) return;
+                        const a = t.closest("td"),
+                            s = null == a ? void 0 : a.querySelector(`.${C}`);
                         if (s) return s.click();
-                        a.querySelector(`.${y}`).click()
+                        n.querySelector(`.${k}`).click()
                     },
-                    columns: w.filter((e => "hidden" !== L[e.id])).map((e => {
+                    columns: b.filter((e => "hidden" !== y[e.id])).map((e => {
                         var t;
                         return {
                             ...e,
                             rank: null !== (t = E.indexOf(e.id)) && void 0 !== t ? t : 10
                         }
                     })).sort(((e, t) => e.rank - t.rank))
                 })))
             }
 
-            function D(e) {
-                const [t, a] = m.useState(e.open);
+            function S(e) {
+                const [t, n] = m.useState(e.open);
                 return m.createElement("details", {
                     onToggle: t => {
-                        a(t.currentTarget.open), e.onToggled && e.onToggled(t.currentTarget.open)
+                        n(t.currentTarget.open), e.onToggled && e.onToggled(t.currentTarget.open)
                     },
-                    className: (0, c.classes)(e.className, "jp-CollapsibleSection"),
+                    className: (0, i.classes)(e.className, "jp-CollapsibleSection"),
                     open: t
                 }, m.createElement("summary", null, m.createElement("div", {
                     className: "jp-CollapsibleSection-CollapserIconWrapper",
                     "aria-hidden": "true"
-                }, m.createElement(c.caretRightIcon.react, {
+                }, m.createElement(i.caretRightIcon.react, {
                     className: "jp-CollapsibleSection-CollapserIcon"
                 })), m.createElement(e.icon.react, {
                     tag: "span",
                     className: "jp-CollapsibleSection-CategoryIcon"
                 }), m.createElement("h3", {
                     className: "jp-CollapsibleSection-Title"
                 }, e.title)), m.createElement("div", {
                     className: "jp-Launcher-CardGroup jp-Launcher-cardContainer"
                 }, e.children))
             }
 
-            function S(e) {
+            function E(e) {
                 const {
                     item: t
                 } = e;
                 return m.createElement("div", {
                     onClick: () => t.execute(),
                     className: "jp-Launcher-TypeCard jp-LauncherCard",
                     title: t.caption,
                     tabIndex: 0
                 }, m.createElement("div", {
                     className: "jp-LauncherCard-icon"
-                }, m.createElement(c.LabIcon.resolveReact, {
+                }, m.createElement(i.LabIcon.resolveReact, {
                     icon: t.icon,
-                    iconClass: (0, c.classes)(t.iconClass, "jp-Icon-cover")
+                    iconClass: (0, i.classes)(t.iconClass, "jp-Icon-cover")
                 })), m.createElement("div", {
                     className: "jp-LauncherCard-label"
                 }, m.createElement("p", null, t.label)))
             }
 
-            function E(e) {
+            function I(e) {
                 var t;
                 const {
-                    trans: a,
-                    cwd: n,
+                    trans: n,
+                    cwd: a,
                     typeItems: s,
                     otherItems: o,
                     favouritesChanged: r
-                } = e, [l, i] = m.useState(""), [, d] = m.useReducer((e => e + 1), 0), [p, g] = m.useState(e.settings.composite.starredSection), [v, f] = m.useState(e.settings.composite.searchAllSections), _ = () => {
+                } = e, [l, c] = m.useState(""), [, d] = m.useReducer((e => e + 1), 0), [p, g] = m.useState(e.settings.composite.starredSection), [v, f] = m.useState(e.settings.composite.searchAllSections), _ = () => {
                     const t = e.settings.composite.starredSection;
                     p !== t && g(t);
-                    const a = e.settings.composite.searchAllSections;
-                    v !== a && f(a)
+                    const n = e.settings.composite.searchAllSections;
+                    v !== n && f(n)
                 };
                 if (m.useEffect((() => (e.settings.changed.connect(_), () => {
                         e.settings.changed.disconnect(_)
                     }))), r) {
                     const e = () => {
                         p && d()
                     };
                     m.useEffect((() => (r.connect(e), () => {
                         r.disconnect(e)
                     })))
                 }
                 const b = new Set;
-                for (const a of e.notebookItems) {
-                    const e = null === (t = a.metadata) || void 0 === t ? void 0 : t.kernel;
+                for (const n of e.notebookItems) {
+                    const e = null === (t = n.metadata) || void 0 === t ? void 0 : t.kernel;
                     if (e)
                         for (const t of Object.keys(e)) b.add(t)
                 }
                 const w = [...e.notebookItems, ...e.consoleItems].filter((e => e.starred)),
-                    C = e.settings.composite.collapsedSections;
+                    y = e.settings.composite.collapsedSections;
                 return m.createElement("div", {
                     className: "jp-LauncherBody"
                 }, m.createElement("div", {
                     className: "jp-NewLauncher-TopBar"
                 }, m.createElement("div", {
                     className: "jp-Launcher-cwd"
-                }, m.createElement("h3", null, a.__("Current folder:"), " ", m.createElement("code", null, n || "/"))), m.createElement("div", {
+                }, m.createElement("h3", null, n.__("Current folder:"), " ", m.createElement("code", null, a || "/"))), m.createElement("div", {
                     className: "jp-NewLauncher-OtherItems"
-                }, o.map((e => m.createElement(S, {
+                }, o.map((e => m.createElement(E, {
                     item: e,
-                    trans: a
+                    trans: n
                 }))))), v ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
-                }, m.createElement(c.FilterBox, {
-                    placeholder: a.__("Filter"),
+                }, m.createElement(i.FilterBox, {
+                    placeholder: n.__("Filter"),
                     updateFilter: (e, t) => {
-                        i(null != t ? t : "")
+                        c(null != t ? t : "")
                     },
                     initialQuery: "",
                     useFuzzyFilter: !1
-                })) : null, m.createElement(D, {
+                })) : null, m.createElement(S, {
                     className: "jp-Launcher-openByType",
-                    title: a.__("Create Empty"),
+                    title: n.__("Create Empty"),
                     icon: h,
-                    open: "collapsed" !== C["create-empty"]
-                }, s.filter((e => !l || -1 !== e.label.toLowerCase().indexOf(l.toLowerCase()))).map((e => m.createElement(S, {
+                    open: "collapsed" !== y["create-empty"]
+                }, s.filter((e => !l || -1 !== e.label.toLowerCase().indexOf(l.toLowerCase()))).map((e => m.createElement(E, {
                     item: e,
-                    trans: a
-                })))), p ? m.createElement(D, {
+                    trans: n
+                })))), p ? m.createElement(S, {
                     className: "jp-Launcher-openByKernel",
-                    title: a.__("Starred"),
+                    title: n.__("Starred"),
                     icon: u,
-                    open: "collapsed" !== C.starred
-                }, w.length > 0 ? m.createElement(L, {
+                    open: "collapsed" !== y.starred
+                }, w.length > 0 ? m.createElement(D, {
                     items: w,
                     commands: e.commands,
                     showSearchBox: !v,
                     showWidgetType: !0,
                     query: l,
                     settings: e.settings,
-                    trans: a,
+                    trans: n,
                     onClick: e => e.execute()
-                }) : "No starred items") : null, m.createElement(D, {
+                }) : "No starred items") : null, m.createElement(S, {
                     className: "jp-Launcher-openByKernel jp-Launcher-launchNotebook",
-                    title: a.__("Launch Notebook"),
-                    icon: c.notebookIcon,
-                    open: "collapsed" !== C["launch-notebook"]
-                }, m.createElement(L, {
+                    title: n.__("Launch Notebook"),
+                    icon: i.notebookIcon,
+                    open: "collapsed" !== y["launch-notebook"]
+                }, m.createElement(D, {
                     items: e.notebookItems,
                     commands: e.commands,
                     showSearchBox: !v,
                     query: l,
                     settings: e.settings,
-                    trans: a,
+                    trans: n,
                     onClick: e => e.execute()
-                })), m.createElement(D, {
+                })), m.createElement(S, {
                     className: "jp-Launcher-openByKernel jp-Launcher-launchConsole",
-                    title: a.__("Launch Console"),
-                    icon: c.consoleIcon,
-                    open: "collapsed" !== C["launch-console"]
-                }, m.createElement(L, {
+                    title: n.__("Launch Console"),
+                    icon: i.consoleIcon,
+                    open: "collapsed" !== y["launch-console"]
+                }, m.createElement(D, {
                     items: e.consoleItems,
                     commands: e.commands,
                     showSearchBox: !v,
                     query: l,
                     settings: e.settings,
-                    trans: a,
+                    trans: n,
                     onClick: e => e.execute()
                 })))
             }
-            const I = "server-proxy:open";
+            const j = "server-proxy:open";
             class N extends r.Launcher {
                 constructor(e) {
-                    super(e), this.renderCommand = e => new g({
+                    super(e), this.renderCommand = e => new v({
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
-                        n = e.__("Console"),
-                        s = [a, n],
+                        n = e.__("Notebook"),
+                        a = e.__("Console"),
+                        s = [n, a],
                         o = this._settings.composite.utilityCommands,
                         r = t.filter((e => o.includes(e.command))).map(this.renderCommand),
-                        l = t.filter((e => (!e.category || !s.includes(e.category)) && !o.includes(e.command) || e.command === I)),
-                        i = {
+                        l = t.filter((e => (!e.category || !s.includes(e.category)) && !o.includes(e.command) || e.command === j)),
+                        c = {
                             "terminal:create-new": 3,
                             "fileeditor:create-new": 6,
                             "fileeditor:create-new-markdown-file": 5
                         };
-                    for (const e of l) e.command in i && (e.rank = i[e.command]);
-                    const c = [{
+                    for (const e of l) e.command in c && (e.rank = c[e.command]);
+                    const i = [{
                             command: "notebook:create-new",
                             rank: 1
                         }, {
                             command: "console:create",
                             rank: 4
                         }, ...l].sort(((e, t) => {
-                            var a, n;
-                            return (null !== (a = null == e ? void 0 : e.rank) && void 0 !== a ? a : 0) - (null !== (n = null == t ? void 0 : t.rank) && void 0 !== n ? n : 0)
+                            var n, a;
+                            return (null !== (n = null == e ? void 0 : e.rank) && void 0 !== n ? n : 0) - (null !== (a = null == t ? void 0 : t.rank) && void 0 !== a ? a : 0)
                         })),
-                        d = t.filter((e => e.category && e.category === a && e.command !== I)).map(this.renderKernelCommand),
-                        u = t.filter((e => e.category && e.category === n && e.command !== I)).map(this.renderKernelCommand),
-                        h = c.map(this.renderCommand);
-                    return m.createElement(E, {
+                        d = t.filter((e => e.category && e.category === n && e.command !== j)).map(this.renderKernelCommand),
+                        u = t.filter((e => e.category && e.category === a && e.command !== j)).map(this.renderKernelCommand),
+                        h = i.map(this.renderCommand);
+                    return m.createElement(I, {
                         trans: this.trans,
                         cwd: this.cwd,
                         commands: this.commands,
                         typeItems: h,
                         notebookItems: d,
                         consoleItems: u,
                         otherItems: r,
@@ -496,84 +505,84 @@
                     })
                 }
             }
             class U extends s.SessionContextDialogs {
                 constructor(e) {
                     var t;
                     super(e), this.options = e;
-                    const a = null !== (t = e.translator) && void 0 !== t ? t : i.nullTranslator;
-                    this.trans = a.load("jupyterlab")
+                    const n = null !== (t = e.translator) && void 0 !== t ? t : c.nullTranslator;
+                    this.trans = n.load("jupyterlab")
                 }
                 async selectKernel(e) {
                     const t = this.trans;
                     if (e.isDisposed) return Promise.resolve();
-                    let a = t.__("Cancel");
-                    e.hasNoKernel && (a = e.kernelDisplayName);
-                    const n = [s.Dialog.cancelButton({
-                            label: a
+                    let n = t.__("Cancel");
+                    e.hasNoKernel && (n = e.kernelDisplayName);
+                    const a = [s.Dialog.cancelButton({
+                            label: n
                         }), s.Dialog.okButton({
                             label: t.__("Select"),
                             ariaLabel: t.__("Select Kernel"),
                             className: "jp-KernelSelector-SelectButton"
                         })],
                         o = e.kernelPreference.autoStartDefault,
                         r = "boolean" == typeof o,
-                        l = await this.options.settingRegistry.load(_),
-                        i = new s.Dialog({
+                        l = await this.options.settingRegistry.load(b),
+                        c = new s.Dialog({
                             title: t.__("Select Kernel"),
-                            body: new x({
+                            body: new B({
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
-                                    i.resolve(1)
+                                    c.resolve(1)
                                 }
                             }),
-                            buttons: n,
+                            buttons: a,
                             checkbox: r ? {
                                 label: t.__("Always start the preferred kernel"),
                                 caption: t.__("Remember my choice and always start the preferred kernel"),
                                 checked: o
                             } : null
                         });
-                    i.node.classList.add("jp-KernelSelector-Dialog");
-                    const c = await i.launch();
-                    if (e.isDisposed || !c.button.accept) return;
-                    r && null !== c.isChecked && (e.kernelPreference = {
+                    c.node.classList.add("jp-KernelSelector-Dialog");
+                    const i = await c.launch();
+                    if (e.isDisposed || !i.button.accept) return;
+                    r && null !== i.isChecked && (e.kernelPreference = {
                         ...e.kernelPreference,
-                        autoStartDefault: c.isChecked
+                        autoStartDefault: i.isChecked
                     });
-                    const d = c.value;
+                    const d = i.value;
                     if (null === d && !e.hasNoKernel) return e.shutdown();
                     d && await e.changeKernel(d)
                 }
             }
-            const j = {
+            const x = {
                 id: "jupyterlab-new-launcher:dialogs",
                 description: "Session dialogs for redesigned JupyterLab launcher",
                 provides: s.ISessionContextDialogs,
                 autoStart: !0,
-                requires: [i.ITranslator, w, l.ISettingRegistry],
-                activate: (e, t, a, n) => new U({
+                requires: [c.ITranslator, y, l.ISettingRegistry],
+                activate: (e, t, n, a) => new U({
                     translator: t,
-                    database: a,
+                    database: n,
                     commands: e.commands,
-                    settingRegistry: n
+                    settingRegistry: a
                 })
             };
-            class x extends s.ReactWidget {
+            class B extends s.ReactWidget {
                 constructor(e) {
-                    super(), this.options = e, this.renderKernelCommand = e => new g({
+                    super(), this.options = e, this.renderKernelCommand = e => new v({
                         item: e,
                         cwd: "",
                         commands: this.commands,
                         lastUsedDatabase: this._lastUsedDatabase,
                         favoritesDatabase: this._favoritesDatabase
                     }), this._selection = null, this.commands = e.commands, this._lastUsedDatabase = e.lastUsedDatabase, this._favoritesDatabase = e.favoritesDatabase, this._settings = e.settings, this.trans = e.trans
                 }
@@ -585,70 +594,70 @@
                         const e = this.node.getBoundingClientRect();
                         this.node.style.minWidth = e.width + "px", this.node.style.minHeight = e.height + "px"
                     }))
                 }
                 render() {
                     var e;
                     const t = [],
-                        a = this.options.data.specs.kernelspecs;
-                    for (const e of Object.values(a)) {
+                        n = this.options.data.specs.kernelspecs;
+                    for (const e of Object.values(n)) {
                         if (!e) continue;
-                        const a = e.resources["logo-svg"] || e.resources["logo-64x64"];
+                        const n = e.resources["logo-svg"] || e.resources["logo-64x64"];
                         t.push({
                             command: "notebook:create-new",
                             args: {
                                 isLauncher: !0,
                                 kernelName: e.name
                             },
-                            kernelIconUrl: a,
+                            kernelIconUrl: n,
                             metadata: {
-                                kernel: f.JSONExt.deepCopy(e.metadata || {})
+                                kernel: _.JSONExt.deepCopy(e.metadata || {})
                             }
                         })
                     }
-                    const n = [];
+                    const a = [];
                     for (const t of this.options.data.sessions) {
                         const s = t.kernel;
                         if (!s) continue;
-                        const o = a[s.name],
+                        const o = n[s.name],
                             r = o.resources["logo-svg"] || o.resources["logo-64x64"];
-                        n.push({
+                        a.push({
                             command: "notebook:create-new",
                             args: {
                                 isLauncher: !0,
                                 kernelName: o.name
                             },
                             kernelIconUrl: r,
                             metadata: {
                                 kernel: {
-                                    ...f.JSONExt.deepCopy(o.metadata || {}),
+                                    ..._.JSONExt.deepCopy(o.metadata || {}),
                                     state: null !== (e = s.execution_state) && void 0 !== e ? e : "running",
                                     "used by": t.name
                                 },
                                 model: s
                             }
                         })
                     }
                     const s = t.map(this.renderKernelCommand),
-                        o = n.map(this.renderKernelCommand);
+                        o = a.map(this.renderKernelCommand);
                     return m.createElement(m.Fragment, null, m.createElement("h3", {
                         className: "jp-KernelSelector-Section"
-                    }, this.trans.__("Start a new kernel")), m.createElement(L, {
+                    }, this.trans.__("Start a new kernel")), m.createElement(D, {
                         trans: this.trans,
                         commands: this.commands,
                         items: s,
                         settings: this._settings,
                         query: "",
                         showSearchBox: !0,
                         onClick: e => {
                             this._selection = e, this.options.acceptDialog()
                         }
                     }), o.length > 0 ? m.createElement(m.Fragment, null, m.createElement("h3", {
                         className: "jp-KernelSelector-Section"
-                    }, this.trans.__("Connect to a running kernel")), m.createElement(L, {
+                    }, this.trans.__("Connect to a running kernel")), m.createElement(D, {
                         trans: this.trans,
                         commands: this.commands,
                         items: o,
                         settings: this._settings,
                         query: "",
                         showSearchBox: !1,
                         onClick: e => {
@@ -660,192 +669,192 @@
                 getValue() {
                     var e;
                     return this._selection ? (null === (e = this._selection.metadata) || void 0 === e ? void 0 : e.model) ? this._selection.metadata.model : {
                         name: this._selection.args.kernelName
                     } : null
                 }
             }
-            var B = a(101);
-            class K {
+            var K = n(101);
+            class T {
                 constructor(e) {
                     this._updateDB = async () => {
                         const e = await this._fetch();
                         this._db = e
                     }, this._db = null, this._stateDB = e.stateDB;
-                    const t = new f.PromiseDelegate;
+                    const t = new _.PromiseDelegate;
                     this.ready = t.promise, this._updateDB().then((() => t.resolve())), window.setInterval(this._updateDB, e.fetchInterval)
                 }
                 _get(e) {
                     return this._db ? this._db[this._itemKey(e)] : (console.error("Database is not ready!"), null)
                 }
                 async _set(e, t) {
-                    const a = await this._fetch();
-                    this._db = a, a[this._itemKey(e)] = t, await this._stateDB.save(this._stateDBKey, a)
+                    const n = await this._fetch();
+                    this._db = n, n[this._itemKey(e)] = t, await this._stateDB.save(this._stateDBKey, n)
                 }
                 async _fetch() {
                     let e = await this._stateDB.fetch(this._stateDBKey);
                     return void 0 === e && (e = await this._stateDB.fetch(this._stateDBKey)), void 0 === e ? {} : e
                 }
             }
-            class T extends K {
+            class M extends T {
                 _itemKey(e) {
                     return e.command + "_" + JSON.stringify(e.args)
                 }
             }
-            class A extends T {
+            class A extends M {
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
-            class R extends T {
+            class R extends M {
                 constructor() {
-                    super(...arguments), this._stateDBKey = "new-launcher:favorites", this._changed = new p.Signal(this)
+                    super(...arguments), this._stateDBKey = "new-launcher:favorites", this._changed = new g.Signal(this)
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
-            const M = {
+            const O = {
                     id: "jupyterlab-new-launcher:database",
                     description: "A redesigned JupyterLab launcher databases",
-                    provides: w,
+                    provides: y,
                     autoStart: !0,
-                    requires: [B.IStateDB],
+                    requires: [K.IStateDB],
                     activate: (e, t) => {
-                        const a = {
+                        const n = {
                             stateDB: t,
                             fetchInterval: 1e4
                         };
                         return {
-                            lastUsed: new A(a),
-                            favorites: new R(a)
+                            lastUsed: new A(n),
+                            favorites: new R(n)
                         }
                     }
                 },
-                O = [{
-                    id: _,
+                F = [{
+                    id: b,
                     description: "A redesigned JupyterLab launcher",
                     provides: r.ILauncher,
                     autoStart: !0,
-                    requires: [i.ITranslator, l.ISettingRegistry, w],
-                    optional: [n.ILabShell, s.ICommandPalette, o.IDefaultFileBrowser],
-                    activate: function(e, t, a, n, o, l, i) {
+                    requires: [c.ITranslator, l.ISettingRegistry, y],
+                    optional: [a.ILabShell, s.ICommandPalette, o.IDefaultFileBrowser],
+                    activate: function(e, t, n, a, o, l, c) {
                         const {
                             commands: m,
                             shell: u
                         } = e, h = t.load("jupyterlab-new-launcher"), p = new r.LauncherModel;
-                        return a.load(_).then((t => {
-                            ! function(e, t, a) {
-                                e.commands.addCommand(b.toggleColumn, {
+                        return n.load(b).then((t => {
+                            ! function(e, t, n) {
+                                e.commands.addCommand(w.toggleColumn, {
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
-                                        const n = e.id;
-                                        if (!n) return console.error("Column ID missing");
-                                        const s = null !== (t = a.user.hiddenColumns) && void 0 !== t ? t : {};
-                                        "visible" !== s[n] && s[n] ? s[n] = "visible" : s[n] = "hidden", await a.set("hiddenColumns", s)
+                                        const a = e.id;
+                                        if (!a) return console.error("Column ID missing");
+                                        const s = null !== (t = n.user.hiddenColumns) && void 0 !== t ? t : {};
+                                        "visible" !== s[a] && s[a] ? s[a] = "visible" : s[a] = "hidden", await n.set("hiddenColumns", s)
                                     },
                                     isToggleable: !0,
                                     isToggled: e => {
                                         var t;
-                                        const n = e.id;
-                                        return n ? "hidden" !== (null !== (t = a.user.hiddenColumns) && void 0 !== t ? t : {})[n] : (console.error("Column ID missing for checking if toggled"), !1)
+                                        const a = e.id;
+                                        return a ? "hidden" !== (null !== (t = n.user.hiddenColumns) && void 0 !== t ? t : {})[a] : (console.error("Column ID missing for checking if toggled"), !1)
                                     }
-                                }), e.commands.addCommand(b.moveColumn, {
+                                }), e.commands.addCommand(w.moveColumn, {
                                     label: e => "left" === e.direction ? t.__("Move Column Left") : "right" === e.direction ? t.__("Move Column Right") : t.__("Move column left or right"),
                                     execute: async e => {
                                         const t = e.order,
-                                            n = e.id,
-                                            s = t.indexOf(n),
+                                            a = e.id,
+                                            s = t.indexOf(a),
                                             o = s + ("left" === e.direction ? -1 : 1);
                                         if (o < 0 || o >= t.length) return void console.log("Cannot move the column any further");
                                         const r = t[o];
-                                        t[o] = n, t[s] = r, await a.set("columnOrder", t)
+                                        t[o] = a, t[s] = r, await n.set("columnOrder", t)
                                     }
                                 })
                             }(e, h, t)
-                        })), m.addCommand(b.create, {
+                        })), m.addCommand(w.create, {
                             label: h.__("New Launcher"),
-                            icon: e => e.toolbar ? c.addIcon : void 0,
+                            icon: e => e.toolbar ? i.addIcon : void 0,
                             execute: async e => {
                                 var r, l;
-                                const g = null !== (l = null !== (r = e.cwd) && void 0 !== r ? r : null == i ? void 0 : i.model.path) && void 0 !== l ? l : "",
-                                    v = "launcher-" + F.id++,
-                                    f = await a.load(_);
-                                await Promise.all([n.lastUsed.ready, n.favorites.ready]);
-                                const b = new N({
+                                const g = null !== (l = null !== (r = e.cwd) && void 0 !== r ? r : null == c ? void 0 : c.model.path) && void 0 !== l ? l : "",
+                                    v = "launcher-" + H.id++,
+                                    f = await n.load(b);
+                                await Promise.all([a.lastUsed.ready, a.favorites.ready]);
+                                const _ = new N({
                                     model: p,
                                     cwd: g,
                                     callback: e => {
                                         (0, d.find)(u.widgets("main"), (t => t === e)) && (u.add(e, "main", {
                                             ref: v
-                                        }), b.dispose())
+                                        }), _.dispose())
                                     },
                                     commands: m,
                                     translator: t,
-                                    lastUsedDatabase: n.lastUsed,
-                                    favoritesDatabase: n.favorites,
+                                    lastUsedDatabase: a.lastUsed,
+                                    favoritesDatabase: a.favorites,
                                     settings: f
                                 });
-                                b.model = p, b.title.icon = c.launcherIcon, b.title.label = h.__("Launcher");
+                                _.model = p, _.title.icon = i.launcherIcon, _.title.label = h.__("Launcher");
                                 const w = new s.MainAreaWidget({
-                                    content: b
+                                    content: _
                                 });
                                 if (w.title.closable = !!Array.from(u.widgets("main")).length, w.id = v, u.add(w, "main", {
                                         activate: e.activate,
                                         ref: e.ref
                                     }), o && o.layoutModified.connect((() => {
                                         w.title.closable = Array.from(o.widgets("main")).length > 1
-                                    }), w), i) {
+                                    }), w), c) {
                                     const e = e => {
-                                        b.cwd = e.path
+                                        _.cwd = e.path
                                     };
-                                    i.model.pathChanged.connect(e), b.disposed.connect((() => {
-                                        i.model.pathChanged.disconnect(e)
+                                    c.model.pathChanged.connect(e), _.disposed.connect((() => {
+                                        c.model.pathChanged.disconnect(e)
                                     }))
                                 }
                                 return w
                             }
-                        }), o && Promise.all([e.restored, null == i ? void 0 : i.model.restored]).then((() => {
+                        }), o && Promise.all([e.restored, null == c ? void 0 : c.model.restored]).then((() => {
                             o.layoutModified.connect((() => {
-                                o.isEmpty("main") && m.execute(b.create)
+                                o.isEmpty("main") && m.execute(w.create)
                             }))
                         })), l && l.addItem({
-                            command: b.create,
+                            command: w.create,
                             category: h.__("Launcher")
                         }), o && (o.addButtonEnabled = !0, o.addRequested.connect(((e, t) => {
-                            var a;
-                            const n = (null === (a = t.currentTitle) || void 0 === a ? void 0 : a.owner.id) || t.titles[t.titles.length - 1].owner.id;
-                            return m.execute(b.create, {
-                                ref: n
+                            var n;
+                            const a = (null === (n = t.currentTitle) || void 0 === n ? void 0 : n.owner.id) || t.titles[t.titles.length - 1].owner.id;
+                            return m.execute(w.create, {
+                                ref: a
                             })
                         }))), p
                     }
-                }, j, M];
-            var F;
+                }, x, O];
+            var H;
             ! function(e) {
                 e.id = 0
-            }(F || (F = {}))
+            }(H || (H = {}))
         }
     }
 ]);
```

### Comparing `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/728.ea49658c85c6542563e2.js` & `jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/static/728.fa379db84cb7d3fbc55e.js`

 * *Files 2% similar despite different names*

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
-            i.push([n.id, ".jp-Launcher-CardGroup {\n  justify-content: center;\n}\n\n.jp-CollapsibleSection {\n  --jp-animation-depth: 10px;\n  --jp-animation-time: 150ms;\n  --jp-title-height: 24px;\n\n  padding: var(--jp-animation-depth);\n  padding-left: 0;\n  padding-right: 0;\n}\n\n.jp-Launcher-cwd > h3 {\n  font-size: var(--jp-ui-font-size1);\n  margin: 0;\n}\n\n.jp-NewLauncher-OtherItems .jp-LauncherCard-label {\n  display: none;\n}\n\n.jp-NewLauncher-OtherItems .jp-Launcher-TypeCard {\n  width: unset;\n  min-height: unset;\n  flex-direction: row;\n  margin: 0;\n  box-shadow: none;\n  border-color: var(--jp-border-color0);\n}\n\n.jp-NewLauncher-OtherItems .jp-LauncherCard-icon {\n  height: 24px;\n}\n\n.jp-NewLauncher-OtherItems .jp-Launcher-TypeCard > .jp-LauncherCard-icon svg {\n  width: 24px;\n  height: 16px;\n}\n\n.jp-NewLauncher-TopBar {\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n  padding: 8px 0;\n}\n\n.jp-Launcher-searchBox input {\n  /* (no longer needed in lab 4.2+) */\n  box-shadow: none;\n}\n\n.jp-Launcher-searchBox input,\n.jp-Launcher-searchBox jp-search::part(root) {\n  border: var(--jp-border-width) solid var(--jp-border-color1);\n}\n\n.jp-Launcher-searchBox .jp-FilterBox {\n  width: 100%;\n}\n\n.jp-CollapsibleSection > summary {\n  cursor: pointer;\n  transition: margin var(--jp-animation-time) ease-out;\n  list-style: none;\n  display: inline-block; /* contain the clickable area */\n  padding-right: 12px; /* but extend it a little */\n  min-width: 185px;\n}\n\n.jp-CollapsibleSection > summary:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.jp-CollapsibleSection[open] > summary {\n  margin-bottom: var(--jp-animation-depth);\n}\n\n.jp-CollapsibleSection-CollapserIcon > svg {\n  transition: transform var(--jp-animation-time) ease-out;\n  width: var(--jp-title-height);\n  height: var(--jp-title-height);\n}\n\n.jp-CollapsibleSection[open] .jp-CollapsibleSection-CollapserIcon > svg {\n  transform: rotate(90deg);\n}\n\n.jp-CollapsibleSection-CollapserIconWrapper {\n  display: inline-block;\n}\n\n.jp-CollapsibleSection-CategoryIcon > svg {\n  width: 24px;\n  height: 24px;\n  margin-left: 4px;\n  margin-right: 8px;\n}\n\n.jp-CollapsibleSection-Title {\n  display: inline-block;\n  line-height: var(--jp-title-height);\n  vertical-align: top;\n  margin: 0;\n  user-select: none;\n  font-weight: normal;\n}\n\n.jp-LauncherBody {\n  padding: 0 24px;\n  height: 100%;\n  overflow-y: auto;\n}\n\n.jp-NewLauncher-table {\n  --jp-icon-size: 16px;\n\n  display: flex;\n  flex-direction: column;\n  overflow: hidden;\n}\n\n.jp-NewLauncher-table .jp-sortable-table {\n  border: var(--jp-border-width) solid var(--jp-border-color2);\n  border-top: 0;\n}\n\n.jp-NewLauncher-table .jp-Launcher-kernelIcon {\n  width: var(--jp-icon-size);\n  height: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-LauncherCard-noKernelIcon {\n  font-size: var(--jp-icon-size);\n  line-height: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-LauncherCard-icon {\n  height: var(--jp-icon-size);\n  width: var(--jp-icon-size);\n  display: inline-block;\n}\n\n.jp-TableKernelItem {\n  display: inline-block;\n  line-height: var(--jp-icon-size);\n  vertical-align: top;\n  padding-left: 4px;\n}\n\n.jp-NewLauncher-table th[data-id='icon'],\n.jp-NewLauncher-table th[data-id='star'] {\n  width: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-starIcon {\n  width: var(--jp-icon-size);\n  height: var(--jp-icon-size);\n}\n\n.jp-starIconButton:hover > .jp-starIcon {\n  border-radius: 50%;\n  box-shadow: 0 0 0 2px var(--jp-layout-color3);\n  background: var(--jp-layout-color1);\n}\n\n.jp-NewLauncher-table-scroller {\n  overflow: auto;\n  margin-top: 4px;\n}\n\n.jp-starIconButton {\n  --jp-transition-transform: rotate(72deg);\n\n  border: 0;\n  margin: 0;\n  padding: 0 6px;\n  background: transparent;\n  cursor: pointer;\n}\n\n.jp-starIcon .jp-star-filled {\n  opacity: 0;\n}\n\n.jp-starIcon .jp-star-filled,\n.jp-starIcon .jp-star-border {\n  transition-property: opacity, transform;\n  transition-duration: 0.2s;\n  transition-timing-function: ease-out;\n  transform-origin: center;\n}\n\n.jp-starIconButton.jp-mod-starred .jp-star-filled {\n  opacity: 1;\n  transform: var(--jp-transition-transform);\n}\n\n.jp-starIconButton.jp-mod-starred .jp-star-border {\n  opacity: 0;\n  transform: var(--jp-transition-transform);\n}\n\n.jp-KernelSelector-Dialog > .jp-Dialog-content {\n  max-height: 80%;\n  max-width: unset;\n}\n\n.jp-KernelSelector-Dialog > .jp-Dialog-content > .jp-Dialog-header {\n  display: none;\n}\n\n.jp-KernelSelector-SelectButton {\n  display: none;\n}\n\n.jp-KernelSelector-Dialog .jp-NewLauncher-table {\n  margin-bottom: 8px;\n}\n\n.jp-KernelSelector-Section {\n  margin: 0;\n  margin-bottom: 4px;\n}\n\n/* Styles for scenario where full row is clickable  */\n\n.jp-NewLauncher-table tr {\n  cursor: pointer;\n}\n\n.jp-Launcher-TypeCard {\n  user-select: none;\n}\n\n.jp-Launcher-TypeCard > .jp-LauncherCard-icon svg {\n  align-items: center;\n  display: flex;\n  height: 52px;\n  width: 52px;\n}\n", ""]);
+            i.push([n.id, ".jp-Launcher-CardGroup {\n  justify-content: center;\n}\n\n.jp-CollapsibleSection {\n  --jp-animation-depth: 10px;\n  --jp-animation-time: 150ms;\n  --jp-title-height: 24px;\n\n  padding: var(--jp-animation-depth);\n  padding-left: 0;\n  padding-right: 0;\n}\n\n.jp-Launcher-cwd > h3 {\n  font-size: var(--jp-ui-font-size1);\n  margin: 0;\n}\n\n.jp-NewLauncher-OtherItems {\n  display: flex;\n  gap: 4px;\n}\n\n.jp-NewLauncher-OtherItems .jp-LauncherCard-label {\n  display: none;\n}\n\n.jp-NewLauncher-OtherItems .jp-Launcher-TypeCard {\n  width: unset;\n  min-height: unset;\n  flex-direction: row;\n  margin: 0;\n  box-shadow: none;\n  border-color: var(--jp-border-color0);\n}\n\n.jp-NewLauncher-OtherItems .jp-LauncherCard-icon {\n  height: 24px;\n}\n\n.jp-NewLauncher-OtherItems .jp-Launcher-TypeCard > .jp-LauncherCard-icon svg {\n  width: 24px;\n  height: 16px;\n}\n\n.jp-NewLauncher-TopBar {\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n  padding: 8px 0;\n}\n\n.jp-Launcher-searchBox input {\n  /* (no longer needed in lab 4.2+) */\n  box-shadow: none;\n}\n\n.jp-Launcher-searchBox input,\n.jp-Launcher-searchBox jp-search::part(root) {\n  border: var(--jp-border-width) solid var(--jp-border-color1);\n}\n\n.jp-Launcher-searchBox .jp-FilterBox {\n  width: 100%;\n}\n\n.jp-CollapsibleSection > summary {\n  cursor: pointer;\n  transition: margin var(--jp-animation-time) ease-out;\n  list-style: none;\n  display: inline-block; /* contain the clickable area */\n  padding-right: 12px; /* but extend it a little */\n  min-width: 185px;\n}\n\n.jp-CollapsibleSection > summary:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.jp-CollapsibleSection[open] > summary {\n  margin-bottom: var(--jp-animation-depth);\n}\n\n.jp-CollapsibleSection-CollapserIcon > svg {\n  transition: transform var(--jp-animation-time) ease-out;\n  width: var(--jp-title-height);\n  height: var(--jp-title-height);\n}\n\n.jp-CollapsibleSection[open] .jp-CollapsibleSection-CollapserIcon > svg {\n  transform: rotate(90deg);\n}\n\n.jp-CollapsibleSection-CollapserIconWrapper {\n  display: inline-block;\n}\n\n.jp-CollapsibleSection-CategoryIcon > svg {\n  width: 24px;\n  height: 24px;\n  margin-left: 4px;\n  margin-right: 8px;\n}\n\n.jp-CollapsibleSection-Title {\n  display: inline-block;\n  line-height: var(--jp-title-height);\n  vertical-align: top;\n  margin: 0;\n  user-select: none;\n  font-weight: normal;\n}\n\n.jp-LauncherBody {\n  padding: 0 24px;\n  height: 100%;\n  overflow-y: auto;\n}\n\n.jp-NewLauncher-table {\n  --jp-icon-size: 16px;\n\n  display: flex;\n  flex-direction: column;\n  overflow: hidden;\n}\n\n.jp-NewLauncher-table .jp-sortable-table {\n  border: var(--jp-border-width) solid var(--jp-border-color2);\n  border-top: 0;\n}\n\n.jp-NewLauncher-table .jp-Launcher-kernelIcon {\n  width: var(--jp-icon-size);\n  height: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-LauncherCard-noKernelIcon {\n  font-size: var(--jp-icon-size);\n  line-height: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-LauncherCard-icon {\n  height: var(--jp-icon-size);\n  width: var(--jp-icon-size);\n  display: inline-block;\n}\n\n.jp-TableKernelItem {\n  display: inline-block;\n  line-height: var(--jp-icon-size);\n  vertical-align: top;\n  padding-left: 4px;\n}\n\n.jp-NewLauncher-table th[data-id='icon'],\n.jp-NewLauncher-table th[data-id='star'] {\n  width: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-starIcon {\n  width: var(--jp-icon-size);\n  height: var(--jp-icon-size);\n}\n\n.jp-starIconButton:hover > .jp-starIcon {\n  border-radius: 50%;\n  box-shadow: 0 0 0 2px var(--jp-layout-color3);\n  background: var(--jp-layout-color1);\n}\n\n.jp-NewLauncher-table-scroller {\n  overflow: auto;\n  margin-top: 4px;\n}\n\n.jp-starIconButton {\n  --jp-transition-transform: rotate(72deg);\n\n  border: 0;\n  margin: 0;\n  padding: 0 6px;\n  background: transparent;\n  cursor: pointer;\n}\n\n.jp-starIcon .jp-star-filled {\n  opacity: 0;\n}\n\n.jp-starIcon .jp-star-filled,\n.jp-starIcon .jp-star-border {\n  transition-property: opacity, transform;\n  transition-duration: 0.2s;\n  transition-timing-function: ease-out;\n  transform-origin: center;\n}\n\n.jp-starIconButton.jp-mod-starred .jp-star-filled {\n  opacity: 1;\n  transform: var(--jp-transition-transform);\n}\n\n.jp-starIconButton.jp-mod-starred .jp-star-border {\n  opacity: 0;\n  transform: var(--jp-transition-transform);\n}\n\n.jp-KernelSelector-Dialog > .jp-Dialog-content {\n  max-height: 80%;\n  max-width: unset;\n}\n\n.jp-KernelSelector-Dialog > .jp-Dialog-content > .jp-Dialog-header {\n  display: none;\n}\n\n.jp-KernelSelector-SelectButton {\n  display: none;\n}\n\n.jp-KernelSelector-Dialog .jp-NewLauncher-table {\n  margin-bottom: 8px;\n}\n\n.jp-KernelSelector-Section {\n  margin: 0;\n  margin-bottom: 4px;\n}\n\n/* Styles for scenario where full row is clickable  */\n\n.jp-NewLauncher-table tr {\n  cursor: pointer;\n}\n\n.jp-Launcher-TypeCard {\n  user-select: none;\n}\n\n.jp-Launcher-TypeCard > .jp-LauncherCard-icon svg {\n  align-items: center;\n  display: flex;\n  height: 52px;\n  width: 52px;\n}\n", ""]);
             const p = i
         },
         314: n => {
             n.exports = function(n) {
                 var e = [];
                 return e.toString = function() {
                     return this.map((function(e) {
```

### Comparing `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/remoteEntry.9b81d6d816ee65d81ed3.js` & `jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/static/remoteEntry.2e1e8df64ea6f9bac940.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, a, o, i, u, l, f, s, d, p, c, h, v, b, g = {
             795: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(21).then((() => () => t(21))),
-                        "./extension": () => t.e(21).then((() => () => t(21))),
+                        "./index": () => t.e(239).then((() => () => t(239))),
+                        "./extension": () => t.e(239).then((() => () => t(239))),
                         "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -43,19 +43,19 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        21: "6aebeef0c48d440fad32",
-        728: "ea49658c85c6542563e2"
+        239: "eba35c75272592009997",
+        728: "fa379db84cb7d3fbc55e"
     } [e] + ".js?v=" + {
-        21: "6aebeef0c48d440fad32",
-        728: "ea49658c85c6542563e2"
+        239: "eba35c75272592009997",
+        728: "fa379db84cb7d3fbc55e"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -102,19 +102,19 @@
                 var o = m.S[t],
                     i = "jupyterlab-new-launcher",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var a = o[e] = o[e] || {},
                         u = a[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
-                        get: () => m.e(21).then((() => () => m(21))),
+                        get: () => m.e(239).then((() => () => m(239))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-new-launcher", "0.2.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-new-launcher", "0.2.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -222,15 +222,15 @@
         602: () => p("default", "@lumino/signaling", [1, 2, 0, 0]),
         626: () => p("default", "@jupyterlab/application", [1, 4, 2, 0]),
         670: () => p("default", "@jupyterlab/filebrowser", [1, 4, 2, 0]),
         702: () => p("default", "@jupyterlab/coreutils", [1, 6, 2, 0]),
         825: () => p("default", "@jupyterlab/settingregistry", [1, 4, 2, 0]),
         923: () => p("default", "@jupyterlab/apputils", [1, 4, 3, 0])
     }, v = {
-        21: [53, 101, 260, 262, 265, 345, 527, 602, 626, 670, 702, 825, 923]
+        239: [53, 101, 260, 262, 265, 345, 527, 602, 626, 670, 702, 825, 923]
     }, b = {}, m.f.consumes = (e, r) => {
         m.o(v, e) && v[e].forEach((e => {
             if (m.o(c, e)) return r.push(c[e]);
             if (!b[e]) {
                 var t = r => {
                     c[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
```

### Comparing `jupyterlab_new_launcher-0.2.1/jupyterlab_new_launcher/labextension/static/third-party-licenses.json` & `jupyterlab_new_launcher-0.2.2/jupyterlab_new_launcher/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/schema/plugin.json` & `jupyterlab_new_launcher-0.2.2/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/src/commands.ts` & `jupyterlab_new_launcher-0.2.2/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/src/database.ts` & `jupyterlab_new_launcher-0.2.2/src/database.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/src/dialogs.tsx` & `jupyterlab_new_launcher-0.2.2/src/dialogs.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/src/index.ts` & `jupyterlab_new_launcher-0.2.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/src/item.ts` & `jupyterlab_new_launcher-0.2.2/src/item.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 // Copyright (c) Nebari Development Team.
 // Distributed under the terms of the Modified BSD License.
 import type { CommandRegistry } from '@lumino/commands';
 import type { VirtualElement } from '@lumino/virtualdom';
-import { ReadonlyJSONObject } from '@lumino/coreutils';
+import { ReadonlyJSONObject, JSONObject } from '@lumino/coreutils';
 import { ILauncher } from '@jupyterlab/launcher';
 import { Signal, ISignal } from '@lumino/signaling';
 import { IItem, IFavoritesDatabase, ILastUsedDatabase } from './types';
+import { codeServerIcon } from './icons';
 
 export class Item implements IItem {
   // base ILauncher.IItemOptions
   command: string;
   args?: ReadonlyJSONObject;
   category?: string;
   rank?: number;
@@ -46,28 +47,38 @@
     this.icon = commands.icon(item.command, args);
     this.caption = commands.caption(item.command, args);
     this.label = commands.label(item.command, args);
     this.lastUsed = lastUsedDatabase.get(item);
     this.starred = favoritesDatabase.get(item) ?? false;
     // special handling for conda-store
     // https://www.nebari.dev/docs/faq/#why-is-there-duplication-in-names-of-environments
+    const kernel = this.metadata['kernel'] as JSONObject;
     const condaStoreMatch = (
-      (this.metadata['conda_env_name'] as string | undefined) ?? ''
+      (kernel['conda_env_name'] as string | undefined) ?? ''
     ).match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
     if (condaStoreMatch && this.metadata) {
       const groups = condaStoreMatch.groups!;
       this.label =
-        (this.metadata['conda_language'] as string | undefined) ??
-        groups.environment;
+        (kernel['conda_language'] as string | undefined) ?? groups.environment;
       this.metadata = {
         ...this.metadata,
-        conda_env_name: groups.environment,
-        Namespace: groups.namespace
+        kernel: {
+          ...kernel,
+          conda_env_name: groups.environment,
+          Namespace: groups.namespace
+        }
       };
     }
+    // set the code-server icon to support dark theme properly
+    if (
+      this.command === 'server-proxy:open' &&
+      this.kernelIconUrl?.endsWith('/vscode')
+    ) {
+      this.icon = codeServerIcon;
+    }
   }
   get lastUsed(): Date | null {
     return this._lastUsed;
   }
   set lastUsed(value: Date | null) {
     this._lastUsed = value;
     this._setRefreshClock();
```

### Comparing `jupyterlab_new_launcher-0.2.1/src/launcher.tsx` & `jupyterlab_new_launcher-0.2.2/src/launcher.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/src/types.ts` & `jupyterlab_new_launcher-0.2.2/src/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/src/components/card.tsx` & `jupyterlab_new_launcher-0.2.2/src/components/card.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/src/components/section.tsx` & `jupyterlab_new_launcher-0.2.2/src/components/section.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/src/components/table.tsx` & `jupyterlab_new_launcher-0.2.2/src/components/table.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/style/base.css` & `jupyterlab_new_launcher-0.2.2/style/base.css`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 }
 
 .jp-Launcher-cwd > h3 {
   font-size: var(--jp-ui-font-size1);
   margin: 0;
 }
 
+.jp-NewLauncher-OtherItems {
+  display: flex;
+  gap: 4px;
+}
+
 .jp-NewLauncher-OtherItems .jp-LauncherCard-label {
   display: none;
 }
 
 .jp-NewLauncher-OtherItems .jp-Launcher-TypeCard {
   width: unset;
   min-height: unset;
```

### Comparing `jupyterlab_new_launcher-0.2.1/style/icons/md/LICENSE` & `jupyterlab_new_launcher-0.2.2/style/icons/md/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/ui-tests/README.md` & `jupyterlab_new_launcher-0.2.2/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/ui-tests/yarn.lock` & `jupyterlab_new_launcher-0.2.2/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts` & `jupyterlab_new_launcher-0.2.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png` & `jupyterlab_new_launcher-0.2.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png` & `jupyterlab_new_launcher-0.2.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png` & `jupyterlab_new_launcher-0.2.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/.gitignore` & `jupyterlab_new_launcher-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/LICENSE` & `jupyterlab_new_launcher-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/README.md` & `jupyterlab_new_launcher-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/pyproject.toml` & `jupyterlab_new_launcher-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.1/PKG-INFO` & `jupyterlab_new_launcher-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-new-launcher
-Version: 0.2.1
+Version: 0.2.2
 Dynamic: Keywords
 Summary: A redesigned JupyterLab launcher
 Project-URL: Homepage, https://github.com/nebari-dev/jupyterlab-new-launcher
 Project-URL: Bug Tracker, https://github.com/nebari-dev/jupyterlab-new-launcher/issues
 Project-URL: Repository, https://github.com/nebari-dev/jupyterlab-new-launcher.git
 Author-email: Nebari development team <internal-it@quansight.com>
 License: BSD 3-Clause License
```

