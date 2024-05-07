# Comparing `tmp/hustmirror_cli-1.1.3.tar.gz` & `tmp/hustmirror_cli-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hustmirror_cli-1.1.3.tar", last modified: Sun Apr 28 07:19:02 2024, max compression
+gzip compressed data, was "hustmirror_cli-1.1.4.tar", last modified: Tue May  7 12:22:22 2024, max compression
```

## Comparing `hustmirror_cli-1.1.3.tar` & `hustmirror_cli-1.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2024-04-28 07:18:48.563934 hustmirror_cli-1.1.3/LICENSE
--rw-r--r--   0        0        0       17 2024-04-28 07:18:48.563934 hustmirror_cli-1.1.3/README.md
--rw-r--r--   0        0        0      470 2024-04-28 07:19:02.827945 hustmirror_cli-1.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-28 07:18:48.563934 hustmirror_cli-1.1.3/src/hustmirror_cli/__init__.py
--rw-r--r--   0        0        0      240 1970-01-01 00:00:00.000000 hustmirror_cli-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-07 12:22:09.154181 hustmirror_cli-1.1.4/LICENSE
+-rw-r--r--   0        0        0       17 2024-05-07 12:22:09.154181 hustmirror_cli-1.1.4/README.md
+-rw-r--r--   0        0        0      470 2024-05-07 12:22:22.954178 hustmirror_cli-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 12:22:09.154181 hustmirror_cli-1.1.4/src/hustmirror_cli/__init__.py
+-rw-r--r--   0        0        0      240 1970-01-01 00:00:00.000000 hustmirror_cli-1.1.4/PKG-INFO
```

### Comparing `hustmirror_cli-1.1.3/LICENSE` & `hustmirror_cli-1.1.4/LICENSE`

 * *Files identical despite different names*

