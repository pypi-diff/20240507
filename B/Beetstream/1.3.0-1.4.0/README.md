# Comparing `tmp/Beetstream-1.3.0.tar.gz` & `tmp/beetstream-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Beetstream-1.3.0.tar", last modified: Sat Mar 16 14:02:12 2024, max compression
+gzip compressed data, was "beetstream-1.4.0.tar", last modified: Tue May  7 14:29:38 2024, max compression
```

## Comparing `Beetstream-1.3.0.tar` & `beetstream-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 sacha     (1001) sacha     (1001)        0 2024-03-16 14:02:12.609340 Beetstream-1.3.0/
-drwxr-xr-x   0 sacha     (1001) sacha     (1001)        0 2024-03-16 14:02:12.609340 Beetstream-1.3.0/Beetstream.egg-info/
--rw-r--r--   0 sacha     (1001) sacha     (1001)     4436 2024-03-16 14:02:12.000000 Beetstream-1.3.0/Beetstream.egg-info/PKG-INFO
--rw-r--r--   0 sacha     (1001) sacha     (1001)      608 2024-03-16 14:02:12.000000 Beetstream-1.3.0/Beetstream.egg-info/SOURCES.txt
--rw-r--r--   0 sacha     (1001) sacha     (1001)        1 2024-03-16 14:02:12.000000 Beetstream-1.3.0/Beetstream.egg-info/dependency_links.txt
--rw-r--r--   0 sacha     (1001) sacha     (1001)       67 2024-03-16 14:02:12.000000 Beetstream-1.3.0/Beetstream.egg-info/requires.txt
--rw-r--r--   0 sacha     (1001) sacha     (1001)       10 2024-03-16 14:02:12.000000 Beetstream-1.3.0/Beetstream.egg-info/top_level.txt
--rw-r--r--   0 sacha     (1001) sacha     (1001)     1067 2020-12-24 17:24:37.000000 Beetstream-1.3.0/LICENSE
--rw-r--r--   0 sacha     (1001) sacha     (1001)     4436 2024-03-16 14:02:12.609340 Beetstream-1.3.0/PKG-INFO
--rw-r--r--   0 sacha     (1001) sacha     (1001)     3445 2023-03-26 21:40:44.000000 Beetstream-1.3.0/README.md
-drwxr-xr-x   0 sacha     (1001) sacha     (1001)        0 2024-03-16 14:02:12.589340 Beetstream-1.3.0/beetsplug/
--rw-r--r--   0 sacha     (1001) sacha     (1001)       75 2020-12-24 17:54:20.000000 Beetstream-1.3.0/beetsplug/__init__.py
-drwxr-xr-x   0 sacha     (1001) sacha     (1001)        0 2024-03-16 14:02:12.609340 Beetstream-1.3.0/beetsplug/beetstream/
--rw-r--r--   0 sacha     (1001) sacha     (1001)     5065 2024-03-16 13:54:24.000000 Beetstream-1.3.0/beetsplug/beetstream/__init__.py
--rw-r--r--   0 sacha     (1001) sacha     (1001)     9476 2022-05-24 12:10:18.000000 Beetstream-1.3.0/beetsplug/beetstream/albums.py
--rw-r--r--   0 sacha     (1001) sacha     (1001)     4526 2022-12-13 21:47:36.000000 Beetstream-1.3.0/beetsplug/beetstream/artists.py
--rw-r--r--   0 sacha     (1001) sacha     (1001)     2087 2024-03-16 13:54:24.000000 Beetstream-1.3.0/beetsplug/beetstream/dummy.py
--rw-r--r--   0 sacha     (1001) sacha     (1001)     3052 2024-03-16 13:54:24.000000 Beetstream-1.3.0/beetsplug/beetstream/playlistprovider.py
--rw-r--r--   0 sacha     (1001) sacha     (1001)     2062 2024-03-16 13:54:24.000000 Beetstream-1.3.0/beetsplug/beetstream/playlists.py
--rw-r--r--   0 sacha     (1001) sacha     (1001)     2389 2022-05-24 12:10:33.000000 Beetstream-1.3.0/beetsplug/beetstream/search.py
--rw-r--r--   0 sacha     (1001) sacha     (1001)     4611 2023-03-26 21:40:44.000000 Beetstream-1.3.0/beetsplug/beetstream/songs.py
--rw-r--r--   0 sacha     (1001) sacha     (1001)      906 2023-03-26 21:40:44.000000 Beetstream-1.3.0/beetsplug/beetstream/stream.py
--rw-r--r--   0 sacha     (1001) sacha     (1001)     1881 2022-05-24 12:10:46.000000 Beetstream-1.3.0/beetsplug/beetstream/users.py
--rw-r--r--   0 sacha     (1001) sacha     (1001)     9144 2024-03-16 13:54:24.000000 Beetstream-1.3.0/beetsplug/beetstream/utils.py
--rw-r--r--   0 sacha     (1001) sacha     (1001)       84 2022-06-12 16:21:36.000000 Beetstream-1.3.0/pyproject.toml
--rw-r--r--   0 sacha     (1001) sacha     (1001)      988 2024-03-16 14:02:12.609340 Beetstream-1.3.0/setup.cfg
-drwxr-xr-x   0 sacha     (1001) sacha     (1001)        0 2024-03-16 14:02:12.609340 Beetstream-1.3.0/test/
--rw-r--r--   0 sacha     (1001) sacha     (1001)      366 2022-05-24 12:18:52.000000 Beetstream-1.3.0/test/test_subsonic.py
+drwxr-xr-x   0 sacha     (1001) sacha     (1001)        0 2024-05-07 14:29:38.049778 beetstream-1.4.0/
+drwxr-xr-x   0 sacha     (1001) sacha     (1001)        0 2024-05-07 14:29:38.049778 beetstream-1.4.0/Beetstream.egg-info/
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     4436 2024-05-07 14:29:37.000000 beetstream-1.4.0/Beetstream.egg-info/PKG-INFO
+-rw-r--r--   0 sacha     (1001) sacha     (1001)      641 2024-05-07 14:29:37.000000 beetstream-1.4.0/Beetstream.egg-info/SOURCES.txt
+-rw-r--r--   0 sacha     (1001) sacha     (1001)        1 2024-05-07 14:29:37.000000 beetstream-1.4.0/Beetstream.egg-info/dependency_links.txt
+-rw-r--r--   0 sacha     (1001) sacha     (1001)       67 2024-05-07 14:29:37.000000 beetstream-1.4.0/Beetstream.egg-info/requires.txt
+-rw-r--r--   0 sacha     (1001) sacha     (1001)       10 2024-05-07 14:29:37.000000 beetstream-1.4.0/Beetstream.egg-info/top_level.txt
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     1067 2020-12-24 17:24:37.000000 beetstream-1.4.0/LICENSE
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     4436 2024-05-07 14:29:38.049778 beetstream-1.4.0/PKG-INFO
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     3445 2023-03-26 21:40:44.000000 beetstream-1.4.0/README.md
+drwxr-xr-x   0 sacha     (1001) sacha     (1001)        0 2024-05-07 14:29:38.039778 beetstream-1.4.0/beetsplug/
+-rw-r--r--   0 sacha     (1001) sacha     (1001)       75 2020-12-24 17:54:20.000000 beetstream-1.4.0/beetsplug/__init__.py
+drwxr-xr-x   0 sacha     (1001) sacha     (1001)        0 2024-05-07 14:29:38.049778 beetstream-1.4.0/beetsplug/beetstream/
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     5176 2024-05-07 14:27:47.000000 beetstream-1.4.0/beetsplug/beetstream/__init__.py
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     8375 2024-05-07 14:27:47.000000 beetstream-1.4.0/beetsplug/beetstream/albums.py
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     4526 2022-12-13 21:47:36.000000 beetstream-1.4.0/beetsplug/beetstream/artists.py
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     2001 2024-05-07 14:27:47.000000 beetstream-1.4.0/beetsplug/beetstream/coverart.py
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     2087 2024-03-16 13:54:24.000000 beetstream-1.4.0/beetsplug/beetstream/dummy.py
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     4563 2024-05-07 14:27:47.000000 beetstream-1.4.0/beetsplug/beetstream/playlistprovider.py
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     2194 2024-05-07 14:27:47.000000 beetstream-1.4.0/beetsplug/beetstream/playlists.py
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     2389 2022-05-24 12:10:33.000000 beetstream-1.4.0/beetsplug/beetstream/search.py
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     4611 2023-03-26 21:40:44.000000 beetstream-1.4.0/beetsplug/beetstream/songs.py
+-rw-r--r--   0 sacha     (1001) sacha     (1001)      906 2023-03-26 21:40:44.000000 beetstream-1.4.0/beetsplug/beetstream/stream.py
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     1881 2022-05-24 12:10:46.000000 beetstream-1.4.0/beetsplug/beetstream/users.py
+-rw-r--r--   0 sacha     (1001) sacha     (1001)     9498 2024-05-07 14:27:47.000000 beetstream-1.4.0/beetsplug/beetstream/utils.py
+-rw-r--r--   0 sacha     (1001) sacha     (1001)       84 2022-06-12 16:21:36.000000 beetstream-1.4.0/pyproject.toml
+-rw-r--r--   0 sacha     (1001) sacha     (1001)      988 2024-05-07 14:29:38.059778 beetstream-1.4.0/setup.cfg
+drwxr-xr-x   0 sacha     (1001) sacha     (1001)        0 2024-05-07 14:29:38.049778 beetstream-1.4.0/test/
+-rw-r--r--   0 sacha     (1001) sacha     (1001)      366 2022-05-24 12:18:52.000000 beetstream-1.4.0/test/test_subsonic.py
```

### Comparing `Beetstream-1.3.0/Beetstream.egg-info/PKG-INFO` & `beetstream-1.4.0/Beetstream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Beetstream
-Version: 1.3.0
+Version: 1.4.0
 Summary: Beets.io plugin that expose SubSonic API endpoints, allowing you to stream your music everywhere.
 Home-page: https://github.com/BinaryBrain/Beetstream
 Author: Binary Brain
 Author-email: me@sachabron.ch
 Project-URL: Bug Tracker, https://github.com/BinaryBrain/Beetstream/issues
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `Beetstream-1.3.0/Beetstream.egg-info/SOURCES.txt` & `beetstream-1.4.0/Beetstream.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Beetstream.egg-info/dependency_links.txt
 Beetstream.egg-info/requires.txt
 Beetstream.egg-info/top_level.txt
 beetsplug/__init__.py
 beetsplug/beetstream/__init__.py
 beetsplug/beetstream/albums.py
 beetsplug/beetstream/artists.py
+beetsplug/beetstream/coverart.py
 beetsplug/beetstream/dummy.py
 beetsplug/beetstream/playlistprovider.py
 beetsplug/beetstream/playlists.py
 beetsplug/beetstream/search.py
 beetsplug/beetstream/songs.py
 beetsplug/beetstream/stream.py
 beetsplug/beetstream/users.py
```

