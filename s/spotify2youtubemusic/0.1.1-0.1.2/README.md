# Comparing `tmp/spotify2youtubemusic-0.1.1.tar.gz` & `tmp/spotify2youtubemusic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify2youtubemusic-0.1.1.tar", last modified: Tue May  7 06:30:04 2024, max compression
+gzip compressed data, was "spotify2youtubemusic-0.1.2.tar", last modified: Tue May  7 06:38:38 2024, max compression
```

## Comparing `spotify2youtubemusic-0.1.1.tar` & `spotify2youtubemusic-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 06:30:04.933369 spotify2youtubemusic-0.1.1/
--rw-rw-rw-   0        0        0       92 2024-05-07 06:30:04.926814 spotify2youtubemusic-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-07 06:30:04.933920 spotify2youtubemusic-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      547 2024-05-07 06:29:48.000000 spotify2youtubemusic-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:30:04.926814 spotify2youtubemusic-0.1.1/spotify2youtubemusic/
--rw-rw-rw-   0        0        0      380 2024-05-07 06:29:44.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic/download.py
-drwxrwxrwx   0        0        0        0 2024-05-07 06:30:04.926814 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/
--rw-rw-rw-   0        0        0       92 2024-05-07 06:30:04.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-05-07 06:30:04.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 06:30:04.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-07 06:30:04.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2024-05-07 06:30:04.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-07 06:30:04.000000 spotify2youtubemusic-0.1.1/spotify2youtubemusic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 06:38:38.474146 spotify2youtubemusic-0.1.2/
+-rw-rw-rw-   0        0        0       92 2024-05-07 06:38:38.474146 spotify2youtubemusic-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-07 06:38:38.474146 spotify2youtubemusic-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      700 2024-05-07 06:38:03.000000 spotify2youtubemusic-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:38:38.458500 spotify2youtubemusic-0.1.2/spotify2youtubemusic/
+-rw-rw-rw-   0        0        0      380 2024-05-07 06:37:07.000000 spotify2youtubemusic-0.1.2/spotify2youtubemusic/download.py
+-rw-rw-rw-   0        0        0      248 2024-05-07 06:36:56.000000 spotify2youtubemusic-0.1.2/spotify2youtubemusic/send.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:38:38.458500 spotify2youtubemusic-0.1.2/spotify2youtubemusic.egg-info/
+-rw-rw-rw-   0        0        0       92 2024-05-07 06:38:38.000000 spotify2youtubemusic-0.1.2/spotify2youtubemusic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-05-07 06:38:38.000000 spotify2youtubemusic-0.1.2/spotify2youtubemusic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 06:38:38.000000 spotify2youtubemusic-0.1.2/spotify2youtubemusic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-07 06:38:38.000000 spotify2youtubemusic-0.1.2/spotify2youtubemusic.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2024-05-07 06:38:38.000000 spotify2youtubemusic-0.1.2/spotify2youtubemusic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-07 06:38:38.000000 spotify2youtubemusic-0.1.2/spotify2youtubemusic.egg-info/top_level.txt
```

