# Comparing `tmp/mode-ng-0.6.1.tar.gz` & `tmp/mode_ng-0.7.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mode-ng-0.6.1.tar", last modified: Thu Dec  8 09:48:50 2022, max compression
+gzip compressed data, was "mode_ng-0.7.0.dev0.tar", last modified: Tue May  7 07:14:23 2024, max compression
```

## Comparing `mode-ng-0.6.1.tar` & `mode_ng-0.7.0.dev0.tar`

### file list

```diff
@@ -1,191 +1,192 @@
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.491251 mode-ng-0.6.1/
--rw-r--r--   0 lqhuang    (501) staff       (20)      462 2022-06-27 08:07:14.000000 mode-ng-0.6.1/AUTHORS
--rw-r--r--   0 lqhuang    (501) staff       (20)     4754 2022-12-08 09:48:07.000000 mode-ng-0.6.1/CHANGELOG.md
--rw-r--r--   0 lqhuang    (501) staff       (20)     2552 2022-06-27 08:08:34.000000 mode-ng-0.6.1/LICENSE
--rw-r--r--   0 lqhuang    (501) staff       (20)      341 2022-06-27 15:00:43.000000 mode-ng-0.6.1/MANIFEST.in
--rw-r--r--   0 lqhuang    (501) staff       (20)    17724 2022-12-08 09:48:50.491373 mode-ng-0.6.1/PKG-INFO
--rw-r--r--   0 lqhuang    (501) staff       (20)    16574 2022-12-08 09:47:38.000000 mode-ng-0.6.1/README.rst
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.453254 mode-ng-0.6.1/docs/
--rw-r--r--   0 lqhuang    (501) staff       (20)      820 2022-10-17 02:44:24.000000 mode-ng-0.6.1/docs/Makefile
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.453649 mode-ng-0.6.1/docs/_static/
--rw-r--r--   0 lqhuang    (501) staff       (20)        0 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/_static/.keep
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.453847 mode-ng-0.6.1/docs/_templates/
--rw-r--r--   0 lqhuang    (501) staff       (20)        0 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/_templates/.keep
--rw-r--r--   0 lqhuang    (501) staff       (20)       61 2022-10-17 02:44:24.000000 mode-ng-0.6.1/docs/changelog.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)     2059 2022-10-17 02:44:24.000000 mode-ng-0.6.1/docs/conf.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     1004 2022-10-17 02:44:24.000000 mode-ng-0.6.1/docs/copyright.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)       50 2022-10-17 02:44:24.000000 mode-ng-0.6.1/docs/faq.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      253 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/glossary.rst
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.455332 mode-ng-0.6.1/docs/images/
--rw-r--r--   0 lqhuang    (501) staff       (20)     1150 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/images/favicon.ico
--rw-r--r--   0 lqhuang    (501) staff       (20)   105363 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/images/logo.png
--rw-r--r--   0 lqhuang    (501) staff       (20)    21770 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/images/tutorial_graph.png
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.456960 mode-ng-0.6.1/docs/includes/
--rw-r--r--   0 lqhuang    (501) staff       (20)     5488 2022-10-17 02:44:24.000000 mode-ng-0.6.1/docs/includes/code-of-conduct.md
--rw-r--r--   0 lqhuang    (501) staff       (20)     4543 2022-10-17 02:44:24.000000 mode-ng-0.6.1/docs/includes/faq.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      891 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/includes/installation.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)     7202 2022-10-17 02:44:24.000000 mode-ng-0.6.1/docs/includes/introduction.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)      378 2022-10-17 02:44:24.000000 mode-ng-0.6.1/docs/index.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      477 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/introduction.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      765 2022-10-17 02:44:24.000000 mode-ng-0.6.1/docs/make.bat
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.467493 mode-ng-0.6.1/docs/reference/
--rw-r--r--   0 lqhuang    (501) staff       (20)      978 2022-10-17 02:44:24.000000 mode-ng-0.6.1/docs/reference/index.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      243 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.debug.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      258 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.exceptions.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      246 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.locals.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      327 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.loop.eventlet.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      323 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.loop.gevent.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      240 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.loop.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      323 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.loop.uvloop.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      243 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.proxy.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      225 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      252 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.services.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      249 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.signals.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      261 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.supervisors.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      249 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.threads.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      246 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.timers.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      243 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.types.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      270 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.types.services.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      267 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.types.signals.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      279 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.types.supervisors.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      261 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.aiter.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      279 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.collections.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      258 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.cron.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      267 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.futures.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      264 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.graphs.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      267 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.imports.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      264 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.locals.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      267 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.logging.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      261 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.loops.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      261 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.mocks.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      267 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.objects.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      264 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.queues.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      258 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.text.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      261 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.times.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      276 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.tracebacks.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      261 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.trees.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      282 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.types.graphs.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      279 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.utils.types.trees.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)      246 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/reference/mode.worker.rst
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.467736 mode-ng-0.6.1/docs/templates/
--rw-r--r--   0 lqhuang    (501) staff       (20)     1334 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/templates/readme.txt
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.468228 mode-ng-0.6.1/docs/userguide/
--rw-r--r--   0 lqhuang    (501) staff       (20)      137 2022-06-04 13:05:00.000000 mode-ng-0.6.1/docs/userguide/index.rst
--rw-r--r--   0 lqhuang    (501) staff       (20)     5868 2022-10-17 02:44:24.000000 mode-ng-0.6.1/docs/userguide/services.rst
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.469199 mode-ng-0.6.1/examples/
--rw-r--r--   0 lqhuang    (501) staff       (20)      720 2022-11-20 10:02:39.000000 mode-ng-0.6.1/examples/integration.py
--rw-r--r--   0 lqhuang    (501) staff       (20)      628 2022-11-20 10:02:39.000000 mode-ng-0.6.1/examples/service.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     4347 2022-06-04 13:05:00.000000 mode-ng-0.6.1/examples/tutorial.py
--rw-r--r--   0 lqhuang    (501) staff       (20)      705 2022-07-04 10:57:23.000000 mode-ng-0.6.1/examples/worker_log_to_file.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     5262 2022-12-08 09:48:07.000000 mode-ng-0.6.1/pyproject.toml
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.471063 mode-ng-0.6.1/requirements/
--rw-r--r--   0 lqhuang    (501) staff       (20)       36 2022-06-04 13:05:00.000000 mode-ng-0.6.1/requirements/ci.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)       92 2022-07-02 12:12:14.000000 mode-ng-0.6.1/requirements/default.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)       88 2022-12-08 08:54:28.000000 mode-ng-0.6.1/requirements/dev.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)       61 2022-10-17 02:44:24.000000 mode-ng-0.6.1/requirements/docs.txt
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.471680 mode-ng-0.6.1/requirements/extras/
--rw-r--r--   0 lqhuang    (501) staff       (20)       29 2022-06-04 13:05:00.000000 mode-ng-0.6.1/requirements/extras/eventlet.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)       15 2022-06-04 13:05:00.000000 mode-ng-0.6.1/requirements/extras/gevent.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)       14 2022-06-04 13:05:00.000000 mode-ng-0.6.1/requirements/extras/uvloop.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)      223 2022-07-02 12:12:14.000000 mode-ng-0.6.1/requirements/flakes.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)       31 2022-07-02 12:12:14.000000 mode-ng-0.6.1/requirements/lint.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)       55 2022-12-08 08:54:32.000000 mode-ng-0.6.1/requirements/release.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)       73 2022-12-04 11:20:49.000000 mode-ng-0.6.1/requirements/test.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)       42 2022-10-20 09:10:05.000000 mode-ng-0.6.1/requirements/typecheck.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)      275 2022-12-08 09:48:50.491797 mode-ng-0.6.1/setup.cfg
--rw-r--r--   0 lqhuang    (501) staff       (20)     1076 2022-06-29 07:34:02.000000 mode-ng-0.6.1/setup.py
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.446148 mode-ng-0.6.1/src/
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.474376 mode-ng-0.6.1/src/mode/
--rw-r--r--   0 lqhuang    (501) staff       (20)     2496 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/__init__.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     2390 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/debug.py
--rw-r--r--   0 lqhuang    (501) staff       (20)      162 2022-06-27 07:26:57.000000 mode-ng-0.6.1/src/mode/exceptions.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    25296 2022-12-08 09:38:53.000000 mode-ng-0.6.1/src/mode/locals.py
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.475452 mode-ng-0.6.1/src/mode/loop/
--rw-r--r--   0 lqhuang    (501) staff       (20)     1904 2022-12-08 09:17:06.000000 mode-ng-0.6.1/src/mode/loop/__init__.py
--rw-r--r--   0 lqhuang    (501) staff       (20)      544 2022-12-08 09:17:06.000000 mode-ng-0.6.1/src/mode/loop/_gevent_loop.py
--rw-r--r--   0 lqhuang    (501) staff       (20)      753 2022-06-27 07:26:57.000000 mode-ng-0.6.1/src/mode/loop/eventlet.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     1645 2022-12-08 09:18:09.000000 mode-ng-0.6.1/src/mode/loop/gevent.py
--rw-r--r--   0 lqhuang    (501) staff       (20)      153 2022-06-27 07:26:57.000000 mode-ng-0.6.1/src/mode/loop/uvloop.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     3150 2022-12-08 09:07:06.000000 mode-ng-0.6.1/src/mode/proxy.py
--rw-r--r--   0 lqhuang    (501) staff       (20)       56 2022-06-27 07:26:57.000000 mode-ng-0.6.1/src/mode/py.typed
--rw-r--r--   0 lqhuang    (501) staff       (20)    37634 2022-12-08 09:02:40.000000 mode-ng-0.6.1/src/mode/services.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     8029 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/signals.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     9052 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/supervisors.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    14267 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/threads.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     6040 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/timers.py
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.476442 mode-ng-0.6.1/src/mode/types/
--rw-r--r--   0 lqhuang    (501) staff       (20)      300 2022-12-04 13:19:41.000000 mode-ng-0.6.1/src/mode/types/__init__.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     3814 2022-12-08 09:09:56.000000 mode-ng-0.6.1/src/mode/types/services.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     3037 2022-12-08 09:10:55.000000 mode-ng-0.6.1/src/mode/types/signals.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     1250 2022-12-08 09:11:06.000000 mode-ng-0.6.1/src/mode/types/supervisors.py
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.481004 mode-ng-0.6.1/src/mode/utils/
--rw-r--r--   0 lqhuang    (501) staff       (20)        0 2022-06-27 07:26:57.000000 mode-ng-0.6.1/src/mode/utils/__init__.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     4395 2022-12-08 09:11:21.000000 mode-ng-0.6.1/src/mode/utils/aiter.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    21845 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/utils/collections.py
--rw-r--r--   0 lqhuang    (501) staff       (20)      666 2022-06-29 07:34:02.000000 mode-ng-0.6.1/src/mode/utils/cron.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     4477 2022-12-08 09:12:02.000000 mode-ng-0.6.1/src/mode/utils/futures.py
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.481887 mode-ng-0.6.1/src/mode/utils/graphs/
--rw-r--r--   0 lqhuang    (501) staff       (20)      122 2022-06-27 07:26:57.000000 mode-ng-0.6.1/src/mode/utils/graphs/__init__.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     4046 2022-06-27 07:26:57.000000 mode-ng-0.6.1/src/mode/utils/graphs/formatter.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     6562 2022-11-20 10:02:39.000000 mode-ng-0.6.1/src/mode/utils/graphs/graph.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    11852 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/utils/imports.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     2727 2022-12-08 09:39:04.000000 mode-ng-0.6.1/src/mode/utils/locals.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     2655 2022-11-20 10:02:39.000000 mode-ng-0.6.1/src/mode/utils/locks.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    31579 2022-12-08 09:13:17.000000 mode-ng-0.6.1/src/mode/utils/logging.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     2432 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/utils/loops.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     2989 2022-11-20 10:02:39.000000 mode-ng-0.6.1/src/mode/utils/mocks.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    16771 2022-12-08 09:14:03.000000 mode-ng-0.6.1/src/mode/utils/objects.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     7511 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/utils/queues.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     6951 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/utils/text.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     8189 2022-12-08 09:14:38.000000 mode-ng-0.6.1/src/mode/utils/times.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     8552 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/utils/tracebacks.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     4866 2022-12-08 09:15:06.000000 mode-ng-0.6.1/src/mode/utils/trees.py
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.482756 mode-ng-0.6.1/src/mode/utils/types/
--rw-r--r--   0 lqhuang    (501) staff       (20)      107 2022-12-08 09:15:22.000000 mode-ng-0.6.1/src/mode/utils/types/__init__.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     2761 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/utils/types/graphs.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     1674 2022-12-08 09:17:05.000000 mode-ng-0.6.1/src/mode/utils/types/trees.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    12638 2022-12-08 09:00:25.000000 mode-ng-0.6.1/src/mode/worker.py
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.484048 mode-ng-0.6.1/src/mode_ng.egg-info/
--rw-r--r--   0 lqhuang    (501) staff       (20)    17724 2022-12-08 09:48:50.000000 mode-ng-0.6.1/src/mode_ng.egg-info/PKG-INFO
--rw-r--r--   0 lqhuang    (501) staff       (20)     4549 2022-12-08 09:48:50.000000 mode-ng-0.6.1/src/mode_ng.egg-info/SOURCES.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)        1 2022-12-08 09:48:50.000000 mode-ng-0.6.1/src/mode_ng.egg-info/dependency_links.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)      139 2022-12-08 09:48:50.000000 mode-ng-0.6.1/src/mode_ng.egg-info/requires.txt
--rw-r--r--   0 lqhuang    (501) staff       (20)        5 2022-12-08 09:48:50.000000 mode-ng-0.6.1/src/mode_ng.egg-info/top_level.txt
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.484640 mode-ng-0.6.1/tests/
--rw-r--r--   0 lqhuang    (501) staff       (20)        0 2022-06-27 11:16:15.000000 mode-ng-0.6.1/tests/__init__.py
--rw-r--r--   0 lqhuang    (501) staff       (20)       78 2022-06-04 13:05:00.000000 mode-ng-0.6.1/tests/conftest.py
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.486148 mode-ng-0.6.1/tests/functional/
--rw-r--r--   0 lqhuang    (501) staff       (20)        0 2022-07-02 13:38:30.000000 mode-ng-0.6.1/tests/functional/__init__.py
--rw-r--r--   0 lqhuang    (501) staff       (20)       89 2022-06-04 13:05:00.000000 mode-ng-0.6.1/tests/functional/test_mode.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     4569 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/functional/test_proxy.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     8204 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/functional/test_service.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     6558 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/functional/test_signals.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     3877 2022-06-04 13:05:00.000000 mode-ng-0.6.1/tests/functional/test_supervisors.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     7650 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/functional/test_timers.py
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.486360 mode-ng-0.6.1/tests/functional/utils/
--rw-r--r--   0 lqhuang    (501) staff       (20)        0 2022-06-04 13:05:00.000000 mode-ng-0.6.1/tests/functional/utils/__init__.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     3701 2022-12-04 13:15:14.000000 mode-ng-0.6.1/tests/test_packaging.py
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.487807 mode-ng-0.6.1/tests/unit/
--rw-r--r--   0 lqhuang    (501) staff       (20)        0 2022-06-04 13:05:00.000000 mode-ng-0.6.1/tests/unit/__init__.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     1441 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/unit/test_debug.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    19278 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/unit/test_locals.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    26958 2022-11-30 15:09:53.000000 mode-ng-0.6.1/tests/unit/test_services.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     5457 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/unit/test_supervisors.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    13033 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/unit/test_threads.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    16013 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/unit/test_worker.py
-drwxr-xr-x   0 lqhuang    (501) staff       (20)        0 2022-12-08 09:48:50.491080 mode-ng-0.6.1/tests/unit/utils/
--rw-r--r--   0 lqhuang    (501) staff       (20)        0 2022-06-04 13:05:00.000000 mode-ng-0.6.1/tests/unit/utils/__init__.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     2125 2022-06-29 07:34:02.000000 mode-ng-0.6.1/tests/unit/utils/test_aiter.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    18816 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/unit/utils/test_collections.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     1043 2022-06-27 11:19:53.000000 mode-ng-0.6.1/tests/unit/utils/test_cron.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     3685 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/unit/utils/test_futures.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     7974 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/unit/utils/test_imports.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     2710 2022-06-04 13:05:00.000000 mode-ng-0.6.1/tests/unit/utils/test_locals.py
--rw-r--r--   0 lqhuang    (501) staff       (20)      139 2022-06-04 13:05:00.000000 mode-ng-0.6.1/tests/unit/utils/test_locks.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    22237 2022-11-20 12:27:27.000000 mode-ng-0.6.1/tests/unit/utils/test_logging.py
--rw-r--r--   0 lqhuang    (501) staff       (20)    10138 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/unit/utils/test_objects.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     5376 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/unit/utils/test_queues.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     4359 2022-07-02 13:40:30.000000 mode-ng-0.6.1/tests/unit/utils/test_text.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     3551 2022-07-02 13:48:47.000000 mode-ng-0.6.1/tests/unit/utils/test_times.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     2433 2022-11-20 10:02:39.000000 mode-ng-0.6.1/tests/unit/utils/test_tracebacks.py
--rw-r--r--   0 lqhuang    (501) staff       (20)     1504 2022-06-04 13:05:00.000000 mode-ng-0.6.1/tests/unit/utils/test_trees.py
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.250686 mode_ng-0.7.0.dev0/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      462 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/AUTHORS
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     4754 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/CHANGELOG.md
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     2552 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/LICENSE
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      341 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/MANIFEST.in
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    18072 2024-05-07 07:14:23.250686 mode_ng-0.7.0.dev0/PKG-INFO
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    16574 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/README.rst
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.226686 mode_ng-0.7.0.dev0/docs/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      820 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/Makefile
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.226686 mode_ng-0.7.0.dev0/docs/_static/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)        0 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/_static/.keep
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.226686 mode_ng-0.7.0.dev0/docs/_templates/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)        0 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/_templates/.keep
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       61 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/changelog.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     2059 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/conf.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     1004 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/copyright.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       50 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/faq.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      253 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/glossary.rst
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.226686 mode_ng-0.7.0.dev0/docs/images/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     1150 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/images/favicon.ico
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)   105363 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/images/logo.png
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    21770 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/images/tutorial_graph.png
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.226686 mode_ng-0.7.0.dev0/docs/includes/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     5488 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/includes/code-of-conduct.md
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     4543 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/includes/faq.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      891 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/includes/installation.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     7202 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/includes/introduction.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      378 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/index.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      477 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/introduction.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      765 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/make.bat
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.234686 mode_ng-0.7.0.dev0/docs/reference/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      978 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/index.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      243 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.debug.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      258 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.exceptions.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      246 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.locals.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      327 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.loop.eventlet.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      323 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.loop.gevent.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      240 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.loop.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      323 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.loop.uvloop.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      243 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.proxy.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      225 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      252 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.services.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      249 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.signals.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      261 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.supervisors.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      249 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.threads.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      246 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.timers.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      243 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.types.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      270 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.types.services.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      267 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.types.signals.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      279 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.types.supervisors.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      261 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.aiter.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      279 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.collections.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      258 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.cron.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      267 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.futures.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      264 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.graphs.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      267 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.imports.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      264 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.locals.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      267 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.logging.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      261 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.loops.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      261 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.mocks.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      267 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.objects.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      264 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.queues.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      258 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.text.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      261 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.times.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      276 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.tracebacks.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      261 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.trees.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      282 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.types.graphs.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      279 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.utils.types.trees.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      246 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/reference/mode.worker.rst
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.234686 mode_ng-0.7.0.dev0/docs/templates/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     1334 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/templates/readme.txt
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.234686 mode_ng-0.7.0.dev0/docs/userguide/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      137 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/userguide/index.rst
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     5868 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/docs/userguide/services.rst
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.234686 mode_ng-0.7.0.dev0/examples/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     1334 2024-04-27 08:48:20.000000 mode_ng-0.7.0.dev0/examples/integration.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    10494 2024-05-07 07:05:19.000000 mode_ng-0.7.0.dev0/examples/notebook-demo.ipynb
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      628 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/examples/service.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      678 2024-04-27 03:22:31.000000 mode_ng-0.7.0.dev0/examples/thread_service.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     4347 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/examples/tutorial.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      705 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/examples/worker_log_to_file.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     5701 2024-05-07 07:09:24.000000 mode_ng-0.7.0.dev0/pyproject.toml
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.238686 mode_ng-0.7.0.dev0/requirements/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       36 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/requirements/ci.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       92 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/requirements/default.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       99 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/requirements/dev.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       61 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/requirements/docs.txt
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.238686 mode_ng-0.7.0.dev0/requirements/extras/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       29 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/requirements/extras/eventlet.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       15 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/requirements/extras/gevent.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       14 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/requirements/extras/uvloop.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      223 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/requirements/flakes.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       31 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/requirements/lint.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       55 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/requirements/release.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      119 2024-04-27 08:48:20.000000 mode_ng-0.7.0.dev0/requirements/test.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       42 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/requirements/typecheck.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      275 2024-05-07 07:14:23.250686 mode_ng-0.7.0.dev0/setup.cfg
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     1076 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/setup.py
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.222686 mode_ng-0.7.0.dev0/src/
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.238686 mode_ng-0.7.0.dev0/src/mode/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     2496 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/__init__.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     2390 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/debug.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      162 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/exceptions.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    25296 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/locals.py
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.242686 mode_ng-0.7.0.dev0/src/mode/loop/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     1904 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/loop/__init__.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      544 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/loop/_gevent_loop.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      753 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/loop/eventlet.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     1645 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/loop/gevent.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      153 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/loop/uvloop.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     3150 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/proxy.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       56 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/py.typed
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    38474 2024-04-27 08:48:20.000000 mode_ng-0.7.0.dev0/src/mode/services.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     8029 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/signals.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     9052 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/supervisors.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    14343 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/threads.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     6040 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/timers.py
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.242686 mode_ng-0.7.0.dev0/src/mode/types/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      300 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/types/__init__.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     3595 2024-04-27 08:48:20.000000 mode_ng-0.7.0.dev0/src/mode/types/services.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     3037 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/types/signals.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     1250 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/types/supervisors.py
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.242686 mode_ng-0.7.0.dev0/src/mode/utils/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)        0 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/__init__.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     4395 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/aiter.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    21845 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/collections.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      666 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/cron.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     4477 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/futures.py
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.242686 mode_ng-0.7.0.dev0/src/mode/utils/graphs/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      122 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/graphs/__init__.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     4046 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/graphs/formatter.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     6562 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/graphs/graph.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    11852 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/imports.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     2727 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/locals.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     2655 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/locks.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    31603 2024-04-27 08:48:20.000000 mode_ng-0.7.0.dev0/src/mode/utils/logging.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     2432 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/loops.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     2989 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/mocks.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    16771 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/objects.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     7511 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/queues.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     6951 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/text.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     8189 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/times.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     8552 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/tracebacks.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     4866 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/trees.py
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.246686 mode_ng-0.7.0.dev0/src/mode/utils/types/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      107 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/types/__init__.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     2761 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/types/graphs.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     1674 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/src/mode/utils/types/trees.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    14174 2024-04-27 10:24:58.000000 mode_ng-0.7.0.dev0/src/mode/worker.py
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.250686 mode_ng-0.7.0.dev0/src/mode_ng.egg-info/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    18072 2024-05-07 07:14:23.000000 mode_ng-0.7.0.dev0/src/mode_ng.egg-info/PKG-INFO
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     4581 2024-05-07 07:14:23.000000 mode_ng-0.7.0.dev0/src/mode_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)        1 2024-05-07 07:14:23.000000 mode_ng-0.7.0.dev0/src/mode_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      139 2024-05-07 07:14:23.000000 mode_ng-0.7.0.dev0/src/mode_ng.egg-info/requires.txt
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)        5 2024-05-07 07:14:23.000000 mode_ng-0.7.0.dev0/src/mode_ng.egg-info/top_level.txt
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.246686 mode_ng-0.7.0.dev0/tests/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)        0 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/__init__.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       78 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/conftest.py
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.246686 mode_ng-0.7.0.dev0/tests/functional/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)        0 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/functional/__init__.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)       89 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/functional/test_mode.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     4569 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/functional/test_proxy.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     8204 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/functional/test_service.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     6558 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/functional/test_signals.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     3877 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/functional/test_supervisors.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     7650 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/functional/test_timers.py
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.246686 mode_ng-0.7.0.dev0/tests/functional/utils/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)        0 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/functional/utils/__init__.py
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.246686 mode_ng-0.7.0.dev0/tests/unit/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)        0 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/__init__.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     1441 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/test_debug.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    19278 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/test_locals.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    26946 2024-04-27 08:48:20.000000 mode_ng-0.7.0.dev0/tests/unit/test_services.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     5457 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/test_supervisors.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    13818 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/test_threads.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    16013 2024-04-27 08:48:20.000000 mode_ng-0.7.0.dev0/tests/unit/test_worker.py
+drwxr-xr-x   0 lqhuang   (1001) lqhuang   (1001)        0 2024-05-07 07:14:23.250686 mode_ng-0.7.0.dev0/tests/unit/utils/
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)        0 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/__init__.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     2125 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_aiter.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    18816 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_collections.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     1043 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_cron.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     3685 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_futures.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     7974 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_imports.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     2710 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_locals.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)      139 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_locks.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    22237 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_logging.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)    10138 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_objects.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     5376 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_queues.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     4359 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_text.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     3551 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_times.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     2433 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_tracebacks.py
+-rw-r--r--   0 lqhuang   (1001) lqhuang   (1001)     1504 2023-10-24 04:02:55.000000 mode_ng-0.7.0.dev0/tests/unit/utils/test_trees.py
```

### Comparing `mode-ng-0.6.1/CHANGELOG.md` & `mode_ng-0.7.0.dev0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/LICENSE` & `mode_ng-0.7.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/PKG-INFO` & `mode_ng-0.7.0.dev0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: mode-ng
-Version: 0.6.1
-Summary: AsyncIO Service-based programming.
-Author-email: Ask Solem <ask@celeryproject.org>
-Maintainer-email: Lanqing Huang <lqhuang@outlook.com>
-License: BSD 3-Clause License
-Project-URL: homepage, https://github.com/lqhuang/mode-ng
-Keywords: asyncio,service,bootsteps,graph,coroutine,actor
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Unix
-Classifier: Environment :: No Input/Output (Daemon)
-Classifier: Framework :: AsyncIO
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-Provides-Extra: gevent
-Provides-Extra: eventlet
-Provides-Extra: uvloop
-License-File: LICENSE
-License-File: AUTHORS
-
 =====================
 Mode AsyncIO Services
 =====================
 
 |license| |wheel| |pyversion| |pyimp| |black|
 
 :Version: 0.6.1