### Comparing `Beetstream-1.3.0/LICENSE` & `beetstream-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Beetstream-1.3.0/PKG-INFO` & `beetstream-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Beetstream
-Version: 1.3.0
+Version: 1.4.0
 Summary: Beets.io plugin that expose SubSonic API endpoints, allowing you to stream your music everywhere.
 Home-page: https://github.com/BinaryBrain/Beetstream
 Author: Binary Brain
 Author-email: me@sachabron.ch
 Project-URL: Bug Tracker, https://github.com/BinaryBrain/Beetstream/issues
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `Beetstream-1.3.0/README.md` & `beetstream-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Beetstream-1.3.0/beetsplug/beetstream/__init__.py` & `beetstream-1.4.0/beetsplug/beetstream/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 @app.route('/')
 def home():
     return "Beetstream server running"
 
 from beetsplug.beetstream.utils import *
 import beetsplug.beetstream.albums
 import beetsplug.beetstream.artists
+import beetsplug.beetstream.coverart
 import beetsplug.beetstream.dummy
 import beetsplug.beetstream.playlists
 import beetsplug.beetstream.search
 import beetsplug.beetstream.songs
 import beetsplug.beetstream.users
 
 # Plugin hook.
@@ -76,15 +77,18 @@
             # Normalizes json output
             app.config['JSONIFY_PRETTYPRINT_REGULAR'] = False
 
             app.config['INCLUDE_PATHS'] = self.config['include_paths']
             app.config['never_transcode'] = self.config['never_transcode']
             playlist_dir = self.config['playlist_dir']
             if not playlist_dir:
-                playlist_dir = config['smartplaylist']['playlist_dir'].get()
+                try:
+                    playlist_dir = config['smartplaylist']['playlist_dir'].get()
+                except:
+                    pass
             app.config['playlist_dir'] = playlist_dir
 
             # Enable CORS if required.
             if self.config['cors']:
                 self._log.info(u'Enabling CORS with origin: {0}',
                                self.config['cors'])
                 app.config['CORS_ALLOW_HEADERS'] = "Content-Type"
```

