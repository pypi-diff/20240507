# Comparing `tmp/weditor-0.7.2.tar.gz` & `tmp/weditor-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weditor-0.7.2.tar", last modified: Fri Nov  3 06:24:03 2023, max compression
+gzip compressed data, was "weditor-0.7.3.tar", last modified: Tue May  7 07:33:11 2024, max compression
```

## Comparing `weditor-0.7.2.tar` & `weditor-0.7.3.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.589191 weditor-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.557189 weditor-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.573190 weditor-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-11-03 06:23:49.000000 weditor-0.7.2/.github/workflows/publish-to-pypi.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.573190 weditor-0.7.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-11-03 06:23:49.000000 weditor-0.7.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-03 06:23:49.000000 weditor-0.7.2/ABOUT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2023-11-03 06:23:49.000000 weditor-0.7.2/API.md
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-11-03 06:24:03.000000 weditor-0.7.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)   966854 2023-11-03 06:23:49.000000 weditor-0.7.2/CHANGELOG.docx
--rw-r--r--   0 runner    (1001) docker     (127)      292 2023-11-03 06:24:03.000000 weditor-0.7.2/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2023-11-03 06:23:49.000000 weditor-0.7.2/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-11-03 06:23:49.000000 weditor-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2023-11-03 06:24:03.589191 weditor-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2023-11-03 06:23:49.000000 weditor-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2023-11-03 06:23:49.000000 weditor-0.7.2/README_ZH.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-03 06:23:49.000000 weditor-0.7.2/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2023-11-03 06:23:49.000000 weditor-0.7.2/log.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-11-03 06:23:49.000000 weditor-0.7.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.573190 weditor-0.7.2/samples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.573190 weditor-0.7.2/samples/ace/
--rw-r--r--   0 runner    (1001) docker     (127)   644638 2023-11-03 06:23:49.000000 weditor-0.7.2/samples/ace/ace.js
--rw-r--r--   0 runner    (1001) docker     (127)    67635 2023-11-03 06:23:49.000000 weditor-0.7.2/samples/ace/ext-language_tools.js
--rw-r--r--   0 runner    (1001) docker     (127)   205106 2023-11-03 06:23:49.000000 weditor-0.7.2/samples/ace/keybinding-vim.js
--rw-r--r--   0 runner    (1001) docker     (127)     8671 2023-11-03 06:23:49.000000 weditor-0.7.2/samples/ace/mode-python.js
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2023-11-03 06:23:49.000000 weditor-0.7.2/samples/ace/theme-monokai.js
--rw-r--r--   0 runner    (1001) docker     (127)    54822 2023-11-03 06:23:49.000000 weditor-0.7.2/samples/bg.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-11-03 06:23:49.000000 weditor-0.7.2/samples/bower.json
--rw-r--r--   0 runner    (1001) docker     (127)    23238 2023-11-03 06:23:49.000000 weditor-0.7.2/samples/index.html
--rw-r--r--   0 runner    (1001) docker     (127)   258966 2023-11-03 06:23:49.000000 weditor-0.7.2/screenshot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-03 06:24:03.589191 weditor-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-03 06:23:49.000000 weditor-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.577190 weditor-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-03 06:23:49.000000 weditor-0.7.2/tests/test_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-11-03 06:23:49.000000 weditor-0.7.2/tests/test_web_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.577190 weditor-0.7.2/weditor/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/page.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.577190 weditor-0.7.2/weditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.581190 weditor-0.7.2/weditor/static/ace/
--rw-r--r--   0 runner    (1001) docker     (127)   644638 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/ace/ace.js
--rw-r--r--   0 runner    (1001) docker     (127)    67635 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/ace/ext-language_tools.js
--rw-r--r--   0 runner    (1001) docker     (127)   205106 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/ace/keybinding-vim.js
--rw-r--r--   0 runner    (1001) docker     (127)     8671 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/ace/mode-python.js
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/ace/theme-monokai.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.565189 weditor-0.7.2/weditor/static/cdn_libraries/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.565189 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.561189 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.565189 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.581190 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/
--rw-r--r--   0 runner    (1001) docker     (127)   121200 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   542194 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.581190 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.581190 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/js/
--rw-r--r--   0 runner    (1001) docker     (127)    37045 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.561189 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.561189 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.581190 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/css/
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/css/bootstrap-select.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.581190 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/
--rw-r--r--   0 runner    (1001) docker     (127)    39003 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    33963 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.581190 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.565189 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.581190 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/
--rw-r--r--   0 runner    (1001) docker     (127)   365464 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ace.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    39225 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-language_tools.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    12001 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-searchbox.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/mode-python.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/theme-monokai.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.565189 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.581190 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/dist/
--rw-r--r--   0 runner    (1001) docker     (127)    86927 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/dist/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.565189 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.581190 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/
--rw-r--r--   0 runner    (1001) docker     (127)   139314 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/jstree.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.565189 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.581190 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/32px.png
--rw-r--r--   0 runner    (1001) docker     (127)    27281 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/style.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/throbber.gif
--rw-r--r--   0 runner    (1001) docker     (127)    15076 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/vue-resource@1.5.1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.581190 weditor-0.7.2/weditor/static/cdn_libraries/unpkg.com/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.565189 weditor-0.7.2/weditor/static/cdn_libraries/unpkg.com/element-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.585190 weditor-0.7.2/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/
--rw-r--r--   0 runner    (1001) docker     (127)   567194 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.585190 weditor-0.7.2/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.585190 weditor-0.7.2/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    28200 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/fonts/element-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   232432 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/index.css
--rw-r--r--   0 runner    (1001) docker     (127)     8699 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/cdn_libraries/unpkg.com/vue-async-computed@3.7.0
--rw-r--r--   0 runner    (1001) docker     (127)    32138 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.585190 weditor-0.7.2/weditor/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/js/common.js
--rw-r--r--   0 runner    (1001) docker     (127)    48120 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/js/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.569189 weditor-0.7.2/weditor/static/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.585190 weditor-0.7.2/weditor/static/libs/css/
--rw-r--r--   0 runner    (1001) docker     (127)    80548 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/libs/css/buttons.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.569189 weditor-0.7.2/weditor/static/libs/fontawesome/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.585190 weditor-0.7.2/weditor/static/libs/fontawesome/css/
--rw-r--r--   0 runner    (1001) docker     (127)    37414 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/libs/fontawesome/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (127)    21778 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/libs/fontawesome/css/font-awesome.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    31000 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/libs/fontawesome/css/font-awesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.585190 weditor-0.7.2/weditor/static/libs/fontawesome/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   134808 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/libs/fontawesome/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (127)   165742 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   444379 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)   165548 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    98024 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    77160 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.589191 weditor-0.7.2/weditor/static/libs/vue-2.5.16/
--rw-r--r--   0 runner    (1001) docker     (127)   289303 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/libs/vue-2.5.16/vue.js
--rw-r--r--   0 runner    (1001) docker     (127)    86452 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/libs/vue-2.5.16/vue.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/loading.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/running.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.589191 weditor-0.7.2/weditor/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    15204 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/templates/widget_preview.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.589191 weditor-0.7.2/weditor/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/web/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.589191 weditor-0.7.2/weditor/web/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/web/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/web/handlers/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/web/handlers/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/web/handlers/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/web/ipyshell-console.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/web/proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/web/uidumplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/web/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-11-03 06:23:49.000000 weditor-0.7.2/weditor/web/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 06:24:03.577190 weditor-0.7.2/weditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2023-11-03 06:24:03.000000 weditor-0.7.2/weditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2023-11-03 06:24:03.000000 weditor-0.7.2/weditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 06:24:03.000000 weditor-0.7.2/weditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-03 06:24:03.000000 weditor-0.7.2/weditor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 06:24:03.000000 weditor-0.7.2/weditor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-03 06:24:03.000000 weditor-0.7.2/weditor.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-11-03 06:24:03.000000 weditor-0.7.2/weditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-03 06:24:03.000000 weditor-0.7.2/weditor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.198913 weditor-0.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.178913 weditor-0.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-07 07:33:01.000000 weditor-0.7.3/.github/workflows/publish-to-pypi.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.178913 weditor-0.7.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 07:33:01.000000 weditor-0.7.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 07:33:01.000000 weditor-0.7.3/ABOUT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-07 07:33:01.000000 weditor-0.7.3/API.md
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 07:33:11.000000 weditor-0.7.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)   966854 2024-05-07 07:33:01.000000 weditor-0.7.3/CHANGELOG.docx
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-07 07:33:11.000000 weditor-0.7.3/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-07 07:33:01.000000 weditor-0.7.3/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 07:33:01.000000 weditor-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-07 07:33:11.198913 weditor-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-07 07:33:01.000000 weditor-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-07 07:33:01.000000 weditor-0.7.3/README_ZH.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 07:33:01.000000 weditor-0.7.3/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-07 07:33:01.000000 weditor-0.7.3/log.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 07:33:01.000000 weditor-0.7.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.182913 weditor-0.7.3/samples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.182913 weditor-0.7.3/samples/ace/
+-rw-r--r--   0 runner    (1001) docker     (127)   644638 2024-05-07 07:33:01.000000 weditor-0.7.3/samples/ace/ace.js
+-rw-r--r--   0 runner    (1001) docker     (127)    67635 2024-05-07 07:33:01.000000 weditor-0.7.3/samples/ace/ext-language_tools.js
+-rw-r--r--   0 runner    (1001) docker     (127)   205106 2024-05-07 07:33:01.000000 weditor-0.7.3/samples/ace/keybinding-vim.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8671 2024-05-07 07:33:01.000000 weditor-0.7.3/samples/ace/mode-python.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-07 07:33:01.000000 weditor-0.7.3/samples/ace/theme-monokai.js
+-rw-r--r--   0 runner    (1001) docker     (127)    54822 2024-05-07 07:33:01.000000 weditor-0.7.3/samples/bg.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-07 07:33:01.000000 weditor-0.7.3/samples/bower.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23238 2024-05-07 07:33:01.000000 weditor-0.7.3/samples/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)   258966 2024-05-07 07:33:01.000000 weditor-0.7.3/screenshot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-07 07:33:11.198913 weditor-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 07:33:01.000000 weditor-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.182913 weditor-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 07:33:01.000000 weditor-0.7.3/tests/test_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-07 07:33:01.000000 weditor-0.7.3/tests/test_web_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.182913 weditor-0.7.3/weditor/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/page.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.186913 weditor-0.7.3/weditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.186913 weditor-0.7.3/weditor/static/ace/
+-rw-r--r--   0 runner    (1001) docker     (127)   644638 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/ace/ace.js
+-rw-r--r--   0 runner    (1001) docker     (127)    67635 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/ace/ext-language_tools.js
+-rw-r--r--   0 runner    (1001) docker     (127)   205106 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/ace/keybinding-vim.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8671 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/ace/mode-python.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/ace/theme-monokai.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/weditor/static/cdn_libraries/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.186913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   121200 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   542194 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.186913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.186913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    37045 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.186913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/css/bootstrap-select.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.186913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    39003 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    33963 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.190913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.190913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/
+-rw-r--r--   0 runner    (1001) docker     (127)   365464 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ace.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    39225 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-language_tools.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-searchbox.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/mode-python.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/theme-monokai.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.190913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)    86927 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/dist/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.190913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)   139314 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/jstree.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.190913 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/32px.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27281 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/style.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/throbber.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    15076 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/vue-resource@1.5.1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.190913 weditor-0.7.3/weditor/static/cdn_libraries/unpkg.com/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/weditor/static/cdn_libraries/unpkg.com/element-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.190913 weditor-0.7.3/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)   567194 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.190913 weditor-0.7.3/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.190913 weditor-0.7.3/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/fonts/element-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   232432 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/cdn_libraries/unpkg.com/vue-async-computed@3.7.0
+-rw-r--r--   0 runner    (1001) docker     (127)    32138 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.194913 weditor-0.7.3/weditor/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/js/common.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48120 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/js/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/weditor/static/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.194913 weditor-0.7.3/weditor/static/libs/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    80548 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/libs/css/buttons.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.174913 weditor-0.7.3/weditor/static/libs/fontawesome/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.194913 weditor-0.7.3/weditor/static/libs/fontawesome/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    37414 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/libs/fontawesome/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (127)    21778 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/libs/fontawesome/css/font-awesome.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/libs/fontawesome/css/font-awesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.194913 weditor-0.7.3/weditor/static/libs/fontawesome/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   134808 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/libs/fontawesome/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.194913 weditor-0.7.3/weditor/static/libs/vue-2.5.16/
+-rw-r--r--   0 runner    (1001) docker     (127)   289303 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/libs/vue-2.5.16/vue.js
+-rw-r--r--   0 runner    (1001) docker     (127)    86452 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/libs/vue-2.5.16/vue.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/loading.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/running.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.198913 weditor-0.7.3/weditor/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    15456 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/templates/widget_preview.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.198913 weditor-0.7.3/weditor/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/web/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.198913 weditor-0.7.3/weditor/web/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/web/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/web/handlers/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/web/handlers/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/web/handlers/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/web/ipyshell-console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/web/proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/web/uidumplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/web/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-07 07:33:01.000000 weditor-0.7.3/weditor/web/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:11.182913 weditor-0.7.3/weditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-07 07:33:11.000000 weditor-0.7.3/weditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-07 07:33:11.000000 weditor-0.7.3/weditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:33:11.000000 weditor-0.7.3/weditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 07:33:11.000000 weditor-0.7.3/weditor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:33:11.000000 weditor-0.7.3/weditor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 07:33:11.000000 weditor-0.7.3/weditor.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 07:33:11.000000 weditor-0.7.3/weditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 07:33:11.000000 weditor-0.7.3/weditor.egg-info/top_level.txt
```

### Comparing `weditor-0.7.2/.github/workflows/publish-to-pypi.yml` & `weditor-0.7.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/API.md` & `weditor-0.7.3/API.md`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/CHANGELOG.docx` & `weditor-0.7.3/CHANGELOG.docx`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/DEVELOP.md` & `weditor-0.7.3/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/LICENSE` & `weditor-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/PKG-INFO` & `weditor-0.7.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 1.2
 Name: weditor
