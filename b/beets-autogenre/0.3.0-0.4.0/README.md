# Comparing `tmp/beets_autogenre-0.3.0-py3-none-any.whl.zip` & `tmp/beets_autogenre-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12042 bytes, number of entries: 9
--rw-r--r--  2.0 unx       75 b- defN 24-Feb-12 00:07 beetsplug/__init__.py
--rw-r--r--  2.0 unx    13430 b- defN 24-Feb-12 00:07 beetsplug/autogenre/__init__.py
--rw-r--r--  2.0 unx      225 b- defN 24-Feb-12 00:07 beetsplug/autogenre/config_default.yaml
--rw-r--r--  2.0 unx     2077 b- defN 24-Feb-12 00:07 beetsplug/autogenre/genretree.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Feb-12 00:12 beets_autogenre-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5509 b- defN 24-Feb-12 00:12 beets_autogenre-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-12 00:12 beets_autogenre-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Feb-12 00:12 beets_autogenre-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      776 b- defN 24-Feb-12 00:12 beets_autogenre-0.3.0.dist-info/RECORD
-9 files, 33551 bytes uncompressed, 10692 bytes compressed:  68.1%
+Zip file size: 12576 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       75 b- defN 24-May-07 02:10 beetsplug/__init__.py
+-rw-r--r--  2.0 unx    15630 b- defN 24-May-07 02:10 beetsplug/autogenre/__init__.py
+-rw-r--r--  2.0 unx      225 b- defN 24-May-07 02:10 beetsplug/autogenre/config_default.yaml
+-rw-r--r--  2.0 unx     2077 b- defN 24-May-07 02:10 beetsplug/autogenre/genretree.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-07 02:11 beets_autogenre-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-07 02:11 beets_autogenre-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 02:11 beets_autogenre-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-07 02:11 beets_autogenre-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      776 b- defN 24-May-07 02:11 beets_autogenre-0.4.0.dist-info/RECORD
+9 files, 35751 bytes uncompressed, 11226 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: beetsplug/autogenre/config_default.yaml
 Comment: 
 
 Filename: beetsplug/autogenre/genretree.py
 Comment: 
 
-Filename: beets_autogenre-0.3.0.dist-info/LICENSE
+Filename: beets_autogenre-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: beets_autogenre-0.3.0.dist-info/METADATA
+Filename: beets_autogenre-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: beets_autogenre-0.3.0.dist-info/WHEEL
+Filename: beets_autogenre-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: beets_autogenre-0.3.0.dist-info/top_level.txt
+Filename: beets_autogenre-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: beets_autogenre-0.3.0.dist-info/RECORD
+Filename: beets_autogenre-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beetsplug/autogenre/__init__.py