```

### Comparing `mode-ng-0.6.1/README.rst` & `mode_ng-0.7.0.dev0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,45 @@
+Metadata-Version: 2.1
+Name: mode-ng
+Version: 0.7.0.dev0
+Summary: AsyncIO Service-based programming.
+Author-email: Ask Solem <ask@celeryproject.org>
+Maintainer-email: Lanqing Huang <lqhuang@outlook.com>
+License: BSD 3-Clause License
+Project-URL: homepage, https://github.com/lqhuang/mode-ng
+Keywords: asyncio,service,bootsteps,graph,coroutine,actor
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Unix
+Classifier: Environment :: No Input/Output (Daemon)
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
+Requires-Dist: colorlog>=2.9.0
+Requires-Dist: croniter>=0.3.16
+Requires-Dist: mypy_extensions
+Provides-Extra: uvloop
+Requires-Dist: uvloop>=0.8.1; extra == "uvloop"
+Provides-Extra: gevent
+Requires-Dist: aiogevent~=0.2; extra == "gevent"
+Provides-Extra: eventlet
+Requires-Dist: aioeventlet~=0.5.1; extra == "eventlet"
+Requires-Dist: dnspython; extra == "eventlet"
+
 =====================
 Mode AsyncIO Services
 =====================
 
 |license| |wheel| |pyversion| |pyimp| |black|
 
 :Version: 0.6.1
