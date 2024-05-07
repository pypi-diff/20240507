# Comparing `tmp/hostess-0.9.1.tar.gz` & `tmp/hostess-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hostess-0.9.1.tar", last modified: Tue Dec 19 20:29:39 2023, max compression
+gzip compressed data, was "hostess-0.9.2.tar", last modified: Tue May  7 18:13:17 2024, max compression
```

## Comparing `hostess-0.9.1.tar` & `hostess-0.9.2.tar`

### file list

```diff
@@ -1,75 +1,79 @@
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-12-19 20:29:39.381929 hostess-0.9.1/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1524 2023-05-03 19:45:04.000000 hostess-0.9.1/LICENSE
--rw-r--r--   0 sierra    (1000) sierra    (1000)     1366 2023-12-19 20:29:39.381929 hostess-0.9.1/PKG-INFO
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3372 2023-12-19 20:25:55.000000 hostess-0.9.1/README.md
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-12-19 20:29:39.373929 hostess-0.9.1/hostess/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       22 2023-12-19 20:25:55.000000 hostess-0.9.1/hostess/__init__.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-12-19 20:29:39.377929 hostess-0.9.1/hostess/aws/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-05-03 19:45:04.000000 hostess-0.9.1/hostess/aws/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)   112540 2023-12-19 20:25:55.000000 hostess-0.9.1/hostess/aws/ec2.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     7160 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/aws/pricing.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    33623 2023-12-19 20:25:55.000000 hostess-0.9.1/hostess/aws/s3.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    12842 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/aws/utilities.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    16404 2023-12-19 20:25:55.000000 hostess-0.9.1/hostess/caller.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-12-19 20:29:39.377929 hostess-0.9.1/hostess/config/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      781 2023-12-19 20:25:55.000000 hostess-0.9.1/hostess/config/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      874 2023-12-19 20:25:55.000000 hostess-0.9.1/hostess/config/config.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      213 2023-05-03 19:45:04.000000 hostess-0.9.1/hostess/config/user_config.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     8269 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/directory.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    22358 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/monitors.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    30934 2023-12-19 20:25:55.000000 hostess-0.9.1/hostess/profilers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    11754 2023-12-19 20:25:55.000000 hostess-0.9.1/hostess/serverpool.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2290 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/shortcuts.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    23660 2023-12-19 20:25:55.000000 hostess-0.9.1/hostess/ssh.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-12-19 20:29:39.377929 hostess-0.9.1/hostess/station/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-11-06 17:06:28.000000 hostess-0.9.1/hostess/station/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    14643 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/actors.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    33940 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/bases.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4127 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/comm.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    28481 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/delegates.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     8229 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/handlers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    22323 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/messages.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-12-19 20:29:39.377929 hostess-0.9.1/hostess/station/proto/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-11-06 17:06:28.000000 hostess-0.9.1/hostess/station/proto/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     7076 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/proto/station.proto
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    14747 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/proto/station_pb2.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3684 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/proto_utils.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-12-19 20:29:39.377929 hostess-0.9.1/hostess/station/situation/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       79 2023-11-06 17:06:28.000000 hostess-0.9.1/hostess/station/situation/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1214 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/situation/_textual_monkeypatch.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     7221 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/situation/app.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     5488 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/situation/interface_organizers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2471 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/situation/loopquery.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     5147 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/situation/response_organizers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     6106 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/situation/sitstation.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     8106 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/situation/widgets.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    36698 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/station.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    23699 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/talkie.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-12-19 20:29:39.377929 hostess-0.9.1/hostess/station/tests/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-11-06 17:06:28.000000 hostess-0.9.1/hostess/station/tests/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      360 2023-11-06 17:06:28.000000 hostess-0.9.1/hostess/station/tests/target_functions.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-12-19 20:29:39.377929 hostess-0.9.1/hostess/station/tests/test_data/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)   309034 2023-11-06 17:06:28.000000 hostess-0.9.1/hostess/station/tests/test_data/squirrel.jpg
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      568 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/tests/test_handler.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     8337 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/tests/test_station.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4725 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/tests/test_talkie.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      489 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/station/tests/testing_actors.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    39200 2023-12-19 20:25:55.000000 hostess-0.9.1/hostess/subutils.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-12-19 20:29:39.377929 hostess-0.9.1/hostess/tests/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-11-06 17:06:28.000000 hostess-0.9.1/hostess/tests/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2023 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/tests/test_caller.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      838 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/tests/test_directory.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1967 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/tests/test_monitors.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4398 2023-12-19 20:25:55.000000 hostess-0.9.1/hostess/tests/test_profilers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      571 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/tests/test_subutils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3703 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/tests/test_utilities.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2516 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/tests/utilz.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    13341 2023-12-08 19:28:53.000000 hostess-0.9.1/hostess/utilities.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-12-19 20:29:39.377929 hostess-0.9.1/hostess.egg-info/
--rw-r--r--   0 sierra    (1000) sierra    (1000)     1366 2023-12-19 20:29:39.000000 hostess-0.9.1/hostess.egg-info/PKG-INFO
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1795 2023-12-19 20:29:39.000000 hostess-0.9.1/hostess.egg-info/SOURCES.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2023-12-19 20:29:39.000000 hostess-0.9.1/hostess.egg-info/dependency_links.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      219 2023-12-19 20:29:39.000000 hostess-0.9.1/hostess.egg-info/requires.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        8 2023-12-19 20:29:39.000000 hostess-0.9.1/hostess.egg-info/top_level.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2023-12-19 20:29:39.381929 hostess-0.9.1/setup.cfg
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1215 2023-12-19 20:25:55.000000 hostess-0.9.1/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-07 18:13:17.296090 hostess-0.9.2/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1524 2023-04-05 16:34:08.000000 hostess-0.9.2/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     1366 2024-05-07 18:13:17.296090 hostess-0.9.2/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3366 2024-05-07 18:09:49.000000 hostess-0.9.2/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-07 18:13:17.292090 hostess-0.9.2/hostess/
+-rw-rw-r--   0 michael   (1000) michael   (1000)       22 2024-05-07 18:09:49.000000 hostess-0.9.2/hostess/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      689 2023-10-20 19:56:41.000000 hostess-0.9.2/hostess/argscratch.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-07 18:13:17.292090 hostess-0.9.2/hostess/aws/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-04-05 16:34:08.000000 hostess-0.9.2/hostess/aws/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)   114105 2024-05-07 18:09:49.000000 hostess-0.9.2/hostess/aws/ec2.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7160 2023-12-09 23:22:23.000000 hostess-0.9.2/hostess/aws/pricing.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    34205 2024-05-07 18:09:49.000000 hostess-0.9.2/hostess/aws/s3.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12898 2024-05-07 18:09:49.000000 hostess-0.9.2/hostess/aws/utilities.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    16404 2024-05-07 18:09:49.000000 hostess-0.9.2/hostess/caller.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-07 18:13:17.292090 hostess-0.9.2/hostess/config/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      781 2024-05-07 18:09:49.000000 hostess-0.9.2/hostess/config/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      874 2024-05-07 18:09:49.000000 hostess-0.9.2/hostess/config/config.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      213 2023-04-05 16:34:08.000000 hostess-0.9.2/hostess/config/user_config.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8269 2024-02-02 20:24:25.000000 hostess-0.9.2/hostess/directory.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    22358 2023-12-09 23:22:23.000000 hostess-0.9.2/hostess/monitors.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    31118 2024-05-07 18:09:49.000000 hostess-0.9.2/hostess/profilers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11754 2024-05-07 18:09:49.000000 hostess-0.9.2/hostess/serverpool.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2290 2023-11-28 21:31:22.000000 hostess-0.9.2/hostess/shortcuts.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    24183 2024-05-07 18:09:49.000000 hostess-0.9.2/hostess/ssh.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-07 18:13:17.292090 hostess-0.9.2/hostess/station/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-10-14 17:53:46.000000 hostess-0.9.2/hostess/station/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    14643 2023-11-28 21:34:19.000000 hostess-0.9.2/hostess/station/actors.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    33940 2023-11-28 21:34:23.000000 hostess-0.9.2/hostess/station/bases.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4127 2023-11-28 21:34:39.000000 hostess-0.9.2/hostess/station/comm.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    28481 2023-11-28 21:34:39.000000 hostess-0.9.2/hostess/station/delegates.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8229 2023-11-28 21:34:44.000000 hostess-0.9.2/hostess/station/handlers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      748 2023-06-22 19:22:50.000000 hostess-0.9.2/hostess/station/launchallscratch.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    22323 2023-12-09 23:22:23.000000 hostess-0.9.2/hostess/station/messages.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-07 18:13:17.292090 hostess-0.9.2/hostess/station/proto/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-10-14 17:53:46.000000 hostess-0.9.2/hostess/station/proto/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7076 2023-12-09 23:22:23.000000 hostess-0.9.2/hostess/station/proto/station.proto
+-rw-rw-r--   0 michael   (1000) michael   (1000)    14747 2023-12-09 23:22:23.000000 hostess-0.9.2/hostess/station/proto/station_pb2.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3684 2023-11-28 21:35:00.000000 hostess-0.9.2/hostess/station/proto_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      504 2023-11-04 23:26:44.000000 hostess-0.9.2/hostess/station/shutscratch.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-07 18:13:17.292090 hostess-0.9.2/hostess/station/situation/
+-rw-rw-r--   0 michael   (1000) michael   (1000)       79 2023-11-22 00:43:35.000000 hostess-0.9.2/hostess/station/situation/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1214 2023-11-28 21:33:54.000000 hostess-0.9.2/hostess/station/situation/_textual_monkeypatch.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7221 2023-11-28 21:33:52.000000 hostess-0.9.2/hostess/station/situation/app.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5488 2023-11-28 21:33:57.000000 hostess-0.9.2/hostess/station/situation/interface_organizers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2471 2023-11-28 21:33:59.000000 hostess-0.9.2/hostess/station/situation/loopquery.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5147 2023-11-28 21:34:00.000000 hostess-0.9.2/hostess/station/situation/response_organizers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6106 2023-11-28 21:34:02.000000 hostess-0.9.2/hostess/station/situation/sitstation.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8106 2023-11-28 21:34:04.000000 hostess-0.9.2/hostess/station/situation/widgets.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    36698 2023-12-09 23:22:23.000000 hostess-0.9.2/hostess/station/station.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    23699 2023-11-28 21:37:11.000000 hostess-0.9.2/hostess/station/talkie.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-07 18:13:17.292090 hostess-0.9.2/hostess/station/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-10-14 17:53:46.000000 hostess-0.9.2/hostess/station/tests/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      360 2023-10-14 17:53:46.000000 hostess-0.9.2/hostess/station/tests/target_functions.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-07 18:13:17.292090 hostess-0.9.2/hostess/station/tests/test_data/
+-rw-rw-r--   0 michael   (1000) michael   (1000)   309034 2023-10-14 17:53:46.000000 hostess-0.9.2/hostess/station/tests/test_data/squirrel.jpg
+-rw-rw-r--   0 michael   (1000) michael   (1000)      568 2023-11-28 21:34:10.000000 hostess-0.9.2/hostess/station/tests/test_handler.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8337 2023-11-28 21:34:12.000000 hostess-0.9.2/hostess/station/tests/test_station.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4725 2023-11-28 21:34:14.000000 hostess-0.9.2/hostess/station/tests/test_talkie.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      489 2023-11-28 21:34:15.000000 hostess-0.9.2/hostess/station/tests/testing_actors.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    40641 2024-05-07 18:09:49.000000 hostess-0.9.2/hostess/subutils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3432 2023-09-07 17:32:36.000000 hostess-0.9.2/hostess/tdscratch.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-07 18:13:17.296090 hostess-0.9.2/hostess/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-10-14 17:53:46.000000 hostess-0.9.2/hostess/tests/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2023 2023-12-09 23:22:23.000000 hostess-0.9.2/hostess/tests/test_caller.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      838 2023-11-22 00:43:35.000000 hostess-0.9.2/hostess/tests/test_directory.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1967 2023-12-09 23:22:23.000000 hostess-0.9.2/hostess/tests/test_monitors.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4398 2024-05-07 18:09:49.000000 hostess-0.9.2/hostess/tests/test_profilers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      571 2023-11-27 19:10:46.000000 hostess-0.9.2/hostess/tests/test_subutils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3703 2023-12-09 23:22:23.000000 hostess-0.9.2/hostess/tests/test_utilities.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2516 2023-11-27 19:10:46.000000 hostess-0.9.2/hostess/tests/utilz.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    13390 2024-05-07 18:09:49.000000 hostess-0.9.2/hostess/utilities.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-07 18:13:17.296090 hostess-0.9.2/hostess.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1366 2024-05-07 18:13:17.000000 hostess-0.9.2/hostess.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1905 2024-05-07 18:13:17.000000 hostess-0.9.2/hostess.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2024-05-07 18:13:17.000000 hostess-0.9.2/hostess.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)      219 2024-05-07 18:13:17.000000 hostess-0.9.2/hostess.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        8 2024-05-07 18:13:17.000000 hostess-0.9.2/hostess.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       38 2024-05-07 18:13:17.296090 hostess-0.9.2/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1215 2024-05-07 18:09:49.000000 hostess-0.9.2/setup.py
```

### Comparing `hostess-0.9.1/LICENSE` & `hostess-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/PKG-INFO` & `hostess-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hostess
-Version: 0.9.1
+Version: 0.9.2
 Summary: intuitive admin library
 Author: Million Concepts
 Author-email: mstclair@millionconcepts.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hostess-0.9.1/README.md` & `hostess-0.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,31 +26,32 @@
 
 ## documentation
 
 Examples for working with EC2 instances can be found [in this jupyter notebook](https://github.com/MillionConcepts/hostess/blob/main/examples/ec2.ipynb).
 
 Examples for working with S3 buckets can be found [in this jupyter notebook](https://github.com/MillionConcepts/hostess/blob/main/examples/s3.ipynb).
 
-[You can find extended documentation and an API reference on readthedocs.](https://hostess.readthedocs.io)
+[You can find an API reference and full changelog on readthedocs.](https://hostess.readthedocs.io)
 [![Documentation Status](https://readthedocs.org/projects/hostess/badge/?version=latest)](https://hostess.readthedocs.io/en/latest/?badge=latest)
 
 ## compatibility
 
 1. `hostess`'s core features are closely linked to the shell, so it is 
 only fully compatible with Unix-scented operating systems. Linux and MacOS 
 count, as does Windows Subsystem for Linux (WSL). Windows *outside* of WSL 
 doesn't.
 2. Some `hostess` modules require network access, specifically `ssh` and the
 `aws` submodules. The `aws` submodules also require an AWS account. See the 
 example Notebooks for more details on this.
 3. `hostess` requires Python >= 3.9.
 4. `hostess` is very lightweight. If a machine has enough resources to run 
 a Python interpreter, it can probably run `hostess`.
-5. `hostess.station` is not fully compatible with MacOS or WSL. MacOS and WSL compatibility
-is planned. All other parts of `hostess` are compatible with MacOS and WSL.
+5. `hostess.station` is not fully compatible with MacOS or WSL. MacOS and WSL 
+compatibility is planned. All other parts of `hostess` are compatible with 
+MacOS and WSL.
 
 ## cautions
 
 `hostess` is a reliable and fairly feature-complete beta in active use on
 multiple projects. However, we do not yet guarantee interface stability or
 backwards compatibility.
```

### Comparing `hostess-0.9.1/hostess/aws/ec2.py` & `hostess-0.9.2/hostess/aws/ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,42 @@
     return instances
 
 
 class Instance:
     """
     Interface to an EC2 instance. Enables remote procedure calls, state
     control, and monitoring.
+
+    Attributes:
+        session (boto3.Session): session for API calls
+        client (botocore.client.BaseClient): client for API calls
+        resource (boto3.resources.base.ServiceResource): resource for API calls
+        instance_ (boto3.EC2.Instance): underlying boto3 `Instance` used for
+            some API operations
+        instance_id (str): AWS instance id
+        instance_type (str): AWS instance type (e.g. 't3a.micro')
+        tags (dict): AWS resource tags for instance
+        launch_time (datetime): Time instance was launched
+        name (Optional[str]): Value of 'Name' tag; None if not present
+        zone (str): AWS Availability Zone
+        uname (Optional[str]): Username for SSH operations (if known)
+        passed_key (Optional[Path]): User-specified path to SSH keyfile, if any
+        state (InstanceState): state of instance (e.g. 'running')
+        _ssh (hostess.ssh.SSH): Underlying `SSH` object for command execution
+        address_type (Literal["private", "public"]): Whether we are using the
+            instance's public or private IP for SSH connections. (Private IP
+            should generally only be used from within AWS).
+        ip (Optional[str]): IPv4 address of instance -- its private
+            IP if `address_type` is "private"; public IP otherwise. None if the
+            instance has no IP (e.g., if it's stopped) or its IP cannot be
+            determined.
+        key (Optional[str]): stringified path to actually-existing SSH keyfile,
+            if found
+        key_errstring (Optional[str]): detailed description of what went wrong
+            with our last attempt to find and load an SSH keyfile, if anything
     """
 
     def __init__(
         self,
         description: Union[InstanceIdentifier, InstanceDescription],
         *,
         uname: str = GENERAL_DEFAULTS["uname"],
@@ -527,15 +555,15 @@
         **kwargs: Union[int, str, float, bool],
     ) -> Processlike:
         """
         run a command in the instance's default interpreter.
 
         Args:
             command: command name or full text of command
-                (see hostess.subutils.RunCommand.__call__() for detailed
+                (see `hostess.subutils.RunCommand.__call__()` for details on
                 calling conventions).
             *args: args to pass to `self._ssh.__call__()`.
             _viewer: if `True`, return a `Viewer` object. otherwise return
                 unwrapped result from `self._ssh.__call__()`.
             _wait: if `True`, block until command terminates (or connection
                 fails). _w is an alias.
             _quiet: if `False`, print stdout and stderr, should the process
@@ -570,15 +598,15 @@
         terminal emulator. pauses for output and pretty-prints it to stdout.
 
         Does not return a process abstraction by default (pass
         _return_viewer=True if you want one). Fun in interactive environments.
 
         Args:
             command: command name or full text of command
-                (see hostess.subutils.RunCommand.__call__() for detailed
+                (see `hostess.subutils.RunCommand.__call__()` for details on
                 calling conventions).
             _poll: polling rate for process output, in seconds
             _timeout: if not None, raise a TimeoutError if this many seconds
                 pass before receiving additional output from process (or
                 process exit).
             _return_viewer: if True, return a Viewer for the process once it
                 exits. Otherwise, return None.
@@ -641,16 +669,16 @@
         """
         self._prep_connection()
         return jupyter_connect(self._ssh, **connect_kwargs)
 
     @connectwrap
     def install_conda(
         self,
-        installer_url=CONDA_DEFAULTS['installer_url'],
-        prefix=CONDA_DEFAULTS['prefix'],
+        installer_url: str = CONDA_DEFAULTS['installer_url'],
+        prefix: str = CONDA_DEFAULTS['prefix'],
         **kwargs: bool
     ) -> Processlike:
         """
         install a Conda Python distribution on the instance.
 
         Args:
             installer_url: url of install script; by default, the latest
@@ -1039,15 +1067,15 @@
                 the shell command.
             env: optional name of conda environment. both `interpreter` and
                 `env` cannot be specified. If neither are specified, simply
                 uses the first `python` binary on the remote user's $PATH,
                 if any.
             compression: compression for payload. 'gzip' or None.
             serialization: how to serialize `payload`. 'json' means serialize
-                to JSON; 'pickle' means serialize using pickle; None means just
+                to knownJSON; 'pickle' means serialize using pickle; None means just
                 use the string representation of `payload`.
             splat: Operator for splatting the payload into the function call.
                 `"*"` means `func(*payload)`, `"**"` means `func(**payload)`;
                 None means `func(payload)`.
             payload_encoded: set to True if you have already
                 compressed/serialized `payload` with the specified methods.
             print_result: if True, the function call will print its result
@@ -1137,20 +1165,15 @@
             return f"{self.instance_id}: {string}"
         return f"{self.name} ({self.instance_id}): {string}"
 
     def __str__(self):
         return self.__repr__()
 
     key = None
-    """path to SSH keyfile"""
     key_errstring = None
-    """
-    detailed description of what's wrong with our attempt to find an SSH 
-    keyfile, if anything
-    """
 
 
 class Cluster:
     """Class offering an interface to multiple EC2 instances at once."""
 
     def __init__(self, instances: Collection[Instance]):
         """
@@ -1215,19 +1238,19 @@
     ) -> ServerPool:
         """
         Internal wrapper function: make multithreaded calls to a specified
         method of this Cluster's Instances with arbitrary number and
         homogeneity of arguments.
 
         Args:
-             method: name of method of Instance to call on Instances
-             argseq: optional args to pass to these method calls -- one
+            method: name of method of Instance to call on Instances
+            argseq: optional args to pass to these method calls -- one
                 sequence of args per Instance. either `args` or `kwargs` must
                 be defined.
-             kwargseq: optional kwargs to pass to these method calls -- one
+            kwargseq: optional kwargs to pass to these method calls -- one
                 `dict` or other `Mapping` of kwargs per Instance.
 
         Returns:
             list containing result of method call from each Instance,
                 including raised Exceptions for failed calls
         """
         argseq, kwargseq = self._format_map_arguments(argseq, kwargseq)
@@ -1249,19 +1272,19 @@
         kwargseq: Optional[Union[Sequence[Mapping[str, Any]], cycle]] = None,
     ) -> list[Any]:
         """"
         Internal wrapper function: make multithreaded calls to a specified
         file I/O method of all this Cluster's Instances.
 
         Args:
-             method: name of file I/O method of Instance
-             argseq: optional args to pass to calls -- one sequence of args,
-                one sequence of args per Instance, or a `cycle`. either `args`
-                or `kwargs` must be defined.
-             kwargseq: optional kwargs to pass to these method calls -- a single
+            method: name of file I/O method of Instance
+            argseq: optional args to pass to calls -- one sequence of args,
+                one sequence of args per Instance, or a `cycle`. either
+                `args` or `kwargs` must be defined.
+            kwargseq: optional kwargs to pass to these method calls -- a single
                 `dict` or other `Mapping`, one `Mapping` of kwargs per
                 Instance, or a `cycle`.
 
         Returns:
             list containing result of method call from each Instance,
                 including raised Exceptions for failed calls
         """
@@ -1873,16 +1896,16 @@
         concatenated = pd.concat(frames)
         if reset_index is False:
             return concatenated
         return concatenated.reset_index(drop=True)
 
     def install_conda(
         self,
-        installer_url=CONDA_DEFAULTS['installer_url'],
-        prefix=CONDA_DEFAULTS['prefix'],
+        installer_url: str = CONDA_DEFAULTS['installer_url'],
+        prefix: str = CONDA_DEFAULTS['prefix'],
         _permissive: bool = False,
         _warn: bool = False,
         **kwargs: bool
     ) -> list[Union[Processlike, Exception]]:
         """
         install a Conda Python distribution on all instances.
```

### Comparing `hostess-0.9.1/hostess/aws/pricing.py` & `hostess-0.9.2/hostess/aws/pricing.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/aws/s3.py` & `hostess-0.9.2/hostess/aws/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,27 +186,33 @@
             setattr(self, name, partial(thing, self, config=self.config))
         self.n_threads = n_threads
 
     def update_contents(
         self,
         prefix: Optional[str] = None,
         cache: Optional[Union[str, Path, IOBase]] = None,
+        fetch_owner: bool = False
     ):
         """
         recursively scan the contents of the bucket and store the result in
         self.contents.
 
         Args:
             prefix: prefix at which to begin scan. if not passed, scans the
                 entire bucket.
             cache: optional file or filelike object to write scan results to
                 in addition to storing them in self.contents.
+            fetch_owner: if True, include owner of objects in response.
         """
         self.contents = self.ls(
-            recursive=True, prefix=prefix, cache=cache, formatting="contents"
+            recursive=True,
+            prefix=prefix,
+            cache=cache,
+            formatting="contents",
+            fetch_owner=fetch_owner,
         )
 
     def chunk_putter_factory(
         self,
         key: str,
         upload_threads: Optional[int] = 4,
         download_threads: Optional[int] = None,
@@ -267,15 +273,14 @@
         """
         Create an S3 object from a byte stream via a managed multipart upload.
         Useful for uploading large files, but can also handle intermittent
         streams, larger-than-memory transfers, direct streams from remote URLs,
         and streams of unknown length.
 
         Args:
-            self: Bucket or name of bucket
             obj: source of stream to upload. May be a path, a URL, a filelike
                 object, or any iterator that yields bytes.
             key: key of object to create from stream (fully-qualified 'path'
                 relative to bucket root)
             config: optional transfer config
             upload_threads: number of subprocesses to use for upload (None
                 means upload serially)
@@ -667,14 +672,15 @@
         self,
         prefix: Optional[str] = None,
         recursive: bool = False,
         formatting: Literal["simple", "contents", "df", "raw"] = "simple",
         cache: Union[str, Path, IOBase, None] = None,
         start_after: Optional[str] = None,
         cache_only: bool = False,
+        fetch_owner: bool = False
     ) -> Union[tuple, pd.DataFrame, None]:
         """
         list objects in a bucket.
 
         Args:
             prefix: prefix ('folder') to list (if not specified, defaults to
                 bucket root)
@@ -687,14 +693,16 @@
                 * "raw": API response as reported by boto3
             cache: optional file or filelike object to write results to.
             start_after: if specified, begin listing objects only "after" this
                 prefix. intended principally for sequential calls.
             cache_only: _only_ write results into the specified cache; do not
                 retain them in memory. intended mainly for cases in which the
                 full list would be larger than available memory.
+            fetch_owner: if True, include owner of objects in output. Not
+                enabled by default due to permissioning and performance issues.
 
         Returns:
             Manifest of contents, format dependent on `formatting`; or None
                 if `cache_only` is True.
         """
         kwargs = {"Bucket": self.name}
         if recursive is False:
@@ -706,14 +714,15 @@
             kwargs["Delimiter"] = "/"
         if recursive is False and prefix is None:
             kwargs["Prefix"] = ""
         elif prefix is not None:
             kwargs["Prefix"] = prefix.lstrip("/")
         if start_after is not None:
             kwargs["StartAfter"] = start_after
+        kwargs["FetchOwner"] = fetch_owner
         # pagination is typically slightly faster than iteratively passing
         # StartAfter based on the last key of a truncated response
         paginator = self.client.get_paginator("list_objects_v2")
         cache = Path(cache) if isinstance(cache, str) else cache
         self._maybe_prep_ls_cache(cache)
         pages = []
         for page in iter(paginator.paginate(**kwargs)):
@@ -734,15 +743,19 @@
         if formatting == "simple":
             return tuple(
                 [obj["Key"] for obj in objects]
                 + [obj["Prefix"] for obj in prefixes]
             )
         if formatting == "contents":
             return tuple(objects)
-        return pd.DataFrame(objects)
+        if fetch_owner is False:
+            return pd.DataFrame(objects)
+        objects = tuple(objects)
+        owner_info = pd.DataFrame([o.pop('Owner') for o in objects])
+        return pd.concat(map(pd.DataFrame, (objects, owner_info)), axis=1)
 
     @staticmethod
     def _maybe_prep_ls_cache(cache: Optional[Union[Path, IO]]):
         if cache is None:
             return
         columns = "Key,LastModified,ETag,Size,StorageClass\n"
         if isinstance(cache, Path):
```

### Comparing `hostess-0.9.1/hostess/aws/utilities.py` & `hostess-0.9.2/hostess/aws/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,25 +42,26 @@
         lines = config_file.readlines()
     if "," in lines[0]:
         # this is a downloaded secret key file.
         parsed = next(csv.DictReader(iter(lines)))
         return {"_".join(k.lower().split(" ")): v for k, v in parsed.items()}
     parsed = {}
     if profile is not None:
-        try:
-            lineno, _ = first(
-                i
-                for i, l in enumerate(lines)
-                if l.strip().startswith(f"[{profile}")
-            )
-        except StopIteration:
-            raise OSError(f"{profile} not described in identity file")
+        err, search = f"{profile} not described in identity file", f"[{profile}"
+    else:
+        err, search = "Identity file empty or malformatted", "["
+    try:
+        lineno = first(
+            i for i, l in enumerate(lines) if l.strip().startswith(search)
+        )
+    except StopIteration:
+        raise OSError(err)
     else:
         try:
-            lineno, _ = first(
+            lineno = first(
                 i for i, l in enumerate(lines) if l.strip().startswith("[")
             )
         except StopIteration:
             raise OSError("Identity file empty or malformatted")
     for line in lines[lineno + 1 :]:
         if line.strip().startswith("["):
             break
@@ -88,15 +89,15 @@
             region if not specified)
 
     Returns:
         boto session.
     """
     if credential_file is None:
         return boto3.Session(profile_name=profile, region_name=region)
-    creds = parse_aws_identity_file(credential_file)
+    creds = parse_aws_identity_file(credential_file, profile)
     for disliked_kwarg in ("user_name", "password"):
         if disliked_kwarg in creds.keys():
             del creds[disliked_kwarg]
     return boto3.Session(**creds, region_name=region)
 
 
 def make_boto_client(
```

### Comparing `hostess-0.9.1/hostess/caller.py` & `hostess-0.9.2/hostess/caller.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/config/__init__.py` & `hostess-0.9.2/hostess/config/__init__.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/config/config.py` & `hostess-0.9.2/hostess/config/config.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/directory.py` & `hostess-0.9.2/hostess/directory.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/monitors.py` & `hostess-0.9.2/hostess/monitors.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/profilers.py` & `hostess-0.9.2/hostess/profilers.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,37 +35,36 @@
 from hostess.utilities import mb
 
 
 class Profiler:
     """
     simple profiling object for specific sections of code.
 
-    example of use:
-    ```
-    from array import array
-    from hostess.monitors import RAM, Stopwatch
-    from hostess.profilers import Profiler
-
-    prof = Profiler({'time': Stopwatch(), 'memory': RAM()})
-    with prof.context("f"):
-        var1 = array("B", [0 for _ in range(1024**2 * 100)])
-    with prof.context("g"):
-        var2 = array("B", [0 for _ in range(1024**2 * 250)])
-    print(prof)
-    ```
-    general form of expected output (exact results are system-dependent):
-    ```
-    Profiler
-    f
-      time: 2.935
-      memory: 105.47
-    g
-      time: 7.171
-      memory: 261.76
-    ```
+    Examples:
+        >>> from array import array
+        >>> from hostess.monitors import RAM, Stopwatch
+        >>> from hostess.profilers import Profiler
+
+        >>> prof = Profiler({'time': Stopwatch(), 'memory': RAM()})
+        >>> with prof.context("f"):
+            >>> var1 = array("B", [0 for _ in range(1024**2 * 100)])
+        >>> with prof.context("g"):
+            >>> var2 = array("B", [0 for _ in range(1024**2 * 250)])
+        >>> print(prof)
+
+        general form of expected output (exact results are system-dependent):
+        ```
+        Profiler
+        f
+          time: 2.935
+          memory: 105.47
+        g
+          time: 7.171
+          memory: 261.76
+        ```
     """
 
     def __init__(self, monitors: MutableMapping[str, AbstractMonitor]):
         """
         Args:
             monitors: dictionary of AbstractMonitor objects
                 (see hostess.monitors for examples)
@@ -632,38 +631,38 @@
     permit_types: Collection[type] = frozenset(),
     globals_: Optional[dict[str, Any]] = None,
     return_objects: bool = False,
 ) -> Union[tuple[list[Refnom], list[Any]], list[Refnom]]:
     """
     analyze 'references' to or from obj. designed for, but not limited to,
     analyzing references tracked by the Python garbage collector.
-    Notes:
 
-    1. TAKE SPECIAL CARE WHEN DECORATING THIS FUNCTION OR CALLING IT FROM
+    Danger: careful use is required to avoid memory leaks
+        TAKE SPECIAL CARE WHEN DECORATING THIS FUNCTION OR CALLING IT FROM
         A LAMBDA FUNCTION OR GENERATOR EXPRESSION, NO MATTER HOW HARMLESS-
         LOOKING. These operations may add references that are difficult to
-        recognize or interpret. Calls that do not add context are much
-        safer.
-    2. This function is only completely compatible with CPython.
-    3. All 'exclude', 'permit', and 'filter' operations are implicitly
-        connected by boolean AND. Represented as a predicate:
-
-            ```
-            (~PRIMITIVE(REF) | ~FILTER_PRMITIVE)
-            & (~HISTORY(REF) | ~FILTER_HISTORY)
-            & (~SCOPEDICT(REF) | ~FILTER_SCOPEDICT)
-            & ((ID(REF) != ID(OBJ)) | ~FILTER_REFLEXIVE)
-            & ~(ID(REF) ∈ EXCLUDE_IDS)
-            & (ID(REF) ∈ PERMIT_IDS | PERMIT_IDS = ∅)
-            & ~(TYPE(REF) ∈ EXCLUDE_TYPES)
-            & (TYPE(REF) ∈ PERMIT_TYPES | PERMIT_TYPES = ∅)
-            ```
+        recognize or interpret. Calls that do not add context are much safer.
+
+    Notes:
+        1. All 'exclude', 'permit', and 'filter' operations are implicitly
+            connected by boolean AND. Represented as a predicate:
+
+                (~PRIMITIVE(REF) | ~FILTER_PRMITIVE)
+                & (~HISTORY(REF) | ~FILTER_HISTORY)
+                & (~SCOPEDICT(REF) | ~FILTER_SCOPEDICT)
+                & ((ID(REF) != ID(OBJ)) | ~FILTER_REFLEXIVE)
+                & ~(ID(REF) ∈ EXCLUDE_IDS)
+                & (ID(REF) ∈ PERMIT_IDS | PERMIT_IDS = ∅)
+                & ~(TYPE(REF) ∈ EXCLUDE_TYPES)
+                & (TYPE(REF) ∈ PERMIT_TYPES | PERMIT_TYPES = ∅)
+
+        2. References from obj to itself are never included. This may change
+           in the future.
+        3. This function is only completely compatible with CPython.
 
-    4. references from obj to itself are never included. This may change
-       in the future.
 
     Args:
         obj: object of referential analysis
         method: Function whose return values define 'references' of
             obj. gc.get_referents and gc.get_referrers are the intended and
             tested values.
         filter_primitive: ignore 'primitive' (str, bool, &c) objects?
@@ -813,15 +812,15 @@
             ignore_dunder: ignore variables with "dunder" names?
         """
         self.verbosity = verbosity
         self.warn_new, self.getstack = warn_new, getstack
         self.ignore_dunder = ignore_dunder
         self.refcaches = defaultdict(list)
 
-    def context(self, name: str = "default"):
+    def context(self, name: str = "default") -> _RefAlarmContext:
         """
         Produce a context manager related to this object.
 
         Args:
             name: name for this context, used for verbose reports and
                 `refcache` keys
```

### Comparing `hostess-0.9.1/hostess/serverpool.py` & `hostess-0.9.2/hostess/serverpool.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/shortcuts.py` & `hostess-0.9.2/hostess/shortcuts.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/ssh.py` & `hostess-0.9.2/hostess/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         keyfile: path to local SSH key file
         local_port: port for proximal end of tunnel
         remote_port: port for distal end of tunnel
         signalbuf: list to receive close-tunnel signal
 
     Returns:
         signal received if closed gracefully; tuple of the Connection
-         object and the Exception if it hits an exception.
+        object and the Exception if it hits an exception.
     """
     conn = SSH.connect(host, uname, keyfile).conn
     try:
         with conn.forward_local(local_port, remote_port):
             while True:
                 if signalbuf is not None:
                     if len(signalbuf) > 0:
@@ -139,30 +139,29 @@
 class SSH(RunCommand):
     """
     callable interface to an SSH connection to a remote host. basically a
     wrapper for a fabric.connection.Connection object with additional
     functionality for managed command execution. NOTE: supports only keyfile
     authentication.
 
-    Example of use:
-
+    Examples:
         >>> ssh = SSH.connect(
         ...    "1.11.11.111", 'remote_user', '/home/user/.ssh/keyfile.pem'
         ... )
         >>> ssh("echo hi > a.txt")
         >>> tail = ssh("tail -f a.txt")
         >>> for n in range(5):
             ... ssh(f"echo {n} >> a.txt")
         >>> print(','.join([s.strip() for s in tail.out]))
         >>> ssh.con('ls -l / | grep dev')
 
-    output:
+        expected output:
 
-        hi, 0, 1, 2, 3
-        drwxr-xr-x  15 root   root     3320 Nov 12 01:50 dev
+            hi, 0, 1, 2, 3
+            drwxr-xr-x  15 root   root     3320 Nov 12 01:50 dev
     """
 
     def __init__(
         self,
         command: Optional[str] = None,
         conn: Optional[Connection] = None,
         key: Optional[str] = None,
@@ -257,14 +256,21 @@
                 io.BytesIO)
             *args: args to pass to underlying get method
             **kwargs: kwargs to pass to underlying get method
 
         Returns:
             dict giving transfer metadata: local, remote, host, and port
         """
+        # TODO, maybe: try to improve speed, possibly by increasing chunksize.
+        #  this may require backing transfers with something other than
+        #  paramiko, which by default uses SFTP and includes dire warnings
+        #  about packet sizes > 32kb. Always caching in-memory before writes
+        #  to disk might also improve speed; requires testing.
+        #  more radical options like actually creating an in-memory sshfs
+        #  filesystem of some kind are also possibilities.
         return unpack_transfer_result(
             self.conn.get(str(source), target, *args, **kwargs)
         )
 
     def read(
         self,
         source: str,
@@ -340,16 +346,16 @@
         *args: Union[int, float, str],
         _quiet: bool = True,
         _viewer: bool = True,
         _wait: bool = False,
         **kwargs: Union[int, float, str, bool],
     ) -> Processlike:
         """
-        run a shell command in the remote host's default interpreter.
-        See RunCommand.__call__ for details on calling conventions and options.
+        run a shell command in the remote host's default interpreter. See
+        `RunCommand.__call__()` for details on calling conventions and options.
 
         Args:
             *args: args to use to construct the command.
             _viewer: if `True`, return a hostess `Viewer` object. otherwise
                 return unwrapped Fabric `Result`.
             _wait: if `True`, block until command terminates (or connection
                 fails). _w is an alias.
@@ -431,16 +437,16 @@
         except KeyboardInterrupt:
             process.kill()
             print("^C")
         if _return_viewer is True:
             return process
 
     def close(self):
-        for process, _ in self.tunnels:
-            process.kill()
+        for kill_signal, _meta in self.tunnels:
+            kill_signal()
         if self.conn is not None:
             self.conn.close()
 
     def __str__(self):
         return f"{super().__str__()}\n{self.uname}@{self.host}"
 
     def __del__(self):
```

### Comparing `hostess-0.9.1/hostess/station/actors.py` & `hostess-0.9.2/hostess/station/actors.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/bases.py` & `hostess-0.9.2/hostess/station/bases.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/comm.py` & `hostess-0.9.2/hostess/station/comm.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/delegates.py` & `hostess-0.9.2/hostess/station/delegates.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/handlers.py` & `hostess-0.9.2/hostess/station/handlers.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/messages.py` & `hostess-0.9.2/hostess/station/messages.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/proto/station.proto` & `hostess-0.9.2/hostess/station/proto/station.proto`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/proto/station_pb2.py` & `hostess-0.9.2/hostess/station/proto/station_pb2.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/proto_utils.py` & `hostess-0.9.2/hostess/station/proto_utils.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/situation/_textual_monkeypatch.py` & `hostess-0.9.2/hostess/station/situation/_textual_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/situation/app.py` & `hostess-0.9.2/hostess/station/situation/app.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/situation/interface_organizers.py` & `hostess-0.9.2/hostess/station/situation/interface_organizers.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/situation/loopquery.py` & `hostess-0.9.2/hostess/station/situation/loopquery.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/situation/response_organizers.py` & `hostess-0.9.2/hostess/station/situation/response_organizers.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/situation/sitstation.py` & `hostess-0.9.2/hostess/station/situation/sitstation.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/situation/widgets.py` & `hostess-0.9.2/hostess/station/situation/widgets.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/station.py` & `hostess-0.9.2/hostess/station/station.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/talkie.py` & `hostess-0.9.2/hostess/station/talkie.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/tests/test_data/squirrel.jpg` & `hostess-0.9.2/hostess/station/tests/test_data/squirrel.jpg`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/tests/test_handler.py` & `hostess-0.9.2/hostess/station/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/tests/test_station.py` & `hostess-0.9.2/hostess/station/tests/test_station.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/station/tests/test_talkie.py` & `hostess-0.9.2/hostess/station/tests/test_talkie.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/subutils.py` & `hostess-0.9.2/hostess/subutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -235,15 +235,15 @@
         Args:
             signaler: an optional niladic function whose output acts as a
                 signal to the step when the callback fires. Otherwise, simply
                 execute the step with no signal.
             step: name of step to execute with this callback.
 
         Returns:
-              a function that takes one or no arguments. If it is called
+            a function that takes one or no arguments. If it is called
                 with no argument, it immediately fires the callback. If it
                 is called with an object with a .wait method, it first
                 calls its .wait method. This function returns whatever
                 executing the step returns.
         """
         return partial(dispatch_callback, self, signaler, step)
 
@@ -439,31 +439,40 @@
     """
 
     def __init__(
         self,
         command: Optional[str] = None,
         ctx: Optional[invoke.context.Context] = None,
         runclass: Optional[type(invoke.Runner)] = None,
+        chunksize: int = 20000,
         **kwargs: Any,
     ):
         """
         Args:
             command: optional string form of a shell command to bind to
                 this object. If you do not pass this, this object will be
                 "generic", able to run any shell command. For instance,
                 ls = RunCommand("ls") constructs a RunCommand _just_ for
                 ls. ls(a=True) will run "ls -a".
             ctx: optional Context object (just makes a new one if not given)
             runclass: optional Runner subclass (uses the default of ctx if
                 not given; if both are None, uses invoke.runners.Local)
+            chunksize: maximum number of bytes to read at once from
+                a child process's stdout/stderr. higher values will generally
+                increase performance but may have undesirable effects in some
+                cases.
             **kwargs: optional keyword arguments to bind to this object;
                 Will be added to any kwargs passed to calls to this object.
                 See __call__ for a complete description of behavior.
         """
         self.command = command
+        # TODO: passing this around and directly assigning the attribute is
+        #  inconvenient, but Invoke doesn't seem to explicitly expose it
+        #  anywhere. Check and make sure.
+        self.chunksize = chunksize
         if ctx is None:
             self.ctx = invoke.context.Context()
         else:
             self.ctx = ctx
         if runclass is None:
             self.runclass = list(self.ctx["runners"].values())[0]
         else:
@@ -478,18 +487,18 @@
         *args: Union[int, float, str],
         args_at_end: bool = True,
         **kwargs: Union[int, float, str],
     ):
         """
         Create a shell command string from *args and **kwargs, including any
         command and kwargs curried into this object. Used as part of the
-        __call__() workflow; can also be used to determine what shell
+        `__call__()` workflow; can also be used to determine what shell
         command this object _would_ execute if you called it.
 
-        See __call__ for a complete description of arg and kwarg parsing.
+        See `__call__` for a complete description of arg and kwarg parsing.
 
         Args:
             args: args to parse into shell command
             args_at_end: place args after the first at the end of the shell
                 command?
             kwargs: kwargs to parse into shell command
         """
@@ -522,122 +531,122 @@
             else:
                 kstring += f" --{k}={v}"
         order = (kstring, astring) if args_at_end else (astring, kstring)
         return f"{command}{''.join(order)}"
 
     def __call__(self, *args, **kwargs) -> Optional["Processlike"]:
         """
-         Execute a shell command parsed from `args` and `kwargs`.
+        Execute a shell command parsed from `args` and `kwargs`.
 
-         This method has two legal calling conventions along with a variety of
-         keyword-argument meta-options that modify _how_ it executes the shell
-         command. The meta-options are not defined in the signature in order
-         to facilitate the parsing process.
-
-         **Meta-options:**
-
-         RunCommand understands any kwarg whose name begins with `'_'` as a
-         meta-option, unless the remainder of the kwarg name is numeric (e.g.
-         `'_0'`). All meta-options are optional. Internally-recognized
-         meta-options:
-
-         * `_bg` (aliases `_asynchronous`, `_async`): if True, execute the
-             process in the background. Roughly equivalent to the '&' control
-             operator in bash. If False, block until process exit. (Default
-             False)
-         * `_out` (alias `_out_stream`): Additional target for process stdout.
-             Must have a `write()` method. (If `_viewer=True`, defaults to
-             `Viewer`'s default behavior. Otherwise, defaults to a `Nullify`
-             object, which simply discards the stream).
-         * `_err` (alias `_err_stream`): Same as `_out`, but for stderr.
-         * `_viewer` (alias `_v`): if True, return a `Viewer` object permitting
-             additional process inspection and management. `_viewer=True`
-             implies `_bg=True`. (default False)
-         * `_args_at_end`: if True, place positional arguments other than the
-             command string at the end of the parsed shell command, after any
-             shell options parsed from kwargs. Otherwise, place them before
-             shell options. (Default True)
-         * `_done`: a niladic function to call on process exit. Valid only if
-           `_viewer=True`.
-
-         Any other meta-options are passed directly to the underlying Runner as
-         keyword arguments with `"_"` stripped from their names. `_disown` is
-         often particularly useful.
-
-         **Calling conventions:**
-
-         These conventions are not mutually exclusive, although it is
-         generally less confusing to pick one or the other.
-
-         **1**
-
-         Pass the shell command as a string. This can be simpler in many cases,
-         and is mandatory for programs with non-standard calling conventions,
-         like the `ffmpeg` command below.
-
-         Examples:
-
-             >>> cmd = RunCommand()
-             >>> cmd('ls')
-             >>> cmd('cp -r /path/to/folder /path/to/other/folder')
-             >>> cmd('ffmpeg -i first.mp4 -filter:v "crop=100:10:20:200" second.mp4')
-
-         **2**
-
-         Construct the shell command using multiple arguments to `__call__`.
-         This allows you to treat the shell command more like a Python
-         function, which can be simpler and less error-prone than dynamic
-         string formatting when you would like to pass variable parameters to a
-         command.
-
-         RunCommand uses the following rules to parse args and kwargs into
-         shell command strings. They are compatible with most, although not
-         all, shell programs:
-
-        * RunCommand treats the first positional argument like a shell command
-          name. This means that passing a positional argument is mandatory if
-          you did not bind a command to the RunCommand when creating it. The
-          parsed command string always starts with this argument.
-        * Subsequent positional arguments are command parameters. By
-          default, the parser places them at the end of the command string,
-          after any command options. Pass `_args_at_end=False` to place them
-          before command options.
-        * Keyword arguments are command options. The parser transforms
-          keyword argument names in order to make Python naming and calling
-          conventions compatible with shell conventions.
-            * It ignores `"_"` characters at the start and end of
-              names. This can be used to pass numeric options, like
-              `"_0=True"`, or options that share a name with a Python
-              reserved keyword, like `"dir_=/opt"`.
-            * it treats single-character names (not counting prefixed or
-              suffixed `"_"`) as options preceded by a `"-"` and does not
-              use an `'='` to separate them from their values.
-              `cmd("ls", I="a*")` is equivalent to `"ls -I a*"`.
-            * it treats longer names as options preceded by `"--"` and uses
-              an `'='` to separate them from their values.
-              `cmd("ls", width=20)` is equivalent to `"ls --width=20"`.
-            * It replaces `"_"` characters within names with `"-"`.
-              `cmd("ls", time_style="iso")` is equivalent to
-              `"ls --time-style=iso"`.
-            * if a keyword argument is True, RunCommand treats it as a
-              "switch". `cmd("ls", a=True)` is equivalent to `"ls -a"`.
-            * if a keyword argument is False, RunCommand ignores it.
-              `cmd("ls", a=False)` is equivalent to `"ls"`.
-
-         In addition to these conventions, bear in mind that if you specified a
-         command when you construct a RunCommand object, that command will
-         always be used as the first positional argument to `__call__`, and if
-         you specified kwargs, they will be added to any kwargs you pass or
-         don't pass to `__call__`.
+        This method has two legal calling conventions along with a variety of
+        keyword-argument meta-options that modify _how_ it executes the shell
+        command.
+
+        Calling conventions:
+            These conventions are not mutually exclusive, although it is
+            generally less confusing to pick one or the other.
+
+            **1**
+
+            Pass the shell command as a string. This can be simpler in many cases,
+            and is mandatory for programs with non-standard calling conventions,
+            like the `ffmpeg` command below.
+
+            Examples:
+                >>> cmd = RunCommand()
+                >>> cmd('ls')
+                >>> cmd('cp -r /path/to/folder /path/to/other/folder')
+                >>> cmd('ffmpeg -i first.mp4 -filter:v "crop=100:10:20:200" second.mp4')
+
+            **2**
+
+            Construct the shell command using multiple arguments to `__call__`.
+            This allows you to treat the shell command more like a Python
+            function, which can be simpler and less error-prone than dynamic
+            string formatting when you would like to pass variable parameters to a
+            command.
+
+            RunCommand uses the following rules to parse args and kwargs into
+            shell command strings. They are compatible with most, although not
+            all, shell programs:
+
+            * RunCommand treats the first positional argument like a shell
+              command name. This means that passing a positional argument is
+              mandatory if you did not bind a command to the RunCommand when
+              creating it. The parsed command string always starts with this
+              argument.
+            * Subsequent positional arguments are command parameters. By
+              default, the parser places them at the end of the command string,
+              after any command options. Pass `_args_at_end=False` to place
+              them before command options.
+            * Keyword arguments are command options. The parser transforms
+              keyword argument names in order to make Python naming and calling
+              conventions compatible with shell conventions.
+                * It ignores `"_"` characters at the start and end of
+                  names. This can be used to pass numeric options, like
+                  `"_0=True"`, or options that share a name with a Python
+                  reserved keyword, like `"dir_=/opt"`.
+                * it treats single-character names (not counting prefixed or
+                  suffixed `"_"`) as options preceded by a `"-"` and does not
+                  use an `'='` to separate them from their values.
+                  `cmd("ls", I="a*")` is equivalent to `"ls -I a*"`.
+                * it treats longer names as options preceded by `"--"` and uses
+                  an `'='` to separate them from their values.
+                  `cmd("ls", width=20)` is equivalent to `"ls --width=20"`.
+                * It replaces `"_"` characters within names with `"-"`.
+                  `cmd("ls", time_style="iso")` is equivalent to
+                  `"ls --time-style=iso"`.
+                * if a keyword argument is True, RunCommand treats it as a
+                  "switch". `cmd("ls", a=True)` is equivalent to `"ls -a"`.
+                * if a keyword argument is False, RunCommand ignores it.
+                  `cmd("ls", a=False)` is equivalent to `"ls"`.
+
+        Meta-options:
+            RunCommand understands any kwarg whose name begins with `'_'` as
+            a meta-option, unless the remainder of the kwarg name is numeric
+            (e.g. `'_0'`). All meta-options are optional. The meta-options are
+            not defined in the signature in order to facilitate the parsing
+            process. Internally-recognized meta-options are:
+
+            * `_bg` (aliases `_asynchronous`, `_async`): if True, execute the
+                 process in the background. Roughly equivalent to the '&'
+                 control operator in bash. If False, block until process exit.
+                 (Default False)
+             * `_out` (alias `_out_stream`): Additional target for process
+                stdout.  Must have a `write()` method. (If `_viewer=True`,
+                defaults to `Viewer`'s default behavior. Otherwise, defaults
+                to a `Nullify` object, which simply discards the stream).
+             * `_err` (alias `_err_stream`): Same as `_out`, but for stderr.
+             * `_viewer` (alias `_v`): if True, return a `Viewer` object
+                permitting additional process inspection and management.
+                `_viewer=True`  implies `_bg=True`. (default False)
+             * `_args_at_end`: if True, place positional arguments other than
+                the command string at the end of the parsed shell command,
+                after any shell options parsed from kwargs. Otherwise, place
+                them before shell options. (Default True)
+             * `_done`: a niladic function to call on process exit. Valid only
+                if `_viewer=True`.
+
+             Any other meta-options are passed directly to the underlying
+             `Runner` as keyword arguments with `"_"` stripped from their
+             names. `_disown` is often particularly useful.
+
+        Tip:
+            In addition to these conventions, bear in mind that if you
+            specified a command when you construct a RunCommand object, that
+            command will always be used as the first positional argument to
+            `__call__()`, and if you specified kwargs, they will be added to
+            any kwargs you pass or don't pass to `__call__()`.
 
          Returns:
-             Interface object for executed process. of variable type: if
+             Interface object for executed process. Of variable type: if
                  `_viewer=True`, a Viewer; if `_viewer=False` and `_bg=True`,
                  an Invoke `Result`; if `_viewer=False` and `_bg=False`, an
-                 Invoke `Runner`.
+                 Invoke `Runner`; if `_viewer=False` and `_disown=True`,
+                 `None` (`_disown=True` overrides the value of `_bg`.)
         """
         rkwargs = keyfilter(
             lambda k: k.startswith("_") and not k.strip("_").isnumeric(),
             self.kwargs | kwargs,
         )
         kwargs = keyfilter(lambda k: k not in rkwargs, self.kwargs | kwargs)
         replace_aliases(
@@ -645,14 +654,17 @@
             {
                 "_out_stream": ("_out",),
                 "_err_stream": ("_err",),
                 "_asynchronous": ("_async", "_bg"),
                 "_viewer": ("_v",),
             },
         )
+        # _asynchronous is redundant with _disown, and it upsets Invoke
+        if "_disown" in rkwargs:
+            rkwargs.pop("_asynchronous", None)
         # do not print to stdout/stderr by default
         verbose = rkwargs.pop("verbose", False)
         if verbose is not True:
             for stream in filter(
                 lambda x: x not in rkwargs, ("_out_stream", "_err_stream")
             ):
                 rkwargs[stream] = Nullify()
@@ -667,19 +679,22 @@
             raise ValueError("no command specified.")
         if rkwargs.pop("_viewer", False) is True:
             output = Viewer.from_command(
                 self,
                 *args,
                 ctx=self.ctx,
                 runclass=self.runclass,
+                chunksize=self.chunksize
                 **(rkwargs | kwargs),
             )
         else:
+            runner = self.runclass(self.ctx)
+            runner.read_chunk_size = self.chunksize
             rkwargs = {k[1:]: v for k, v in rkwargs.items()}
-            output = self.runclass(self.ctx).run(cstring, **rkwargs)
+            output = runner.run(cstring, **rkwargs)
         # disowned case
         if output is None:
             return
         # need the runner/result to actually create a thread to watch the
         # done callback. we also never want to actually return a Promise
         # object because it tends to behave badly.
         if ("runner" in dir(output)) and (not isinstance(output, Viewer)):
@@ -801,14 +816,15 @@
     def from_command(
         cls,
         command: Union[str, RunCommand],
         *args: Any,
         ctx: Optional[invoke.context.Context] = None,
         runclass: Optional[invoke.Runner] = None,
         cbuffer: Optional[CBuffer] = None,
+        chunksize: int = 20000,
         **kwargs: Any,
     ) -> "Viewer":
         """
         Construct a `Viewer` from a command. This is the most convenient
         constructor for `Viewer` and should generally be preferred to
         `Viewer.__init__`.
 
@@ -821,25 +837,26 @@
                 if not specified.
             runclass: underlying Invoke `Runner` class for this `Viewer`. if
                 not specified, defaults to the default runclass of `command`,
                 if it has one, and the default `runclass` of `RunCommand` if it
                 does not.
             cbuffer: context buffer for `Viewer`. Creates a new `CBuffer` if
                 not specified.
+            chunksize: number of bytes to read at once from stdout/stderr.
             kwargs: additional keyword arguments for the executed shell
                 command. See `RunCommand.__call__()` for a detailed
                 description of behavior.
 
         Returns:
             a `Viewer` constructed from `command` .
         """
         if cbuffer is None:
             cbuffer = CBuffer()
         if not isinstance(command, RunCommand):
-            command = RunCommand(command, ctx, runclass)
+            command = RunCommand(command, ctx, runclass, chunksize=chunksize)
         # note that Viewers _only_ run commands asynchronously. use the wait
         # or wait_for_output methods if you want to block.
         base_kwargs = {
             "_bg": True,
             "_out": cbuffer.buffers["out"],
             "_err": cbuffer.buffers["err"],
         }
@@ -1106,14 +1123,16 @@
 
 
 def runv(*args, **kwargs):
     """run a command in a Viewer"""
     return Viewer.from_command(*args, **kwargs)
 
 
-def run(*args, **kwargs):
+def run(*args, **kwargs) -> Optional[str]:
     """run a command not in a Viewer"""
-    return RunCommand(*args, **kwargs)().stdout
+    # return value should be None iff caller passes _disown=True
+    if (cmd := RunCommand(*args, **kwargs)()) is not None:
+        return cmd.stdout
 
 
 Processlike = Union[Viewer, invoke.runners.Runner, invoke.runners.Result]
 """union of expected types for interfaces to processes."""
```

### Comparing `hostess-0.9.1/hostess/tests/test_caller.py` & `hostess-0.9.2/hostess/tests/test_caller.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/tests/test_directory.py` & `hostess-0.9.2/hostess/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/tests/test_monitors.py` & `hostess-0.9.2/hostess/tests/test_monitors.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/tests/test_profilers.py` & `hostess-0.9.2/hostess/tests/test_profilers.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/tests/test_subutils.py` & `hostess-0.9.2/hostess/tests/test_subutils.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/tests/test_utilities.py` & `hostess-0.9.2/hostess/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/tests/utilz.py` & `hostess-0.9.2/hostess/tests/utilz.py`

 * *Files identical despite different names*

### Comparing `hostess-0.9.1/hostess/utilities.py` & `hostess-0.9.2/hostess/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,26 +260,29 @@
     from cytoolz import curry as _curry
 
     return _curry(func, *args, **kwargs)
 
 
 class Aliased:
     """
-    generic wrapper for aliasing a class method. for instance, if you'd like a
-    library function to `append` to a list, but it's only willing to `write`:
+    generic wrapper for aliasing a class method.
 
-    ```
-    >>> import json
-    >>> my_list = []
-    >>> writeable_list = Aliased(my_list, ("write",), "append")
-    >>> json.dump([1, 2, 3], writeable_list)
-    >>> print(writeable_list)
-    Aliased: ('write',) -> append:
-    ['[1', ', 2', ', 3', ']']
-    ```
+    Examples:
+        If you'd like a library function to `append` to a list, but it's only
+        willing to `write`:
+
+        ```
+        >>> import json
+        >>> my_list = []
+        >>> writeable_list = Aliased(my_list, ("write",), "append")
+        >>> json.dump([1, 2, 3], writeable_list)
+        >>> print(writeable_list)
+        Aliased: ('write',) -> append:
+        ['[1', ', 2', ', 3', ']']
+        ```
     """
 
     def __init__(self, wrapped: Any, aliases: Sequence[str], referent: str):
         self.obj = wrapped
         self.method = referent
         self.aliases = aliases
         for alias in aliases:
```

### Comparing `hostess-0.9.1/hostess.egg-info/PKG-INFO` & `hostess-0.9.2/hostess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hostess
-Version: 0.9.1
+Version: 0.9.2
 Summary: intuitive admin library
 Author: Million Concepts
 Author-email: mstclair@millionconcepts.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hostess-0.9.1/hostess.egg-info/SOURCES.txt` & `hostess-0.9.2/hostess.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
 README.md
 setup.py
 hostess/__init__.py
+hostess/argscratch.py
 hostess/caller.py
 hostess/directory.py
 hostess/monitors.py
 hostess/profilers.py
 hostess/serverpool.py
 hostess/shortcuts.py
 hostess/ssh.py
 hostess/subutils.py
+hostess/tdscratch.py
 hostess/utilities.py
 hostess.egg-info/PKG-INFO
 hostess.egg-info/SOURCES.txt
 hostess.egg-info/dependency_links.txt
 hostess.egg-info/requires.txt
 hostess.egg-info/top_level.txt
 hostess/aws/__init__.py
@@ -26,16 +28,18 @@
 hostess/config/user_config.py
 hostess/station/__init__.py
 hostess/station/actors.py
 hostess/station/bases.py
 hostess/station/comm.py
 hostess/station/delegates.py
 hostess/station/handlers.py
+hostess/station/launchallscratch.py
 hostess/station/messages.py
 hostess/station/proto_utils.py
+hostess/station/shutscratch.py
 hostess/station/station.py
 hostess/station/talkie.py
 hostess/station/proto/__init__.py
 hostess/station/proto/station.proto
 hostess/station/proto/station_pb2.py
 hostess/station/situation/__init__.py
 hostess/station/situation/_textual_monkeypatch.py
```

### Comparing `hostess-0.9.1/setup.py` & `hostess-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="hostess",
-    version="0.9.1",
+    version="0.9.2",
     description="intuitive admin library",
     author="Million Concepts",
     author_email="mstclair@millionconcepts.com",
     packages=find_packages(),
     package_data={
         "": ["station/tests/test_data/*.*", "station/proto/*.*"]
     },
```

