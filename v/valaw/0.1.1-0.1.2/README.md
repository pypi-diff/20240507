# Comparing `tmp/valaw-0.1.1.tar.gz` & `tmp/valaw-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valaw-0.1.1.tar", last modified: Tue Mar 19 16:27:49 2024, max compression
+gzip compressed data, was "valaw-0.1.2.tar", last modified: Tue May  7 16:05:16 2024, max compression
```

## Comparing `valaw-0.1.1.tar` & `valaw-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:27:49.177687 valaw-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-19 16:27:39.000000 valaw-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-19 16:27:49.177687 valaw-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-19 16:27:39.000000 valaw-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 16:27:49.177687 valaw-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-19 16:27:39.000000 valaw-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:27:49.173687 valaw-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:27:49.173687 valaw-0.1.1/src/valaw/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-19 16:27:39.000000 valaw-0.1.1/src/valaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-03-19 16:27:39.000000 valaw-0.1.1/src/valaw/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:27:49.177687 valaw-0.1.1/src/valaw/objects/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-19 16:27:39.000000 valaw-0.1.1/src/valaw/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-19 16:27:39.000000 valaw-0.1.1/src/valaw/objects/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-19 16:27:39.000000 valaw-0.1.1/src/valaw/objects/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-19 16:27:39.000000 valaw-0.1.1/src/valaw/objects/match.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-19 16:27:39.000000 valaw-0.1.1/src/valaw/objects/ranked.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-19 16:27:39.000000 valaw-0.1.1/src/valaw/objects/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:27:49.177687 valaw-0.1.1/src/valaw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-19 16:27:49.000000 valaw-0.1.1/src/valaw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-19 16:27:49.000000 valaw-0.1.1/src/valaw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 16:27:49.000000 valaw-0.1.1/src/valaw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-19 16:27:49.000000 valaw-0.1.1/src/valaw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-19 16:27:49.000000 valaw-0.1.1/src/valaw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:05:16.835331 valaw-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-07 16:05:12.000000 valaw-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-07 16:05:16.835331 valaw-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-07 16:05:12.000000 valaw-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:05:16.835331 valaw-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-07 16:05:12.000000 valaw-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:05:16.831331 valaw-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:05:16.831331 valaw-0.1.2/src/valaw/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-07 16:05:12.000000 valaw-0.1.2/src/valaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-05-07 16:05:12.000000 valaw-0.1.2/src/valaw/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:05:16.835331 valaw-0.1.2/src/valaw/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-07 16:05:12.000000 valaw-0.1.2/src/valaw/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-07 16:05:12.000000 valaw-0.1.2/src/valaw/objects/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-07 16:05:12.000000 valaw-0.1.2/src/valaw/objects/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-07 16:05:12.000000 valaw-0.1.2/src/valaw/objects/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-07 16:05:12.000000 valaw-0.1.2/src/valaw/objects/ranked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-07 16:05:12.000000 valaw-0.1.2/src/valaw/objects/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:05:16.835331 valaw-0.1.2/src/valaw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-07 16:05:16.000000 valaw-0.1.2/src/valaw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-07 16:05:16.000000 valaw-0.1.2/src/valaw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:05:16.000000 valaw-0.1.2/src/valaw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 16:05:16.000000 valaw-0.1.2/src/valaw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 16:05:16.000000 valaw-0.1.2/src/valaw.egg-info/top_level.txt
```

### Comparing `valaw-0.1.1/LICENSE` & `valaw-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `valaw-0.1.1/PKG-INFO` & `valaw-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valaw
-Version: 0.1.1
+Version: 0.1.2
 Summary: An asynchronous API wrapper for VALORANT's API
 Home-page: https://github.com/Jet612/valaw
 Author: Jet612
 Project-URL: Source, https://github.com/Jet612/valaw
 Project-URL: Documentation, https://valaw.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/Jet612/valaw/issues
 Project-URL: Chat/Support, https://discord.gg/mVXpvunBbF
```