-Version: 0.7.2
+Version: 0.7.3
 Summary: tool for writing atx script
 Home-page: https://github.com/openatx/weditor
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
-Description: # WEditor
+Description: # Because it is difficult to reconstruct this project, I wrote a new one. Visit <https://appinspector.devsleep.com/> and have a try
+        
+        ## WEditor
         [![image](https://img.shields.io/pypi/v/weditor.svg?style=flat-square)](https://pypi.python.org/pypi/weditor)
         [![image](https://img.shields.io/github/stars/alibaba/web-editor.svg?style=social&label=Star&style=flat-square)](https://github.com/alibaba/web-editor)
         [![image](https://travis-ci.org/alibaba/web-editor.svg?branch=master)](https://travis-ci.org/alibaba/web-editor)
         
         [中文文档](README_ZH.md)
         
         This project is subproject for smart phone test framework [openatx](https://github.com/openatx)
```

### Comparing `weditor-0.7.2/README.md` & `weditor-0.7.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# WEditor
+# Because it is difficult to reconstruct this project, I wrote a new one. Visit <https://appinspector.devsleep.com/> and have a try
+
+## WEditor
 [![image](https://img.shields.io/pypi/v/weditor.svg?style=flat-square)](https://pypi.python.org/pypi/weditor)
 [![image](https://img.shields.io/github/stars/alibaba/web-editor.svg?style=social&label=Star&style=flat-square)](https://github.com/alibaba/web-editor)
 [![image](https://travis-ci.org/alibaba/web-editor.svg?branch=master)](https://travis-ci.org/alibaba/web-editor)
 
 [中文文档](README_ZH.md)
 
 This project is subproject for smart phone test framework [openatx](https://github.com/openatx)
```

### Comparing `weditor-0.7.2/README_ZH.md` & `weditor-0.7.3/README_ZH.md`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/log.txt` & `weditor-0.7.3/log.txt`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/samples/ace/ace.js` & `weditor-0.7.3/samples/ace/ace.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/samples/ace/ext-language_tools.js` & `weditor-0.7.3/samples/ace/ext-language_tools.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/samples/ace/keybinding-vim.js` & `weditor-0.7.3/samples/ace/keybinding-vim.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/samples/ace/mode-python.js` & `weditor-0.7.3/samples/ace/mode-python.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/samples/ace/theme-monokai.js` & `weditor-0.7.3/samples/ace/theme-monokai.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/samples/bg.jpg` & `weditor-0.7.3/samples/bg.jpg`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/samples/index.html` & `weditor-0.7.3/samples/index.html`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/screenshot.jpg` & `weditor-0.7.3/screenshot.jpg`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/tests/test_web_utils.py` & `weditor-0.7.3/tests/test_web_utils.py`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/__main__.py` & `weditor-0.7.3/weditor/__main__.py`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/page.xml` & `weditor-0.7.3/weditor/page.xml`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/ace/ace.js` & `weditor-0.7.3/weditor/static/ace/ace.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/ace/ext-language_tools.js` & `weditor-0.7.3/weditor/static/ace/ext-language_tools.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/ace/keybinding-vim.js` & `weditor-0.7.3/weditor/static/ace/keybinding-vim.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/ace/mode-python.js` & `weditor-0.7.3/weditor/static/ace/mode-python.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/ace/theme-monokai.js` & `weditor-0.7.3/weditor/static/ace/theme-monokai.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css.map` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff2` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/js/bootstrap.min.js` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap/3.3.7/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/css/bootstrap-select.min.css` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/css/bootstrap-select.min.css`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.js.map` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.js.map`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.min.js` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/bootstrap.select/1.12.2/js/bootstrap-select.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ace.min.js` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ace.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-language_tools.min.js` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-language_tools.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-searchbox.min.js` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/ext-searchbox.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/mode-python.min.js` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/mode-python.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/theme-monokai.js` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/ace-builds@1.4.12/src-noconflict/theme-monokai.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/dist/jquery.min.js` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jquery@3.3.1/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/jstree.min.js` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/jstree.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/32px.png` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/32px.png`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/style.min.css` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/style.min.css`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/throbber.gif` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/jstree@3.3.8/dist/themes/default/throbber.gif`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/vue-resource@1.5.1` & `weditor-0.7.3/weditor/static/cdn_libraries/cdn.jsdelivr.net/npm/vue-resource@1.5.1`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/index.js` & `weditor-0.7.3/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/index.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/fonts/element-icons.woff` & `weditor-0.7.3/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/fonts/element-icons.woff`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/index.css` & `weditor-0.7.3/weditor/static/cdn_libraries/unpkg.com/element-ui/lib/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/cdn_libraries/unpkg.com/vue-async-computed@3.7.0` & `weditor-0.7.3/weditor/static/cdn_libraries/unpkg.com/vue-async-computed@3.7.0`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/favicon.ico` & `weditor-0.7.3/weditor/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/js/common.js` & `weditor-0.7.3/weditor/static/js/common.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/js/index.js` & `weditor-0.7.3/weditor/static/js/index.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/libs/css/buttons.css` & `weditor-0.7.3/weditor/static/libs/css/buttons.css`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/libs/fontawesome/css/font-awesome.css` & `weditor-0.7.3/weditor/static/libs/fontawesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/libs/fontawesome/css/font-awesome.css.map` & `weditor-0.7.3/weditor/static/libs/fontawesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/libs/fontawesome/css/font-awesome.min.css` & `weditor-0.7.3/weditor/static/libs/fontawesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/libs/fontawesome/fonts/FontAwesome.otf` & `weditor-0.7.3/weditor/static/libs/fontawesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.eot` & `weditor-0.7.3/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.svg` & `weditor-0.7.3/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.ttf` & `weditor-0.7.3/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff` & `weditor-0.7.3/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff2` & `weditor-0.7.3/weditor/static/libs/fontawesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/libs/vue-2.5.16/vue.js` & `weditor-0.7.3/weditor/static/libs/vue-2.5.16/vue.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/libs/vue-2.5.16/vue.min.js` & `weditor-0.7.3/weditor/static/libs/vue-2.5.16/vue.min.js`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/loading.svg` & `weditor-0.7.3/weditor/static/loading.svg`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/running.svg` & `weditor-0.7.3/weditor/static/running.svg`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/static/style.css` & `weditor-0.7.3/weditor/static/style.css`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/templates/index.html` & `weditor-0.7.3/weditor/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -54,18 +54,21 @@
             Connect
             <i v-if="connecting" class="fa fa-spinner fa-spin"></i>
             <span v-if="deviceId" class="glyphicon glyphicon-grain color-green"></span>
           </button>
           <button :disabled="loading || connecting" class="btn btn-default" v-on:click="dumpHierarchyWithScreen()">
             <i class="fa fa-refresh" :class='{"fa-spin": dumping}'></i> Dump Hierarchy
           </button>
-          <template v-if="platform == 'Android'">
+          <template v-if="platform == 'Beta'">
             <el-switch v-model="liveScreen" active-text="实时" inactive-text="静态">
             </el-switch>
           </template>
+          <div class="form-group">
+            <span style="color: red">因原有的weditor修改难度过大，所以我重新写了一个新工具<a target="_blank" href="https://uiauto.dev">https://uiauto.dev</a>，欢迎试用</span>
+          </div>
         </form>
         <ul class="nav navbar-nav navbar-right">
           <!-- <li><a href="#">Link</a></li> -->
           <li class="dropdown">
             <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true"
               aria-expanded="false">相关文档 <span class="caret"></span></a>
             <ul class="dropdown-menu">
```

#### html2text {}

```diff
@@ -2,14 +2,15 @@
 _A_T_X_ _WW_EE_dd_ii_tt_oo_rr
 [One of: Android UIAutomator2/Android ADB/iOS][                    ]
 disabled="connecting"> Connect
 disabled="loading || connecting" class="btn btn-default" v-on:
 click="dumpHierarchyWithScreen()">
 class='{"fa-spin": dumping}'>
  Dump Hierarchy
+因原有的weditor修改难度过大，所以我重新写了一个新工具_h_t_t_p_s_:_/_/_u_i_a_u_t_o_._d_e_v，欢迎试用
     * _相_关_文_档
           o _o_p_e_n_a_t_x_/_w_e_d_i_t_o_r
           o _u_i_a_u_t_o_m_a_t_o_r_2_快_速_参_考
           o _o_p_e_n_a_t_x_/_u_i_a_u_t_o_m_a_t_o_r_2
           o _o_p_e_n_a_t_x_/_f_a_c_e_b_o_o_k_-_w_d_a
 dblclick="doTap(nodeSelected)" class="canvas-fg" v-bind:style="canvasStyle"> [/
 static/loading.svg]
```

### Comparing `weditor-0.7.2/weditor/templates/widget_preview.html` & `weditor-0.7.3/weditor/templates/widget_preview.html`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/web/device.py` & `weditor-0.7.3/weditor/web/device.py`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/web/handlers/page.py` & `weditor-0.7.3/weditor/web/handlers/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,16 @@
             })
         else:
             ret = {
                 "deviceId": id,
                 'success': True,
             }
             if platform == "android":
-                ws_addr = get_device(id).device.address.replace("http://", "ws://") # yapf: disable
-                ret['screenWebSocketUrl'] = ws_addr + "/minicap"
+                # ws_addr = get_device(id).device.address.replace("http://", "ws://") # yapf: disable
+                ret['screenWebSocketUrl'] = None #ws_addr + "/minicap"
             self.write(ret)
 
 
 class DeviceHierarchyHandler(BaseHandler):
     def get(self, device_id):
         d = get_device(device_id)
         self.write(d.dump_hierarchy())
```

### Comparing `weditor-0.7.2/weditor/web/handlers/proxy.py` & `weditor-0.7.3/weditor/web/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/web/handlers/shell.py` & `weditor-0.7.3/weditor/web/handlers/shell.py`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/web/ipyshell-console.py` & `weditor-0.7.3/weditor/web/ipyshell-console.py`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor/web/uidumplib.py` & `weditor-0.7.3/weditor/web/uidumplib.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     '_type': safe_xmlstr, # node className
     # Android
     'rect': parse_bounds,
     'text': convstr,
     'resourceId': convstr,
     'package': convstr,
     'checkable': str2bool,
+    'checked': str2bool,
     'scrollable': str2bool,
     'focused': str2bool,
     'clickable': str2bool,
     'selected': str2bool,
     'longClickable': str2bool,
     'focusable': str2bool,
     'password': str2bool,
@@ -141,19 +142,19 @@
     def travel(node):
         node['_id'] = str(uuid.uuid4())
         node['_type'] = node.pop('type', "null")
         if node.get('rect'):
             rect = node['rect']
             nrect = {}
             for k, v in rect.items():
-                nrect[k] = v * scale
+                nrect[k] = v * scale if isinstance(v, int) else "null"
             node['rect'] = nrect
 
         for child in node.get('children', []):
             travel(child)
         return node
 
     return travel(sourcejson)
 
 
 def get_webview_hierarchy(d):
-    pass
+    pass
```

### Comparing `weditor-0.7.2/weditor/web/utils.py` & `weditor-0.7.3/weditor/web/utils.py`

 * *Files identical despite different names*

### Comparing `weditor-0.7.2/weditor.egg-info/PKG-INFO` & `weditor-0.7.3/weditor.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 1.2
 Name: weditor
-Version: 0.7.2
+Version: 0.7.3
 Summary: tool for writing atx script
 Home-page: https://github.com/openatx/weditor
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
-Description: # WEditor
+Description: # Because it is difficult to reconstruct this project, I wrote a new one. Visit <https://appinspector.devsleep.com/> and have a try
+        
+        ## WEditor
         [![image](https://img.shields.io/pypi/v/weditor.svg?style=flat-square)](https://pypi.python.org/pypi/weditor)
         [![image](https://img.shields.io/github/stars/alibaba/web-editor.svg?style=social&label=Star&style=flat-square)](https://github.com/alibaba/web-editor)
         [![image](https://travis-ci.org/alibaba/web-editor.svg?branch=master)](https://travis-ci.org/alibaba/web-editor)
         
         [中文文档](README_ZH.md)
         
         This project is subproject for smart phone test framework [openatx](https://github.com/openatx)
```

### Comparing `weditor-0.7.2/weditor.egg-info/SOURCES.txt` & `weditor-0.7.3/weditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

