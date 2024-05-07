# Comparing `tmp/HdRezkaApi-7.0.1.tar.gz` & `tmp/HdRezkaApi-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HdRezkaApi-7.0.1.tar", last modified: Mon May  6 16:16:09 2024, max compression
+gzip compressed data, was "HdRezkaApi-7.1.0.tar", last modified: Tue May  7 09:08:47 2024, max compression
```

## Comparing `HdRezkaApi-7.0.1.tar` & `HdRezkaApi-7.1.0.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 16:16:09.069477 HdRezkaApi-7.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-06 16:16:09.012651 HdRezkaApi-7.0.1/HdRezkaApi/
--rw-rw-rw-   0        0        0     9119 2024-02-07 21:31:39.000000 HdRezkaApi-7.0.1/HdRezkaApi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:16:09.066971 HdRezkaApi-7.0.1/HdRezkaApi/utils/
-drwxrwxrwx   0        0        0        0 2024-05-06 16:16:09.069477 HdRezkaApi-7.0.1/HdRezkaApi/utils/__pycache__/
--rw-rw-rw-   0        0        0     5034 2024-02-07 21:20:07.000000 HdRezkaApi-7.0.1/HdRezkaApi/utils/__pycache__/stream.cpython-311.pyc
--rw-rw-rw-   0        0        0     3806 2024-02-07 21:04:17.000000 HdRezkaApi-7.0.1/HdRezkaApi/utils/__pycache__/types.cpython-311.pyc
--rw-rw-rw-   0        0        0     2004 2024-02-07 21:17:28.000000 HdRezkaApi-7.0.1/HdRezkaApi/utils/stream.py
--rw-rw-rw-   0        0        0     1039 2023-08-31 12:26:52.000000 HdRezkaApi-7.0.1/HdRezkaApi/utils/types.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:16:09.046401 HdRezkaApi-7.0.1/HdRezkaApi.egg-info/
--rw-rw-rw-   0        0        0     4361 2024-05-06 16:16:08.000000 HdRezkaApi-7.0.1/HdRezkaApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-05-06 16:16:08.000000 HdRezkaApi-7.0.1/HdRezkaApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 16:16:08.000000 HdRezkaApi-7.0.1/HdRezkaApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-06 16:16:08.000000 HdRezkaApi-7.0.1/HdRezkaApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-06 16:16:08.000000 HdRezkaApi-7.0.1/HdRezkaApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       30 2024-05-06 16:16:07.000000 HdRezkaApi-7.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4361 2024-05-06 16:16:09.070803 HdRezkaApi-7.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3829 2024-05-06 16:14:47.000000 HdRezkaApi-7.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 16:16:09.071904 HdRezkaApi-7.0.1/setup.cfg
--rw-rw-rw-   0        0        0      683 2024-05-06 16:16:07.000000 HdRezkaApi-7.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:08:47.175967 HdRezkaApi-7.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-07 09:08:47.145590 HdRezkaApi-7.1.0/HdRezkaApi/
+-rw-rw-rw-   0        0        0     9226 2024-05-07 09:00:33.000000 HdRezkaApi-7.1.0/HdRezkaApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:08:47.175967 HdRezkaApi-7.1.0/HdRezkaApi/utils/
+-rw-rw-rw-   0        0        0     2004 2024-02-07 21:17:28.000000 HdRezkaApi-7.1.0/HdRezkaApi/utils/stream.py
+-rw-rw-rw-   0        0        0     1039 2023-08-31 12:26:52.000000 HdRezkaApi-7.1.0/HdRezkaApi/utils/types.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:08:47.160210 HdRezkaApi-7.1.0/HdRezkaApi.egg-info/
+-rw-rw-rw-   0        0        0     4361 2024-05-07 09:08:47.000000 HdRezkaApi-7.1.0/HdRezkaApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-07 09:08:47.000000 HdRezkaApi-7.1.0/HdRezkaApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 09:08:47.000000 HdRezkaApi-7.1.0/HdRezkaApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 09:08:47.000000 HdRezkaApi-7.1.0/HdRezkaApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-07 09:08:47.000000 HdRezkaApi-7.1.0/HdRezkaApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       30 2024-05-07 09:08:46.000000 HdRezkaApi-7.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4361 2024-05-07 09:08:47.177485 HdRezkaApi-7.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3829 2024-05-07 09:04:13.000000 HdRezkaApi-7.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 09:08:47.177485 HdRezkaApi-7.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      683 2024-05-07 09:08:46.000000 HdRezkaApi-7.1.0/setup.py
```

### Comparing `HdRezkaApi-7.0.1/HdRezkaApi/__init__.py` & `HdRezkaApi-7.1.0/HdRezkaApi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import requests
 from bs4 import BeautifulSoup
 import base64
 from itertools import product
 from functools import cached_property