### Comparing `Beetstream-1.3.0/beetsplug/beetstream/albums.py` & `beetstream-1.4.0/beetsplug/beetstream/albums.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,45 +107,14 @@
 
             for album in albums:
                 a = ET.SubElement(album_list_xml, 'album')
                 map_album_xml(a, album)
 
             return Response(xml_to_string(root), mimetype='text/xml')
 
-@app.route('/rest/getCoverArt', methods=["GET", "POST"])
-@app.route('/rest/getCoverArt.view', methods=["GET", "POST"])
-def cover_art_file():
-    query_id = int(album_subid_to_beetid(request.values.get('id')) or -1)
-    size = request.values.get('size')
-    album = g.lib.get_album(query_id)
-
-    # Fallback on item id. Some apps use this
-    if not album:
-        item = g.lib.get_item(query_id)
-        if item is not None and item.album_id is not None:
-            album = g.lib.get_album(item.album_id)
-        else:
-            flask.abort(404)
-
-    if album and album.artpath:
-        image_path = album.artpath.decode('utf-8')
-
-        if size is not None and int(size) > 0:
-            size = int(size)
-            with Image.open(image_path) as image:
-                bytes_io = io.BytesIO()
-                image = image.resize((size, size))
-                image.convert('RGB').save(bytes_io, 'PNG')
-                bytes_io.seek(0)
-                return flask.send_file(bytes_io, mimetype='image/png')
-
-        return flask.send_file(image_path)
-    else:
-        return flask.abort(404)
-
 @app.route('/rest/getGenres', methods=["GET", "POST"])
 @app.route('/rest/getGenres.view', methods=["GET", "POST"])
 def genres():
     res_format = request.values.get('f') or 'xml'
     with g.lib.transaction() as tx:
         mixed_genres = list(tx.query("""
             SELECT genre, COUNT(*) AS n_song, "" AS n_album FROM items GROUP BY genre
```

### Comparing `Beetstream-1.3.0/beetsplug/beetstream/artists.py` & `beetstream-1.4.0/beetsplug/beetstream/artists.py`

 * *Files identical despite different names*

### Comparing `Beetstream-1.3.0/beetsplug/beetstream/dummy.py` & `beetstream-1.4.0/beetsplug/beetstream/dummy.py`

 * *Files identical despite different names*

### Comparing `Beetstream-1.3.0/beetsplug/beetstream/playlistprovider.py` & `beetstream-1.4.0/beetsplug/beetstream/playlistprovider.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,107 @@
 import glob
 import os
 import pathlib
 import re
+import sys
+from beetsplug.beetstream.utils import strip_accents
+from flask import current_app as app
 from werkzeug.utils import safe_join
 
 extinf_regex = re.compile(r'^#EXTINF:([0-9]+)( [^,]+)?,[\s]*(.*)')
+highint32 = 1<<31
 
 class PlaylistProvider:
     def __init__(self, dir):
-        self._dir = dir
+        self.dir = dir
         self._playlists = {}
 
     def _refresh(self):
-        paths = glob.glob(os.path.join(self._dir, "**.m3u8"))
-        paths += glob.glob(os.path.join(self._dir, "**.m3u"))
+        self._playlists = {p.id: p for p in self._load_playlists()}
+        app.logger.debug(f"Loaded {len(self._playlists)} playlists")
+
+    def _load_playlists(self):
+        if not self.dir:
+            return
+        paths = glob.glob(os.path.join(self.dir, "**.m3u8"))
+        paths += glob.glob(os.path.join(self.dir, "**.m3u"))
         paths.sort()
-        self._playlists = {self._path2id(p): self._playlist(p) for p in paths}
+        for path in paths:
+            try:
+                yield self._playlist(path)
+            except Exception as e:
+                app.logger.error(f"Failed to load playlist {filepath}: {e}")
 
     def playlists(self):
         self._refresh()
-        ids = [k for k in self._playlists]
+        playlists = self._playlists
+        ids = [k for k, v in playlists.items() if v]
         ids.sort()
-        return [self._playlists[id] for id in ids]
+        return [playlists[id] for id in ids]
 
     def playlist(self, id):
-        self._refresh()
-        filepath = safe_join(self._dir, id)
-        return self._playlist(filepath)
+        filepath = safe_join(self.dir, id)
+        playlist = self._playlist(filepath)
+        if playlist.id not in self._playlists: #  add to cache
+            playlists = self._playlists.copy()
+            playlists[playlist.id] = playlist
+            self._playlists = playlists
+        return playlist
 
     def _playlist(self, filepath):
         id = self._path2id(filepath)
         name = pathlib.Path(os.path.basename(filepath)).stem
         playlist = self._playlists.get(id)
         mtime = pathlib.Path(filepath).stat().st_mtime
         if playlist and playlist.modified == mtime:
-            return playlist # cached
+            return playlist # cached metadata
+        app.logger.debug(f"Loading playlist {filepath}")
         return Playlist(id, name, mtime, filepath)
 
     def _path2id(self, filepath):
-        return os.path.relpath(filepath, self._dir)
+        return os.path.relpath(filepath, self.dir)
 
-class Playlist():
+class Playlist:
     def __init__(self, id, name, modified, path):
         self.id = id
         self.name = name
         self.modified = modified
         self.path = path
         self.count = 0
         self.duration = 0
-        for item in parse_m3u_playlist(self.path):
+        artists = {}
+        max_artists = 10
+        for item in self.items():
             self.count += 1
             self.duration += item.duration
+            artist = Artist(item.title.split(' - ')[0])
+            found = artists.get(artist.key)
+            if found:
+                found.count += 1
+            else:
+                if len(artists) > max_artists:
+                    l = _sortedartists(artists)[:max_artists]
+                    artists = {a.key: a for a in l}
+                artists[artist.key] = artist
+        self.artists = ', '.join([a.name for a in _sortedartists(artists)])
 
     def items(self):
         return parse_m3u_playlist(self.path)
 
+def _sortedartists(artists):
+    l = [a for _,a in artists.items()]
+    l.sort(key=lambda a: (highint32-a.count, a.name))
+    return l
+
+class Artist:
+    def __init__(self, name):
+        self.key = strip_accents(name.lower())
+        self.name = name
+        self.count = 1
+
 def parse_m3u_playlist(filepath):
     '''
     Parses an M3U playlist and yields its items, one at a time.
     CAUTION: Attribute values that contain ',' or ' ' are not supported!
     '''
     with open(filepath, 'r', encoding='UTF-8') as file:
         linenum = 0
```

### Comparing `Beetstream-1.3.0/beetsplug/beetstream/playlists.py` & `beetstream-1.4.0/beetsplug/beetstream/playlists.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,9 +45,12 @@
             map_song_xml(entry, song)
         return Response(xml_to_string(root), mimetype='text/xml')
 
 def _song(id):
     return map_song(g.lib.get_item(int(id)))
 
 def playlist_provider():
-    _playlist_provider._dir = app.config['playlist_dir']
+    if 'playlist_dir' in app.config:
+        _playlist_provider.dir = app.config['playlist_dir']
+    if not _playlist_provider.dir:
+        app.logger.warning('No playlist_dir configured')
     return _playlist_provider
```

### Comparing `Beetstream-1.3.0/beetsplug/beetstream/search.py` & `beetstream-1.4.0/beetsplug/beetstream/search.py`

 * *Files identical despite different names*

### Comparing `Beetstream-1.3.0/beetsplug/beetstream/songs.py` & `beetstream-1.4.0/beetsplug/beetstream/songs.py`

 * *Files identical despite different names*

### Comparing `Beetstream-1.3.0/beetsplug/beetstream/stream.py` & `beetstream-1.4.0/beetsplug/beetstream/stream.py`

 * *Files identical despite different names*

### Comparing `Beetstream-1.3.0/beetsplug/beetstream/users.py` & `beetstream-1.4.0/beetsplug/beetstream/users.py`

 * *Files identical despite different names*

### Comparing `Beetstream-1.3.0/beetsplug/beetstream/utils.py` & `beetstream-1.4.0/beetsplug/beetstream/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,19 +7,23 @@
 import mimetypes
 import os
 import posixpath
 import xml.etree.cElementTree as ET
 from math import ceil
 from xml.dom import minidom
 
+DEFAULT_MIME_TYPE = 'application/octet-stream'
 EXTENSION_TO_MIME_TYPE_FALLBACK = {
     '.aac'  : 'audio/aac',
     '.flac' : 'audio/flac',
     '.mp3'  : 'audio/mpeg',
+    '.mp4'  : 'audio/mp4',
+    '.m4a'  : 'audio/mp4',
     '.ogg'  : 'audio/ogg',
+    '.opus' : 'audio/opus',
 }
 
 def strip_accents(s):
     return ''.join(c for c in unicodedata.normalize('NFD', s) if unicodedata.category(c) != 'Mn')
 
 def timestamp_to_iso(timestamp):
     return datetime.fromtimestamp(int(timestamp)).isoformat()
@@ -142,15 +146,15 @@
         "title": song["title"],
         "name": song["title"],
         "album": song["album"],
         "artist": song["albumartist"],
         "track": song["track"],
         "year": song["year"],
         "genre": song["genre"],
-        "coverArt": album_beetid_to_subid(str(song["album_id"])) or "",
+        "coverArt": _cover_art_id(song),
         "size": os.path.getsize(path),
         "contentType": path_to_content_type(path),
         "suffix": song["format"].lower(),
         "duration": ceil(song["length"]),
         "bitRate": ceil(song["bitrate"]/1000),
         "path": path,
         "playCount": 1, #TODO
@@ -171,29 +175,34 @@
     xml.set("title", song["title"])
     xml.set("name", song["title"])
     xml.set("album", song["album"])
     xml.set("artist", song["albumartist"])
     xml.set("track", str(song["track"]))
     xml.set("year", str(song["year"]))
     xml.set("genre", song["genre"])
-    xml.set("coverArt", album_beetid_to_subid(str(song["album_id"])) or "")
+    xml.set("coverArt", _cover_art_id(song)),
     xml.set("size", str(os.path.getsize(path)))
     xml.set("contentType", path_to_content_type(path))
     xml.set("suffix", song["format"].lower())
     xml.set("duration", str(ceil(song["length"])))
     xml.set("bitRate", str(ceil(song["bitrate"]/1000)))
     xml.set("path", path)
     xml.set("playCount", str(1)) #TODO
     xml.set("created", timestamp_to_iso(song["added"]))
     xml.set("albumId", album_beetid_to_subid(str(song["album_id"])))
     xml.set("artistId", artist_name_to_id(song["albumartist"]))
     xml.set("type", "music")
     if song["disc"]:
         xml.set("discNumber", str(song["disc"]))
 
+def _cover_art_id(song):
+    if song['album_id']:
+        return album_beetid_to_subid(str(song['album_id']))
+    return song_beetid_to_subid(str(song['id']))
+
 def map_artist(artist_name):
     return {
         "id": artist_name_to_id(artist_name),
         "name": artist_name,
         # TODO
         # "starred": "2021-07-03T06:15:28.757Z", # nothing if not starred
         "coverArt": "",
@@ -210,22 +219,24 @@
 
 def map_playlist(playlist):
     return {
         'id': playlist.id,
         'name': playlist.name,
         'songCount': playlist.count,
         'duration': playlist.duration,
+        'comment': playlist.artists,
         'created': timestamp_to_iso(playlist.modified),
     }
 
 def map_playlist_xml(xml, playlist):
     xml.set('id', playlist.id)
     xml.set('name', playlist.name)
     xml.set('songCount', str(playlist.count))
     xml.set('duration', str(ceil(playlist.duration)))
+    xml.set('comment', playlist.artists)
     xml.set('created', timestamp_to_iso(playlist.modified))
 
 def artist_name_to_id(name):
     base64_name = base64.b64encode(name.encode('utf-8')).decode('utf-8')
     return f"{ARTIST_ID_PREFIX}{base64_name}"
 
 def artist_id_to_name(id):
@@ -253,15 +264,17 @@
     # our mimetype database didn't have information about this file extension.
     base, ext = posixpath.splitext(path)
     result = EXTENSION_TO_MIME_TYPE_FALLBACK.get(ext)
 
     if result:
         return result
 
-    raise RuntimeError(f"Unable to determine content type for {path}")
+    flask.current_app.logger.warning(f"No mime type mapped for {ext} extension: {path}")
+
+    return DEFAULT_MIME_TYPE
 
 def handleSizeAndOffset(collection, size, offset):
     if size is not None:
         if offset is not None:
             return collection[offset:offset + size]
         else:
             return collection[0:size]
```

### Comparing `Beetstream-1.3.0/setup.cfg` & `beetstream-1.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Beetstream
-version = 1.3.0
+version = 1.4.0
 author = Binary Brain
 author_email = me@sachabron.ch
 description = Beets.io plugin that expose SubSonic API endpoints, allowing you to stream your music everywhere.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BinaryBrain/Beetstream
 project_urls =
```