```diff
@@ -1,13 +1,13 @@
 import codecs
 import mediafile
 import os
 import re
 import yaml
-from beets import ui
+from collections import Counter
 from beets.plugins import BeetsPlugin
 from beets.dbcore import types
 from beets.dbcore.query import FixedFieldSort
 from beets.library import Item, parse_query_parts
 from beets.ui import Subcommand, decargs
 from beets import config
 from optparse import OptionParser
@@ -54,14 +54,45 @@
         assert _is_plugin_enabled('lastgenre'), "The 'lastgenre' plugin is not enabled!"
         assert _is_plugin_enabled('xtractor'), "The 'xtractor' plugin is not enabled!"
         self._lastgenre = LastGenrePlugin()
         self._xtractor = XtractorCommand(config['xtractor'])
         self._lastgenre_conf = config['lastgenre'].get() or {}
         self._separator = self._lastgenre_conf.get('separator') or ', '
         self._remix_regex = re.compile(r'.+[^\w](remix|bootleg|remake)', re.IGNORECASE)
+        self._genre_tree = None
+        # TODO: add auto-detect support
+
+    def imported(self, session, task):
+        """Event hook called when an import task finishes."""
+        if task.is_album:
+            for item in task.album.items():
+                self._update_item_genre(item)
+
+            self._update_album_genre(task.album)
+        else:
+            self._update_item_genre(task.item)
+
+    def _update_item_genre(self, item):
+        genre, genres, source = self._item_genre(item, True, True)
+        self._log.info("Set track genre '{}' ({}): {}", genre, source, item)
+        item.genre = genre
+        item.genres = genres
+        item.genre_source = source
+        if not self.config['pretend'].get():
+            if config['import']['write'].get():
+                item.try_write()
+            item.store(['genre', 'genres', 'genre_source'])
+
+    def _update_album_genre(self, album):
+        genre = _most_common([item.genre for item in album.items()])
+        if album.genre != genre and genre:
+            album.genre = genre
+            self._log.info("Set genre '{}' for album {}", album.genre, album)
+            if not self.config['pretend'].get():
+                album.store(['genre'])
 
     def commands(self):
         p = OptionParser()
         p.add_option('--pretend', action='store_true',
             default=self.config['pretend'].get(),
             help='do not persist item changes but log them')
         p.add_option('-f', '--force', action='store_true',
@@ -101,91 +132,98 @@
             dest='genre', help='specify the genre to assign to the selected items')
 
         c = Subcommand('autogenre', parser=p, help='derive and assign song genres')
         c.func = self._run_autogenre_cmd
         return [c]
 
     def _run_autogenre_cmd(self, lib, opts, args):
-        genre_tree_file = self._lastgenre_conf.get('canonical')
-        if not genre_tree_file:
-            genre_tree_file = os.path.join(os.path.dirname(__file__), '..', 'lastgenre', 'genres-tree.yaml')
-        genre_wh_file = self._lastgenre_conf.get('whitelist')
-        assert genre_wh_file, "Config option lastgenre.whitelist is not specified!"
-        with open(genre_wh_file, 'r') as f:
-            genre_whitelist = [genre.strip().lower() for genre in f.readlines() if genre.strip()]
-        with codecs.open(genre_tree_file, 'r', encoding='utf-8') as f:
-            genre_tree_yaml = yaml.safe_load(f)
-        genre_tree = GenreTree(genre_tree_yaml, genre_whitelist)
+        self._apply_opts_to_config(opts)
         if opts.genre:
-            ok = genre_tree.contains(opts.genre)
+            ok = self._genres().contains(opts.genre)
             assert args, "Must specify selector when --genre provided"
             assert ok, "Provided genre '{}' is not registered within genre tree!".format(opts.genre)
         query = decargs(args)
         parsed_query, parsed_sort = parse_query_parts(query, Item)
         parsed_sort = FixedFieldSort("albumartist", ascending=True)
         items = lib.items(parsed_query, parsed_sort)
         all = opts.all or opts.genre is not None
         force = opts.force or opts.genre is not None
+        pretend = self.config['pretend'].get()
         filtered_items = [item for item in items if _filter_item(item, all, force)]
         self._log.info('Selected {} items for genre update...', len(filtered_items))
-        for item in items:
-            genres, source = self._item_genres(item, all, force, opts, genre_tree)
-            genrel = self._str2list(genres)
-            genre = genres and genrel[0] or None
-
-            if genres:
-                if opts.parent_genres and genre:
-                    # Append primary genre's parent genres to genre list
-                    parent_genres = genre_tree.parents(genre)
-                    parent_genres = [self._format_genre(g) for g in parent_genres]
-                    genrel = genrel + [g for g in parent_genres if g not in genrel]
-                    genres = self._list2str(genrel)
-
+        # Update items
+        for item in filtered_items:
+            genre, genres, source = self._item_genre(item, all, force, opts.genre)
             genre_changed = genre != item.get('genre')
             genres_changed = genres != item.get('genres')
             genre_source_changed = source != item.get('genre_source')
             changed = genre_changed or genres_changed or genre_source_changed
             if changed and genres is not None:
-                msg = "Changing genre from '{}' to '{}' ({}) for item: {}"
+                msg = "Change genre from '{}' to '{}' ({}) for item: {}"
                 self._log.info(msg, item.get('genre'), genre, source, item)
-                write = ui.should_write()
-                if not opts.pretend:
+                if not pretend:
                     item.genre = genre
                     item.genres = genres
                     item.genre_source = source
-                    if write:
+                    if config['import']['write'].get():
                         item.try_write()
                     item.store()
         # TODO: match remix artist within title and get genre from artist: TITLE (ARTIST remix)
+        # Update albums
+        album_ids = set([item.album_id for item in filtered_items if item.album_id])
+        for album_id in album_ids:
+            album = lib.get_album(album_id)
+            if album:
+                self._update_album_genre(album)
+
+    def _apply_opts_to_config(self, opts):
+        for k, v in opts.__dict__.items():
+            if v is not None and k in self.config:
+                self.config[k] = v
+
+    def _item_genre(self, item, all, force, force_genre=None):
+        genres, source = self._item_genres(item, all, force, force_genre)
+        genrel = self._str2list(genres)
+        genre = genres and genrel[0] or None
+
+        if genres:
+            if self.config['parent_genres'].get() and genre:
+                # Append primary genre's parent genres to genre list
+                parent_genres = self._genres().parents(genre)
+                parent_genres = [self._format_genre(g) for g in parent_genres]
+                genrel = genrel + [g for g in parent_genres if g not in genrel]
+                genres = self._list2str(genrel)
+
+        return genre, genres, source
 
-    def _item_genres(self, item, all, force, opts, genre_tree):
+    def _item_genres(self, item, all, force, force_genre):
         genre = item.get('genres')
         if not genre:
             genre = item.get('genre')
         source = item.get('genre_source')
         orig_genre = genre
         orig_source = source
         if _filter_item(item, all, force):
-            if opts.genre is not None:
-                source = opts.genre and 'user' or None
-                genre = self._format_genre(opts.genre.lower())
+            if force_genre is not None:
+                source = force_genre and 'user' or None
+                genre = self._format_genre(force_genre.lower())
             if source != 'user' or not genre:
                 # auto-detect genre
-                if opts.lastgenre:
+                if self.config['lastgenre'].get():
                     genre = self._lastfm_genre(item)
                     if genre is not None:
                         source = 'lastfm'
-                if genre is None and opts.xtractor:
+                if self.config['from_title'].get():
+                    genre, matched = self._fix_remix_genre(item, genre)
+                    if matched and genre is not None:
+                        source = 'title'
+                if genre is None and self.config['xtractor'].get():
                     genre = self._essentia_genre(item)
                     if genre is not None:
                         source = 'essentia'
-                if opts.from_title:
-                    genre, matched = self._fix_remix_genre(item, genre, genre_tree)
-                    if matched and genre is not None:
-                        source = 'title'
         return genre, source
 
     def _is_remix(self, title):
         return self._remix_regex.match(title) is not None
 
     def _lastfm_genre(self, item):
         genre = None
@@ -204,26 +242,26 @@
         else:
             genre, src = self._lastgenre._get_genre(item)
         if genre:
             msg = "Got last.fm genre '{}' based on {} for item: {}"
             self._log.debug(msg, genre, src, item)
         return genre
 
-    def _fix_remix_genre(self, item, genre, genre_tree):
+    def _fix_remix_genre(self, item, genre):
         '''Match genre within title or album and prepend to genre list.
         This fixes remixes that are wrongly tagged on last.fm'''
         title = item.get('title')
         album = item.get('album')
         genres = self._str2list(genre)
-        matched = genre_tree.match(title)
+        matched = self._genres().match(title)
         if matched:
             source = 'title'
         elif album:
             source = 'album'
-            matched = genre_tree.match(album)
+            matched = self._genres().match(album)
         prepend_genre = None
         if matched:
             prepend_genre = matched.lower()
         if prepend_genre:
             prepend_genre = self._format_genre(prepend_genre)
             genres = [g for g in genres if g != prepend_genre]
             genre = self._list2str([prepend_genre] + genres)
@@ -264,18 +302,32 @@
                 genres = self._str2list(genre)
                 if 'electronic' not in genres:
                     genre = self._list2str(genres + ['electronic'])
             elif genre == 'dance':
                 genre = 'electronic'
 
         genre = self._format_genre(genre)
-        msg = "Got essentia genre '{}' for item: {}"
-        self._log.debug(msg, genre, item)
+        self._log.debug("Got essentia genre '{}' for item: {}", genre, item)
         return genre
 
+    def _genres(self):
+        if not self._genre_tree:
+            genre_tree_file = self._lastgenre_conf.get('canonical')
+            if not genre_tree_file:
+                genre_tree_file = os.path.join(os.path.dirname(__file__), '..', 'lastgenre', 'genres-tree.yaml')
+            genre_wh_file = self._lastgenre_conf.get('whitelist')
+            assert genre_wh_file, "Config option lastgenre.whitelist is not specified!"
+            with open(genre_wh_file, 'r') as f:
+                genre_whitelist = [genre.strip().lower() for genre in f.readlines() if genre.strip()]
+            with codecs.open(genre_tree_file, 'r', encoding='utf-8') as f:
+                genre_tree_yaml = yaml.safe_load(f)
+            self._genre_tree = GenreTree(genre_tree_yaml, genre_whitelist)
+
+        return self._genre_tree
+
     def _format_genre(self, genre):
         return self._lastgenre._format_tag(genre)
 
     def _str2list(self, str):
         return str and str.split(self._separator) or []
 
     def _list2str(self, list):
@@ -286,7 +338,12 @@
     src = item.get('genre_source')
     empty = not item.get('genre')
     return (empty or src in SOURCES or not src and all) and (empty or force)
 
 def _is_plugin_enabled(plugin_name):
     enabled_plugins = config['plugins'].get() if config['plugins'].exists() else []
     return plugin_name in enabled_plugins
+
+def _most_common(names):
+    r = Counter([name for name in names if name]).most_common(1)
+    if len(r) == 1:
+        return r[0][0]
```

## Comparing `beets_autogenre-0.3.0.dist-info/LICENSE` & `beets_autogenre-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `beets_autogenre-0.3.0.dist-info/METADATA` & `beets_autogenre-0.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-autogenre
-Version: 0.3.0
+Version: 0.4.0
 Summary: Detect the genres for each song within your beets library
 Home-page: https://github.com/mgoltzsche/beets-autogenre
 Author: Max Goltzsche
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: Apache Software License
```