+from urllib.parse import urlparse
 import time
 
 try:
 	from utils.types import (HdRezkaTVSeries, HdRezkaMovie, HdRezkaRating)
 	from utils.stream import HdRezkaStream
 except ImportError:
 	from .utils.types import (HdRezkaTVSeries, HdRezkaMovie, HdRezkaRating)
 	from .utils.stream import HdRezkaStream
 
 class BeautifulSoupCustom(BeautifulSoup):
 	def __repr__(self):
 		return "<HTMLDocument>"
 
 class HdRezkaApi():
-	__version__ = "7.0.0"
+	__version__ = "7.1.0"
 	def __init__(self, url, proxy={}, headers={}):
 		self.url = url.split(".html")[0] + ".html"
+		uri = urlparse(self.url)
+		self.origin = f'{uri.scheme}://{uri.netloc}'
 		self.proxy = proxy
 		self.HEADERS = {
 			'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.138 Safari/537.36',
 			**headers
 		}
 
 	@cached_property
@@ -148,27 +151,27 @@
 		arr = {}
 		for i in self.translators:
 			js = {
 				"id": self.id,
 				"translator_id": self.translators[i],
 				"action": "get_episodes"
 			}
-			r = requests.post("https://rezka.ag/ajax/get_cdn_series/", data=js, headers=self.HEADERS, proxies=self.proxy)
+			r = requests.post(f"{self.origin}/ajax/get_cdn_series/", data=js, headers=self.HEADERS, proxies=self.proxy)
 			response = r.json()
 			if response['success']:
 				seasons, episodes = self.getEpisodes(response['seasons'], response['episodes'])
 				arr[i] = {
 					"translator_id": self.translators[i],
 					"seasons": seasons, "episodes": episodes
 				}
 		return arr
 
 	def getStream(self, season=None, episode=None, translation=None, index=0):
 		def makeRequest(data):
-			r = requests.post("https://rezka.ag/ajax/get_cdn_series/", data=data, headers=self.HEADERS, proxies=self.proxy)
+			r = requests.post(f"{self.origin}/ajax/get_cdn_series/", data=data, headers=self.HEADERS, proxies=self.proxy)
 			r = r.json()
 			if r['success']:
 				arr = self.clearTrash(r['url']).split(",")
 				stream = HdRezkaStream( season=season, episode=episode,
 										name=self.name, translator_id=data['translator_id'],
 										subtitles={'data':  r['subtitle'], 'codes': r['subtitle_lns']}
 									  )
```

### Comparing `HdRezkaApi-7.0.1/HdRezkaApi/utils/stream.py` & `HdRezkaApi-7.1.0/HdRezkaApi/utils/stream.py`

 * *Files identical despite different names*

### Comparing `HdRezkaApi-7.0.1/HdRezkaApi/utils/types.py` & `HdRezkaApi-7.1.0/HdRezkaApi/utils/types.py`

 * *Files identical despite different names*

### Comparing `HdRezkaApi-7.0.1/HdRezkaApi.egg-info/PKG-INFO` & `HdRezkaApi-7.1.0/HdRezkaApi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: HdRezkaApi
-Version: 7.0.1
+Version: 7.1.0
 Home-page: https://github.com/SuperZombi/HdRezkaApi
 Author: Super_Zombi
 Author-email: super.zombi.yt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # HdRezkaApi
 
