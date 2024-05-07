# Comparing `tmp/ytmusic_deleter-2.2.2.tar.gz` & `tmp/ytmusic_deleter-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusic_deleter-2.2.2.tar", last modified: Tue Apr 23 02:54:28 2024, max compression
+gzip compressed data, was "ytmusic_deleter-2.3.0.tar", last modified: Tue May  7 02:32:09 2024, max compression
```

## Comparing `ytmusic_deleter-2.2.2.tar` & `ytmusic_deleter-2.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-04-23 02:54:12.319599 ytmusic_deleter-2.2.2/LICENSE
--rw-r--r--   0        0        0     1493 2024-04-23 02:54:28.243501 ytmusic_deleter-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     5030 2024-04-23 02:54:12.327599 ytmusic_deleter-2.2.2/tests/conftest.py
--rw-r--r--   0        0        0     1304 2024-04-23 02:54:12.327599 ytmusic_deleter-2.2.2/tests/resources/test.example.cfg
--rw-r--r--   0        0        0     2869 2024-04-23 02:54:12.327599 ytmusic_deleter-2.2.2/tests/test_cli.py
--rw-r--r--   0        0        0     5475 2024-04-23 02:54:12.327599 ytmusic_deleter-2.2.2/ytmusic_deleter/README.md
--rw-r--r--   0        0        0       22 2024-04-23 02:54:28.243501 ytmusic_deleter-2.2.2/ytmusic_deleter/_version.py
--rw-r--r--   0        0        0     1270 2024-04-23 02:54:12.327599 ytmusic_deleter-2.2.2/ytmusic_deleter/auth.py
--rw-r--r--   0        0        0    17213 2024-04-23 02:54:12.327599 ytmusic_deleter-2.2.2/ytmusic_deleter/cli.py
--rw-r--r--   0        0        0      168 2024-04-23 02:54:12.327599 ytmusic_deleter-2.2.2/ytmusic_deleter/constants.py
--rw-r--r--   0        0        0      319 2024-04-23 02:54:12.327599 ytmusic_deleter-2.2.2/ytmusic_deleter/progress.py
--rw-r--r--   0        0        0     9521 2024-04-23 02:54:12.327599 ytmusic_deleter-2.2.2/ytmusic_deleter/uploads.py
--rw-r--r--   0        0        0     5846 1970-01-01 00:00:00.000000 ytmusic_deleter-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-07 02:31:49.361217 ytmusic_deleter-2.3.0/LICENSE
+-rw-r--r--   0        0        0     1447 2024-05-07 02:32:09.001088 ytmusic_deleter-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5794 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1304 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/tests/resources/test.example.cfg
+-rw-r--r--   0        0        0     4090 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/tests/test_cli.py
+-rw-r--r--   0        0        0     5475 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/ytmusic_deleter/README.md
+-rw-r--r--   0        0        0       22 2024-05-07 02:32:09.001088 ytmusic_deleter-2.3.0/ytmusic_deleter/_version.py
+-rw-r--r--   0        0        0     1142 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/ytmusic_deleter/auth.py
+-rw-r--r--   0        0        0    20465 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/ytmusic_deleter/cli.py
+-rw-r--r--   0        0        0      168 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/ytmusic_deleter/constants.py
+-rw-r--r--   0        0        0      319 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/ytmusic_deleter/progress.py
+-rw-r--r--   0        0        0     9521 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/ytmusic_deleter/uploads.py
+-rw-r--r--   0        0        0     5846 1970-01-01 00:00:00.000000 ytmusic_deleter-2.3.0/PKG-INFO
```

### Comparing `ytmusic_deleter-2.2.2/LICENSE` & `ytmusic_deleter-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.2.2/pyproject.toml` & `ytmusic_deleter-2.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,19 +5,19 @@
     { name = "apastel", email = "alex.r.pastel@gmail.com" },
 ]
 description = "Easily delete your YouTube Music library"
 dependencies = [
     "click>=8.1.7",
     "enlighten>=1.12.4",
     "thefuzz>=0.22.1",
-    "ytmusicapi>=1.6.0",
+    "ytmusicapi>=1.7.0",
 ]
 requires-python = "<3.13,>=3.8.1"
 readme = "ytmusic_deleter/README.md"
-version = "2.2.2"
+version = "2.3.0"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.scripts]
 ytmusic-deleter = "ytmusic_deleter.cli:cli"
 
@@ -57,20 +57,18 @@
     "fbs[licensing,sentry,upload]>=1.2.1",
     "PySide6>=6.6.3.1",
 ]
 
 [tool.pdm.scripts]
 fbs = "sh fbs.sh"
 ytmusic-deleter = "ytmusic-deleter"
+generate = "bash gui/scripts/generate_ui_files.sh"
 version = "bash bump_versions.sh"
 freeze-prep = "bash gui/scripts/freeze_prep.sh"
 
