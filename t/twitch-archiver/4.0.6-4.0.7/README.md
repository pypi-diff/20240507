# Comparing `tmp/twitch-archiver-4.0.6.tar.gz` & `tmp/twitch_archiver-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-archiver-4.0.6.tar", last modified: Wed Mar  6 05:22:15 2024, max compression
+gzip compressed data, was "twitch_archiver-4.0.7.tar", last modified: Tue May  7 03:18:42 2024, max compression
```

## Comparing `twitch-archiver-4.0.6.tar` & `twitch_archiver-4.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 05:22:15.263236 twitch-archiver-4.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-03-06 05:22:15.263236 twitch-archiver-4.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8643 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 05:22:15.263236 twitch-archiver-4.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 05:22:15.263236 twitch-archiver-4.0.6/twitch_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-03-06 05:22:15.000000 twitch-archiver-4.0.6/twitch_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-06 05:22:15.000000 twitch-archiver-4.0.6/twitch_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 05:22:15.000000 twitch-archiver-4.0.6/twitch_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-06 05:22:15.000000 twitch-archiver-4.0.6/twitch_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-06 05:22:15.000000 twitch-archiver-4.0.6/twitch_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-06 05:22:15.000000 twitch-archiver-4.0.6/twitch_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 05:22:15.263236 twitch-archiver-4.0.6/twitcharchiver/
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 05:22:15.263236 twitch-archiver-4.0.6/twitcharchiver/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/downloaders/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/downloaders/realtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    23662 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/downloaders/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    32460 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/downloaders/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23657 2024-03-06 05:22:11.000000 twitch-archiver-4.0.6/twitcharchiver/vod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:18:42.338221 twitch_archiver-4.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-07 03:18:42.338221 twitch_archiver-4.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8643 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:18:42.338221 twitch_archiver-4.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:18:42.338221 twitch_archiver-4.0.7/twitch_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-07 03:18:42.000000 twitch_archiver-4.0.7/twitch_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-07 03:18:42.000000 twitch_archiver-4.0.7/twitch_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 03:18:42.000000 twitch_archiver-4.0.7/twitch_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 03:18:42.000000 twitch_archiver-4.0.7/twitch_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 03:18:42.000000 twitch_archiver-4.0.7/twitch_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 03:18:42.000000 twitch_archiver-4.0.7/twitch_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:18:42.338221 twitch_archiver-4.0.7/twitcharchiver/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:18:42.338221 twitch_archiver-4.0.7/twitcharchiver/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/downloaders/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/downloaders/realtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/downloaders/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32460 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/downloaders/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23657 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/vod.py
```

### Comparing `twitch-archiver-4.0.6/LICENSE` & `twitch_archiver-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/PKG-INFO` & `twitch_archiver-4.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 4.0.6
+Version: 4.0.7
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `twitch-archiver-4.0.6/README.md` & `twitch_archiver-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/pyproject.toml` & `twitch_archiver-4.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "twitch-archiver"
-version = "4.0.6"
+version = "4.0.7"
 dependencies = [
     "requests>=2.28.0",
     "m3u8>=0.3.12",
 ]
 authors = [
   { name="Brisppy", email="brisppy@protonmail.com" },
 ]
```

### Comparing `twitch-archiver-4.0.6/twitch_archiver.egg-info/PKG-INFO` & `twitch_archiver-4.0.7/twitch_archiver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 4.0.6
+Version: 4.0.7
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `twitch-archiver-4.0.6/twitch_archiver.egg-info/SOURCES.txt` & `twitch_archiver-4.0.7/twitch_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/__init__.py` & `twitch_archiver-4.0.7/twitcharchiver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from twitcharchiver.utils import (
     getenv,
     check_update_available,
     get_latest_version,
     get_temp_dir,
 )
 
-__version__ = "4.0.6"
+__version__ = "4.0.7"
 
 from twitcharchiver.vod import Vod, ArchivedVod
 
 
 def main():
     """
     Main processing for twitch-archiver.
```