### Comparing `valaw-0.1.1/README.md` & `valaw-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `valaw-0.1.1/setup.py` & `valaw-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as readme:
     long_desc = readme.read()
 
 url = "https://github.com/Jet612/valaw"
 
 setup(
     name="valaw",
-    version="0.1.01",
+    version="0.1.02",
     author="Jet612",
     description="An asynchronous API wrapper for VALORANT's API",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/Jet612/valaw",
     project_urls={
         "Source": url,
```

### Comparing `valaw-0.1.1/src/valaw/client.py` & `valaw-0.1.2/src/valaw/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### Imports ###
 import aiohttp
 import json
 from dataclass_wizard import fromdict
-from typing import Union, Dict
+from typing import Union, Dict, List
 
 from .objects import (
     AccountDto,
     ActiveShardDto,
     ContentDto,
     MatchDto,
     MatchlistDto,
@@ -99,16 +99,15 @@
         self.raw_data = raw_data
 
     ##################
     ### ACCOUNT-V1 ###
     ##################
 
     async def GET_getByPuuid(self, puuid: str, cluster: str = None) -> Union[AccountDto, Dict]:
-        """
-        Get account by PUUID.
+        """Get account by PUUID.
         
         :param puuid: The PUUID of the account.
         :type puuid: :class:`str`
         :param cluster: The cluster to retreive from. Defaults to self.cluster.
         :type cluster: :class:`str`
         :rtype: Union[AccountDto, :class:`Dict`]
         """
@@ -451,8 +450,54 @@
             async with session.get(f"https://{region}.api.riotgames.com/val/status/v1/platform-data", headers=headers) as resp:
                 raw_response = await verify_content(response=resp)
                 if self.raw_data == True:
                     return raw_response
                 if raw_response.get("status") != None:
                     raise Exceptions.RiotAPIResponseError(raw_response["status"]["status_code"], raw_response["status"]["message"])
                 else:
-                    return fromdict(PlatformDataDto, raw_response)
+                    return fromdict(PlatformDataDto, raw_response)
+
+    ###########
+    ### RSO ###
+    ###########
+
+    def create_RSO_link(self, redirect_uri: str, client_id: str, response_type: str, scopes: List[str], login_hint: str = None, ui_locales: List[str] = None, state: str = None):
+        """Create a Riot Sign-On Link.
+
+        :param redirect_uri: OAuth2 callback route
+        :type redirect_uri: :class:`str`
+        :param client_id: Client ID of the RSO application
+        :type client_id: :class:`str`
+        :param response_type: OAuth2 response type, should be 'code' for authorization code flow
+        :type response_type: :class:`str`
+        :param scopes: List of scopes to request, must include 'openid' to authenticate, addition scopes are 'cpid', and 'offline_access'
+        :type scopes: List[:class:`str`]
+        :param login_hint: Used to specify hints to pre-populate data on the login page. Formats {regioncode}, {regioncode}|{username}, {regioncode}#{userid}. Defaults to None
+        :type login_hint: :class:`str`
+        :param ui_locales: List of BCP47 language tag values in order of most to least preferred. Defaults to None
+        :type ui_locales: List[:class:`str`]
+        :param state: Opaque value provided to authorize the endpoint, the same value will be returned to the redirect_uri. Defaults to None
+        :type state: :class:`str`
+
+        :returns: :class:`str`
+
+        For more information on RSO, visit https://developer.riotgames.com/docs/valorant#rso-integration
+        """
+
+        scopes = "+".join(scopes)
+
+        if login_hint != None:
+            login_hint = f"&login_hint={login_hint}"
+        else:
+            login_hint = ""
+        
+        if ui_locales != None:
+            ui_locales = f"&ui_locales={' '.join(ui_locales)}"
+        else:
+            ui_locales = ""
+
+        if state != None:
+            state = f"&state={state}"
+        else:
+            state = ""
+
+        return f"https://auth.riotgames.com/authorize?redirect_uri={redirect_uri}&client_id={client_id}&response_type={response_type}&scope={scopes}{login_hint}{ui_locales}{state}"
```

### Comparing `valaw-0.1.1/src/valaw/objects/__init__.py` & `valaw-0.1.2/src/valaw/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `valaw-0.1.1/src/valaw/objects/content.py` & `valaw-0.1.2/src/valaw/objects/content.py`

 * *Files identical despite different names*

### Comparing `valaw-0.1.1/src/valaw/objects/match.py` & `valaw-0.1.2/src/valaw/objects/match.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,16 +131,18 @@
     gameName: str
     tagLine: str
     teamId: str
     partyId: str
     characterId: str
     stats: PlayerStatsDto
     competitiveTier: int
+    isObserver: bool
     playerCard: str
     playerTitle: str
+    accountLevel: int
 
 @dataclass
 class MatchInfoDto:
     matchId: str
     mapId: str
     gameLengthMillis: int
     gameStartMillis: int
```

### Comparing `valaw-0.1.1/src/valaw/objects/ranked.py` & `valaw-0.1.2/src/valaw/objects/ranked.py`

 * *Files identical despite different names*

### Comparing `valaw-0.1.1/src/valaw/objects/status.py` & `valaw-0.1.2/src/valaw/objects/status.py`

 * *Files identical despite different names*

### Comparing `valaw-0.1.1/src/valaw.egg-info/PKG-INFO` & `valaw-0.1.2/src/valaw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valaw
-Version: 0.1.1
+Version: 0.1.2
 Summary: An asynchronous API wrapper for VALORANT's API
 Home-page: https://github.com/Jet612/valaw
 Author: Jet612
 Project-URL: Source, https://github.com/Jet612/valaw
 Project-URL: Documentation, https://valaw.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/Jet612/valaw/issues
 Project-URL: Chat/Support, https://discord.gg/mVXpvunBbF
```

