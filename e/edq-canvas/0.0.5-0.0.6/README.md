# Comparing `tmp/edq-canvas-0.0.5.tar.gz` & `tmp/edq_canvas-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edq-canvas-0.0.5.tar", last modified: Thu Apr 11 23:02:10 2024, max compression
+gzip compressed data, was "edq_canvas-0.0.6.tar", last modified: Tue May  7 11:03:41 2024, max compression
```

## Comparing `edq-canvas-0.0.5.tar` & `edq_canvas-0.0.6.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 23:02:10.885417 edq-canvas-0.0.5/
--rw-rw----   0 eriq      (1000) eriq      (1000)     1071 2024-02-03 22:26:13.000000 edq-canvas-0.0.5/LICENSE
--rw-r--r--   0 eriq      (1000) eriq      (1000)    11022 2024-04-11 23:02:10.885417 edq-canvas-0.0.5/PKG-INFO
--rw-rw----   0 eriq      (1000) eriq      (1000)     9109 2024-04-11 22:00:49.000000 edq-canvas-0.0.5/README.md
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 23:02:10.882084 edq-canvas-0.0.5/canvas/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-03 22:28:32.000000 edq-canvas-0.0.5/canvas/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      201 2024-03-07 16:13:16.000000 edq-canvas-0.0.5/canvas/__main__.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 23:02:10.882084 edq-canvas-0.0.5/canvas/api/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 23:59:27.000000 edq-canvas-0.0.5/canvas/api/__init__.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 23:02:10.882084 edq-canvas-0.0.5/canvas/api/assignment/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:28:53.000000 edq-canvas-0.0.5/canvas/api/assignment/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      633 2024-03-07 19:12:01.000000 edq-canvas-0.0.5/canvas/api/assignment/common.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1312 2024-03-07 19:35:20.000000 edq-canvas-0.0.5/canvas/api/assignment/fetch.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     2418 2024-03-07 21:36:19.000000 edq-canvas-0.0.5/canvas/api/assignment/fetchscores.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      819 2024-03-07 19:12:56.000000 edq-canvas-0.0.5/canvas/api/assignment/list.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     2845 2024-03-07 19:33:43.000000 edq-canvas-0.0.5/canvas/api/assignment/resolve.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     2962 2024-04-11 22:59:36.000000 edq-canvas-0.0.5/canvas/api/assignment/uploadscores.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     3435 2024-03-09 13:59:12.000000 edq-canvas-0.0.5/canvas/api/common.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 23:02:10.882084 edq-canvas-0.0.5/canvas/api/gradebook/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:26:51.000000 edq-canvas-0.0.5/canvas/api/gradebook/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     3166 2024-02-17 15:14:24.000000 edq-canvas-0.0.5/canvas/api/gradebook/fetch.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     3194 2024-03-10 23:57:17.000000 edq-canvas-0.0.5/canvas/api/gradebook/upload.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 23:02:10.885417 edq-canvas-0.0.5/canvas/api/user/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 05:13:50.000000 edq-canvas-0.0.5/canvas/api/user/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      815 2024-03-07 21:55:23.000000 edq-canvas-0.0.5/canvas/api/user/common.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1319 2024-02-17 15:02:45.000000 edq-canvas-0.0.5/canvas/api/user/fetch.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      877 2024-02-17 14:57:23.000000 edq-canvas-0.0.5/canvas/api/user/list.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     3557 2024-04-11 22:57:33.000000 edq-canvas-0.0.5/canvas/api/user/resolve.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 23:02:10.885417 edq-canvas-0.0.5/canvas/cli/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 23:48:49.000000 edq-canvas-0.0.5/canvas/cli/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      409 2024-03-07 15:45:52.000000 edq-canvas-0.0.5/canvas/cli/__main__.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 23:02:10.885417 edq-canvas-0.0.5/canvas/cli/assignment/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:28:53.000000 edq-canvas-0.0.5/canvas/cli/assignment/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      318 2024-03-07 16:09:16.000000 edq-canvas-0.0.5/canvas/cli/assignment/__main__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      324 2024-02-15 17:43:24.000000 edq-canvas-0.0.5/canvas/cli/assignment/common.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1483 2024-03-10 22:45:10.000000 edq-canvas-0.0.5/canvas/cli/assignment/fetch-scores.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1961 2024-03-07 19:15:25.000000 edq-canvas-0.0.5/canvas/cli/assignment/fetch.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1649 2024-02-15 17:43:24.000000 edq-canvas-0.0.5/canvas/cli/assignment/list.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1361 2024-03-11 15:58:40.000000 edq-canvas-0.0.5/canvas/cli/assignment/upload-score.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     2659 2024-03-11 15:49:58.000000 edq-canvas-0.0.5/canvas/cli/assignment/upload-scores.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1159 2024-03-18 22:04:11.000000 edq-canvas-0.0.5/canvas/cli/common.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 23:02:10.885417 edq-canvas-0.0.5/canvas/cli/gradebook/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:26:51.000000 edq-canvas-0.0.5/canvas/cli/gradebook/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      316 2024-03-07 16:10:20.000000 edq-canvas-0.0.5/canvas/cli/gradebook/__main__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     2912 2024-03-08 16:20:14.000000 edq-canvas-0.0.5/canvas/cli/gradebook/fetch.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     3706 2024-03-11 00:08:28.000000 edq-canvas-0.0.5/canvas/cli/gradebook/upload.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 23:02:10.885417 edq-canvas-0.0.5/canvas/cli/user/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 04:32:06.000000 edq-canvas-0.0.5/canvas/cli/user/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      306 2024-03-07 16:10:42.000000 edq-canvas-0.0.5/canvas/cli/user/__main__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      267 2024-02-17 05:36:04.000000 edq-canvas-0.0.5/canvas/cli/user/common.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1891 2024-03-07 19:15:25.000000 edq-canvas-0.0.5/canvas/cli/user/fetch.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1649 2024-03-10 21:53:47.000000 edq-canvas-0.0.5/canvas/cli/user/list.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     4706 2024-04-11 21:58:26.000000 edq-canvas-0.0.5/canvas/config.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      803 2024-02-13 16:16:03.000000 edq-canvas-0.0.5/canvas/log.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 23:02:10.885417 edq-canvas-0.0.5/canvas/util/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 23:49:12.000000 edq-canvas-0.0.5/canvas/util/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     2872 2024-03-07 16:35:41.000000 edq-canvas-0.0.5/canvas/util/cli.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      341 2024-02-04 23:50:26.000000 edq-canvas-0.0.5/canvas/util/code.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 23:02:10.885417 edq-canvas-0.0.5/edq_canvas.egg-info/
--rw-r--r--   0 eriq      (1000) eriq      (1000)    11022 2024-04-11 23:02:10.000000 edq-canvas-0.0.5/edq_canvas.egg-info/PKG-INFO
--rw-rw----   0 eriq      (1000) eriq      (1000)     1437 2024-04-11 23:02:10.000000 edq-canvas-0.0.5/edq_canvas.egg-info/SOURCES.txt
--rw-rw----   0 eriq      (1000) eriq      (1000)        1 2024-04-11 23:02:10.000000 edq-canvas-0.0.5/edq_canvas.egg-info/dependency_links.txt
--rw-rw----   0 eriq      (1000) eriq      (1000)       52 2024-04-11 23:02:10.000000 edq-canvas-0.0.5/edq_canvas.egg-info/requires.txt
--rw-rw----   0 eriq      (1000) eriq      (1000)        7 2024-04-11 23:02:10.000000 edq-canvas-0.0.5/edq_canvas.egg-info/top_level.txt
--rw-rw----   0 eriq      (1000) eriq      (1000)      918 2024-04-11 23:00:42.000000 edq-canvas-0.0.5/pyproject.toml
--rw-rw----   0 eriq      (1000) eriq      (1000)       38 2024-04-11 23:02:10.885417 edq-canvas-0.0.5/setup.cfg
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-05-07 11:03:41.807712 edq_canvas-0.0.6/
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1071 2024-02-03 22:26:13.000000 edq_canvas-0.0.6/LICENSE
+-rw-r--r--   0 eriq      (1000) eriq      (1000)    11660 2024-05-07 11:03:41.807712 edq_canvas-0.0.6/PKG-INFO
+-rw-rw----   0 eriq      (1000) eriq      (1000)     9747 2024-05-07 10:59:47.000000 edq_canvas-0.0.6/README.md
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-05-07 11:03:41.801042 edq_canvas-0.0.6/canvas/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-03 22:28:32.000000 edq_canvas-0.0.6/canvas/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      201 2024-03-07 16:13:16.000000 edq_canvas-0.0.6/canvas/__main__.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-05-07 11:03:41.801042 edq_canvas-0.0.6/canvas/api/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 23:59:27.000000 edq_canvas-0.0.6/canvas/api/__init__.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-05-07 11:03:41.801042 edq_canvas-0.0.6/canvas/api/assignment/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:28:53.000000 edq_canvas-0.0.6/canvas/api/assignment/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      643 2024-05-07 10:59:47.000000 edq_canvas-0.0.6/canvas/api/assignment/common.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1312 2024-03-07 19:35:20.000000 edq_canvas-0.0.6/canvas/api/assignment/fetch.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     2443 2024-05-07 10:59:47.000000 edq_canvas-0.0.6/canvas/api/assignment/fetchscores.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     4262 2024-05-07 10:59:47.000000 edq_canvas-0.0.6/canvas/api/assignment/fetchsubmissionfiles.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      819 2024-03-07 19:12:56.000000 edq_canvas-0.0.6/canvas/api/assignment/list.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     2855 2024-05-07 10:59:47.000000 edq_canvas-0.0.6/canvas/api/assignment/resolve.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     2962 2024-04-11 22:59:36.000000 edq_canvas-0.0.6/canvas/api/assignment/uploadscores.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     3435 2024-03-09 13:59:12.000000 edq_canvas-0.0.6/canvas/api/common.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-05-07 11:03:41.801042 edq_canvas-0.0.6/canvas/api/gradebook/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:26:51.000000 edq_canvas-0.0.6/canvas/api/gradebook/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     3166 2024-02-17 15:14:24.000000 edq_canvas-0.0.6/canvas/api/gradebook/fetch.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     3194 2024-03-10 23:57:17.000000 edq_canvas-0.0.6/canvas/api/gradebook/upload.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-05-07 11:03:41.801042 edq_canvas-0.0.6/canvas/api/user/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 05:13:50.000000 edq_canvas-0.0.6/canvas/api/user/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      815 2024-03-07 21:55:23.000000 edq_canvas-0.0.6/canvas/api/user/common.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1319 2024-02-17 15:02:45.000000 edq_canvas-0.0.6/canvas/api/user/fetch.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      877 2024-02-17 14:57:23.000000 edq_canvas-0.0.6/canvas/api/user/list.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     3567 2024-05-07 10:59:47.000000 edq_canvas-0.0.6/canvas/api/user/resolve.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-05-07 11:03:41.801042 edq_canvas-0.0.6/canvas/cli/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 23:48:49.000000 edq_canvas-0.0.6/canvas/cli/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      409 2024-03-07 15:45:52.000000 edq_canvas-0.0.6/canvas/cli/__main__.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-05-07 11:03:41.804377 edq_canvas-0.0.6/canvas/cli/assignment/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:28:53.000000 edq_canvas-0.0.6/canvas/cli/assignment/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      318 2024-03-07 16:09:16.000000 edq_canvas-0.0.6/canvas/cli/assignment/__main__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      324 2024-02-15 17:43:24.000000 edq_canvas-0.0.6/canvas/cli/assignment/common.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1483 2024-03-10 22:45:10.000000 edq_canvas-0.0.6/canvas/cli/assignment/fetch-scores.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1090 2024-05-07 10:59:47.000000 edq_canvas-0.0.6/canvas/cli/assignment/fetch-submission-files.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1961 2024-03-07 19:15:25.000000 edq_canvas-0.0.6/canvas/cli/assignment/fetch.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1649 2024-02-15 17:43:24.000000 edq_canvas-0.0.6/canvas/cli/assignment/list.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1361 2024-03-11 15:58:40.000000 edq_canvas-0.0.6/canvas/cli/assignment/upload-score.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     2659 2024-03-11 15:49:58.000000 edq_canvas-0.0.6/canvas/cli/assignment/upload-scores.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1159 2024-03-18 22:04:11.000000 edq_canvas-0.0.6/canvas/cli/common.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-05-07 11:03:41.804377 edq_canvas-0.0.6/canvas/cli/gradebook/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:26:51.000000 edq_canvas-0.0.6/canvas/cli/gradebook/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      316 2024-03-07 16:10:20.000000 edq_canvas-0.0.6/canvas/cli/gradebook/__main__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     2912 2024-03-08 16:20:14.000000 edq_canvas-0.0.6/canvas/cli/gradebook/fetch.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     3706 2024-03-11 00:08:28.000000 edq_canvas-0.0.6/canvas/cli/gradebook/upload.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-05-07 11:03:41.804377 edq_canvas-0.0.6/canvas/cli/user/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 04:32:06.000000 edq_canvas-0.0.6/canvas/cli/user/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      306 2024-03-07 16:10:42.000000 edq_canvas-0.0.6/canvas/cli/user/__main__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      267 2024-02-17 05:36:04.000000 edq_canvas-0.0.6/canvas/cli/user/common.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1891 2024-03-07 19:15:25.000000 edq_canvas-0.0.6/canvas/cli/user/fetch.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1649 2024-03-10 21:53:47.000000 edq_canvas-0.0.6/canvas/cli/user/list.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     4706 2024-04-11 21:58:26.000000 edq_canvas-0.0.6/canvas/config.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      803 2024-02-13 16:16:03.000000 edq_canvas-0.0.6/canvas/log.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-05-07 11:03:41.804377 edq_canvas-0.0.6/canvas/util/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 23:49:12.000000 edq_canvas-0.0.6/canvas/util/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     2872 2024-03-07 16:35:41.000000 edq_canvas-0.0.6/canvas/util/cli.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      341 2024-02-04 23:50:26.000000 edq_canvas-0.0.6/canvas/util/code.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     2178 2024-05-07 10:59:47.000000 edq_canvas-0.0.6/canvas/util/file.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-05-07 11:03:41.804377 edq_canvas-0.0.6/edq_canvas.egg-info/
+-rw-r--r--   0 eriq      (1000) eriq      (1000)    11660 2024-05-07 11:03:41.000000 edq_canvas-0.0.6/edq_canvas.egg-info/PKG-INFO
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1551 2024-05-07 11:03:41.000000 edq_canvas-0.0.6/edq_canvas.egg-info/SOURCES.txt
+-rw-rw----   0 eriq      (1000) eriq      (1000)        1 2024-05-07 11:03:41.000000 edq_canvas-0.0.6/edq_canvas.egg-info/dependency_links.txt
+-rw-rw----   0 eriq      (1000) eriq      (1000)       52 2024-05-07 11:03:41.000000 edq_canvas-0.0.6/edq_canvas.egg-info/requires.txt
+-rw-rw----   0 eriq      (1000) eriq      (1000)        7 2024-05-07 11:03:41.000000 edq_canvas-0.0.6/edq_canvas.egg-info/top_level.txt
+-rw-rw----   0 eriq      (1000) eriq      (1000)      918 2024-05-07 11:01:26.000000 edq_canvas-0.0.6/pyproject.toml
+-rw-rw----   0 eriq      (1000) eriq      (1000)       38 2024-05-07 11:03:41.807712 edq_canvas-0.0.6/setup.cfg
```

### Comparing `edq-canvas-0.0.5/LICENSE` & `edq_canvas-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/PKG-INFO` & `edq_canvas-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edq-canvas
-Version: 0.0.5
+Version: 0.0.6
 Summary: A suite of tools and Python interface for Instructure's Canvas LMS.
 Author-email: Eriq Augustine <eaugusti@ucsc.edu>
 License: MIT License
         
         Copyright (c) 2023 Eriq Augustine
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -52,14 +52,15 @@
     - [Assignment Queries](#assignment-queries)
  - [CLI Tools](#cli-tools)
     - [List Course Users](#list-course-users)
     - [Fetch a Single User](#fetch-a-single-user)
     - [List Assignments](#list-assignments)
     - [Fetch a Single Assignment](#fetch-a-single-assignment)
     - [Fetch Assignment Scores](#fetch-assignment-scores)
+    - [Fetch Assignment Submission Files](#fetch-assignment-submission-files)
     - [Upload Assignment Scores](#upload-assignment-scores)
     - [Upload Single Assignment Score](#upload-single-assignment-score)
     - [Fetch Gradebook](#fetch-gradebook)
     - [Upload Gradebook](#upload-gradebook)
 
 ## Installation
 
@@ -187,29 +188,47 @@
 ### Fetch a Single Assignment
 
 Fetch information about a single assignment using the `canvas.cli.assignment.fetch` tool.
 For example:
 ```
 python3 -m canvas.cli.assignment.fetch 123456
 
+# Or
 python3 -m canvas.cli.assignment.fetch 'My Assignment'
 ```
 
 ### Fetch Assignment Scores
 
 To fetch the scores for a specific assignment, use the `canvas.cli.assignment.fetch-scores` tool.
 For example:
 ```
 python3 -m canvas.cli.assignment.fetch-scores 123456
 
+# Or
 python3 -m canvas.cli.assignment.fetch-scores 'My Assignment'
 ```
 
 The student's email and score will be written to stdout as a tab-separated row.
 
+### Fetch Assignment Submission Files
+
+To fetch the files students have submitted for an assignment, use the `canvas.cli.assignment.fetch-submission-files` tool.
+For example:
+```
+python3 -m canvas.cli.assignment.fetch-submission-files 123456
+
+# Or
+python3 -m canvas.cli.assignment.fetch-submission-files 'My Assignment'
+```
+
+Only assignment with a submission type of "Online - Text Entry" or "Online - File Uploads" will be downloaded.
+
+By default, files will be written to the `out` directory.
+This can be controlled with the `--out-dir` argument.
+
 ### Upload Assignment Scores
 
 Uploading scores for an assignment can be done with the `canvas.cli.assignment.upload-scores` tool:
 ```
 python3 -m canvas.cli.assignment.upload-scores <assignment query> <path>
 ```
```

### Comparing `edq-canvas-0.0.5/README.md` & `edq_canvas-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     - [Assignment Queries](#assignment-queries)
  - [CLI Tools](#cli-tools)
     - [List Course Users](#list-course-users)
     - [Fetch a Single User](#fetch-a-single-user)
     - [List Assignments](#list-assignments)
     - [Fetch a Single Assignment](#fetch-a-single-assignment)
     - [Fetch Assignment Scores](#fetch-assignment-scores)
+    - [Fetch Assignment Submission Files](#fetch-assignment-submission-files)
     - [Upload Assignment Scores](#upload-assignment-scores)
     - [Upload Single Assignment Score](#upload-single-assignment-score)
     - [Fetch Gradebook](#fetch-gradebook)
     - [Upload Gradebook](#upload-gradebook)
 
 ## Installation
 
@@ -147,29 +148,47 @@
 ### Fetch a Single Assignment
 
 Fetch information about a single assignment using the `canvas.cli.assignment.fetch` tool.
 For example:
 ```
 python3 -m canvas.cli.assignment.fetch 123456
 
+# Or
 python3 -m canvas.cli.assignment.fetch 'My Assignment'
 ```
 
 ### Fetch Assignment Scores
 
 To fetch the scores for a specific assignment, use the `canvas.cli.assignment.fetch-scores` tool.
 For example:
 ```
 python3 -m canvas.cli.assignment.fetch-scores 123456
 
+# Or
 python3 -m canvas.cli.assignment.fetch-scores 'My Assignment'
 ```
 
 The student's email and score will be written to stdout as a tab-separated row.
 
+### Fetch Assignment Submission Files
+
+To fetch the files students have submitted for an assignment, use the `canvas.cli.assignment.fetch-submission-files` tool.
+For example:
+```
+python3 -m canvas.cli.assignment.fetch-submission-files 123456
+
+# Or
+python3 -m canvas.cli.assignment.fetch-submission-files 'My Assignment'
+```
+
+Only assignment with a submission type of "Online - Text Entry" or "Online - File Uploads" will be downloaded.
+
+By default, files will be written to the `out` directory.
+This can be controlled with the `--out-dir` argument.
+
 ### Upload Assignment Scores
 
 Uploading scores for an assignment can be done with the `canvas.cli.assignment.upload-scores` tool:
 ```
 python3 -m canvas.cli.assignment.upload-scores <assignment query> <path>
 ```
```

### Comparing `edq-canvas-0.0.5/canvas/api/assignment/common.py` & `edq_canvas-0.0.6/canvas/api/assignment/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,12 +16,12 @@
     output = []
 
     while (url is not None):
         _, url, new_assignments = canvas.api.common.make_get_request(url, headers)
 
         for new_assignment in new_assignments:
             if (keys is not None):
-                new_assignment = {key: new_assignment[key] for key in keys}
+                new_assignment = {key: new_assignment.get(key, None) for key in keys}
 
             output.append(new_assignment)
 
     return output
```

### Comparing `edq-canvas-0.0.5/canvas/api/assignment/fetch.py` & `edq_canvas-0.0.6/canvas/api/assignment/fetch.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/api/assignment/fetchscores.py` & `edq_canvas-0.0.6/canvas/api/assignment/fetchscores.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         assignment_keys = canvas.api.assignment.common.DEFAULT_KEYS, user_keys = canvas.api.user.common.DEFAULT_KEYS,
         **kwargs):
     server = canvas.api.common.validate_param(server, 'server')
     token = canvas.api.common.validate_param(token, 'token')
     course = canvas.api.common.validate_param(course, 'course', param_type = int)
     assignment = canvas.api.common.validate_param(assignment, 'assignment')
 
-    logging.info("Fetching scores for assignement ('%s' (course '%s')) from '%s'." % (assignment, str(course), server))
+    logging.info("Fetching information for assignement ('%s' (course '%s')) from '%s'." % (assignment, str(course), server))
 
     resolved_assignments = canvas.api.assignment.fetch.request(server = server, token = token, course = course,
             assignments = [assignment], keys = assignment_keys)
 
     if (len(resolved_assignments) == 0):
         raise ValueError("Unable to resolve assignment query '%s'." % (assignment))
 
@@ -51,16 +51,16 @@
             user_id = item.get('user_id', None)
             if (user_id is None):
                 continue
 
             if (user_id not in all_users):
                 continue
 
-            item = {key: item[key] for key in keys}
-            user = {key: all_users[user_id][key] for key in user_keys}
+            item = {key: item.get(key, None) for key in keys}
+            user = {key: all_users[user_id].get(key, None) for key in user_keys}
 
             item['user'] = user
             item['assignment'] = assignment_info
 
             submissions.append(item)
 
     return submissions
```

### Comparing `edq-canvas-0.0.5/canvas/api/assignment/list.py` & `edq_canvas-0.0.6/canvas/api/assignment/list.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/api/assignment/resolve.py` & `edq_canvas-0.0.6/canvas/api/assignment/resolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
             course = course, keys = None)
 
     assignments = resolve_assignments(assignment_queries, course_assignments)
 
     if (keys is None):
         return assignments
 
-    return [{key: assignment[key] for key in keys} for assignment in assignments]
+    return [{key: assignment.get(key, None) for key in keys} for assignment in assignments]
 
 def resolve_assignments(assignment_queries, course_assignments, id_field = 'id'):
     """
     Try to match each assignment query to an acutal assignment.
     """
 
     assignments = []
```

### Comparing `edq-canvas-0.0.5/canvas/api/assignment/uploadscores.py` & `edq_canvas-0.0.6/canvas/api/assignment/uploadscores.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/api/common.py` & `edq_canvas-0.0.6/canvas/api/common.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/api/gradebook/fetch.py` & `edq_canvas-0.0.6/canvas/api/gradebook/fetch.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/api/gradebook/upload.py` & `edq_canvas-0.0.6/canvas/api/gradebook/upload.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/api/user/common.py` & `edq_canvas-0.0.6/canvas/api/user/common.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/api/user/fetch.py` & `edq_canvas-0.0.6/canvas/api/user/fetch.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/api/user/list.py` & `edq_canvas-0.0.6/canvas/api/user/list.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/api/user/resolve.py` & `edq_canvas-0.0.6/canvas/api/user/resolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return users
 
     result = []
     for user in users:
         if (user is None):
             result.append(None)
         else:
-            result.append({key: user[key] for key in keys})
+            result.append({key: user.get(key, None) for key in keys})
 
     return result
 
 def resolve_users(user_queries, course_users, id_field = 'id', fill_missing = False):
     """
     Try to match each user query to an actual user.
```

### Comparing `edq-canvas-0.0.5/canvas/cli/assignment/fetch-scores.py` & `edq_canvas-0.0.6/canvas/cli/assignment/fetch-scores.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/cli/assignment/fetch.py` & `edq_canvas-0.0.6/canvas/cli/assignment/fetch.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/cli/assignment/list.py` & `edq_canvas-0.0.6/canvas/cli/assignment/list.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/cli/assignment/upload-score.py` & `edq_canvas-0.0.6/canvas/cli/assignment/upload-score.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/cli/assignment/upload-scores.py` & `edq_canvas-0.0.6/canvas/cli/assignment/upload-scores.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/cli/common.py` & `edq_canvas-0.0.6/canvas/cli/common.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/cli/gradebook/fetch.py` & `edq_canvas-0.0.6/canvas/cli/gradebook/fetch.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/cli/gradebook/upload.py` & `edq_canvas-0.0.6/canvas/cli/gradebook/upload.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/cli/user/fetch.py` & `edq_canvas-0.0.6/canvas/cli/user/fetch.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/cli/user/list.py` & `edq_canvas-0.0.6/canvas/cli/user/list.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/config.py` & `edq_canvas-0.0.6/canvas/config.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/log.py` & `edq_canvas-0.0.6/canvas/log.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/canvas/util/cli.py` & `edq_canvas-0.0.6/canvas/util/cli.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.5/edq_canvas.egg-info/PKG-INFO` & `edq_canvas-0.0.6/edq_canvas.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edq-canvas
-Version: 0.0.5
+Version: 0.0.6
 Summary: A suite of tools and Python interface for Instructure's Canvas LMS.
 Author-email: Eriq Augustine <eaugusti@ucsc.edu>
 License: MIT License
         
         Copyright (c) 2023 Eriq Augustine
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -52,14 +52,15 @@
     - [Assignment Queries](#assignment-queries)
  - [CLI Tools](#cli-tools)
     - [List Course Users](#list-course-users)
     - [Fetch a Single User](#fetch-a-single-user)
     - [List Assignments](#list-assignments)
     - [Fetch a Single Assignment](#fetch-a-single-assignment)
     - [Fetch Assignment Scores](#fetch-assignment-scores)
+    - [Fetch Assignment Submission Files](#fetch-assignment-submission-files)
     - [Upload Assignment Scores](#upload-assignment-scores)
     - [Upload Single Assignment Score](#upload-single-assignment-score)
     - [Fetch Gradebook](#fetch-gradebook)
     - [Upload Gradebook](#upload-gradebook)
 
 ## Installation
 
@@ -187,29 +188,47 @@
 ### Fetch a Single Assignment
 
 Fetch information about a single assignment using the `canvas.cli.assignment.fetch` tool.
 For example:
 ```
 python3 -m canvas.cli.assignment.fetch 123456
 
+# Or
 python3 -m canvas.cli.assignment.fetch 'My Assignment'
 ```
 
 ### Fetch Assignment Scores
 
 To fetch the scores for a specific assignment, use the `canvas.cli.assignment.fetch-scores` tool.
 For example:
 ```
 python3 -m canvas.cli.assignment.fetch-scores 123456
 
+# Or
 python3 -m canvas.cli.assignment.fetch-scores 'My Assignment'
 ```
 
 The student's email and score will be written to stdout as a tab-separated row.
 
+### Fetch Assignment Submission Files
+
+To fetch the files students have submitted for an assignment, use the `canvas.cli.assignment.fetch-submission-files` tool.
+For example:
+```
+python3 -m canvas.cli.assignment.fetch-submission-files 123456
+
+# Or
+python3 -m canvas.cli.assignment.fetch-submission-files 'My Assignment'
+```
+
+Only assignment with a submission type of "Online - Text Entry" or "Online - File Uploads" will be downloaded.
+
+By default, files will be written to the `out` directory.
+This can be controlled with the `--out-dir` argument.
+
 ### Upload Assignment Scores
 
 Uploading scores for an assignment can be done with the `canvas.cli.assignment.upload-scores` tool:
 ```
 python3 -m canvas.cli.assignment.upload-scores <assignment query> <path>
 ```
```

### Comparing `edq-canvas-0.0.5/edq_canvas.egg-info/SOURCES.txt` & `edq_canvas-0.0.6/edq_canvas.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 canvas/log.py
 canvas/api/__init__.py
 canvas/api/common.py
 canvas/api/assignment/__init__.py
 canvas/api/assignment/common.py
 canvas/api/assignment/fetch.py
 canvas/api/assignment/fetchscores.py
+canvas/api/assignment/fetchsubmissionfiles.py
 canvas/api/assignment/list.py
 canvas/api/assignment/resolve.py
 canvas/api/assignment/uploadscores.py
 canvas/api/gradebook/__init__.py
 canvas/api/gradebook/fetch.py
 canvas/api/gradebook/upload.py
 canvas/api/user/__init__.py
@@ -25,14 +26,15 @@
 canvas/cli/__init__.py
 canvas/cli/__main__.py
 canvas/cli/common.py
 canvas/cli/assignment/__init__.py
 canvas/cli/assignment/__main__.py
 canvas/cli/assignment/common.py
 canvas/cli/assignment/fetch-scores.py
+canvas/cli/assignment/fetch-submission-files.py
 canvas/cli/assignment/fetch.py
 canvas/cli/assignment/list.py
 canvas/cli/assignment/upload-score.py
 canvas/cli/assignment/upload-scores.py
 canvas/cli/gradebook/__init__.py
 canvas/cli/gradebook/__main__.py
 canvas/cli/gradebook/fetch.py
@@ -41,12 +43,13 @@
 canvas/cli/user/__main__.py
 canvas/cli/user/common.py
 canvas/cli/user/fetch.py
 canvas/cli/user/list.py
 canvas/util/__init__.py
 canvas/util/cli.py
 canvas/util/code.py
+canvas/util/file.py
 edq_canvas.egg-info/PKG-INFO
 edq_canvas.egg-info/SOURCES.txt
 edq_canvas.egg-info/dependency_links.txt
 edq_canvas.egg-info/requires.txt
 edq_canvas.egg-info/top_level.txt
```

### Comparing `edq-canvas-0.0.5/pyproject.toml` & `edq_canvas-0.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "packaging>=21.3",
     "twine",
     "vermin",
 ]
 
 [project]
 name = "edq-canvas"
-version = "0.0.5"
+version = "0.0.6"
 description = "A suite of tools and Python interface for Instructure's Canvas LMS."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 
 authors = [
     {name = "Eriq Augustine", email = "eaugusti@ucsc.edu"},
```