-[tool.pdm.scripts.generate]
-shell = "cd %PDM_PROJECT_ROOT%/gui && scripts/generate_ui_files.sh"
-
 [tool.pdm.build]
 includes = [
     "ytmusic_deleter/**/*.py",
 ]
 
 [tool.pdm.version]
 source = "scm"
```

### Comparing `ytmusic_deleter-2.2.2/tests/resources/test.example.cfg` & `ytmusic_deleter-2.3.0/tests/resources/test.example.cfg`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.2.2/tests/test_cli.py` & `ytmusic_deleter-2.3.0/tests/test_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 
 from click.testing import CliRunner
+from ytmusic_deleter.cli import check_for_duplicates
 from ytmusic_deleter.cli import cli
 from ytmusicapi import YTMusic
 
 
 class TestCli:
     def test_delete_uploads(self, yt_browser: YTMusic, upload_song):
         assert upload_song
@@ -54,7 +55,30 @@
         print(result.stdout)
         assert result.exit_code == 0
         songs_unliked, songs_total = result.return_value
         assert songs_unliked >= 1, f"No songs were unliked. {songs_total} liked songs were found in total."
         time.sleep(5)
         likes_remaining = yt_oauth.get_liked_songs(limit=None)["tracks"]
         assert len(likes_remaining) == 0, f"There were still {len(likes_remaining)} liked songs remaining"
+
+    def test_delete_playlists(self, yt_oauth: YTMusic, create_playlist):
+        assert create_playlist
+        runner = CliRunner()
+        result = runner.invoke(cli, ["delete-playlists"], standalone_mode=False, obj=yt_oauth)
+        print(result.stdout)
+        assert result.exit_code == 0
+
+        playlists_deleted, playlists_total = result.return_value
+        assert playlists_deleted >= 1, f"No playlists were deleted. {playlists_total} were found in total."
+
+    def test_delete_playlist_duplicates(self, yt_oauth: YTMusic, playlist_with_dupes):
+        assert playlist_with_dupes
+        assert (
+            len(check_for_duplicates(playlist_with_dupes, yt_oauth)) > 0
+        ), "Playlist to work on did not contain any duplicates"
+        runner = CliRunner()
+        result = runner.invoke(cli, ["remove-duplicates", "Test Playlist"], standalone_mode=False, obj=yt_oauth)
+        print(result.stdout)
+        assert result.exit_code == 0
+
+        playlist_without_dupes = yt_oauth.get_playlist(playlist_with_dupes, limit=None)["id"]
+        assert len(check_for_duplicates(playlist_without_dupes, yt_oauth)) == 0, "Playlist still contained duplicates"
```

### Comparing `ytmusic_deleter-2.2.2/ytmusic_deleter/README.md` & `ytmusic_deleter-2.3.0/ytmusic_deleter/README.md`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.2.2/ytmusic_deleter/auth.py` & `ytmusic_deleter-2.3.0/ytmusic_deleter/auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,12 +25,9 @@
     except JSONDecodeError:
         logging.info(f"Creating file: {const.OAUTH_FILENAME}")
         ytmusicapi.setup_oauth(filepath=oauth_file_path, open_browser=True)
         yt_auth = YTMusic(oauth_file_path)
         logging.info(f'Created: {oauth_file_path}"')
     finally:
         if yt_auth:
-            try:
-                logging.info(f"Logged in as {yt_auth.get_account_info().get('accountName')!r}")
-            except KeyError:
-                logging.error("Unable to get account name of logged-in user")
+            logging.info(f"Logged in as {yt_auth.get_account_info().get('accountName')!r}")
     return yt_auth
```

### Comparing `ytmusic_deleter-2.2.2/ytmusic_deleter/cli.py` & `ytmusic_deleter-2.3.0/ytmusic_deleter/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import logging
+import logging.handlers
 import os
 import re
 import sys
+from itertools import groupby
+from operator import itemgetter
 from pathlib import Path
 from random import shuffle as unsort
 from time import strftime
 
 import click
 from click import get_current_context
 from ytmusic_deleter import constants as const
@@ -15,58 +17,66 @@
 from ytmusic_deleter.uploads import maybe_delete_uploaded_albums
 from ytmusicapi import YTMusic
 
 
 @click.group()
 @click.version_option(__version__)
 @click.option(
-    "--log-dir",
-    "-l",
-    default=os.getcwd(),
-    help="Custom directory in which to write log files, instead of current working directory.",
-)
-@click.option(
     "--credential-dir",
     "-c",
     default=os.getcwd(),
     help="Custom directory in which to locate/create JSON credential file, instead of current working directory",
 )
 @click.option(
     "--static-progress",
     "-p",
     is_flag=True,
     help="Log the progress statically instead of an animated progress bar",
 )
