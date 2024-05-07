# Comparing `tmp/sparrowEncryptionDecryption-0.1.tar.gz` & `tmp/sparrowEncryptionDecryption-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparrowEncryptionDecryption-0.1.tar", last modified: Mon Apr 15 06:58:38 2024, max compression
+gzip compressed data, was "sparrowEncryptionDecryption-0.1.1.tar", last modified: Tue May  7 03:03:41 2024, max compression
```

## Comparing `sparrowEncryptionDecryption-0.1.tar` & `sparrowEncryptionDecryption-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 06:58:38.696931 sparrowEncryptionDecryption-0.1/
--rw-rw-rw-   0        0        0      144 2024-04-15 06:58:38.695727 sparrowEncryptionDecryption-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 06:58:38.697728 sparrowEncryptionDecryption-0.1/setup.cfg
--rw-rw-rw-   0        0        0      265 2024-04-15 06:58:18.000000 sparrowEncryptionDecryption-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 06:58:38.686855 sparrowEncryptionDecryption-0.1/sparrowEncryptionDecryption/
--rw-rw-rw-   0        0        0      314 2024-04-15 06:56:58.000000 sparrowEncryptionDecryption-0.1/sparrowEncryptionDecryption/__init__.py
--rw-rw-rw-   0        0        0     9231 2024-04-12 08:50:44.000000 sparrowEncryptionDecryption-0.1/sparrowEncryptionDecryption/config.py
--rw-rw-rw-   0        0        0     7251 2024-04-15 06:56:58.000000 sparrowEncryptionDecryption-0.1/sparrowEncryptionDecryption/encryption_decryption.py
-drwxrwxrwx   0        0        0        0 2024-04-15 06:58:38.693808 sparrowEncryptionDecryption-0.1/sparrowEncryptionDecryption.egg-info/
--rw-rw-rw-   0        0        0      144 2024-04-15 06:58:38.000000 sparrowEncryptionDecryption-0.1/sparrowEncryptionDecryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-15 06:58:38.000000 sparrowEncryptionDecryption-0.1/sparrowEncryptionDecryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 06:58:38.000000 sparrowEncryptionDecryption-0.1/sparrowEncryptionDecryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-15 06:58:38.000000 sparrowEncryptionDecryption-0.1/sparrowEncryptionDecryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 03:03:41.628660 sparrowEncryptionDecryption-0.1.1/
+-rw-rw-rw-   0        0        0      146 2024-05-07 03:03:41.627324 sparrowEncryptionDecryption-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-07 03:03:41.629324 sparrowEncryptionDecryption-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      267 2024-05-07 03:03:26.000000 sparrowEncryptionDecryption-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:03:41.610363 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption/
+-rw-rw-rw-   0        0        0      217 2024-05-07 02:13:28.000000 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption/__init__.py
+-rw-rw-rw-   0        0        0     1013 2024-05-07 02:57:30.000000 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption/encryption_decryption.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:03:41.622323 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption/function/
+-rw-rw-rw-   0        0        0      158 2024-05-07 02:02:00.000000 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption/function/__init__.py
+-rw-rw-rw-   0        0        0     9114 2024-05-07 02:13:09.000000 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption/function/config.py
+-rw-rw-rw-   0        0        0     4636 2024-05-07 03:01:58.000000 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption/function/decryption.py
+-rw-rw-rw-   0        0        0     3760 2024-05-07 02:53:20.000000 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption/function/encryption.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:03:41.626331 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption/tools/
+-rw-rw-rw-   0        0        0     1162 2024-05-07 02:53:20.000000 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption/tools/__init__.py
+-rw-rw-rw-   0        0        0     2694 2024-05-07 02:50:31.000000 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption/tools/error.py
+-rw-rw-rw-   0        0        0     2821 2024-05-07 01:49:43.000000 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption/tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:03:41.617042 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption.egg-info/
+-rw-rw-rw-   0        0        0      146 2024-05-07 03:03:41.000000 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      635 2024-05-07 03:03:41.000000 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 03:03:41.000000 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-07 03:03:41.000000 sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption.egg-info/top_level.txt
```

### Comparing `sparrowEncryptionDecryption-0.1/sparrowEncryptionDecryption/config.py` & `sparrowEncryptionDecryption-0.1.1/sparrowEncryptionDecryption/function/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,14 +354,10 @@
             "&+": "プ",
             "&=": "ペ",
             "*_": "ポ",
             "*-": "ガ",
             "*=": "ギ",
             "*+": "グ",
         }
-# 秘钥过期提示
-OUT_TIME = "解密已过期，无法解密"
-# 秘钥错误提示
-KEY_ERROR = "秘钥错误"
```

