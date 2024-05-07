# Comparing `tmp/beaker_kernel-1.5.0.tar.gz` & `tmp/beaker_kernel-1.5.1.tar.gz`

## Comparing `beaker_kernel-1.5.0.tar` & `beaker_kernel-1.5.1.tar`

### file list

```diff
@@ -1,173 +1,173 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/kernel.json
--rw-r--r--   0        0        0    21334 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/kernel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/default/__init__.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/default/agent.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/default/context.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/default/default_payload.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/pypackage/__init__.py
--rw-r--r--   0        0        0     6485 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/pypackage/agent.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/pypackage/context.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/pypackage/default_payload.json
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/pypackage/procedures/python3/get_documentation.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/pypackage/procedures/python3/get_package_structure.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/pypackage/procedures/python3/get_variable_info.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/pypackage/procedures/python3/get_variables.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/contexts/pypackage/procedures/python3/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/lib/__init__.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/lib/agent.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/lib/agent_tasks.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/lib/autodiscovery.py
--rw-r--r--   0        0        0    16135 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/lib/context.py
--rw-r--r--   0        0        0    13694 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/lib/jupyter_kernel_proxy.py
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/lib/utils.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/lib/subkernels/__init__.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/lib/subkernels/base.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/lib/subkernels/julia.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/lib/subkernels/python.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/lib/subkernels/rlang.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/__init__.py
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/admin_utils.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/dev.py
--rw-r--r--   0        0        0    13482 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/.empty
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/admin.html
--rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/beaker.svg
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/favicon.ico
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/index.html
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/css/admin.06bbaee6.css
--rw-r--r--   0        0        0   122158 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/css/chunk-vendors.f59cad43.css
--rw-r--r--   0        0        0    12969 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/css/index.622cafdc.css
--rw-r--r--   0        0        0    72204 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/fonts/primeicons.0112589c.ttf
--rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/fonts/primeicons.ba3f916d.woff2
--rw-r--r--   0        0        0    72280 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/fonts/primeicons.f8b9e8a4.woff
--rw-r--r--   0        0        0    72380 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/fonts/primeicons.ffecb254.eot
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/add-above.ee286b1c.svg
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/add-below.bcf3422e.svg
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/add.8f2126a6.svg
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/bad.2c188c60.svg
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/bell.bccaf100.svg
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/blank.a4bbd63d.svg
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/bug-dot.326bc45a.svg
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/bug.e30064ad.svg
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/build.e3fdf668.svg
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/caret-down-empty-thin.f6894985.svg
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/caret-down-empty.16b5c137.svg
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/caret-down.1600b64a.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/caret-left.d607c024.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/caret-right.45b8bd09.svg
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/caret-up-empty-thin.912759a9.svg
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/caret-up.9b98d201.svg
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/case-sensitive.eaefe455.svg
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/check.0991dc26.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/circle-empty.4dad54e2.svg
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/circle.114607e4.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/clear.f255d27d.svg
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/close.563b4f49.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/code-check.99d4f00e.svg
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/code.fbdeee94.svg
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/collapse-all.41b2dc7a.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/console.57361ea6.svg
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/copy.2bfc5d39.svg
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/copyright.f38f4ec0.svg
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/cut.18edde39.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/delete.a777a562.svg
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/download.e0245bbf.svg
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/duplicate.8815451e.svg
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/edit.7fbc6db4.svg
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/ellipses.dba28113.svg
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/error.0caf9ea6.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/expand-all.81b631fe.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/extension.50386a9c.svg
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/fast-forward.f82230c4.svg
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/file-upload.44fd837e.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/file.80a9f304.svg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/filter-dot.47fa93c4.svg
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/filter-list.9e70c93a.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/filter.538fe88b.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/folder-favorite.7f8c9bd5.svg
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/folder.0d235aaf.svg
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/home.32ae995c.svg
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/html5.ea435392.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/image.82357447.svg
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/info.4d82eb41.svg
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/inspector.791cc05d.svg
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/json.a2c296bb.svg
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/julia.499ac74e.svg
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/jupyter-favicon.b19d8551.svg
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/jupyter.a48871a7.svg
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/jupyterlab-wordmark.6280567a.svg
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/kernel.273d3780.svg
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/keyboard.3b314c65.svg
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/launch.6417683d.svg
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/launcher.0453ed19.svg
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/line-form.3e38ab09.svg
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/link.170ecd8b.svg
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/list.c48a0dd4.svg
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/markdown.60974264.svg
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/move-down.5e4a3948.svg
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/move-up.fa81409d.svg
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/new-folder.e3dd5db9.svg
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/not-trusted.8bc17823.svg
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/notebook.9b4747ea.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/numbering.60a6786d.svg
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/offline-bolt.8d942d9a.svg
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/palette.14c4709b.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/paste.3d3cadcf.svg
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/pdf.f6a1dc59.svg
--rw-r--r--   0        0        0   291454 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/primeicons.943ab24c.svg
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/python.0ffed0a2.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/r-kernel.cb4265e1.svg
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/react.c81f1b87.svg
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/redo.ecef5f0c.svg
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/refresh.dae7f1f4.svg
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/regex.fa85da44.svg
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/run.cbdeb7c0.svg
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/running.9890c96a.svg
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/save.2c9f21a7.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/search.77371ff0.svg
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/settings.454fe53f.svg
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/share.ccbe241a.svg
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/spreadsheet.486ad38c.svg
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/stop.88696d03.svg
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/tab.67683cb0.svg
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/table-rows.1053696f.svg
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/tag.8887c8e5.svg
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/terminal.0a8eb862.svg
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/text-editor.52a85e17.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/toc.05490e17.svg
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/tree-view.0a94d13b.svg
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/trusted.3ac2122f.svg
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/undo.0c5afedd.svg
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/user.a13160b1.svg
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/users.cba8edb3.svg
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/vega.c0ae7146.svg
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/word.c993422c.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/yaml.267ef972.svg
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/js/admin.595fbd46.js
--rw-r--r--   0        0        0    53400 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/js/admin.595fbd46.js.map
--rw-r--r--   0        0        0  3111348 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js
--rw-r--r--   0        0        0 10024731 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js.map
--rw-r--r--   0        0        0    80016 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/js/index.e38a09de.js
--rw-r--r--   0        0        0   369507 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/static/js/index.e38a09de.js.map
--rw-r--r--   0        0        0   187164 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/theme.css
--rw-r--r--   0        0        0    32196 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff
--rw-r--r--   0        0        0    24836 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff2
--rw-r--r--   0        0        0    30356 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff
--rw-r--r--   0        0        0    24712 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff2
--rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff
--rw-r--r--   0        0        0    25320 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff2
--rw-r--r--   0        0        0   178553 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/theme.css
--rw-r--r--   0        0        0    32196 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff
--rw-r--r--   0        0        0    24836 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff2
--rw-r--r--   0        0        0    30356 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff
--rw-r--r--   0        0        0    24712 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff2
--rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff
--rw-r--r--   0        0        0    25320 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff2
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/LICENSE.txt
--rw-r--r--   0        0        0     7906 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/README.md
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/hatch_build.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 beaker_kernel-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/kernel.json
+-rw-r--r--   0        0        0    21439 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/kernel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/default/__init__.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/default/agent.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/default/context.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/default/default_payload.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/__init__.py
+-rw-r--r--   0        0        0     6485 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/agent.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/context.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/default_payload.json
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/get_documentation.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/get_package_structure.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/get_variable_info.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/get_variables.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/__init__.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/agent.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/agent_tasks.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/autodiscovery.py
+-rw-r--r--   0        0        0    16185 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/context.py
+-rw-r--r--   0        0        0    13694 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/jupyter_kernel_proxy.py
+-rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/utils.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/__init__.py
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/base.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/julia.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/python.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/rlang.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/__init__.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/admin_utils.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/dev.py
+-rw-r--r--   0        0        0    13482 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/.empty
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/admin.html
+-rw-r--r--   0        0        0    20752 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/beaker.svg
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/favicon.ico
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/index.html
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/css/admin.06bbaee6.css
+-rw-r--r--   0        0        0   122158 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/css/chunk-vendors.f59cad43.css
+-rw-r--r--   0        0        0    12969 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/css/index.622cafdc.css
+-rw-r--r--   0        0        0    72204 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.0112589c.ttf
+-rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.ba3f916d.woff2
+-rw-r--r--   0        0        0    72280 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.f8b9e8a4.woff
+-rw-r--r--   0        0        0    72380 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.ffecb254.eot
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/add-above.ee286b1c.svg
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/add-below.bcf3422e.svg
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/add.8f2126a6.svg
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bad.2c188c60.svg
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bell.bccaf100.svg
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/blank.a4bbd63d.svg
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bug-dot.326bc45a.svg
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bug.e30064ad.svg
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/build.e3fdf668.svg
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-down-empty-thin.f6894985.svg
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-down-empty.16b5c137.svg
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-down.1600b64a.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-left.d607c024.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-right.45b8bd09.svg
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-up-empty-thin.912759a9.svg
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/caret-up.9b98d201.svg
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/case-sensitive.eaefe455.svg
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/check.0991dc26.svg
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/circle-empty.4dad54e2.svg
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/circle.114607e4.svg
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/clear.f255d27d.svg
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/close.563b4f49.svg
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/code-check.99d4f00e.svg
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/code.fbdeee94.svg
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/collapse-all.41b2dc7a.svg
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/console.57361ea6.svg
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/copy.2bfc5d39.svg
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/copyright.f38f4ec0.svg
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/cut.18edde39.svg
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/delete.a777a562.svg
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/download.e0245bbf.svg
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/duplicate.8815451e.svg
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/edit.7fbc6db4.svg
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/ellipses.dba28113.svg
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/error.0caf9ea6.svg
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/expand-all.81b631fe.svg
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/extension.50386a9c.svg
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/fast-forward.f82230c4.svg
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/file-upload.44fd837e.svg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/file.80a9f304.svg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/filter-dot.47fa93c4.svg
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/filter-list.9e70c93a.svg
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/filter.538fe88b.svg
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/folder-favorite.7f8c9bd5.svg
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/folder.0d235aaf.svg
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/home.32ae995c.svg
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/html5.ea435392.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/image.82357447.svg
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/info.4d82eb41.svg
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/inspector.791cc05d.svg
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/json.a2c296bb.svg
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/julia.499ac74e.svg
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/jupyter-favicon.b19d8551.svg
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/jupyter.a48871a7.svg
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/jupyterlab-wordmark.6280567a.svg
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/kernel.273d3780.svg
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/keyboard.3b314c65.svg
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/launch.6417683d.svg
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/launcher.0453ed19.svg
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/line-form.3e38ab09.svg
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/link.170ecd8b.svg
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/list.c48a0dd4.svg
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/markdown.60974264.svg
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/move-down.5e4a3948.svg
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/move-up.fa81409d.svg
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/new-folder.e3dd5db9.svg
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/not-trusted.8bc17823.svg
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/notebook.9b4747ea.svg
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/numbering.60a6786d.svg
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/offline-bolt.8d942d9a.svg
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/palette.14c4709b.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/paste.3d3cadcf.svg
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/pdf.f6a1dc59.svg
+-rw-r--r--   0        0        0   291454 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/primeicons.943ab24c.svg
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/python.0ffed0a2.svg
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/r-kernel.cb4265e1.svg
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/react.c81f1b87.svg
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/redo.ecef5f0c.svg
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/refresh.dae7f1f4.svg
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/regex.fa85da44.svg
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/run.cbdeb7c0.svg
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/running.9890c96a.svg
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/save.2c9f21a7.svg
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/search.77371ff0.svg
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/settings.454fe53f.svg
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/share.ccbe241a.svg
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/spreadsheet.486ad38c.svg
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/stop.88696d03.svg
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/tab.67683cb0.svg
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/table-rows.1053696f.svg
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/tag.8887c8e5.svg
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/terminal.0a8eb862.svg
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/text-editor.52a85e17.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/toc.05490e17.svg
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/tree-view.0a94d13b.svg
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/trusted.3ac2122f.svg
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/undo.0c5afedd.svg
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/user.a13160b1.svg
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/users.cba8edb3.svg
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/vega.c0ae7146.svg
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/word.c993422c.svg
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/yaml.267ef972.svg
+-rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/admin.595fbd46.js
+-rw-r--r--   0        0        0    53400 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/admin.595fbd46.js.map
+-rw-r--r--   0        0        0  3111348 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js
+-rw-r--r--   0        0        0 10024731 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js.map
+-rw-r--r--   0        0        0    80016 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/index.e38a09de.js
+-rw-r--r--   0        0        0   369507 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/index.e38a09de.js.map
+-rw-r--r--   0        0        0   187164 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/theme.css
+-rw-r--r--   0        0        0    32196 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff
+-rw-r--r--   0        0        0    24836 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff2
+-rw-r--r--   0        0        0    30356 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff
+-rw-r--r--   0        0        0    24712 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff2
+-rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff
+-rw-r--r--   0        0        0    25320 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff2
+-rw-r--r--   0        0        0   178553 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/theme.css
+-rw-r--r--   0        0        0    32196 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff
+-rw-r--r--   0        0        0    24836 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff2
+-rw-r--r--   0        0        0    30356 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff
+-rw-r--r--   0        0        0    24712 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff2
+-rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff
+-rw-r--r--   0        0        0    25320 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff2
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     7906 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/README.md
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/hatch_build.py
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 beaker_kernel-1.5.1/PKG-INFO
```

