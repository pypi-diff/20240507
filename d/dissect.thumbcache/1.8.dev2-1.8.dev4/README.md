# Comparing `tmp/dissect.thumbcache-1.8.dev2.tar.gz` & `tmp/dissect.thumbcache-1.8.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.thumbcache-1.8.dev2.tar", last modified: Thu Mar 21 10:17:19 2024, max compression
+gzip compressed data, was "dissect.thumbcache-1.8.dev4.tar", last modified: Thu Apr 11 11:58:20 2024, max compression
```

## Comparing `dissect.thumbcache-1.8.dev2.tar` & `dissect.thumbcache-1.8.dev4.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:19.561108 dissect.thumbcache-1.8.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-21 10:17:19.561108 dissect.thumbcache-1.8.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:19.521108 dissect.thumbcache-1.8.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:19.525108 dissect.thumbcache-1.8.dev2/dissect/thumbcache/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/dissect/thumbcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/dissect/thumbcache/c_thumbcache.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/dissect/thumbcache/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/dissect/thumbcache/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/dissect/thumbcache/thumbcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/dissect/thumbcache/thumbcache_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:19.525108 dissect.thumbcache-1.8.dev2/dissect/thumbcache/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/dissect/thumbcache/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/dissect/thumbcache/tools/extract_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/dissect/thumbcache/tools/extract_with_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/dissect/thumbcache/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/dissect/thumbcache/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:19.561108 dissect.thumbcache-1.8.dev2/dissect.thumbcache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-21 10:17:19.000000 dissect.thumbcache-1.8.dev2/dissect.thumbcache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-03-21 10:17:19.000000 dissect.thumbcache-1.8.dev2/dissect.thumbcache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:17:19.000000 dissect.thumbcache-1.8.dev2/dissect.thumbcache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-21 10:17:19.000000 dissect.thumbcache-1.8.dev2/dissect.thumbcache.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-21 10:17:19.000000 dissect.thumbcache-1.8.dev2/dissect.thumbcache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 10:17:19.000000 dissect.thumbcache-1.8.dev2/dissect.thumbcache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-21 10:17:13.000000 dissect.thumbcache-1.8.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:17:19.561108 dissect.thumbcache-1.8.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:19.529108 dissect.thumbcache-1.8.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:19.521108 dissect.thumbcache-1.8.dev2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:19.537108 dissect.thumbcache-1.8.dev2/tests/data/windows_10/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_1280.db
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_16.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_1920.db
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_2560.db
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_48.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_768.db
--rw-r--r--   0 runner    (1001) docker     (127)  3145728 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_custom_stream.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_exif.db
--rw-r--r--   0 runner    (1001) docker     (127)    14688 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_sr.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_wide.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_wide_alternate.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:19.545108 dissect.thumbcache-1.8.dev2/tests/data/windows_11/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_1280.db
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_16.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_1920.db
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_2560.db
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_48.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_768.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_custom_stream.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_exif.db
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_sr.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_wide.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_wide_alternate.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:19.549108 dissect.thumbcache-1.8.dev2/tests/data/windows_7/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_7/thumbcache_1024.db
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_7/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_7/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_7/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_7/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_7/thumbcache_sr.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:19.553108 dissect.thumbcache-1.8.dev2/tests/data/windows_81/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_1024.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_16.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_1600.db
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_48.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_exif.db
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_sr.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_wide.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_wide_alternate.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:19.561108 dissect.thumbcache-1.8.dev2/tests/data/windows_vista/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_vista/thumbcache_1024.db
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_vista/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_vista/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_vista/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_vista/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/data/windows_vista/thumbcache_sr.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:19.561108 dissect.thumbcache-1.8.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/test_thumbcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tests/test_thumbcachefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-21 10:17:06.000000 dissect.thumbcache-1.8.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:20.395298 dissect.thumbcache-1.8.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-11 11:58:20.395298 dissect.thumbcache-1.8.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:20.355298 dissect.thumbcache-1.8.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:20.359298 dissect.thumbcache-1.8.dev4/dissect/thumbcache/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/dissect/thumbcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/dissect/thumbcache/c_thumbcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/dissect/thumbcache/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/dissect/thumbcache/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/dissect/thumbcache/thumbcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/dissect/thumbcache/thumbcache_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:20.363298 dissect.thumbcache-1.8.dev4/dissect/thumbcache/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/dissect/thumbcache/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/dissect/thumbcache/tools/extract_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/dissect/thumbcache/tools/extract_with_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/dissect/thumbcache/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/dissect/thumbcache/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:20.395298 dissect.thumbcache-1.8.dev4/dissect.thumbcache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-11 11:58:20.000000 dissect.thumbcache-1.8.dev4/dissect.thumbcache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-11 11:58:20.000000 dissect.thumbcache-1.8.dev4/dissect.thumbcache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:58:20.000000 dissect.thumbcache-1.8.dev4/dissect.thumbcache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-11 11:58:20.000000 dissect.thumbcache-1.8.dev4/dissect.thumbcache.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 11:58:20.000000 dissect.thumbcache-1.8.dev4/dissect.thumbcache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 11:58:20.000000 dissect.thumbcache-1.8.dev4/dissect.thumbcache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-11 11:58:15.000000 dissect.thumbcache-1.8.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:58:20.395298 dissect.thumbcache-1.8.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:20.363298 dissect.thumbcache-1.8.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:20.355298 dissect.thumbcache-1.8.dev4/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:20.371298 dissect.thumbcache-1.8.dev4/tests/data/windows_10/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_1280.db
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_16.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_1920.db
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_2560.db
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_48.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_768.db
+-rw-r--r--   0 runner    (1001) docker     (127)  3145728 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_custom_stream.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_exif.db
+-rw-r--r--   0 runner    (1001) docker     (127)    14688 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_sr.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_wide.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_wide_alternate.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:20.379298 dissect.thumbcache-1.8.dev4/tests/data/windows_11/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_1280.db
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_16.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_1920.db
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_2560.db
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_48.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_768.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_custom_stream.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_exif.db
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_sr.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_wide.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_wide_alternate.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:20.383298 dissect.thumbcache-1.8.dev4/tests/data/windows_7/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_7/thumbcache_1024.db
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_7/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_7/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_7/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_7/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_7/thumbcache_sr.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:20.387298 dissect.thumbcache-1.8.dev4/tests/data/windows_81/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_1024.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_16.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_1600.db
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_48.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_exif.db
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_sr.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_wide.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_wide_alternate.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:20.395298 dissect.thumbcache-1.8.dev4/tests/data/windows_vista/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_vista/thumbcache_1024.db
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_vista/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_vista/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_vista/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_vista/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 11:58:09.000000 dissect.thumbcache-1.8.dev4/tests/data/windows_vista/thumbcache_sr.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:58:20.395298 dissect.thumbcache-1.8.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/tests/test_thumbcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/tests/test_thumbcachefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-11 11:58:08.000000 dissect.thumbcache-1.8.dev4/tox.ini
```

### Comparing `dissect.thumbcache-1.8.dev2/LICENSE` & `dissect.thumbcache-1.8.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/PKG-INFO` & `dissect.thumbcache-1.8.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.thumbcache
-Version: 1.8.dev2
+Version: 1.8.dev4
 Summary: A Dissect module implementing parsers for the thumbcache of Windows systems.
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.thumbcache
 Project-URL: repository, https://github.com/fox-it/dissect.thumbcache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.thumbcache-1.8.dev2/README.md` & `dissect.thumbcache-1.8.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/dissect/thumbcache/c_thumbcache.py` & `dissect.thumbcache-1.8.dev4/dissect/thumbcache/c_thumbcache.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/dissect/thumbcache/index.py` & `dissect.thumbcache-1.8.dev4/dissect/thumbcache/index.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/dissect/thumbcache/thumbcache.py` & `dissect.thumbcache-1.8.dev4/dissect/thumbcache/thumbcache.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/dissect/thumbcache/thumbcache_file.py` & `dissect.thumbcache-1.8.dev4/dissect/thumbcache/thumbcache_file.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/dissect/thumbcache/tools/extract_images.py` & `dissect.thumbcache-1.8.dev4/dissect/thumbcache/tools/extract_images.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/dissect/thumbcache/tools/extract_with_index.py` & `dissect.thumbcache-1.8.dev4/dissect/thumbcache/tools/extract_with_index.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/dissect/thumbcache/tools/utils.py` & `dissect.thumbcache-1.8.dev4/dissect/thumbcache/tools/utils.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/dissect.thumbcache.egg-info/PKG-INFO` & `dissect.thumbcache-1.8.dev4/dissect.thumbcache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.thumbcache
