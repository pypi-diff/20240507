# Comparing `tmp/mov_cli_youtube-1.2.0a5.tar.gz` & `tmp/mov_cli_youtube-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli_youtube-1.2.0a5.tar", last modified: Fri Apr 26 11:28:55 2024, max compression
+gzip compressed data, was "mov_cli_youtube-1.2.1.tar", last modified: Tue May  7 19:29:23 2024, max compression
```

## Comparing `mov_cli_youtube-1.2.0a5.tar` & `mov_cli_youtube-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 11:28:55.274617 mov_cli_youtube-1.2.0a5/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:22:29.000000 mov_cli_youtube-1.2.0a5/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-26 11:28:55.274617 mov_cli_youtube-1.2.0a5/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      674 2024-03-21 15:27:20.000000 mov_cli_youtube-1.2.0a5/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 11:28:55.271284 mov_cli_youtube-1.2.0a5/mov_cli_youtube/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      656 2024-04-26 11:28:36.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2460 2024-04-26 11:27:05.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube/pytube.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3765 2024-04-26 11:27:25.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube/yt_dlp.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 11:28:55.274617 mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-26 11:28:55.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      306 2024-04-26 11:28:55.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-26 11:28:55.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       97 2024-04-26 11:28:55.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       16 2024-04-26 11:28:55.000000 mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1295 2024-04-26 00:34:40.000000 mov_cli_youtube-1.2.0a5/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-26 11:28:55.274617 mov_cli_youtube-1.2.0a5/setup.cfg
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-07 19:29:23.633771 mov_cli_youtube-1.2.1/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1064 2024-05-07 19:19:11.000000 mov_cli_youtube-1.2.1/LICENSE
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2927 2024-05-07 19:29:23.633771 mov_cli_youtube-1.2.1/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      613 2024-05-07 19:19:11.000000 mov_cli_youtube-1.2.1/README.md
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-07 19:29:23.630438 mov_cli_youtube-1.2.1/mov_cli_youtube/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      650 2024-05-07 19:22:03.000000 mov_cli_youtube-1.2.1/mov_cli_youtube/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2462 2024-05-07 19:21:46.000000 mov_cli_youtube-1.2.1/mov_cli_youtube/pytube.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3765 2024-05-07 19:19:11.000000 mov_cli_youtube-1.2.1/mov_cli_youtube/yt_dlp.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-07 19:29:23.633771 mov_cli_youtube-1.2.1/mov_cli_youtube.egg-info/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2927 2024-05-07 19:29:23.000000 mov_cli_youtube-1.2.1/mov_cli_youtube.egg-info/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      306 2024-05-07 19:29:23.000000 mov_cli_youtube-1.2.1/mov_cli_youtube.egg-info/SOURCES.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-05-07 19:29:23.000000 mov_cli_youtube-1.2.1/mov_cli_youtube.egg-info/dependency_links.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       97 2024-05-07 19:29:23.000000 mov_cli_youtube-1.2.1/mov_cli_youtube.egg-info/requires.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       16 2024-05-07 19:29:23.000000 mov_cli_youtube-1.2.1/mov_cli_youtube.egg-info/top_level.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1295 2024-05-07 19:19:11.000000 mov_cli_youtube-1.2.1/pyproject.toml
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-05-07 19:29:23.633771 mov_cli_youtube-1.2.1/setup.cfg
```

### Comparing `mov_cli_youtube-1.2.0a5/LICENSE` & `mov_cli_youtube-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli_youtube-1.2.0a5/PKG-INFO` & `mov_cli_youtube-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.2.0a5
+Version: 1.2.1
 Summary: A mov-cli v4 plugin for watching youtube.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -52,17 +52,14 @@
   # mov-cli-youtube
   <sub>A mov-cli v4 plugin for watching youtube.</sub>
 
   <img src="https://github.com/mov-cli/mov-cli-youtube/assets/66202304/7b586dd2-2084-4d6c-b008-92e0539f5123">
 
 </div>
 