-<img src="https://shields.io/badge/version-v7.0-blue">
+<img src="https://shields.io/badge/version-v7.1-blue">
 
 ### Install:
 ```
 pip install HdRezkaApi
 ```
 
 ### Usage:
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: HdRezkaApi Version: 7.0.1 Home-page: https://
+Metadata-Version: 2.1 Name: HdRezkaApi Version: 7.1.0 Home-page: https://
 github.com/SuperZombi/HdRezkaApi Author: Super_Zombi Author-email:
 super.zombi.yt@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown # HdRezkaApi [https://shields.io/badge/version-v7.0-blue]### Install:
+markdown # HdRezkaApi [https://shields.io/badge/version-v7.1-blue]### Install:
 ``` pip install HdRezkaApi ``` ### Usage: ```python from HdRezkaApi import *
 url = "https://hdrezka.ag/ __YOUR_URL__ .html" rezka = HdRezkaApi(url) print
 (rezka.name) print(rezka.thumbnail) print( rezka.rating.value ) print
 ( rezka.rating.votes ) print( rezka.translators ) print( rezka.otherParts )
 print( rezka.seriesInfo ) print(rezka.type) print(rezka.type == HdRezkaTVSeries
 == HdRezkaTVSeries() == "tv_series") print( rezka.getStream()('720p') ) # if
 movie print( rezka.getStream('1', '1')('720p') ) print( dict
```

### Comparing `HdRezkaApi-7.0.1/PKG-INFO` & `HdRezkaApi-7.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: HdRezkaApi
-Version: 7.0.1
+Version: 7.1.0
 Home-page: https://github.com/SuperZombi/HdRezkaApi
 Author: Super_Zombi
 Author-email: super.zombi.yt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # HdRezkaApi
 
-<img src="https://shields.io/badge/version-v7.0-blue">
+<img src="https://shields.io/badge/version-v7.1-blue">
 
 ### Install:
 ```
 pip install HdRezkaApi
 ```
 
 ### Usage:
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: HdRezkaApi Version: 7.0.1 Home-page: https://
+Metadata-Version: 2.1 Name: HdRezkaApi Version: 7.1.0 Home-page: https://
 github.com/SuperZombi/HdRezkaApi Author: Super_Zombi Author-email:
 super.zombi.yt@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown # HdRezkaApi [https://shields.io/badge/version-v7.0-blue]### Install:
+markdown # HdRezkaApi [https://shields.io/badge/version-v7.1-blue]### Install:
 ``` pip install HdRezkaApi ``` ### Usage: ```python from HdRezkaApi import *
 url = "https://hdrezka.ag/ __YOUR_URL__ .html" rezka = HdRezkaApi(url) print
 (rezka.name) print(rezka.thumbnail) print( rezka.rating.value ) print
 ( rezka.rating.votes ) print( rezka.translators ) print( rezka.otherParts )
 print( rezka.seriesInfo ) print(rezka.type) print(rezka.type == HdRezkaTVSeries
 == HdRezkaTVSeries() == "tv_series") print( rezka.getStream()('720p') ) # if
 movie print( rezka.getStream('1', '1')('720p') ) print( dict
```

### Comparing `HdRezkaApi-7.0.1/README.md` & `HdRezkaApi-7.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HdRezkaApi
 
-<img src="https://shields.io/badge/version-v7.0-blue">
+<img src="https://shields.io/badge/version-v7.1-blue">
 
 ### Install:
 ```
 pip install HdRezkaApi
 ```
 
 ### Usage:
```

### Comparing `HdRezkaApi-7.0.1/setup.py` & `HdRezkaApi-7.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open(r'C:\Users\rost\Downloads\README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='HdRezkaApi',
-	version='7.0.1',
+	version='7.1.0',
 	author='Super_Zombi',
 	author_email='super.zombi.yt@gmail.com',
 	description='',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://github.com/SuperZombi/HdRezkaApi',
 	packages=['HdRezkaApi'],
```