+@click.option(
+    "--log-dir",
+    "-l",
+    default=os.getcwd(),
+    help="Custom directory in which to write log files, instead of current working directory.",
+)
+@click.option("--no-logfile", "-n", is_flag=True, help="Only log to stdout, no file logging")
+@click.option("--verbose", "-v", is_flag=True, help="Enable verbose (debug) logging")
 @click.pass_context
-def cli(ctx, log_dir, credential_dir, static_progress):
+def cli(ctx, log_dir, credential_dir, static_progress, no_logfile, verbose):
     """Perform batch delete operations on your YouTube Music library."""
 
+    handlers = [logging.StreamHandler(sys.stdout)]
+    if not no_logfile:
+        handlers.append(logging.FileHandler(Path(log_dir) / f"ytmusic-deleter-cli_{strftime('%Y-%m-%d')}.log"))
     logging.basicConfig(
         force=True,
-        level=logging.INFO,
+        level=logging.DEBUG if verbose else logging.INFO,
         format="[%(asctime)s] %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
-        handlers=[
-            logging.FileHandler(Path(log_dir) / f"ytmusic-deleter_{strftime('%Y-%m-%d')}.log"),
-            logging.StreamHandler(sys.stdout),
-        ],
+        handlers=handlers,
     )
 
     if ctx.obj is not None:
         # Allows yt_auth to be provided by pytest
         yt_auth: YTMusic = ctx.obj
         logging.info(f"Logged in as {yt_auth.get_account_info().get('accountName')!r}")
     else:
         yt_auth: YTMusic = ensure_auth(credential_dir)
     ctx.ensure_object(dict)
     ctx.obj["STATIC_PROGRESS"] = static_progress
     ctx.obj["YT_AUTH"] = yt_auth
 
 
 @cli.command()