-Version: 1.8.dev2
+Version: 1.8.dev4
 Summary: A Dissect module implementing parsers for the thumbcache of Windows systems.
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.thumbcache
 Project-URL: repository, https://github.com/fox-it/dissect.thumbcache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.thumbcache-1.8.dev2/dissect.thumbcache.egg-info/SOURCES.txt` & `dissect.thumbcache-1.8.dev4/dissect.thumbcache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/pyproject.toml` & `dissect.thumbcache-1.8.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_16.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_16.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_256.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_32.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_96.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_96.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_10/thumbcache_idx.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_10/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_16.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_16.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_256.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_32.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_48.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_48.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_11/thumbcache_idx.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_11/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_7/thumbcache_256.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_7/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_7/thumbcache_idx.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_7/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_256.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_32.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_81/thumbcache_idx.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_81/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_vista/thumbcache_256.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_vista/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_vista/thumbcache_32.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_vista/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_vista/thumbcache_96.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_vista/thumbcache_96.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/data/windows_vista/thumbcache_idx.db` & `dissect.thumbcache-1.8.dev4/tests/data/windows_vista/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/docs/Makefile` & `dissect.thumbcache-1.8.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/docs/conf.py` & `dissect.thumbcache-1.8.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/test_index.py` & `dissect.thumbcache-1.8.dev4/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/test_thumbcache.py` & `dissect.thumbcache-1.8.dev4/tests/test_thumbcache.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tests/test_thumbcachefile.py` & `dissect.thumbcache-1.8.dev4/tests/test_thumbcachefile.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.8.dev2/tox.ini` & `dissect.thumbcache-1.8.dev4/tox.ini`

 * *Files identical despite different names*