### Comparing `beaker_kernel-1.5.0/beaker_kernel/kernel.py` & `beaker_kernel-1.5.1/beaker_kernel/kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         return data
 
     @magic("set_context")
     async def set_context_magic(self, cell_content: str, magic_word=None, parent_header=None):
         context_name, language, context_config = cell_content.split(maxsplit=2)
         context_info = json.loads(context_config)
         self.stdout(f"Switching from context {self.context.slug} to {context_name}...", parent_header=parent_header)
-        await self.set_context(context_name=context_name, language=language, context_info=context_info, parent_header=parent_header)
+        await self.set_context(context_name=context_name, context_info=context_info, language=language, parent_header=parent_header)
 
         # Send message to trigger updating the context info
         self.send_response(
             stream="iopub",
             msg_or_type="context_info_update",
             content={},
             parent_header=parent_header,
@@ -236,16 +236,21 @@
         if not context_cls:
             # TODO: Should we return an error if the requested context isn't available?
             return False
 
         # Cleanup the old context, then create and setup the new context
         if self.context:
             self.context.cleanup()
-        self.context = context_cls(beaker_kernel=self, config=context_info)
-        await self.context.setup(config=context_info, parent_header=parent_header)
+
+        config = {
+            "language": language,
+            "context_info": context_info
+        }
+        self.context = context_cls(beaker_kernel=self, config=config)
+        await self.context.setup(context_info=context_info, parent_header=parent_header)
         await self.send_preview(parent_header=parent_header)
         await self.update_connection_file(context={"name": context_name, "config": context_info})
 
     async def post_execute(self, queue, message_id, data):
         message = JupyterMessage.parse(data)
 
         # Only run if there is an active context
```

### Comparing `beaker_kernel-1.5.0/beaker_kernel/contexts/default/agent.py` & `beaker_kernel-1.5.1/beaker_kernel/contexts/default/agent.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/contexts/default/context.py` & `beaker_kernel-1.5.1/beaker_kernel/contexts/default/context.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/contexts/pypackage/agent.py` & `beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/agent.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/contexts/pypackage/context.py` & `beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,10 +15,10 @@
     agent_cls: "BaseAgent" = PyPackageAgent
 
     def __init__(self, beaker_kernel: "LLMKernel", config: Dict[str, Any]):
         super().__init__(beaker_kernel, self.agent_cls, config)
         if not isinstance(self.subkernel, PythonSubkernel):
             raise ValueError("This context is only valid for Python.")
 
-    async def setup(self, config=None, parent_header=None):
+    async def setup(self, context_info=None, parent_header=None):
         await self.execute(self.get_code("setup", {}))
-        return await super().setup(config, parent_header)
+        return await super().setup(config["context_info"], parent_header)
```

### Comparing `beaker_kernel-1.5.0/beaker_kernel/contexts/pypackage/procedures/python3/get_documentation.py` & `beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/get_documentation.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/contexts/pypackage/procedures/python3/setup.py` & `beaker_kernel-1.5.1/beaker_kernel/contexts/pypackage/procedures/python3/setup.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/lib/agent.py` & `beaker_kernel-1.5.1/beaker_kernel/lib/agent.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/lib/agent_tasks.py` & `beaker_kernel-1.5.1/beaker_kernel/lib/agent_tasks.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/lib/autodiscovery.py` & `beaker_kernel-1.5.1/beaker_kernel/lib/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/lib/context.py` & `beaker_kernel-1.5.1/beaker_kernel/lib/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,20 +72,20 @@
                     template_name, _ = os.path.splitext(template_file)
                     template = self.jinja_env.get_template(template_file)
                     self.templates[template_name] = template
                 except UnicodeDecodeError:
                     # For templates, this indicates a binary file which can't be a template, so throw a warning and skip.
                     logger.warn(f"File '{template_name}' in context '{self.__class__.__name__}' is not a valid template file as it cannot be decoded to a unicode string.")
 
-    async def setup(self, config=None, parent_header=None):
-        if config:
-            self.config = config
+    async def setup(self, context_info=None, parent_header=None):
+        if context_info:
+            self.config["context_info"] = context_info
 
         if callable(getattr(self.agent, 'setup', None)):
-            await self.agent.setup(self.config, parent_header=parent_header)
+            await self.agent.setup(self.config["context_info"], parent_header=parent_header)
 
     def cleanup(self):
         self.subkernel.cleanup()
         for msg_type, intercept_func, stream in self.intercepts:
             self.beaker_kernel.remove_intercept(msg_type=msg_type, func=intercept_func, stream=stream)
         del self.agent
```

### Comparing `beaker_kernel-1.5.0/beaker_kernel/lib/jupyter_kernel_proxy.py` & `beaker_kernel-1.5.1/beaker_kernel/lib/jupyter_kernel_proxy.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/lib/utils.py` & `beaker_kernel-1.5.1/beaker_kernel/lib/utils.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/lib/subkernels/base.py` & `beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/base.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/lib/subkernels/julia.py` & `beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/julia.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/lib/subkernels/python.py` & `beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/python.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/lib/subkernels/rlang.py` & `beaker_kernel-1.5.1/beaker_kernel/lib/subkernels/rlang.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/admin_utils.py` & `beaker_kernel-1.5.1/beaker_kernel/server/admin_utils.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/dev.py` & `beaker_kernel-1.5.1/beaker_kernel/server/dev.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/main.py` & `beaker_kernel-1.5.1/beaker_kernel/server/main.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/admin.html` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/admin.html`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/beaker.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/beaker.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/favicon.ico` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/index.html` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/index.html`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/css/admin.06bbaee6.css` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/css/admin.06bbaee6.css`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/css/chunk-vendors.f59cad43.css` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/css/chunk-vendors.f59cad43.css`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/css/index.622cafdc.css` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/css/index.622cafdc.css`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/fonts/primeicons.0112589c.ttf` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.0112589c.ttf`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/fonts/primeicons.ba3f916d.woff2` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.ba3f916d.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/fonts/primeicons.f8b9e8a4.woff` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.f8b9e8a4.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/fonts/primeicons.ffecb254.eot` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/fonts/primeicons.ffecb254.eot`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/add-above.ee286b1c.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/add-above.ee286b1c.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/add-below.bcf3422e.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/add-below.bcf3422e.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/bell.bccaf100.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bell.bccaf100.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/bug-dot.326bc45a.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bug-dot.326bc45a.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/bug.e30064ad.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/bug.e30064ad.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/build.e3fdf668.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/build.e3fdf668.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/case-sensitive.eaefe455.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/case-sensitive.eaefe455.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/copyright.f38f4ec0.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/copyright.f38f4ec0.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/cut.18edde39.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/cut.18edde39.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/duplicate.8815451e.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/duplicate.8815451e.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/html5.ea435392.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/html5.ea435392.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/info.4d82eb41.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/info.4d82eb41.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/json.a2c296bb.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/json.a2c296bb.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/julia.499ac74e.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/julia.499ac74e.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/jupyter-favicon.b19d8551.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/jupyter-favicon.b19d8551.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/jupyter.a48871a7.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/jupyter.a48871a7.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/jupyterlab-wordmark.6280567a.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/jupyterlab-wordmark.6280567a.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/move-down.5e4a3948.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/move-down.5e4a3948.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/move-up.fa81409d.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/move-up.fa81409d.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/not-trusted.8bc17823.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/not-trusted.8bc17823.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/palette.14c4709b.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/palette.14c4709b.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/pdf.f6a1dc59.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/pdf.f6a1dc59.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/primeicons.943ab24c.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/primeicons.943ab24c.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/python.0ffed0a2.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/python.0ffed0a2.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/react.c81f1b87.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/react.c81f1b87.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/regex.fa85da44.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/regex.fa85da44.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/settings.454fe53f.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/settings.454fe53f.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/share.ccbe241a.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/share.ccbe241a.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/tag.8887c8e5.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/tag.8887c8e5.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/terminal.0a8eb862.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/terminal.0a8eb862.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/trusted.3ac2122f.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/trusted.3ac2122f.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/users.cba8edb3.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/users.cba8edb3.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/img/word.c993422c.svg` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/img/word.c993422c.svg`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/js/admin.595fbd46.js` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/admin.595fbd46.js`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/js/admin.595fbd46.js.map` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/admin.595fbd46.js.map`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js.map` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/chunk-vendors.a7a87064.js.map`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/js/index.e38a09de.js` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/index.e38a09de.js`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/static/js/index.e38a09de.js.map` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/static/js/index.e38a09de.js.map`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/theme.css` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/theme.css`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff2` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-300.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff2` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-700.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff2` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-dark/fonts/lato-v17-latin-ext_latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/theme.css` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/theme.css`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff2` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-300.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff2` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-700.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff2` & `beaker_kernel-1.5.1/beaker_kernel/server/ui/themes/soho-light/fonts/lato-v17-latin-ext_latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/.gitignore` & `beaker_kernel-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/LICENSE.txt` & `beaker_kernel-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/README.md` & `beaker_kernel-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/hatch_build.py` & `beaker_kernel-1.5.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `beaker_kernel-1.5.0/pyproject.toml` & `beaker_kernel-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "jupyter-client"]
 build-backend = "hatchling.build"
 
 [project]
 name = "beaker-kernel"
-version = "1.5.0"
+version = "1.5.1"
 description = ""
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Matthew Printz", email = "matt@jataware.com" },
```

### Comparing `beaker_kernel-1.5.0/PKG-INFO` & `beaker_kernel-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: beaker-kernel
-Version: 1.5.0
+Version: 1.5.1
 Project-URL: Documentation, https://github.com/unknown/beaker-kernel#readme
 Project-URL: Issues, https://github.com/unknown/beaker-kernel/issues
 Project-URL: Source, https://github.com/unknown/beaker-kernel
 Author-email: Matthew Printz <matt@jataware.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