+def whoami():
+    """Print the name of the authenticated user, or sign in"""
+    pass
+
+
+@cli.command()
 @click.option(
     "--add-to-library",
     "-a",
     is_flag=True,
     help="Add the corresponding album to your library before deleting a song from uploads.",
 )
 @click.option(
@@ -149,15 +159,15 @@
 
 def remove_library_podcasts():
     yt_auth: YTMusic = get_current_context().obj["YT_AUTH"]
     logging.info("Retreiving all podcasts...")
     library_podcasts = yt_auth.get_library_podcasts(limit=None)
     # Filter out the "New Episodes" auto-playlist that can't be deleted
     library_podcasts = list(filter(lambda podcast: podcast["channel"]["id"], library_podcasts))
-    logging.info(f"Retrieved {len(library_podcasts)} from your library.")
+    logging.info(f"Retrieved {len(library_podcasts)} podcasts from your library.")
     global progress_bar
     progress_bar = manager.counter(
         total=len(library_podcasts),
         desc="Podcasts Removed",
         unit="podcasts",
         enabled=not get_current_context().obj["STATIC_PROGRESS"],
     )
@@ -271,26 +281,29 @@
     global progress_bar
     progress_bar = manager.counter(
         total=len(library_playlists),
         desc="Playlists Deleted",
         unit="playlists",
         enabled=not ctx.obj["STATIC_PROGRESS"],
     )
+    playlists_deleted = 0
     for playlist in library_playlists:
         logging.info(f"Processing playlist: {playlist['title']}")
         try:
             response = yt_auth.delete_playlist(playlist["playlistId"])
             if response:
                 logging.info(f"\tRemoved playlist {playlist['title']!r} from your library.")
+                playlists_deleted += 1
             else:
                 logging.error(f"\tFailed to remove playlist {playlist['title']!r} from your library.")
         except Exception:
             logging.error(f"\tCould not delete playlist {playlist['title']}. It might be a YT Music curated playlist.")
         update_progress()
-    logging.info("Finished deleting all playlists")
+    logging.info(f"Deleted {playlists_deleted} out of {len(library_playlists)} from your library.")
+    return (playlists_deleted, len(library_playlists))
 
 
 @cli.command()
 @click.pass_context
 def delete_history(ctx: click.Context):
     """
     Delete your play history. This does not currently work with brand accounts.
@@ -367,15 +380,15 @@
             desc=f'{selected_playlist["title"]!r} Tracks {"Shuffled" if shuffle else "Sorted"}',
             unit="tracks",
             enabled=not ctx.obj["STATIC_PROGRESS"],
         )
         for cur_track in desired_tracklist:
             cur_idx = desired_tracklist.index(cur_track)
             track_after = current_tracklist[cur_idx]
-            logging.debug(  # No way to actually enable debug logging yet
+            logging.debug(
                 f"Moving {cur_track['artists'][0]['name']} - {cur_track['title']} "
                 f"before {track_after['artists'][0]['name']} - {track_after['title']}"
             )
             if cur_track != track_after:
                 try:
                     response = yt_auth.edit_playlist(
                         playlist["id"],
@@ -418,14 +431,80 @@
         album_title = album["name"] if album else "z"
         return (re.sub(r"^(the |a )", "", artist), album_title, track["title"])
     except Exception:
         logging.exception(f"Track {track} could not be sorted.")
         raise
 
 
+@cli.command()
+@click.argument("playlist_title")
+@click.pass_context
+def remove_duplicates(ctx: click.Context, playlist_title):
+    """Delete all duplicates in a given playlist"""
+    yt_auth: YTMusic = ctx.obj["YT_AUTH"]
+    # Get all playlists
+    all_playlists = yt_auth.get_library_playlists(limit=None)
+    # Get the ID of the matching playlist
+    selected_playlist_id = next(
+        (
+            playlist["playlistId"]
+            for playlist in all_playlists
+            if playlist.get("title").lower() == playlist_title.lower()
+        ),
+        None,
+    )
+    if not selected_playlist_id:
+        raise click.BadParameter(
+            f"No playlist found named {playlist_title!r}. Double-check your playlist name "
+            '(or surround it "with quotes") and try again.'
+        )
+    # Get a list of all the sets of duplicates
+    duplicates = check_for_duplicates(selected_playlist_id)
+    if not duplicates:
+        logging.info("No duplicates found. If you think this is an error open an issue on GitHub or message on Discord")
+    # For each dupe group, remove all but the first song
+    for duplicate_group in duplicates:
+        master_track = duplicate_group[0]
+        logging.info(
+            f"The following track(s) are a duplicate of {master_track.get('artist')} - {master_track.get('title')!r} "
+            "and will be removed:"
+        )
+        items_to_remove = duplicate_group[1:]
+        for item in items_to_remove:
+            logging.info(f"\t{item.get('artist')} - {item.get('title')!r}")
+        yt_auth.remove_playlist_items(selected_playlist_id, items_to_remove)
+
+
+def check_for_duplicates(playlist_id: str, yt_auth: YTMusic = None):
+    # Allow passing in yt_auth from pytest
+    if not yt_auth:
+        yt_auth: YTMusic = get_current_context().obj["YT_AUTH"]
+    # Get the playlist object
+    playlist = yt_auth.get_playlist(playlist_id)
+    logging.info(f"Checking for duplicates in playlist {playlist.get('title')!r}")
+    tracks = playlist.get("tracks")
+    # Trim the fat of the tracks object
+    tracks = [
+        {
+            "artist": track.get("artists")[0].get("name"),
+            "title": track.get("title"),
+            "videoId": track.get("videoId"),
+            "setVideoId": track.get("setVideoId"),
+        }
+        for track in tracks
+    ]
+
+    # Create a list of groups of duplicate tracks, where dupes are determined by having the same videoId
+    tracks.sort(key=itemgetter("videoId"))
+    grouped_tracks = [(key, list(group)) for key, group in groupby(tracks, lambda item: item["videoId"])]
+    grouped_tracks = [group for key, group in grouped_tracks if len(group) > 1]
+
+    return grouped_tracks
+
+
 def update_progress():
     global progress_bar
     progress_bar.update()
     if get_current_context().obj["STATIC_PROGRESS"]:
         logging.info(f"Total complete: {round(progress_bar.count / progress_bar.total * 100)}%")
```

### Comparing `ytmusic_deleter-2.2.2/ytmusic_deleter/uploads.py` & `ytmusic_deleter-2.3.0/ytmusic_deleter/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.2.2/PKG-INFO` & `ytmusic_deleter-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ytmusic-deleter
-Version: 2.2.2
+Version: 2.3.0
 Summary: Easily delete your YouTube Music library
 Author-Email: apastel <alex.r.pastel@gmail.com>
 License: GPL-3.0
 Requires-Python: <3.13,>=3.8.1
 Requires-Dist: click>=8.1.7
 Requires-Dist: enlighten>=1.12.4
 Requires-Dist: thefuzz>=0.22.1
-Requires-Dist: ytmusicapi>=1.6.0
+Requires-Dist: ytmusicapi>=1.7.0
 Description-Content-Type: text/markdown
 
 # ytmusic-deleter: Delete your YouTube Music library
 ![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/apastel/ytmusic-deleter/total?label=.exe%20Downloads)  
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ytmusic-deleter?logo=pypi&logoColor=yellow&label=PyPI%20Downloads)](https://pypi.org/project/ytmusic-deleter/)  
 ![GitHub Release](https://img.shields.io/github/v/release/apastel/ytmusic-deleter)  
 [![Release test](https://github.com/apastel/ytmusic-deleter/actions/workflows/build-exe.yml/badge.svg)](https://github.com/apastel/ytmusic-deleter/actions/workflows/build-exe.yml)
```

