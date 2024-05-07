# Comparing `tmp/amino.light.py-0.1.9.tar.gz` & `tmp/amino.light.py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.light.py-0.1.9.tar", last modified: Sat May  4 09:48:32 2024, max compression
+gzip compressed data, was "amino.light.py-0.2.0.tar", last modified: Tue May  7 04:49:05 2024, max compression
```

## Comparing `amino.light.py-0.1.9.tar` & `amino.light.py-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 09:48:32.050848 amino.light.py-0.1.9/
-drwxrwxrwx   0        0        0        0 2024-05-04 09:48:31.913033 amino.light.py-0.1.9/AminoLightPy/
--rw-rw-rw-   0        0        0      297 2024-05-04 09:47:40.000000 amino.light.py-0.1.9/AminoLightPy/__init__.py
--rw-rw-rw-   0        0        0    14819 2024-04-24 14:56:57.000000 amino.light.py-0.1.9/AminoLightPy/acm.py
--rw-rw-rw-   0        0        0    16533 2024-04-28 15:38:37.000000 amino.light.py-0.1.9/AminoLightPy/amino_socket.py
--rw-rw-rw-   0        0        0    74754 2024-04-30 14:32:26.000000 amino.light.py-0.1.9/AminoLightPy/client.py
--rw-rw-rw-   0        0        0     2704 2024-04-24 14:56:35.000000 amino.light.py-0.1.9/AminoLightPy/constants.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:48:31.920015 amino.light.py-0.1.9/AminoLightPy/lib/
--rw-rw-rw-   0        0        0        0 2024-04-19 03:59:31.000000 amino.light.py-0.1.9/AminoLightPy/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:48:31.932847 amino.light.py-0.1.9/AminoLightPy/lib/util/
--rw-rw-rw-   0        0        0       75 2024-04-19 03:26:32.000000 amino.light.py-0.1.9/AminoLightPy/lib/util/__init__.py
--rw-rw-rw-   0        0        0    32832 2024-04-24 14:57:25.000000 amino.light.py-0.1.9/AminoLightPy/lib/util/exceptions.py
--rw-rw-rw-   0        0        0     1846 2024-04-24 14:57:20.000000 amino.light.py-0.1.9/AminoLightPy/lib/util/helpers.py
--rw-rw-rw-   0        0        0    94997 2024-04-28 16:41:32.000000 amino.light.py-0.1.9/AminoLightPy/lib/util/objects.py
--rw-rw-rw-   0        0        0      894 2024-04-30 14:33:17.000000 amino.light.py-0.1.9/AminoLightPy/managers.py
--rw-rw-rw-   0        0        0    67523 2024-04-23 09:48:37.000000 amino.light.py-0.1.9/AminoLightPy/sub_client.py
--rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     3630 2024-05-04 09:48:32.049847 amino.light.py-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2834 2024-04-19 02:52:28.000000 amino.light.py-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 09:48:32.047857 amino.light.py-0.1.9/amino.light.py.egg-info/
--rw-rw-rw-   0        0        0     3630 2024-05-04 09:48:30.000000 amino.light.py-0.1.9/amino.light.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      565 2024-05-04 09:48:30.000000 amino.light.py-0.1.9/amino.light.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 09:48:30.000000 amino.light.py-0.1.9/amino.light.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-04 09:48:30.000000 amino.light.py-0.1.9/amino.light.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-04 09:48:30.000000 amino.light.py-0.1.9/amino.light.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 09:48:32.053849 amino.light.py-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1298 2024-05-04 09:47:20.000000 amino.light.py-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 04:49:05.537038 amino.light.py-0.2.0/
+drwxrwxrwx   0        0        0        0 2024-05-07 04:49:05.505969 amino.light.py-0.2.0/AminoLightPy/
+-rw-rw-rw-   0        0        0      297 2024-05-04 09:47:40.000000 amino.light.py-0.2.0/AminoLightPy/__init__.py
+-rw-rw-rw-   0        0        0    17290 2024-05-07 00:05:13.000000 amino.light.py-0.2.0/AminoLightPy/acm.py
+-rw-rw-rw-   0        0        0    16534 2024-05-06 23:33:52.000000 amino.light.py-0.2.0/AminoLightPy/amino_socket.py
+-rw-rw-rw-   0        0        0    74712 2024-05-06 23:01:47.000000 amino.light.py-0.2.0/AminoLightPy/client.py
+-rw-rw-rw-   0        0        0     2780 2024-05-07 00:09:32.000000 amino.light.py-0.2.0/AminoLightPy/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-07 04:49:05.505969 amino.light.py-0.2.0/AminoLightPy/lib/
+-rw-rw-rw-   0        0        0        0 2024-04-19 03:59:31.000000 amino.light.py-0.2.0/AminoLightPy/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 04:49:05.505969 amino.light.py-0.2.0/AminoLightPy/lib/util/
+-rw-rw-rw-   0        0        0       75 2024-04-19 03:26:32.000000 amino.light.py-0.2.0/AminoLightPy/lib/util/__init__.py
+-rw-rw-rw-   0        0        0    32832 2024-04-24 14:57:25.000000 amino.light.py-0.2.0/AminoLightPy/lib/util/exceptions.py
+-rw-rw-rw-   0        0        0     1846 2024-04-24 14:57:20.000000 amino.light.py-0.2.0/AminoLightPy/lib/util/helpers.py
+-rw-rw-rw-   0        0        0    83090 2024-05-07 04:48:34.000000 amino.light.py-0.2.0/AminoLightPy/lib/util/objects.py
+-rw-rw-rw-   0        0        0      896 2024-05-06 23:33:35.000000 amino.light.py-0.2.0/AminoLightPy/managers.py
+-rw-rw-rw-   0        0        0    67423 2024-05-06 23:34:09.000000 amino.light.py-0.2.0/AminoLightPy/sub_client.py
+-rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3630 2024-05-07 04:49:05.537038 amino.light.py-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2834 2024-04-19 02:52:28.000000 amino.light.py-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 04:49:05.537038 amino.light.py-0.2.0/amino.light.py.egg-info/
+-rw-rw-rw-   0        0        0     3630 2024-05-07 04:49:04.000000 amino.light.py-0.2.0/amino.light.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2024-05-07 04:49:04.000000 amino.light.py-0.2.0/amino.light.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 04:49:04.000000 amino.light.py-0.2.0/amino.light.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-07 04:49:04.000000 amino.light.py-0.2.0/amino.light.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-07 04:49:04.000000 amino.light.py-0.2.0/amino.light.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 04:49:05.537038 amino.light.py-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2024-05-07 04:47:25.000000 amino.light.py-0.2.0/setup.py
```

### Comparing `amino.light.py-0.1.9/AminoLightPy/amino_socket.py` & `amino.light.py-0.2.0/AminoLightPy/amino_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
                 "ndcId": comId,
             },
             "t": 306 if stop else 304
         }
         data = dumps(data)
         self.client.send(data)
 