```

### Comparing `mode-ng-0.6.1/docs/Makefile` & `mode_ng-0.7.0.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/docs/conf.py` & `mode_ng-0.7.0.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/docs/copyright.rst` & `mode_ng-0.7.0.dev0/docs/copyright.rst`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/docs/images/favicon.ico` & `mode_ng-0.7.0.dev0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/docs/images/logo.png` & `mode_ng-0.7.0.dev0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/docs/images/tutorial_graph.png` & `mode_ng-0.7.0.dev0/docs/images/tutorial_graph.png`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/docs/includes/code-of-conduct.md` & `mode_ng-0.7.0.dev0/docs/includes/code-of-conduct.md`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/docs/includes/faq.rst` & `mode_ng-0.7.0.dev0/docs/includes/faq.rst`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/docs/includes/installation.txt` & `mode_ng-0.7.0.dev0/docs/includes/installation.txt`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/docs/includes/introduction.txt` & `mode_ng-0.7.0.dev0/docs/includes/introduction.txt`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/docs/make.bat` & `mode_ng-0.7.0.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/docs/reference/index.rst` & `mode_ng-0.7.0.dev0/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/docs/templates/readme.txt` & `mode_ng-0.7.0.dev0/docs/templates/readme.txt`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/docs/userguide/services.rst` & `mode_ng-0.7.0.dev0/docs/userguide/services.rst`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/examples/service.py` & `mode_ng-0.7.0.dev0/examples/service.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/examples/tutorial.py` & `mode_ng-0.7.0.dev0/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/examples/worker_log_to_file.py` & `mode_ng-0.7.0.dev0/examples/worker_log_to_file.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/pyproject.toml` & `mode_ng-0.7.0.dev0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,29 @@
   "wheel",
   "pip",
 ] # `pip` is required to install in editable mode
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mode-ng"
-version = "0.6.1"
+version = "0.7.0.dev0"
 description = "AsyncIO Service-based programming."
 readme = "README.rst"
 requires-python = ">=3.10"
 license = { text = "BSD 3-Clause License" }
 authors = [{ name = "Ask Solem", email = "ask@celeryproject.org" }]
 maintainers = [{ name = "Lanqing Huang", email = "lqhuang@outlook.com" }]
 keywords = ["asyncio", "service", "bootsteps", "graph", "coroutine", "actor"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Operating System :: POSIX",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Unix",
   "Environment :: No Input/Output (Daemon)",
   "Framework :: AsyncIO",
@@ -39,15 +40,15 @@
 exclude = ["tests", "docs", "scripts", "examples"]
 namespaces = false
 
 [tool.setuptools.package-data]
 mode = ["py.typed"]
 
 # ========================
-#          MYPY
+#     MYPY
 # ========================
 
 [tool.mypy]
 # doc: https://mypy.readthedocs.io/en/stable/config_file.html
 # --strict but not --no-implicit-optional
 # Import discovery
 ignore_missing_imports = true
@@ -93,15 +94,25 @@
 module = "tests.*"
 disallow_untyped_defs = false
 disallow_incomplete_defs = false
 check_untyped_defs = true
 disallow_untyped_calls = false
 
 # ========================
-#          BLACK
+#     Pyright (pylance)
+# ========================
+
+[tool.pyright]
+# https://github.com/microsoft/pyright/blob/main/docs/configuration.md#main-pyright-config-options
+typeCheckingMode = "basic"
+reportGeneralTypeIssues = false
+# reportPrivateUsage = false
+
+# ========================
+#     black & isort
 # ========================
 
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python. Multiline strings are treated as
 # verbose regular expressions by Black. Use [ ] to denote a significant space
 # character.
 [tool.black]
@@ -126,32 +137,28 @@
   | dist
 )
 '''
 
 [tool.isort]
 profile = "black"
 # line_length = 79
-known_typing = "typing"
+known_typing = ["typing", "typing_extensions", "collections.abc"]
 known_first_party = "mode"
 sections = "FUTURE,TYPING,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 
-# [tool.bandit]
-# # B101: assert_used
-# # B104: hardcoded_bind_all_interfaces
-# skips = ["B101", "B104"]
-
 # ========================
-#     Pyright (pylance)
+#     docformatter
 # ========================
 
-[tool.pyright]
-# https://github.com/microsoft/pyright/blob/main/docs/configuration.md#main-pyright-config-options
-typeCheckingMode = "basic"
-reportGeneralTypeIssues = false
-# reportPrivateUsage = false
+[tool.docformatter]
+recursive = true
+syntax = "google"      # One of sphinx, numpy, or google
+black = true           # Formats docstrings to be compatible with black.
+wrap-summaries = 72    # PEP8: comments and docstrings are still wrapped at 72 characters
+wrap-descriptions = 72
 
 # ========================
 #     Ruff
 # ========================
 
 [tool.ruff]
 line-length = 88
@@ -175,15 +182,20 @@
 unfixable = ["I"]
 
 ignore-init-module-imports = true
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"] # imported but unused
 
+# [tool.bandit]
+# # B101: assert_used
+# # B104: hardcoded_bind_all_interfaces
+# skips = ["B101", "B104"]
+
 # ========================
-#          Pytest
+#     Pytest
 # ========================
 
 [tool.pytest.ini_options]
 python_classes = "test_*"
 testpaths = ["tests"]
 asyncio_mode = "strict"   # for `pytest-asyncio`
```

### Comparing `mode-ng-0.6.1/setup.py` & `mode_ng-0.7.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/__init__.py` & `mode_ng-0.7.0.dev0/src/mode/__init__.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/debug.py` & `mode_ng-0.7.0.dev0/src/mode/debug.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/locals.py` & `mode_ng-0.7.0.dev0/src/mode/locals.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/loop/__init__.py` & `mode_ng-0.7.0.dev0/src/mode/loop/__init__.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/loop/_gevent_loop.py` & `mode_ng-0.7.0.dev0/src/mode/loop/_gevent_loop.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/loop/eventlet.py` & `mode_ng-0.7.0.dev0/src/mode/loop/eventlet.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/loop/gevent.py` & `mode_ng-0.7.0.dev0/src/mode/loop/gevent.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/proxy.py` & `mode_ng-0.7.0.dev0/src/mode/proxy.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/services.py` & `mode_ng-0.7.0.dev0/src/mode/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """Async I/O services that can be started/stopped/shutdown."""
-from typing import (
-    Any,
-    AsyncContextManager,
+
+from collections.abc import (
     AsyncIterator,
     Awaitable,
     Callable,
-    ClassVar,
-    ContextManager,
     Coroutine,
     Iterable,
     Mapping,
     MutableSequence,
-    NamedTuple,
     Sequence,
-    cast,
 )
+from typing import Any, ClassVar, NamedTuple, cast
 
 import asyncio
 import logging
 import sys
 from asyncio.events import AbstractEventLoop
 from asyncio.locks import Event
-from contextlib import AsyncExitStack, ExitStack
+from contextlib import (
+    AbstractAsyncContextManager,
+    AbstractContextManager,
+    AsyncExitStack,
+    ExitStack,
+)
 from datetime import tzinfo
 from functools import wraps
 from time import monotonic, perf_counter
 from types import TracebackType
 
 from mode.types import DiagT, ServiceT
 
@@ -613,25 +614,25 @@
         """Stop and remove dependency of this service."""
         await service.stop()
         self._children.remove(service)
         if service.beacon is not None:
             service.beacon.detach(self.beacon)
         return service
 
-    async def add_async_context(self, context: AsyncContextManager) -> Any:
-        if isinstance(context, AsyncContextManager):
+    async def add_async_context(self, context: AbstractAsyncContextManager) -> Any:
+        if isinstance(context, AbstractAsyncContextManager):
             return await self.async_exit_stack.enter_async_context(context)
-        elif isinstance(context, ContextManager):  # type: ignore
+        elif isinstance(context, AbstractContextManager):  # type: ignore
             raise TypeError("Use `self.add_context(ctx)` for non-async context")
         raise TypeError(f"Not a context/async context: {type(context)!r}")
 
-    def add_context(self, context: ContextManager) -> Any:
-        if isinstance(context, AsyncContextManager):
+    def add_context(self, context: AbstractContextManager) -> Any:
+        if isinstance(context, AbstractAsyncContextManager):
             raise TypeError("Use `await self.add_async_context(ctx)` for async context")
-        elif isinstance(context, ContextManager):
+        elif isinstance(context, AbstractContextManager):
             return self.exit_stack.enter_context(context)
         raise TypeError(f"Not a context/async context: {type(context)!r}")
 
     def add_future(self, coro: Awaitable) -> asyncio.Task[None]:
         """Add relationship to asyncio.Future.
 
         The future will be joined when this service is stopped.
@@ -805,16 +806,15 @@
             fut.cancel()
         assert self._crashed.is_set() or self._stopped.is_set()
 
     async def start(self) -> None:
         await self._default_start()
 
     async def _default_start(self) -> None:
-        loop = self.loop
-        assert loop  # make sure loop is set
+        assert self.loop  # make sure loop is set
         assert not self._started.is_set()
         self._started.set()
         await self._actually_start()
 
     async def _actually_start(self) -> None:
         """Start the service."""
         for _ in [1]:  # to use break
@@ -838,19 +838,38 @@
                 for child in self._children:
                     if child is not None:
                         await child.maybe_start()
                     if self.should_stop:
                         break
                 self.log.debug("Started.")
                 await self.on_started()
+
+                # # Good enough, but worker will be broken due to eternal loop
+                while True:
+                    for child in self._children:
+                        if not child._stopped.is_set() and child._is_taskq_empty():
+                            await child.stop()
+
+                    all_children_stopped = all(
+                        child._stopped.is_set() for child in self._children
+                    )
+
+                    if all_children_stopped:
+                        break
+                    else:
+                        await asyncio.sleep(0.01)
+
             except BaseException:
                 self.exit_stack.__exit__(*sys.exc_info())
                 await self.async_exit_stack.__aexit__(*sys.exc_info())
                 raise
 
+    def _is_taskq_empty(self) -> bool:
+        return not self._futures
+
     async def _execute_task(self, task: Awaitable) -> None:
         try:
             await task
         except asyncio.CancelledError:
             if not self.should_stop:
                 self._log_mundane("Terminating cancelled task: %r", task)
         except RuntimeError as exc:
@@ -917,15 +936,15 @@
                     self._shutdown.wait(),
                     self.shutdown_timeout,
                 )
                 self.log.debug("Shutting down now")
             await self._stop_futures()
             await self._stop_exit_stacks()
             await self.on_shutdown()
-            self.log.debug("-Stopped!")
+            self.log.info("Stopped!")
 
     def _stopped_set(self) -> None:
         self._stopped.set()
 
     async def _stop_children(self) -> None:
         await self._default_stop_children()
 
@@ -990,27 +1009,32 @@
     async def restart(self) -> None:
         """Restart this service."""
         await self.stop()
         self.service_reset()
         await self.on_restart()
         await self.start()
 
-    def service_reset(self) -> None:
-        self.restart_count += 1
+    def service_reset(self, restart: bool = True) -> None:
+        if restart:
+            self.restart_count += 1
         for ev in (
             self._started,
             self._stopped,
             self._shutdown,
             self._crashed,
         ):
             ev.clear()
         self.crash_reason = None
+
+        # Breaking change
+        self._children.clear()
+
         for child in self._children:
             if child is not None:
-                child.service_reset()
+                child.service_reset(restart)
 
     async def wait_until_stopped(self) -> None:
         """Wait until the service is signalled to stop."""
         await self.wait()
 
     def set_shutdown(self) -> None:
         """Set the shutdown signal.
```

### Comparing `mode-ng-0.6.1/src/mode/signals.py` & `mode_ng-0.7.0.dev0/src/mode/signals.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/supervisors.py` & `mode_ng-0.7.0.dev0/src/mode/supervisors.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/threads.py` & `mode_ng-0.7.0.dev0/src/mode/threads.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,16 @@
     async def maybe_start(self) -> bool:
         if not self._thread_started.is_set():
             await self.start()
             return True
         return False
 
     async def start(self) -> None:
-        assert not self._thread_started.is_set()
+        if self._thread_started.is_set():
+            raise RuntimeError(f"ServiceThread {repr(self)} may has been started.")
         self._thread_started.set()
         self._thread_running = asyncio.Future(loop=self.parent_loop)
         self.add_future(self._keepalive2())
         try:
             self._thread = self.Worker(self)
             self._thread.start()
             if not self.should_stop and self.wait_for_thread:
@@ -171,21 +172,20 @@
                 # wait for thread to be fully started
                 await self._thread_running
         finally:
             self._thread_running = None
 
     async def _keepalive2(self) -> None:
         while not self.should_stop:
-            await self.sleep(1.1)
+            await self.sleep(3.0)
             if self.last_wakeup_at:
                 if monotonic() - self.last_wakeup_at > 3.0:
                     self.log.error("Thread keepalive is not responding...")
-            asyncio.run_coroutine_threadsafe(
-                self._wakeup_timer_in_thread(), self.thread_loop
-            )
+            await asyncio.sleep(0.0)  # for unittest to invoke `call_soon`
+            await self._wakeup_timer_in_thread()
 
     async def _wakeup_timer_in_thread(self) -> None:
         self.last_wakeup_at = monotonic()
         await self.sleep(0)
         asyncio.run_coroutine_threadsafe(asyncio.sleep(0), self.parent_loop)
 
     async def crash(self, exc: BaseException) -> None:
```

### Comparing `mode-ng-0.6.1/src/mode/timers.py` & `mode_ng-0.7.0.dev0/src/mode/timers.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/types/services.py` & `mode_ng-0.7.0.dev0/src/mode/types/services.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type classes for :mod:`mode.services`."""
+
 from __future__ import annotations
 
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncContextManager,
     Awaitable,
@@ -34,24 +35,21 @@
 class DiagT(abc.ABC):
     """Diag keeps track of a services diagnostic flags."""
 
     flags: set[str]
     last_transition: MutableMapping[str, float]
 
     @abc.abstractmethod
-    def __init__(self, service: "ServiceT") -> None:
-        ...
+    def __init__(self, service: ServiceT) -> None: ...
 
     @abc.abstractmethod
-    def set_flag(self, flag: str) -> None:
-        ...
+    def set_flag(self, flag: str) -> None: ...
 
     @abc.abstractmethod
-    def unset_flag(self, flag: str) -> None:
-        ...
+    def unset_flag(self, flag: str) -> None: ...
 
 
 class ServiceT(AsyncContextManager):
     """Abstract type for an asynchronous service that can be started/stopped.
 
     See Also:
         :class:`mode.Service`.
@@ -70,121 +68,94 @@
 
     @abc.abstractmethod
     def __init__(
         self,
         *,
         beacon: NodeT | None = None,
         loop: asyncio.AbstractEventLoop | None = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abc.abstractmethod
-    def add_dependency(self, service: ServiceT) -> ServiceT:
-        ...
+    def add_dependency(self, service: ServiceT) -> ServiceT: ...
 
     @abc.abstractmethod
-    async def add_runtime_dependency(self, service: ServiceT) -> ServiceT:
-        ...
+    async def add_runtime_dependency(self, service: ServiceT) -> ServiceT: ...
 
     @abc.abstractmethod
-    async def add_async_context(self, context: AsyncContextManager) -> Any:
-        ...
+    async def add_async_context(self, context: AsyncContextManager) -> Any: ...
 
     @abc.abstractmethod
-    def add_context(self, context: ContextManager) -> Any:
-        ...
+    def add_context(self, context: ContextManager) -> Any: ...
 
     @abc.abstractmethod
-    async def start(self) -> None:
-        ...
+    async def start(self) -> None: ...
 
     @abc.abstractmethod
-    async def maybe_start(self) -> bool:
-        ...
+    async def maybe_start(self) -> bool: ...
 
     @abc.abstractmethod
-    async def crash(self, reason: BaseException) -> None:
-        ...
+    async def crash(self, reason: BaseException) -> None: ...
 
     @abc.abstractmethod
-    def _crash(self, reason: BaseException) -> None:
-        ...
+    def _crash(self, reason: BaseException) -> None: ...
 
     @abc.abstractmethod
-    async def stop(self) -> None:
-        ...
+    async def stop(self) -> None: ...
 
     @abc.abstractmethod
-    def service_reset(self) -> None:
-        ...
+    def service_reset(self, restart: bool = True) -> None: ...
 
     @abc.abstractmethod
-    async def restart(self) -> None:
-        ...
+    async def restart(self) -> None: ...
 
     @abc.abstractmethod
-    async def wait_until_stopped(self) -> None:
-        ...
+    async def wait_until_stopped(self) -> None: ...
 
     @abc.abstractmethod
-    def set_shutdown(self) -> None:
-        ...
+    def set_shutdown(self) -> None: ...
 
     @abc.abstractmethod
-    def _repr_info(self) -> str:
-        ...
+    def _repr_info(self) -> str: ...
 
     @property
     @abc.abstractmethod
-    def started(self) -> bool:
-        ...
+    def started(self) -> bool: ...
 
     @property
     @abc.abstractmethod
-    def crashed(self) -> bool:
-        ...
+    def crashed(self) -> bool: ...
 
     @property
     @abc.abstractmethod
-    def should_stop(self) -> bool:
-        ...
+    def should_stop(self) -> bool: ...
 
     @property
     @abc.abstractmethod
-    def state(self) -> str:
-        ...
+    def state(self) -> str: ...
 
     @property
     @abc.abstractmethod
-    def label(self) -> str:
-        ...
+    def label(self) -> str: ...
 
     @property
     @abc.abstractmethod
-    def shortlabel(self) -> str:
-        ...
+    def shortlabel(self) -> str: ...
 
     @property
-    def beacon(self) -> NodeT:
-        ...
+    def beacon(self) -> NodeT: ...
 
     @beacon.setter
-    def beacon(self, beacon: NodeT) -> None:
-        ...
+    def beacon(self, beacon: NodeT) -> None: ...
 
     @property
     @abc.abstractmethod
-    def loop(self) -> asyncio.AbstractEventLoop:
-        ...
+    def loop(self) -> asyncio.AbstractEventLoop: ...
 
     @loop.setter
-    def loop(self, loop: asyncio.AbstractEventLoop) -> None:
-        ...
+    def loop(self, loop: asyncio.AbstractEventLoop) -> None: ...
 
     @property
     @abc.abstractmethod
-    def crash_reason(self) -> BaseException | None:
-        ...
+    def crash_reason(self) -> BaseException | None: ...
 
     @crash_reason.setter
-    def crash_reason(self, reason: BaseException | None) -> None:
-        ...
+    def crash_reason(self, reason: BaseException | None) -> None: ...
```

### Comparing `mode-ng-0.6.1/src/mode/types/signals.py` & `mode_ng-0.7.0.dev0/src/mode/types/signals.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/types/supervisors.py` & `mode_ng-0.7.0.dev0/src/mode/types/supervisors.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/aiter.py` & `mode_ng-0.7.0.dev0/src/mode/utils/aiter.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/collections.py` & `mode_ng-0.7.0.dev0/src/mode/utils/collections.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/cron.py` & `mode_ng-0.7.0.dev0/src/mode/utils/cron.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/futures.py` & `mode_ng-0.7.0.dev0/src/mode/utils/futures.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/graphs/formatter.py` & `mode_ng-0.7.0.dev0/src/mode/utils/graphs/formatter.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/graphs/graph.py` & `mode_ng-0.7.0.dev0/src/mode/utils/graphs/graph.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/imports.py` & `mode_ng-0.7.0.dev0/src/mode/utils/imports.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/locals.py` & `mode_ng-0.7.0.dev0/src/mode/utils/locals.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/locks.py` & `mode_ng-0.7.0.dev0/src/mode/utils/locks.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/logging.py` & `mode_ng-0.7.0.dev0/src/mode/utils/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """Logging utilities."""
+
 from __future__ import annotations
 
+from collections.abc import Callable, Iterable, Iterator, Mapping
 from typing import (
     IO,
     Any,
     AnyStr,
     BinaryIO,
-    Callable,
     ClassVar,
-    ContextManager,
-    Iterable,
-    Iterator,
-    Mapping,
     NamedTuple,
     Protocol,
     TextIO,
     cast,
 )
 
 import asyncio
@@ -25,15 +22,15 @@
 import re
 import sys
 import threading
 import time
 import traceback
 from abc import abstractmethod
 from asyncio import AbstractEventLoop, all_tasks, current_task
-from contextlib import ExitStack, contextmanager
+from contextlib import AbstractContextManager, ExitStack, contextmanager
 from functools import singledispatch, wraps
 from itertools import count
 from logging import Logger
 from pprint import pprint
 from types import TracebackType
 
 import colorlog
@@ -85,19 +82,22 @@
     "pathname",
     "process",
     "processName",
     "relativeCreated",
     "stack_info",
     "thread",
     "threadName",
+    "taskName",
 }
 
-DEFAULT_FORMAT: str = """
+DEFAULT_FORMAT: str = (
+    """
 [%(asctime)s] [%(process)d:%(thread)d] [%(levelname)s]: %(message)s %(extra)s
 """.strip()
+)
 
 DEFAULT_COLOR_FORMAT = """
 [%(asctime)s] [%(process)d:%(thread)d] [%(levelname)s] %(log_color)s%(message)s %(extra)s
 """.strip()
 
 DEFAULT_COLORS = {
     **colorlog.default_log_colors,
@@ -184,16 +184,15 @@
         ...            severity: int,
         ...            message: str,
         ...            *args: Any, **kwargs: Any) -> None:
         ...        return self.logger.log(severity, message, *args, **kwargs)
     """
 
     @abstractmethod
-    def log(self, severity: int, message: str, *args: Any, **kwargs: Any) -> None:
-        ...
+    def log(self, severity: int, message: str, *args: Any, **kwargs: Any) -> None: ...
 
     def dev(self, message: str, *args: Any, **kwargs: Any) -> None:
         kwargs.setdefault("stacklevel", 3)
         if DEVLOG:
             self.log(logging.INFO, message, *args, **kwargs)
 
     def debug(self, message: str, *args: Any, **kwargs: Any) -> None:
@@ -652,15 +651,15 @@
     severity: int
     message: str
     asctime: str
     args: tuple[Any, ...]
     kwargs: dict[str, Any]
 
 
-class flight_recorder(ContextManager, LogSeverityMixin):
+class flight_recorder(AbstractContextManager, LogSeverityMixin):
     """Flight Recorder context for use with :keyword:`with` statement.
 
     This is a logging utility to log stuff only when something
     times out.
 
     For example if you have a background thread that is sometimes
     hanging::
@@ -950,16 +949,15 @@
     def line_buffering(self) -> bool:
         return False
 
     @property
     def newlines(self) -> bool:
         return False
 
-    def flush(self) -> None:
-        ...
+    def flush(self) -> None: ...
 
     @property
     def mode(self) -> str:
         return "w"
 
     @property
     def name(self) -> str:
@@ -1015,16 +1013,15 @@
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] = None,
         exc_val: BaseException = None,
         exc_tb: TracebackType = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
 
 @contextmanager
 def redirect_stdouts(
     logger: Logger = redirect_logger,
     *,
     severity: Severity | None = None,
```

### Comparing `mode-ng-0.6.1/src/mode/utils/loops.py` & `mode_ng-0.7.0.dev0/src/mode/utils/loops.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/mocks.py` & `mode_ng-0.7.0.dev0/src/mode/utils/mocks.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/objects.py` & `mode_ng-0.7.0.dev0/src/mode/utils/objects.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/queues.py` & `mode_ng-0.7.0.dev0/src/mode/utils/queues.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/text.py` & `mode_ng-0.7.0.dev0/src/mode/utils/text.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/times.py` & `mode_ng-0.7.0.dev0/src/mode/utils/times.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/tracebacks.py` & `mode_ng-0.7.0.dev0/src/mode/utils/tracebacks.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/trees.py` & `mode_ng-0.7.0.dev0/src/mode/utils/trees.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/types/graphs.py` & `mode_ng-0.7.0.dev0/src/mode/utils/types/graphs.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/utils/types/trees.py` & `mode_ng-0.7.0.dev0/src/mode/utils/types/trees.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/src/mode/worker.py` & `mode_ng-0.7.0.dev0/src/mode/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 """Worker - Starts services from the command-line.
 
 Workers add signal handling, logging, and other things
 required to start and manage services in a process environment.
 """
+
 from __future__ import annotations
 
-from typing import (
-    IO,
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    ClassVar,
-    Iterable,
-    Iterator,
-    NoReturn,
-    cast,
-)
+from collections.abc import Callable, Iterable, Iterator
+from typing import IO, TYPE_CHECKING, Any, ClassVar, NoReturn, cast
 
 import asyncio
 import logging as _logging
 import os
 import reprlib
 import signal
 import sys
@@ -99,15 +91,15 @@
 
     # signals can be called multiple times,
     # so when stopped by signal we record the time to make sure
     # we don't start the process multiple times.
     _signal_stop_time: float | None = None
     _signal_stop_future: asyncio.Future | None = None
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         *services: ServiceT,
         debug: bool = False,
         quiet: bool = False,
         log_level: Severity = _logging.INFO,
         log_file: str | os.PathLike | IO | None = None,
         log_handlers: list[Handler] | None = None,
@@ -173,16 +165,15 @@
         if self.override_logging:
             self._setup_logging()
         await self.on_execute()
         if self.debug:
             await self._add_monitor()
         self.install_signal_handlers()
 
-    async def on_execute(self) -> None:
-        ...
+    async def on_execute(self) -> None: ...
 
     def _setup_logging(self) -> None:
         _loglevel: int = 0
         try:
             _loglevel = logging.setup_logging(
                 log_level=self.log_level,
                 log_file=self.log_file,
@@ -208,36 +199,47 @@
 
         if self.redirect_stdouts:
             self._redirect_stdouts()
 
     def _redirect_stdouts(self) -> None:
         self.add_context(logging.redirect_stdouts(severity=self.redirect_stdouts_level))
 
-    def on_setup_root_logger(self, logger: Logger, level: int) -> None:
-        ...
+    def on_setup_root_logger(self, logger: Logger, level: int) -> None: ...
 
     async def maybe_start_blockdetection(self) -> None:
         if self.debug:
             await self.blocking_detector.maybe_start()
 
     def install_signal_handlers(self) -> None:
         if sys.platform == "win32":
             self._install_signal_handlers_windows()
         else:
             self._install_signal_handlers_unix()
 
+    def uninstall_signal_handlers(self) -> None:
+        if sys.platform == "win32":
+            raise NotImplementedError("Windows does not support uninstalling signals")
+        else:
+            self._uninstall_signal_handlers_unix()
+
     def _install_signal_handlers_windows(self) -> None:
         signal.signal(signal.SIGTERM, self._on_win_sigterm)
 
     def _install_signal_handlers_unix(self) -> None:
         self.loop.add_signal_handler(signal.SIGINT, self._on_sigint)
         self.loop.add_signal_handler(signal.SIGTERM, self._on_sigterm)
         self.loop.add_signal_handler(signal.SIGUSR1, self._on_sigusr1)
         self.loop.add_signal_handler(signal.SIGUSR2, self._on_sigusr2)
 
+    def _uninstall_signal_handlers_unix(self) -> None:
+        self.loop.remove_signal_handler(signal.SIGINT)
+        self.loop.remove_signal_handler(signal.SIGTERM)
+        self.loop.remove_signal_handler(signal.SIGUSR1)
+        self.loop.remove_signal_handler(signal.SIGUSR2)
+
     def _on_sigint(self) -> None:
         self.carp("-INT- -INT- -INT- -INT- -INT- -INT-")
         self._schedule_shutdown(signal.SIGINT)
 
     def _on_sigterm(self) -> None:
         self._schedule_shutdown(signal.SIGTERM)
 
@@ -276,18 +278,20 @@
         with exiting(file=self.stderr):
             try:
                 self.loop.run_until_complete(self.join())
             except asyncio.CancelledError:
                 pass
             finally:
                 self._shutdown_loop()
+                self.log.info("Worker shutdown completely.")
         # for mypy NoReturn
         raise SystemExit(EX_OK)
 
     def start_system(self) -> None:
+        self.restart_count = 0  # FIXME: hacky way to reset restart count
         self._starting_fut = asyncio.ensure_future(self.start(), loop=self.loop)
 
     async def join(self) -> None:
         # TODO: Due to `object AsyncMock can't be used in 'await' expression`,
         #       have not be fully covered by unittests yet.
         if self._starting_fut is None:
             raise RuntimeError("Please start system before join it.")
@@ -300,18 +304,28 @@
             raise
         except Exception as exc:
             self.log.exception("Error: %r", exc)
             raise
         finally:
             maybe_cancel(self._starting_fut)
             await self.on_worker_shutdown()
-            await self.stop_and_shutdown()
 
-    async def on_worker_shutdown(self) -> None:
-        ...
+            # check stoped or not, if not, stop it.
+            if not self._shutdown.is_set():
+                await self.stop()
+
+            # Gather futures created by us.
+            self.log.info("Gathering service tasks...")
+            with suppress(asyncio.CancelledError):
+                await self._gather_futures()
+
+            self.uninstall_signal_handlers()
+            self.service_reset(restart=False)
+
+    async def on_worker_shutdown(self) -> None: ...
 
     async def stop_and_shutdown(self) -> None:
         if self._signal_stop_future and not self._signal_stop_future.done():
             await self._signal_stop_future
         elif not self._stopped.is_set():
             await self.stop()
 
@@ -359,14 +373,29 @@
             await asyncio.sleep(0.1)
         for task in all_tasks(loop=self.loop):
             task.cancel()
 
     async def on_started(self) -> None:
         if self.daemon:
             await self.wait_until_stopped()
+        else:
+            while True:
+                for child in self.services:
+                    if not child._stopped.is_set() and child._is_taskq_empty():
+                        await child.stop()
+                    else:
+                        break
+
+                all_stopped = all(child._stopped.is_set() for child in self._children)
+                if all_stopped:
+                    break
+                else:
+                    await asyncio.sleep(0.01)
+
+            self._schedule_shutdown(signal.SIGINT)
 
     async def _add_monitor(self) -> Any:
         try:
             import aiomonitor
         except ImportError:
             self.log.warning("Cannot start console: aiomonitor is not installed")
         else:
```

### Comparing `mode-ng-0.6.1/src/mode_ng.egg-info/PKG-INFO` & `mode_ng-0.7.0.dev0/src/mode_ng.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 Metadata-Version: 2.1
 Name: mode-ng
-Version: 0.6.1
+Version: 0.7.0.dev0
 Summary: AsyncIO Service-based programming.
 Author-email: Ask Solem <ask@celeryproject.org>
 Maintainer-email: Lanqing Huang <lqhuang@outlook.com>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/lqhuang/mode-ng
 Keywords: asyncio,service,bootsteps,graph,coroutine,actor
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
-Provides-Extra: gevent
-Provides-Extra: eventlet
-Provides-Extra: uvloop
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: colorlog>=2.9.0
+Requires-Dist: croniter>=0.3.16
+Requires-Dist: mypy_extensions
+Provides-Extra: uvloop
+Requires-Dist: uvloop>=0.8.1; extra == "uvloop"
+Provides-Extra: gevent
+Requires-Dist: aiogevent~=0.2; extra == "gevent"
+Provides-Extra: eventlet
+Requires-Dist: aioeventlet~=0.5.1; extra == "eventlet"
+Requires-Dist: dnspython; extra == "eventlet"
 
 =====================
 Mode AsyncIO Services
 =====================
 
 |license| |wheel| |pyversion| |pyimp| |black|
```

### Comparing `mode-ng-0.6.1/src/mode_ng.egg-info/SOURCES.txt` & `mode_ng-0.7.0.dev0/src/mode_ng.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -62,15 +62,17 @@
 docs/reference/mode.utils.types.graphs.rst
 docs/reference/mode.utils.types.trees.rst
 docs/reference/mode.worker.rst
 docs/templates/readme.txt
 docs/userguide/index.rst
 docs/userguide/services.rst
 examples/integration.py
+examples/notebook-demo.ipynb
 examples/service.py
+examples/thread_service.py
 examples/tutorial.py
 examples/worker_log_to_file.py
 requirements/ci.txt
 requirements/default.txt
 requirements/dev.txt
 requirements/docs.txt
 requirements/flakes.txt
@@ -128,15 +130,14 @@
 src/mode_ng.egg-info/PKG-INFO
 src/mode_ng.egg-info/SOURCES.txt
 src/mode_ng.egg-info/dependency_links.txt
 src/mode_ng.egg-info/requires.txt
 src/mode_ng.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
-tests/test_packaging.py
 tests/functional/__init__.py
 tests/functional/test_mode.py
 tests/functional/test_proxy.py
 tests/functional/test_service.py
 tests/functional/test_signals.py
 tests/functional/test_supervisors.py
 tests/functional/test_timers.py
```

### Comparing `mode-ng-0.6.1/tests/functional/test_proxy.py` & `mode_ng-0.7.0.dev0/tests/functional/test_proxy.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/functional/test_service.py` & `mode_ng-0.7.0.dev0/tests/functional/test_service.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/functional/test_signals.py` & `mode_ng-0.7.0.dev0/tests/functional/test_signals.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/functional/test_supervisors.py` & `mode_ng-0.7.0.dev0/tests/functional/test_supervisors.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/functional/test_timers.py` & `mode_ng-0.7.0.dev0/tests/functional/test_timers.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/test_debug.py` & `mode_ng-0.7.0.dev0/tests/unit/test_debug.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/test_locals.py` & `mode_ng-0.7.0.dev0/tests/unit/test_locals.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/test_services.py` & `mode_ng-0.7.0.dev0/tests/unit/test_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,16 +522,15 @@
 
     def test_get_set_loop(self, *, service):
         m = Mock()
         service.loop = m
         assert service.loop is m
 
     def test__get_tasks__no_tasks(self, *, service):
-        class X(type(service)):
-            ...
+        class X(type(service)): ...
 
         X._tasks = []
         assert list(X()._get_tasks()) == []
 
     @pytest.mark.asyncio
     async def test__execute_task__loop_is_closed(self, *, service):
         async def raises():
```

### Comparing `mode-ng-0.6.1/tests/unit/test_supervisors.py` & `mode_ng-0.7.0.dev0/tests/unit/test_supervisors.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/test_threads.py` & `mode_ng-0.7.0.dev0/tests/unit/test_threads.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,25 @@
     def Worker(self):
         return Mock(spec=WorkerThread, name="Worker")
 
     @pytest.fixture
     def thread(self, *, Worker, loop, thread_loop):
         return ServiceThread(Worker=Worker, loop=loop, thread_loop=thread_loop)
 
+    async def _wait_for_event(self, thread):
+        count = 0
+        while thread._thread_running is None:
+            await asyncio.sleep(0.5)
+            count += 1
+            if count >= 10:  # fast fail to avoid block tests
+                raise RuntimeError("Test failed after 10 tries.")
+
+        if not thread._thread_running.done():
+            thread._thread_running.set_result(None)
+
     @pytest.mark.asyncio
     async def test_on_thread_stop(self, *, thread):
         await thread.on_thread_stop()
 
     def test_constructor_worker_argument(self):
         Worker = Mock(spec=WorkerThread)
         assert ServiceThread(Worker=Worker).Worker is Worker
@@ -82,20 +93,23 @@
 
         thread._thread_started.clear()
         await thread.maybe_start()
         thread.start.assert_awaited_once()
 
     @pytest.mark.asyncio
     async def test_start(self, *, event_loop, thread):
-        thread.add_future = AsyncMock(name="thread.add_future")
-        thread._thread_running = None
+        thread.add_future = Mock(name="thread.add_future")
+        thread._keepalive2 = AsyncMock(name="thread._keepalive2")
         assert thread.parent_loop == event_loop
+
+        thread._thread_running = None
         asyncio.ensure_future(self._wait_for_event(thread))
         await thread.start()
 
+        thread._keepalive2.assert_called_once()
         thread.Worker.assert_called_once_with(thread)
         thread.Worker.return_value.start.assert_called_once_with()
 
         assert thread._thread_started.is_set()
 
     @pytest.mark.asyncio
     async def test_start__no_wait(self, *, event_loop, thread):
@@ -107,29 +121,18 @@
         await thread.start()
 
         thread.Worker.assert_called_once_with(thread)
         thread.Worker.return_value.start.assert_called_once_with()
 
         assert thread._thread_started.is_set()
 
-    async def _wait_for_event(self, thread):
-        count = 0
-        while thread._thread_running is None:
-            await asyncio.sleep(0.1)
-            count += 1
-            if count >= 10:  # fast fail to avoid block tests
-                raise RuntimeError("Test failed")
-
-        if not thread._thread_running.done():
-            thread._thread_running.set_result(None)
-
     @pytest.mark.asyncio
     async def test_start__already_started_raises(self, *, thread):
         thread._thread_started.set()
-        with pytest.raises(AssertionError):
+        with pytest.raises(RuntimeError):
             await thread.start()
 
     def test_start_thread(self, *, thread):
         thread._serve = Mock(name="thread._serve")
         with patch("asyncio.set_event_loop") as set_event_loop:
             thread._start_thread()
             set_event_loop.assert_called_once_with(thread.loop)
@@ -152,14 +155,31 @@
         thread._started.clear()
         await thread.stop()
         thread._started.set()
         thread._shutdown.set()
         await thread.stop()
 
     @pytest.mark.asyncio
+    async def test__wakeup_timer_in_thread(self, *, thread, event_loop):
+        thread.add_future = Mock(name="thread.add_future")
+        thread._wakeup_timer_in_thread = AsyncMock()
+        thread._stopped.is_set = Mock(return_value=False)
+        thread._crashed.is_set = Mock(return_value=False)
+        thread.sleep = AsyncMock()
+
+        def cb():
+            thread._stopped.is_set.return_value = True
+            assert thread.should_stop
+
+        event_loop.call_soon(cb)
+        await thread._keepalive2()
+
+        thread._wakeup_timer_in_thread.assert_awaited()
+
+    @pytest.mark.asyncio
     async def test_stop_children(self, *, thread):
         await thread._stop_children()
 
     @pytest.mark.asyncio
     async def test_stop_futures(self, *, thread):
         await thread._stop_futures()
 
@@ -229,14 +249,15 @@
         with pytest.raises(KeyError):
             await thread._serve()
 
         thread.crash.assert_awaited_once_with(exc)
         thread._shutdown_thread.assert_awaited_once_with()
 
     def mock_for_serve(self, thread):
+        # thread._keepalive2 = AsyncMock(name="_keepalive2")
         thread._default_start = AsyncMock(name="start")
         thread.wait_until_stopped = AsyncMock(name="wait_until_stopped")
         thread.crash = AsyncMock(name="crash")
         thread.on_crash = Mock(name="on_crash")
         thread.beacon = Mock(name="beacon")
         thread.beacon.root.data.crash = AsyncMock(name="root.crash")
         thread._shutdown_thread = AsyncMock(name="shutdown_thread")
```

### Comparing `mode-ng-0.6.1/tests/unit/test_worker.py` & `mode_ng-0.7.0.dev0/tests/unit/test_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import signal
 import sys
 from contextlib import contextmanager
 from signal import Signals
-from unittest.mock import AsyncMock, patch, Mock
+from unittest.mock import AsyncMock, Mock, patch
 
 import pytest
 
 from mode import Service
 from mode.debug import BlockingDetector
 from mode.utils.mocks import call, mask_module, patch_module
 from mode.worker import Worker, exiting
```

### Comparing `mode-ng-0.6.1/tests/unit/utils/test_aiter.py` & `mode_ng-0.7.0.dev0/tests/unit/utils/test_aiter.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/utils/test_collections.py` & `mode_ng-0.7.0.dev0/tests/unit/utils/test_collections.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/utils/test_cron.py` & `mode_ng-0.7.0.dev0/tests/unit/utils/test_cron.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/utils/test_futures.py` & `mode_ng-0.7.0.dev0/tests/unit/utils/test_futures.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/utils/test_imports.py` & `mode_ng-0.7.0.dev0/tests/unit/utils/test_imports.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/utils/test_locals.py` & `mode_ng-0.7.0.dev0/tests/unit/utils/test_locals.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/utils/test_logging.py` & `mode_ng-0.7.0.dev0/tests/unit/utils/test_logging.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/utils/test_objects.py` & `mode_ng-0.7.0.dev0/tests/unit/utils/test_objects.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/utils/test_queues.py` & `mode_ng-0.7.0.dev0/tests/unit/utils/test_queues.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/utils/test_text.py` & `mode_ng-0.7.0.dev0/tests/unit/utils/test_text.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/utils/test_times.py` & `mode_ng-0.7.0.dev0/tests/unit/utils/test_times.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/utils/test_tracebacks.py` & `mode_ng-0.7.0.dev0/tests/unit/utils/test_tracebacks.py`

 * *Files identical despite different names*

### Comparing `mode-ng-0.6.1/tests/unit/utils/test_trees.py` & `mode_ng-0.7.0.dev0/tests/unit/utils/test_trees.py`

 * *Files identical despite different names*