-> [!NOTE]
-> Currently work in progress, expect slow speeds.
-
 ## Installation 🛠️
 Here's how to install and add the plugin to mov-cli.
 
 1. Install the pip package.
 ```sh
 pip install mov-cli-youtube
 ```
```

### Comparing `mov_cli_youtube-1.2.0a5/README.md` & `mov_cli_youtube-1.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,14 @@
   # mov-cli-youtube
   <sub>A mov-cli v4 plugin for watching youtube.</sub>
 
   <img src="https://github.com/mov-cli/mov-cli-youtube/assets/66202304/7b586dd2-2084-4d6c-b008-92e0539f5123">
 
 </div>
 
-> [!NOTE]
-> Currently work in progress, expect slow speeds.
-
 ## Installation 🛠️
 Here's how to install and add the plugin to mov-cli.
 
 1. Install the pip package.
 ```sh
 pip install mov-cli-youtube
 ```
```

### Comparing `mov_cli_youtube-1.2.0a5/mov_cli_youtube/__init__.py` & `mov_cli_youtube-1.2.1/mov_cli_youtube/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,8 +18,8 @@
         "IOS.DEFAULT": PyTubeScraper, 
 
         "yt-dlp": YTDlpScraper, 
         "pytube": PyTubeScraper, 
     }
 }
 
-__version__ = "1.2.0alpha5"
+__version__ = "1.2.1"
```

### Comparing `mov_cli_youtube-1.2.0a5/mov_cli_youtube/pytube.py` & `mov_cli_youtube-1.2.1/mov_cli_youtube/pytube.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
     from mov_cli import Config
     from mov_cli.http_client import HTTPClient
     from mov_cli.scraper import ScraperOptionsT
 
 import os
 import sys
-from pytube import YouTube, Search
+from pytubefix import YouTube, Search
 
 from mov_cli.scraper import Scraper
 from mov_cli.utils import EpisodeSelector
 from mov_cli import Single, Metadata, MetadataType
 
 __all__ = ("PyTubeScraper",)
 
 class PyTubeScraper(Scraper):
     def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
         super().__init__(config, http_client, options)
 
     def search(self, query: str, limit: int = None) -> Generator[Metadata, Any, None]:
         search_query = Search(query)
-        search_results: List[YouTube] = search_query.results
+        search_results: List[YouTube] = search_query.videos
 
         max_videos = 20 if limit is None else limit
 
         # suppress pytube's stupid errors from getting to the console and ruining fzf output.
         sys.stderr = open(os.devnull, "w")
 
         for index, video in enumerate(search_results):
```

### Comparing `mov_cli_youtube-1.2.0a5/mov_cli_youtube/yt_dlp.py` & `mov_cli_youtube-1.2.1/mov_cli_youtube/yt_dlp.py`

 * *Files identical despite different names*

### Comparing `mov_cli_youtube-1.2.0a5/mov_cli_youtube.egg-info/PKG-INFO` & `mov_cli_youtube-1.2.1/mov_cli_youtube.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.2.0a5
+Version: 1.2.1
 Summary: A mov-cli v4 plugin for watching youtube.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -52,17 +52,14 @@
   # mov-cli-youtube
   <sub>A mov-cli v4 plugin for watching youtube.</sub>
 
   <img src="https://github.com/mov-cli/mov-cli-youtube/assets/66202304/7b586dd2-2084-4d6c-b008-92e0539f5123">
 
 </div>
 
-> [!NOTE]
-> Currently work in progress, expect slow speeds.
-
 ## Installation 🛠️
 Here's how to install and add the plugin to mov-cli.
 
 1. Install the pip package.
 ```sh
 pip install mov-cli-youtube
 ```
```

### Comparing `mov_cli_youtube-1.2.0a5/pyproject.toml` & `mov_cli_youtube-1.2.1/pyproject.toml`

 * *Files identical despite different names*