-    def recording_reqest(self, comId: int, chatId: str, stop: bool):
+    def recording_request(self, comId: int, chatId: str, stop: bool):
         data = {
             "o": {
                 "actions": ["Recording"],
                 "target": f"ndc://x{comId}/chat-thread/{chatId}",
                 "ndcId": comId,
             },
             "t": 306 if stop else 304
```

### Comparing `amino.light.py-0.1.9/AminoLightPy/client.py` & `amino.light.py-0.2.0/AminoLightPy/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1003,15 +1003,15 @@
         Send a Message to a Chat.
 
         **Parameters**
             - **message** : Message to be sent
             - **chatId** : ID of the Chat.
             - **file** : File to be sent.
             - **fileType** : Type of the file.
-                - ``audio``, ``image``, ``gif``
+                - It's deprecated
             - **messageType** : Type of the Message.
             - **mentionUserIds** : List of User IDS to mention. '@' needed in the Message.
             - **replyTo** : Message ID to reply to.
             - **stickerId** : Sticker ID to be sent.
             - **embedTitle** : Title of the Embed.
             - **embedContent** : Content of the Embed.
             - **embedLink** : Link of the Embed.
@@ -1043,15 +1043,15 @@
             if embedTitle:
                 attachedObject["title"] = embedTitle
 
             if embedContent:
                 attachedObject["content"] = embedContent
 
             if embedImage:
-                attachedObject["mediaList"] = [[100, upload_media(self, embedImage, "image"), None]]
+                attachedObject["mediaList"] = [[100, upload_media(self, embedImage), None]]
             data["attachedObject"] = attachedObject
         if mentionUserIds:
             mentions = [{"uid": mention_uid} for mention_uid in mentionUserIds]
             data["extensions"] = {"mentionedArray": mentions}
 
         if replyTo:
             data["replyMessageId"] = replyTo
@@ -1059,15 +1059,15 @@
         if stickerId:
             data["content"] = None
             data["stickerId"] = stickerId
             data["type"] = 3
 
         if file:
             data["content"] = None
-            url = upload_media(self, file, fileType)
+            url = upload_media(self, file)
 
             data["mediaValue"] = url
 
         response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/message", json=data)
         return response.status_code
 
     def delete_message(self, chatId: str, messageId: str, asStaff: bool = False, reason: str = None):
@@ -1478,15 +1478,15 @@
             "mediaList": None,
             "eventSource": "UserProfileView",
         }
 
         if nickname:
             data["nickname"] = nickname
         if icon:
-            data["icon"] = upload_media(self, icon, "image")
+            data["icon"] = upload_media(self, icon)
         if content:
             data["content"] = content
         if backgroundColor:
             data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if backgroundImage:
             data["extensions"] = {"style": {"backgroundMediaList": [[100, backgroundImage, None, None, None]]}}
         if defaultBubbleId:
```

### Comparing `amino.light.py-0.1.9/AminoLightPy/constants.py` & `amino.light.py-0.2.0/AminoLightPy/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from time import time
 from json import dumps
 from hashlib import sha1
 from typing import BinaryIO
 from collections import OrderedDict
 from requests import Session
+from mimetypes import guess_type
 
 from .lib.util.exceptions import SpecifyType
 from .lib.util import signature, gen_deviceId
 from .lib.util.exceptions import CheckException
 
 # add by August Light
 
 api = "http://service.aminoapps.com:80/api/v1"
 device_id = gen_deviceId()
 cache = OrderedDict()
+cache_len = 32
 
 class AminoSession(Session):
     def __init__(self) -> None:
         super().__init__()
         self.headers.update({
             "NDCDEVICEID": device_id,
             "Accept-Encoding": "gzip, deflate",
@@ -50,15 +52,15 @@
 
         if response.status_code != 200:
             CheckException(response.text)
 
         return response
 
 
-def upload_media(self, file: BinaryIO, fileType: str) -> str:
+def upload_media(self, file: BinaryIO) -> str:
     """
     Upload file to the amino servers.
 
     **Parameters**
         - **file** : File to be uploaded.
 
     **Returns**
@@ -67,32 +69,30 @@
         - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
     """
     data = file.read()
 
     file_hash  = sha1(data).hexdigest()
     if file_hash in cache:
         return cache[file_hash]
-
-    if fileType == "audio":
-        t = "audio/aac"
-    elif fileType == "image":
-        t = "image/jpg"
-    elif fileType == "gif":
-        t = "image/gif"
-    else: raise SpecifyType(fileType)
-
+        
+    fileType = guess_type(file.name)[0]
+    if fileType not in (
+        "image/gif", "image/jpg",
+        "audio/aac", "audio/png"
+    ): raise SpecifyType(fileType) #but this check can be removed, I think
+        
     custom_headers = self.session.headers
-    custom_headers["Content-Type"] = t
+    custom_headers["Content-Type"] = fileType
 
     response = self.session.post(
         url=f"{api}/g/s/media/upload",
         data=data,
         headers=custom_headers,
         stream=True
     )
 
     cache[file_hash] = response.json()["mediaValue"]
-    if len(cache) >= 32:
+    if len(cache) >= cache_len:
         cache.popitem(last=False)
 
     return cache[file_hash]
-    
+
```

### Comparing `amino.light.py-0.1.9/AminoLightPy/lib/util/exceptions.py` & `amino.light.py-0.2.0/AminoLightPy/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.9/AminoLightPy/lib/util/helpers.py` & `amino.light.py-0.2.0/AminoLightPy/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.9/AminoLightPy/managers.py` & `amino.light.py-0.2.0/AminoLightPy/managers.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 class Recording():
     def __init__(self, context, chatId: str, comId: int = None) -> None:
         self.chatId = chatId
         self.context = context
         self.comId = 0 if not comId else comId
 
     def __enter__(self):
-        self.context.recording_reqest(self.comId, self.chatId, False)
+        self.context.recording_request(self.comId, self.chatId, False)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.context.recording_reqest(self.comId, self.chatId, True) 
+        self.context.recording_request(self.comId, self.chatId, True)
```

### Comparing `amino.light.py-0.1.9/AminoLightPy/sub_client.py` & `amino.light.py-0.2.0/AminoLightPy/sub_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,20 +103,20 @@
 		**Raises**
 			- **Exceptions** : :meth:`Exceptions <AminoLightPy.lib.util.exceptions>` if the request fails.
 		"""
 		mediaList = []
 
 		if captionList is not None:
 			for image, caption in zip(imageList, captionList):
-				mediaList.append([100, upload_media(self, image, "image"), caption])
+				mediaList.append([100, upload_media(self, image), caption])
 
 		else:
 			if imageList is not None:
 				for image in imageList:
-					mediaList.append([100, upload_media(self, image, "image"), None])
+					mediaList.append([100, upload_media(self, image), None])
 
 		data = {
 			"address": None,
 			"content": content,
 			"title": title,
 			"mediaList": mediaList,
 			"extensions": extensions,
@@ -168,15 +168,15 @@
 
 	def edit_blog(self, blogId: str, title: str = None, content: str = None,
 				imageList: list = None, categoriesList: list = None,
 				backgroundColor: str = None, fansOnly: bool = False):
 		mediaList = []
 
 		for image in imageList:
-			mediaList.append([100, upload_media(self, image, "image"), None])
+			mediaList.append([100, upload_media(self, image), None])
 
 		data = {
 			"address": None,
 			"mediaList": mediaList,
 			"latitude": 0,
 			"longitude": 0,
 			"eventSource": "PostDetailView",
@@ -234,28 +234,28 @@
 							captionList: list = None, backgroundImage: str = None,
 							backgroundColor: str = None, titles: list = None, colors: list = None,
 							defaultBubbleId: str = None):
 		mediaList = []
 		data = {}
 		if captionList is not None:
 			for image, caption in zip(imageList, captionList):
-				mediaList.append([100, upload_media(self, image, "image"), caption])
+				mediaList.append([100, upload_media(self, image), caption])
 
 		else:
 			if imageList is not None:
 				for image in imageList:
-					mediaList.append([100, upload_media(self, image, "image"), None])
+					mediaList.append([100, upload_media(self, image), None])
 
 		if imageList is not None or captionList is not None:
 			data["mediaList"] = mediaList
 
 		if nickname:
 			data["nickname"] = nickname
 		if icon:
-			data["icon"] = upload_media(self, icon, "image")
+			data["icon"] = upload_media(self, icon)
 		if content:
 			data["content"] = content
 
 		if chatRequestPrivilege:
 			data["extensions"] = {"privilegeOfChatInviteRequest": chatRequestPrivilege}
 		if backgroundImage:
 			data["extensions"] = {"style": {
@@ -712,15 +712,15 @@
 		Send a Message to a Chat.
 
 		**Parameters**
 			- **message** : Message to be sent
 			- **chatId** : ID of the Chat.
 			- **file** : File to be sent.
 			- **fileType** : Type of the file.
-				- ``audio``, ``image``, ``gif``
+				- It's deprecated
 			- **messageType** : Type of the Message.
 			- **mentionUserIds** : List of User IDS to mention. '@' needed in the Message.
 			- **replyTo** : Message ID to reply to.
 			- **stickerId** : Sticker ID to be sent.
 			- **embedTitle** : Title of the Embed.
 			- **embedContent** : Content of the Embed.
 			- **embedLink** : Link of the Embed.
@@ -753,15 +753,15 @@
 			if embedTitle:
 				attachedObject["title"] = embedTitle
 
 			if embedContent:
 				attachedObject["content"] = embedContent
 
 			if embedImage:
-				attachedObject["mediaList"] = [[100, upload_media(self, embedImage, "image"), None]]
+				attachedObject["mediaList"] = [[100, upload_media(self, embedImage), None]]
 
 			data["attachedObject"] = attachedObject
 
 		if mentionUserIds:
 			mentions = [{"uid": mention_uid} for mention_uid in mentionUserIds]
 			data["extensions"] = {"mentionedArray": mentions}
 
@@ -770,27 +770,27 @@
 		if stickerId:
 			data["content"] = None
 			data["stickerId"] = stickerId
 			data["type"] = 3
 
 		if file:
 			data["content"] = None
-			url = upload_media(self, file, fileType)
+			url = upload_media(self, file)
 
 			data["mediaValue"] = url
 
 		response = self.session.post(
 			url=f"{api}/x{self.comId}/s/chat/thread/{chatId}/message",
 			json=data
 		)
 
 		return response.status_code
 
 	def full_embed(self, link: str, image: BinaryIO, message: str, chatId: str):
-		url = upload_media(self, image, "image/png")
+		url = upload_media(self, image)
 		data = {
 			"type": 0,
 			"content": message,
 			"extensions": {
 				"linkSnippetList": [{
 					"link": link,
 					"mediaValue": url
```

### Comparing `amino.light.py-0.1.9/LICENSE` & `amino.light.py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.9/PKG-INFO` & `amino.light.py-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.1.9
+Version: 0.2.0
 Summary: Best Amino.py alternative
 Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
 Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.9 Summary: Best
+Metadata-Version: 2.1 Name: amino.light.py Version: 0.2.0 Summary: Best
 Amino.py alternative Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight License: MIT Keywords:
 amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-
 bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `amino.light.py-0.1.9/README.md` & `amino.light.py-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.9/amino.light.py.egg-info/PKG-INFO` & `amino.light.py-0.2.0/amino.light.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.1.9
+Version: 0.2.0
 Summary: Best Amino.py alternative
 Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
 Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.9 Summary: Best
+Metadata-Version: 2.1 Name: amino.light.py Version: 0.2.0 Summary: Best
 Amino.py alternative Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight License: MIT Keywords:
 amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-
 bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `amino.light.py-0.1.9/amino.light.py.egg-info/SOURCES.txt` & `amino.light.py-0.2.0/amino.light.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.9/setup.py` & `amino.light.py-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "augustlight",
     "aminolightpy",
     "amino.py"
 ]
 
 setup(
     name="amino.light.py",
-    version="0.1.9",
+    version="0.2.0",
     url="https://github.com/AugustLigh/AminoLightPy",
     license="MIT",
     description="Best Amino.py alternative",
     author="AugustLight",
     packages=find_packages(),
     install_requires=["requests", "websocket-client"],
     long_description=long_description,
```