### Comparing `twitch-archiver-4.0.6/twitcharchiver/api.py` & `twitch_archiver-4.0.7/twitcharchiver/api.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/arguments.py` & `twitch_archiver-4.0.7/twitcharchiver/arguments.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/channel.py` & `twitch_archiver-4.0.7/twitcharchiver/channel.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/configuration.py` & `twitch_archiver-4.0.7/twitcharchiver/configuration.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/database.py` & `twitch_archiver-4.0.7/twitcharchiver/database.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/downloader.py` & `twitch_archiver-4.0.7/twitcharchiver/downloader.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/downloaders/chat.py` & `twitch_archiver-4.0.7/twitcharchiver/downloaders/chat.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/downloaders/realtime.py` & `twitch_archiver-4.0.7/twitcharchiver/downloaders/realtime.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/downloaders/stream.py` & `twitch_archiver-4.0.7/twitcharchiver/downloaders/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,35 +480,54 @@
         )
 
     def _fetch_advertised_parts(self):
         """
         Fetch parts being advertised by Twitch for stream.
         """
         # attempt to grab new parts from Twitch
-        try:
-            # fetch advertised stream parts
-            announced_parts = m3u8.loads(
-                self.channel.get_stream_playlist(self._index_uri)
-            ).segments
-            self._last_part_announce = (
-                announced_parts[-1]
-                .program_date_time.replace(tzinfo=timezone.utc)
-                .timestamp()
-            )
+        for _ in range(5):
+            if _ >= 4:
+                self._log.error(
+                    "Failed to fetch advertised parts from stream by %s.",
+                    self.channel.name,
+                )
+                raise StreamFetchError(self.channel)
+
+            try:
+                # fetch advertised stream parts
+                announced_parts = m3u8.loads(
+                    self.channel.get_stream_playlist(self._index_uri)
+                ).segments
+                self._last_part_announce = (
+                    announced_parts[-1]
+                    .program_date_time.replace(tzinfo=timezone.utc)
+                    .timestamp()
+                )
+
+                for _part in [StreamSegment.Part(_p) for _p in announced_parts]:
+                    # add new parts to part buffer
+                    if _part not in self._processed_parts:
+                        self._processed_parts.add(_part)
+                        self._incoming_part_buffer.append(_part)
+                        self.vod.duration = int(_part.timestamp - self.vod.created_at)
+
+                return
+
+            # 404 can be received if fetching stream playlist very soon after it goes live as the endpoint is not yet
+            # available.
+            except TwitchAPIErrorNotFound:
+                self._log.debug(
+                    "404 returned when fetching stream playlist, retrying..."
+                )
+                sleep(5)
+                continue
 
-            for _part in [StreamSegment.Part(_p) for _p in announced_parts]:
-                # add new parts to part buffer
-                if _part not in self._processed_parts:
-                    self._processed_parts.add(_part)
-                    self._incoming_part_buffer.append(_part)
-                    self.vod.duration = int(_part.timestamp - self.vod.created_at)
-
-        # retry if request times out
-        except Exception as exc:
-            raise StreamFetchError(self.channel.name) from exc
+            # retry if request times out
+            except Exception as exc:
+                raise StreamFetchError(self.channel) from exc
 
     def _build_download_queue(self):
         """
         Creates queue of segments being downloaded using the incoming part buffer and already processed segments.
         """
         # add parts to the associated segment
         for _part in self._incoming_part_buffer:
@@ -615,15 +634,15 @@
                     )
                     self._completed_segments.add(segment)
                     self._log.debug("Stream segment: %s completed.", segment.id)
                     break
 
                 except Exception as exc:
                     raise StreamSegmentDownloadError(
-                        segment.id, self.channel.name
+                        segment, self.channel.name
                     ) from exc
 
     def _get_final_segment(self):
         """
         Downloads the final stream segment.
         """
         # ensure final segment present
```

### Comparing `twitch-archiver-4.0.6/twitcharchiver/downloaders/video.py` & `twitch_archiver-4.0.7/twitcharchiver/downloaders/video.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/exceptions.py` & `twitch_archiver-4.0.7/twitcharchiver/exceptions.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/logger.py` & `twitch_archiver-4.0.7/twitcharchiver/logger.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/processing.py` & `twitch_archiver-4.0.7/twitcharchiver/processing.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/twitch.py` & `twitch_archiver-4.0.7/twitcharchiver/twitch.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/utils.py` & `twitch_archiver-4.0.7/twitcharchiver/utils.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-4.0.6/twitcharchiver/vod.py` & `twitch_archiver-4.0.7/twitcharchiver/vod.py`

 * *Files identical despite different names*

