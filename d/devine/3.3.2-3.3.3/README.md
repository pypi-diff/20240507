# Comparing `tmp/devine-3.3.2.tar.gz` & `tmp/devine-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devine-3.3.2.tar", max compression
+gzip compressed data, was "devine-3.3.3.tar", max compression
```

## Comparing `devine-3.3.2.tar` & `devine-3.3.3.tar`

### file list

```diff
@@ -1,69 +1,71 @@
--rw-r--r--   0        0        0    55720 2024-04-16 05:07:34.820728 devine-3.3.2/CHANGELOG.md
--rw-r--r--   0        0        0    35822 2024-04-16 05:07:34.820728 devine-3.3.2/LICENSE
--rw-r--r--   0        0        0    20271 2024-04-16 05:07:34.820728 devine-3.3.2/README.md
--rw-r--r--   0        0        0       80 2024-04-16 05:07:34.820728 devine-3.3.2/devine/__main__.py
--rw-r--r--   0        0        0        0 2024-04-16 05:07:34.820728 devine-3.3.2/devine/commands/__init__.py
--rw-r--r--   0        0        0     3293 2024-04-16 05:07:34.820728 devine-3.3.2/devine/commands/cfg.py
--rw-r--r--   0        0        0    45886 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/dl.py
--rw-r--r--   0        0        0     2182 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/env.py
--rw-r--r--   0        0        0     7986 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/kv.py
--rw-r--r--   0        0        0     6574 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/search.py
--rw-r--r--   0        0        0     1743 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/serve.py
--rw-r--r--   0        0        0     9243 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/util.py
--rw-r--r--   0        0        0     9920 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/wvd.py
--rw-r--r--   0        0        0       22 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/__init__.py
--rw-r--r--   0        0        0     2857 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/__main__.py
--rw-r--r--   0        0        0     6195 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/cacher.py
--rw-r--r--   0        0        0     1215 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/commands.py
--rw-r--r--   0        0        0     4481 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/config.py
--rw-r--r--   0        0        0    15343 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/console.py
--rw-r--r--   0        0        0     1065 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/constants.py
--rw-r--r--   0        0        0     3380 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/credential.py
--rw-r--r--   0        0        0      159 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/downloaders/__init__.py
--rw-r--r--   0        0        0    13339 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/downloaders/aria2c.py
--rw-r--r--   0        0        0    11697 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/downloaders/curl_impersonate.py
--rw-r--r--   0        0        0    11930 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/downloaders/requests.py
--rw-r--r--   0        0        0      199 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/drm/__init__.py
--rw-r--r--   0        0        0     4020 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/drm/clearkey.py
--rw-r--r--   0        0        0    11898 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/drm/widevine.py
--rw-r--r--   0        0        0     2818 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/events.py
--rw-r--r--   0        0        0       71 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/manifests/__init__.py
--rw-r--r--   0        0        0    31280 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/manifests/dash.py
--rw-r--r--   0        0        0    28517 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/manifests/hls.py
--rw-r--r--   0        0        0      117 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/proxies/__init__.py
--rw-r--r--   0        0        0     1893 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/proxies/basic.py
--rw-r--r--   0        0        0     2290 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/proxies/hola.py
--rw-r--r--   0        0        0     5565 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/proxies/nordvpn.py
--rw-r--r--   0        0        0     1048 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/proxies/proxy.py
--rw-r--r--   0        0        0     1714 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/search_result.py
--rw-r--r--   0        0        0    12729 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/service.py
--rw-r--r--   0        0        0     3001 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/services.py
--rw-r--r--   0        0        0      298 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/titles/__init__.py
--rw-r--r--   0        0        0     8002 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/titles/episode.py
--rw-r--r--   0        0        0     5538 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/titles/movie.py
--rw-r--r--   0        0        0     4689 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/titles/song.py
--rw-r--r--   0        0        0     2595 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/titles/title.py
--rw-r--r--   0        0        0      277 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/tracks/__init__.py
--rw-r--r--   0        0        0     2132 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/attachment.py
--rw-r--r--   0        0        0     7412 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/audio.py
--rw-r--r--   0        0        0     2976 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/chapter.py
--rw-r--r--   0        0        0     5352 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/chapters.py
--rw-r--r--   0        0        0    24647 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/subtitle.py
--rw-r--r--   0        0        0    21612 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/track.py
--rw-r--r--   0        0        0    17269 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/tracks.py
--rw-r--r--   0        0        0    16638 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/video.py
--rw-r--r--   0        0        0    10741 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utilities.py
--rw-r--r--   0        0        0        0 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utils/__init__.py
--rw-r--r--   0        0        0     6227 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utils/click_types.py
--rw-r--r--   0        0        0     1532 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utils/collections.py
--rw-r--r--   0        0        0     3699 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utils/sslciphers.py
--rw-r--r--   0        0        0      845 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utils/subprocess.py
--rw-r--r--   0        0        0      791 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utils/xml.py
--rw-r--r--   0        0        0     1711 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/vault.py
--rw-r--r--   0        0        0     2518 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/vaults.py
--rw-r--r--   0        0        0     6414 2024-04-16 05:07:34.828728 devine-3.3.2/devine/vaults/API.py
--rw-r--r--   0        0        0     8485 2024-04-16 05:07:34.828728 devine-3.3.2/devine/vaults/MySQL.py
--rw-r--r--   0        0        0     6076 2024-04-16 05:07:34.828728 devine-3.3.2/devine/vaults/SQLite.py
--rw-r--r--   0        0        0        0 2024-04-16 05:07:34.828728 devine-3.3.2/devine/vaults/__init__.py
--rw-r--r--   0        0        0     2496 2024-04-16 05:07:34.828728 devine-3.3.2/pyproject.toml
--rw-r--r--   0        0        0    22752 1970-01-01 00:00:00.000000 devine-3.3.2/PKG-INFO
+-rw-r--r--   0        0        0    56512 2024-05-07 06:10:55.594800 devine-3.3.3/CHANGELOG.md
+-rw-r--r--   0        0        0    35822 2024-05-07 06:10:55.594800 devine-3.3.3/LICENSE
+-rw-r--r--   0        0        0    20271 2024-05-07 06:10:55.594800 devine-3.3.3/README.md
+-rw-r--r--   0        0        0       80 2024-05-07 06:10:55.594800 devine-3.3.3/devine/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:10:55.594800 devine-3.3.3/devine/commands/__init__.py
+-rw-r--r--   0        0        0     3293 2024-05-07 06:10:55.598800 devine-3.3.3/devine/commands/cfg.py
+-rw-r--r--   0        0        0    46349 2024-05-07 06:10:55.598800 devine-3.3.3/devine/commands/dl.py
+-rw-r--r--   0        0        0     3139 2024-05-07 06:10:55.598800 devine-3.3.3/devine/commands/env.py
+-rw-r--r--   0        0        0     7986 2024-05-07 06:10:55.598800 devine-3.3.3/devine/commands/kv.py
+-rw-r--r--   0        0        0     6546 2024-05-07 06:10:55.598800 devine-3.3.3/devine/commands/search.py
+-rw-r--r--   0        0        0     1688 2024-05-07 06:10:55.598800 devine-3.3.3/devine/commands/serve.py
+-rw-r--r--   0        0        0     9125 2024-05-07 06:10:55.598800 devine-3.3.3/devine/commands/util.py
+-rw-r--r--   0        0        0     9920 2024-05-07 06:10:55.598800 devine-3.3.3/devine/commands/wvd.py
+-rw-r--r--   0        0        0       22 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/__init__.py
+-rw-r--r--   0        0        0     2857 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/__main__.py
+-rw-r--r--   0        0        0      981 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/binaries.py
+-rw-r--r--   0        0        0     6195 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/cacher.py
+-rw-r--r--   0        0        0     1215 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/commands.py
+-rw-r--r--   0        0        0     4337 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/config.py
+-rw-r--r--   0        0        0    15343 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/console.py
+-rw-r--r--   0        0        0     1065 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/constants.py
+-rw-r--r--   0        0        0     3380 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/credential.py
+-rw-r--r--   0        0        0      159 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/downloaders/__init__.py
+-rw-r--r--   0        0        0    13311 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/downloaders/aria2c.py
+-rw-r--r--   0        0        0    11411 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/downloaders/curl_impersonate.py
+-rw-r--r--   0        0        0    11930 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/downloaders/requests.py
+-rw-r--r--   0        0        0      199 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/drm/__init__.py
+-rw-r--r--   0        0        0     4020 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/drm/clearkey.py
+-rw-r--r--   0        0        0    11723 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/drm/widevine.py
+-rw-r--r--   0        0        0     2818 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/events.py
+-rw-r--r--   0        0        0       71 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/manifests/__init__.py
+-rw-r--r--   0        0        0    31826 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/manifests/dash.py
+-rw-r--r--   0        0        0    28680 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/manifests/hls.py
+-rw-r--r--   0        0        0      117 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/proxies/__init__.py
+-rw-r--r--   0        0        0     1893 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/proxies/basic.py
+-rw-r--r--   0        0        0     2262 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/proxies/hola.py
+-rw-r--r--   0        0        0     5565 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/proxies/nordvpn.py
+-rw-r--r--   0        0        0     1048 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/proxies/proxy.py
+-rw-r--r--   0        0        0     1714 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/search_result.py
+-rw-r--r--   0        0        0    12729 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/service.py
+-rw-r--r--   0        0        0     3001 2024-05-07 06:10:55.598800 devine-3.3.3/devine/core/services.py
+-rw-r--r--   0        0        0      298 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/titles/__init__.py
+-rw-r--r--   0        0        0     8002 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/titles/episode.py
+-rw-r--r--   0        0        0     5538 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/titles/movie.py
+-rw-r--r--   0        0        0     4689 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/titles/song.py
+-rw-r--r--   0        0        0     2595 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/titles/title.py
+-rw-r--r--   0        0        0      277 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/tracks/__init__.py
+-rw-r--r--   0        0        0     2132 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/tracks/attachment.py
+-rw-r--r--   0        0        0     7412 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/tracks/audio.py
+-rw-r--r--   0        0        0     2976 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/tracks/chapter.py
+-rw-r--r--   0        0        0     5352 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/tracks/chapters.py
+-rw-r--r--   0        0        0    25890 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/tracks/subtitle.py
+-rw-r--r--   0        0        0    21591 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/tracks/track.py
+-rw-r--r--   0        0        0    17269 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/tracks/tracks.py
+-rw-r--r--   0        0        0    16508 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/tracks/video.py
+-rw-r--r--   0        0        0    10497 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/utilities.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/utils/__init__.py
+-rw-r--r--   0        0        0     6227 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/utils/click_types.py
+-rw-r--r--   0        0        0     1532 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/utils/collections.py
+-rw-r--r--   0        0        0     3699 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/utils/sslciphers.py
+-rw-r--r--   0        0        0     1008 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/utils/subprocess.py
+-rw-r--r--   0        0        0     7411 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/utils/webvtt.py
+-rw-r--r--   0        0        0      791 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/utils/xml.py
+-rw-r--r--   0        0        0     1711 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/vault.py
+-rw-r--r--   0        0        0     2518 2024-05-07 06:10:55.602800 devine-3.3.3/devine/core/vaults.py
+-rw-r--r--   0        0        0     6414 2024-05-07 06:10:55.602800 devine-3.3.3/devine/vaults/API.py
+-rw-r--r--   0        0        0     8485 2024-05-07 06:10:55.602800 devine-3.3.3/devine/vaults/MySQL.py
+-rw-r--r--   0        0        0     6076 2024-05-07 06:10:55.602800 devine-3.3.3/devine/vaults/SQLite.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:10:55.602800 devine-3.3.3/devine/vaults/__init__.py
+-rw-r--r--   0        0        0     2450 2024-05-07 06:10:55.602800 devine-3.3.3/pyproject.toml
+-rw-r--r--   0        0        0    22664 1970-01-01 00:00:00.000000 devine-3.3.3/PKG-INFO
```

### Comparing `devine-3.3.2/CHANGELOG.md` & `devine-3.3.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,33 @@
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Versions [3.0.0] and older use a format based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 but versions thereafter use a custom changelog format using [git-cliff](https://git-cliff.org).
 
+## [3.3.3] - 2024-05-07
+
+### Bug Fixes
+
+- *dl*: Automatically convert TTML Subs to WebVTT for MKV support
+- *Subtitle*: Correct timestamps when merging fragmented WebVTT
+
+### Changes
+
+- *env*: List all directories as table in info
+- *env*: List possible config path locations when not found
+- *binaries*: Move all binary definitions to core/binaries file
+- *curl-impersonate*: Remove manual fix for curl proxy SSL
+- *curl-impersonate*: Update the default browser to chrome124
+- *Config*: Move possible config paths out of func to constant
+- *utilities*: Remove get_binary_path, use binaries.find instead
+- *dl*: Improve readability of download worker errors
+- *env*: Shorten paths on Windows with env vars
+
 ## [3.3.2] - 2024-04-16
 
 ### Bug Fixes
 
 - *Video*: Ensure track is supported in change_color_range()
 - *Video*: Optionalise constructor args, add doc-string & checks
 - *Audio*: Optionalise constructor args, add doc-string & checks
@@ -791,14 +810,15 @@
 - Fixed crash when adding a Cookie using `auth add` to a Service that has no directory yet.
 - Fixed crash when adding a Credential using `auth add` when it's the first ever credential, or first for the Service.
 
 ## [1.0.0] - 2023-02-06
 
 Initial public release under the name Devine.
 
+[3.3.3]: https://github.com/devine-dl/devine/releases/tag/v3.3.3
 [3.3.2]: https://github.com/devine-dl/devine/releases/tag/v3.3.2
 [3.3.1]: https://github.com/devine-dl/devine/releases/tag/v3.3.1
 [3.3.0]: https://github.com/devine-dl/devine/releases/tag/v3.3.0
 [3.2.0]: https://github.com/devine-dl/devine/releases/tag/v3.2.0
 [3.1.0]: https://github.com/devine-dl/devine/releases/tag/v3.1.0
 [3.0.0]: https://github.com/devine-dl/devine/releases/tag/v3.0.0
 [2.2.0]: https://github.com/devine-dl/devine/releases/tag/v2.2.0
```

### Comparing `devine-3.3.2/LICENSE` & `devine-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/README.md` & `devine-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/commands/cfg.py` & `devine-3.3.3/devine/commands/cfg.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/commands/dl.py` & `devine-3.3.3/devine/commands/dl.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,28 +34,29 @@
 from rich.panel import Panel
 from rich.progress import BarColumn, Progress, SpinnerColumn, TaskID, TextColumn, TimeRemainingColumn
 from rich.rule import Rule
 from rich.table import Table
 from rich.text import Text
 from rich.tree import Tree
 
+from devine.core import binaries
 from devine.core.config import config
 from devine.core.console import console
 from devine.core.constants import DOWNLOAD_LICENCE_ONLY, AnyTrack, context_settings
 from devine.core.credential import Credential
 from devine.core.drm import DRM_T, Widevine
 from devine.core.events import events
 from devine.core.proxies import Basic, Hola, NordVPN
 from devine.core.service import Service
 from devine.core.services import Services
 from devine.core.titles import Movie, Song, Title_T
 from devine.core.titles.episode import Episode
 from devine.core.tracks import Audio, Subtitle, Tracks, Video
 from devine.core.tracks.attachment import Attachment
-from devine.core.utilities import get_binary_path, get_system_fonts, is_close_match, time_elapsed_since
+from devine.core.utilities import get_system_fonts, is_close_match, time_elapsed_since
 from devine.core.utils.click_types import LANGUAGE_RANGE, QUALITY_LIST, SEASON_RANGE, ContextData, MultipleChoice
 from devine.core.utils.collections import merge_dict
 from devine.core.utils.subprocess import ffprobe
 from devine.core.vaults import Vaults
 
 
 class dl:
@@ -194,15 +195,15 @@
             ctx.params["proxy"] = None
         else:
             with console.status("Loading Proxy Providers...", spinner="dots"):
                 if config.proxy_providers.get("basic"):
                     self.proxy_providers.append(Basic(**config.proxy_providers["basic"]))
                 if config.proxy_providers.get("nordvpn"):
                     self.proxy_providers.append(NordVPN(**config.proxy_providers["nordvpn"]))
-                if get_binary_path("hola-proxy"):
+                if binaries.HolaProxy:
                     self.proxy_providers.append(Hola())
                 for proxy_provider in self.proxy_providers:
                     self.log.info(f"Loaded {proxy_provider.__class__.__name__}: {proxy_provider}")
 
             if proxy:
                 requested_provider = None
                 if re.match(r"^[a-z]+:.+$", proxy, re.IGNORECASE):
@@ -542,22 +543,25 @@
                     ":x: Download Cancelled...",
                     (0, 5, 1, 5)
                 ))
                 return
             except Exception as e:  # noqa
                 error_messages = [
                     ":x: Download Failed...",
-                    "   One of the track downloads had an error!",
-                    "   See the error trace above for more information."
                 ]
-                if isinstance(e, subprocess.CalledProcessError):
-                    # ignore process exceptions as proper error logs are already shown
-                    error_messages.append(f"   Process exit code: {e.returncode}")
+                if isinstance(e, EnvironmentError):
+                    error_messages.append(f"   {e}")
                 else:
-                    console.print_exception()
+                    error_messages.append("   An unexpected error occurred in one of the download workers.",)
+                    if hasattr(e, "returncode"):
+                        error_messages.append(f"   Binary call failed, Process exit code: {e.returncode}")
+                    error_messages.append("   See the error trace above for more information.")
+                    if isinstance(e, subprocess.CalledProcessError):
+                        # CalledProcessError already lists the exception trace
+                        console.print_exception()
                 console.print(Padding(
                     Group(*error_messages),
                     (1, 5)
                 ))
                 return
 
             if skip_dl:
@@ -606,19 +610,22 @@
                         except EnvironmentError:
                             self.log.error(
                                 "Cannot extract Closed Captions as the ccextractor executable was not found..."
                             )
                             break
                     video_track_n += 1
 
-                if sub_format:
-                    with console.status(f"Converting Subtitles to {sub_format.name}..."):
-                        for subtitle in title.tracks.subtitles:
+                with console.status("Converting Subtitles..."):
+                    for subtitle in title.tracks.subtitles:
+                        if sub_format:
                             if subtitle.codec != sub_format:
                                 subtitle.convert(sub_format)
+                        elif subtitle.codec == Subtitle.Codec.TimedTextMarkupLang:
+                            # MKV does not support TTML, VTT is the next best option
+                            subtitle.convert(Subtitle.Codec.WebVTT)
 
                 with console.status("Checking Subtitles for Fonts..."):
                     font_names = []
                     for subtitle in title.tracks.subtitles:
                         if subtitle.codec == Subtitle.Codec.SubStationAlphav4:
                             for line in subtitle.path.read_text("utf8").splitlines():
                                 if line.startswith("Style: "):
```

### Comparing `devine-3.3.2/devine/commands/kv.py` & `devine-3.3.3/devine/commands/kv.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/commands/search.py` & `devine-3.3.3/devine/commands/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 import click
 import yaml
 from rich.padding import Padding
 from rich.rule import Rule
 from rich.tree import Tree
 
 from devine.commands.dl import dl
+from devine.core import binaries
 from devine.core.config import config
 from devine.core.console import console
 from devine.core.constants import context_settings
 from devine.core.proxies import Basic, Hola, NordVPN
 from devine.core.service import Service
 from devine.core.services import Services
-from devine.core.utilities import get_binary_path
 from devine.core.utils.click_types import ContextData
 from devine.core.utils.collections import merge_dict
 
 
 @click.command(
     short_help="Search for titles from a Service.",
     cls=Services,
@@ -68,15 +68,15 @@
         ctx.params["proxy"] = None
     else:
         with console.status("Loading Proxy Providers...", spinner="dots"):
             if config.proxy_providers.get("basic"):
                 proxy_providers.append(Basic(**config.proxy_providers["basic"]))
             if config.proxy_providers.get("nordvpn"):
                 proxy_providers.append(NordVPN(**config.proxy_providers["nordvpn"]))
-            if get_binary_path("hola-proxy"):
+            if binaries.HolaProxy:
                 proxy_providers.append(Hola())
             for proxy_provider in proxy_providers:
                 log.info(f"Loaded {proxy_provider.__class__.__name__}: {proxy_provider}")
 
         if proxy:
             requested_provider = None
             if re.match(r"^[a-z]+:.+$", proxy, re.IGNORECASE):
```

### Comparing `devine-3.3.2/devine/commands/serve.py` & `devine-3.3.3/devine/commands/serve.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import subprocess
 
 import click
 
+from devine.core import binaries
 from devine.core.config import config
 from devine.core.constants import context_settings
-from devine.core.utilities import get_binary_path
 
 
 @click.command(
     short_help="Serve your Local Widevine Devices for Remote Access.",
     context_settings=context_settings)
 @click.option("-h", "--host", type=str, default="0.0.0.0", help="Host to serve from.")
 @click.option("-p", "--port", type=int, default=8786, help="Port to serve from.")
@@ -25,19 +25,18 @@
     You may serve with Caddy at the same time with --caddy. You can use Caddy
     as a reverse-proxy to serve with HTTPS. The config used will be the Caddyfile
     next to the devine config.
     """
     from pywidevine import serve
 
     if caddy:
-        executable = get_binary_path("caddy")
-        if not executable:
+        if not binaries.Caddy:
             raise click.ClickException("Caddy executable \"caddy\" not found but is required for --caddy.")
         caddy_p = subprocess.Popen([
-            executable,
+            binaries.Caddy,
             "run",
             "--config", str(config.directories.user_configs / "Caddyfile")
         ])
     else:
         caddy_p = None
 
     try:
```

### Comparing `devine-3.3.2/devine/commands/util.py` & `devine-3.3.3/devine/commands/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import subprocess
 from pathlib import Path
 
 import click
 from pymediainfo import MediaInfo
 
+from devine.core import binaries
 from devine.core.constants import context_settings
-from devine.core.utilities import get_binary_path
 
 
 @click.group(short_help="Various helper scripts and programs.", context_settings=context_settings)
 def util() -> None:
     """Various helper scripts and programs."""
 
 
@@ -34,16 +34,15 @@
     cases, again due to sub-sampled chroma.
 
     It's recommended that you try -o about 10 or so pixels and lower it until
     you get as close in as possible. Do make sure it's not over-cropping either
     as it may go from being 2px away from a perfect crop, to 20px over-cropping
     again due to sub-sampled chroma.
     """
-    executable = get_binary_path("ffmpeg")
-    if not executable:
+    if not binaries.FFMPEG:
         raise click.ClickException("FFmpeg executable \"ffmpeg\" not found but is required.")
 
     if path.is_dir():
         paths = list(path.glob("*.mkv")) + list(path.glob("*.mp4"))
     else:
         paths = [path]
     for video_path in paths:
@@ -83,23 +82,23 @@
                     # ffmpeg's MKV muxer does not yet support HDR
                     "HEVC": "h265",
                     "AVC": "h264"
                 }.get(video_track.commercial_name, ".mp4")
             ]))))]
 
         ffmpeg_call = subprocess.Popen([
-            executable, "-y",
+            binaries.FFMPEG, "-y",
             "-i", str(video_path),
             "-map", "0:v:0",
             "-c", "copy",
             "-bsf:v", crop_filter
         ] + out_path, stdout=subprocess.PIPE)
         try:
             if preview:
-                previewer = get_binary_path("mpv", "ffplay")
+                previewer = binaries.MPV or binaries.FFPlay
                 if not previewer:
                     raise click.ClickException("MPV/FFplay executables weren't found but are required for previewing.")
                 subprocess.Popen((previewer, "-"), stdin=ffmpeg_call.stdout)
         finally:
             if ffmpeg_call.stdout:
                 ffmpeg_call.stdout.close()
             ffmpeg_call.wait()
@@ -116,16 +115,15 @@
     Losslessly set the Video Range flag to full or limited at the bit-stream level.
     You may provide a path to a file, or a folder of mkv and/or mp4 files.
 
     If you ever notice blacks not being quite black, and whites not being quite white,
     then you're video may have the range set to the wrong value. Flip its range to the
     opposite value and see if that fixes it.
     """
-    executable = get_binary_path("ffmpeg")
-    if not executable:
+    if not binaries.FFMPEG:
         raise click.ClickException("FFmpeg executable \"ffmpeg\" not found but is required.")
 
     if path.is_dir():
         paths = list(path.glob("*.mkv")) + list(path.glob("*.mp4"))
     else:
         paths = [path]
     for video_path in paths:
@@ -153,23 +151,23 @@
                     # ffmpeg's MKV muxer does not yet support HDR
                     "HEVC": "h265",
                     "AVC": "h264"
                 }.get(video_track.commercial_name, ".mp4")
             ]))))]
 
         ffmpeg_call = subprocess.Popen([
-            executable, "-y",
+            binaries.FFMPEG, "-y",
             "-i", str(video_path),
             "-map", "0:v:0",
             "-c", "copy",
             "-bsf:v", f"{metadata_key}=video_full_range_flag={int(full)}"
         ] + out_path, stdout=subprocess.PIPE)
         try:
             if preview:
-                previewer = get_binary_path("mpv", "ffplay")
+                previewer = binaries.MPV or binaries.FFPlay
                 if not previewer:
                     raise click.ClickException("MPV/FFplay executables weren't found but are required for previewing.")
                 subprocess.Popen((previewer, "-"), stdin=ffmpeg_call.stdout)
         finally:
             if ffmpeg_call.stdout:
                 ffmpeg_call.stdout.close()
             ffmpeg_call.wait()
@@ -184,26 +182,25 @@
     Decode an entire video and check for any corruptions or errors using FFmpeg.
     You may provide a path to a file, or a folder of mkv and/or mp4 files.
 
     Tests all streams within the file by default. Subtitles cannot be tested.
     You may choose specific streams using the -m/--map parameter. E.g.,
     '0:v:0' to test the first video stream, or '0:a' to test all audio streams.
     """
-    executable = get_binary_path("ffmpeg")
-    if not executable:
+    if not binaries.FFMPEG:
         raise click.ClickException("FFmpeg executable \"ffmpeg\" not found but is required.")
 
     if path.is_dir():
         paths = list(path.glob("*.mkv")) + list(path.glob("*.mp4"))
     else:
         paths = [path]
     for video_path in paths:
         print("Starting...")
         p = subprocess.Popen([
-            executable, "-hide_banner",
+            binaries.FFMPEG, "-hide_banner",
             "-benchmark",
             "-i", str(video_path),
             "-map", map_,
             "-sn",
             "-f", "null",
             "-"
         ], stderr=subprocess.PIPE, universal_newlines=True)
```

### Comparing `devine-3.3.2/devine/commands/wvd.py` & `devine-3.3.3/devine/commands/wvd.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/__main__.py` & `devine-3.3.3/devine/core/__main__.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/cacher.py` & `devine-3.3.3/devine/core/cacher.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/commands.py` & `devine-3.3.3/devine/core/commands.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/config.py` & `devine-3.3.3/devine/core/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,37 +73,35 @@
         if not path.exists():
             raise FileNotFoundError(f"Config file path ({path}) was not found")
         if not path.is_file():
             raise FileNotFoundError(f"Config file path ({path}) is not to a file.")
         return cls(**yaml.safe_load(path.read_text(encoding="utf8")) or {})
 
 
-def get_config_path() -> Optional[Path]:
-    """
-    Get Path to Config from various locations.
+# noinspection PyProtectedMember
+POSSIBLE_CONFIG_PATHS = (
+    # The Devine Namespace Folder (e.g., %appdata%/Python/Python311/site-packages/devine)
+    Config._Directories.namespace_dir / Config._Filenames.root_config,
+    # The Parent Folder to the Devine Namespace Folder (e.g., %appdata%/Python/Python311/site-packages)
+    Config._Directories.namespace_dir.parent / Config._Filenames.root_config,
+    # The AppDirs User Config Folder (e.g., %localappdata%/devine)
+    Config._Directories.user_configs / Config._Filenames.root_config
+)
 
-    Looks for a config file in the following folders in order:
 
-    1. The Devine Namespace Folder (e.g., %appdata%/Python/Python311/site-packages/devine)
-    2. The Parent Folder to the Devine Namespace Folder (e.g., %appdata%/Python/Python311/site-packages)
-    3. The AppDirs User Config Folder (e.g., %localappdata%/devine)
+def get_config_path() -> Optional[Path]:
+    """
+    Get Path to Config from any one of the possible locations.
 
     Returns None if no config file could be found.
     """
-    # noinspection PyProtectedMember
-    path = Config._Directories.namespace_dir / Config._Filenames.root_config
-    if not path.exists():
-        # noinspection PyProtectedMember
-        path = Config._Directories.namespace_dir.parent / Config._Filenames.root_config
-    if not path.exists():
-        # noinspection PyProtectedMember
-        path = Config._Directories.user_configs / Config._Filenames.root_config
-    if not path.exists():
-        path = None
-    return path
+    for path in POSSIBLE_CONFIG_PATHS:
+        if path.exists():
+            return path
+    return None
 
 
 config_path = get_config_path()
 if config_path:
     config = Config.from_yaml(config_path)
 else:
     config = Config()
```

### Comparing `devine-3.3.2/devine/core/console.py` & `devine-3.3.3/devine/core/console.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/constants.py` & `devine-3.3.3/devine/core/constants.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/credential.py` & `devine-3.3.3/devine/core/credential.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/downloaders/aria2c.py` & `devine-3.3.3/devine/core/downloaders/aria2c.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 import requests
 from Crypto.Random import get_random_bytes
 from requests import Session
 from requests.cookies import cookiejar_from_dict, get_cookie_header
 from rich import filesize
 from rich.text import Text
 
+from devine.core import binaries
 from devine.core.config import config
 from devine.core.console import console
 from devine.core.constants import DOWNLOAD_CANCELLED
-from devine.core.utilities import get_binary_path, get_extension, get_free_port
+from devine.core.utilities import get_extension, get_free_port
 
 
 def rpc(caller: Callable, secret: str, method: str, params: Optional[list[Any]] = None) -> Any:
     """Make a call to Aria2's JSON-RPC API."""
     try:
         rpc_res = caller(
             json={
@@ -83,16 +84,15 @@
         max_workers = min(32, (os.cpu_count() or 1) + 4)
     elif not isinstance(max_workers, int):
         raise TypeError(f"Expected max_workers to be {int}, not {type(max_workers)}")
 
     if not isinstance(urls, list):
         urls = [urls]
 
-    executable = get_binary_path("aria2c", "aria2")
-    if not executable:
+    if not binaries.Aria2:
         raise EnvironmentError("Aria2c executable not found...")
 
     if proxy and not proxy.lower().startswith("http://"):
         raise ValueError("Only HTTP proxies are supported by aria2(c)")
 
     if cookies and not isinstance(cookies, CookieJar):
         cookies = cookiejar_from_dict(cookies)
@@ -182,15 +182,15 @@
         arguments.extend(["--header", f"{header}: {value}"])
 
     yield dict(total=len(urls))
 
     try:
         p = subprocess.Popen(
             [
-                executable,
+                binaries.Aria2,
                 *arguments
             ],
             stdin=subprocess.PIPE,
             stdout=subprocess.DEVNULL
         )
 
         p.stdin.write(url_file.encode())
```

### Comparing `devine-3.3.2/devine/core/downloaders/curl_impersonate.py` & `devine-3.3.3/devine/core/downloaders/curl_impersonate.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 import time
 from concurrent import futures
 from concurrent.futures.thread import ThreadPoolExecutor
 from http.cookiejar import CookieJar
 from pathlib import Path
 from typing import Any, Generator, MutableMapping, Optional, Union
 
-from curl_cffi import CurlOpt
 from curl_cffi.requests import Session
 from rich import filesize
 
 from devine.core.config import config
 from devine.core.constants import DOWNLOAD_CANCELLED
 from devine.core.utilities import get_extension
 
 MAX_ATTEMPTS = 5
 RETRY_WAIT = 2
 CHUNK_SIZE = 1024
 PROGRESS_WINDOW = 5
-BROWSER = config.curl_impersonate.get("browser", "chrome120")
+BROWSER = config.curl_impersonate.get("browser", "chrome124")
 
 
 def download(
     url: str,
     save_path: Path,
     session: Session,
     **kwargs: Any
@@ -49,19 +48,14 @@
         session: The Requests or Curl-Impersonate Session to make HTTP requests with.
             Useful to set Header, Cookie, and Proxy data. Connections are saved and
             re-used with the session so long as the server keeps the connection alive.
         kwargs: Any extra keyword arguments to pass to the session.get() call. Use this
             for one-time request changes like a header, cookie, or proxy. For example,
             to request Byte-ranges use e.g., `headers={"Range": "bytes=0-128"}`.
     """
-    # https://github.com/yifeikong/curl_cffi/issues/6#issuecomment-2028518677
-    # must be applied here since the `session.curl` is thread-localized
-    # noinspection PyProtectedMember
-    session.curl.setopt(CurlOpt.PROXY_CAINFO, session.curl._cacert)
-
     save_dir = save_path.parent
     control_file = save_path.with_name(f"{save_path.name}.!dev")
 
     save_dir.mkdir(parents=True, exist_ok=True)
 
     if control_file.exists():
         # consider the file corrupt if the control file exists
```

### Comparing `devine-3.3.2/devine/core/downloaders/requests.py` & `devine-3.3.3/devine/core/downloaders/requests.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/drm/clearkey.py` & `devine-3.3.3/devine/core/drm/clearkey.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/drm/widevine.py` & `devine-3.3.3/devine/core/drm/widevine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 
 import base64
 import shutil
 import subprocess
-import sys
 import textwrap
 from pathlib import Path
 from typing import Any, Callable, Optional, Union
 from uuid import UUID
 
 import m3u8
 from construct import Container
 from pymp4.parser import Box
 from pywidevine.cdm import Cdm as WidevineCdm
 from pywidevine.pssh import PSSH
 from requests import Session
 from rich.text import Text
 
+from devine.core import binaries
 from devine.core.config import config
 from devine.core.console import console
 from devine.core.constants import AnyTrack
-from devine.core.utilities import get_binary_path, get_boxes
+from devine.core.utilities import get_boxes
 from devine.core.utils.subprocess import ffprobe
 
 
 class Widevine:
     """Widevine DRM System."""
     def __init__(self, pssh: PSSH, kid: Union[UUID, str, bytes, None] = None, **kwargs: Any):
         if not pssh:
@@ -219,17 +219,15 @@
             EnvironmentError if the Shaka Packager executable could not be found.
             ValueError if the track has not yet been downloaded.
             SubprocessError if Shaka Packager returned a non-zero exit code.
         """
         if not self.content_keys:
             raise ValueError("Cannot decrypt a Track without any Content Keys...")
 
-        platform = {"win32": "win", "darwin": "osx"}.get(sys.platform, sys.platform)
-        executable = get_binary_path("shaka-packager", "packager", f"packager-{platform}", f"packager-{platform}-x64")
-        if not executable:
+        if not binaries.ShakaPackager:
             raise EnvironmentError("Shaka Packager executable not found but is required.")
         if not path or not path.exists():
             raise ValueError("Tried to decrypt a file that does not exist.")
 
         output_path = path.with_stem(f"{path.stem}_decrypted")
         config.directories.temp.mkdir(parents=True, exist_ok=True)
 
@@ -248,15 +246,15 @@
                         for i, (kid, key) in enumerate(self.content_keys.items(), len(self.content_keys))
                     ]
                 ]),
                 "--temp_dir", config.directories.temp
             ]
 
             p = subprocess.Popen(
-                [executable, *arguments],
+                [binaries.ShakaPackager, *arguments],
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.PIPE,
                 universal_newlines=True
             )
 
             stream_skipped = False
             had_error = False
```

### Comparing `devine-3.3.2/devine/core/events.py` & `devine-3.3.3/devine/core/events.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/manifests/dash.py` & `devine-3.3.3/devine/core/manifests/dash.py`

 * *Files 3% similar despite different names*

```diff
@@ -281,20 +281,23 @@
             segment_list = adaptation_set.find("SegmentList")
 
         segment_base = representation.find("SegmentBase")
         if segment_base is None:
             segment_base = adaptation_set.find("SegmentBase")
 
         segments: list[tuple[str, Optional[str]]] = []
+        segment_timescale: float = 0
+        segment_durations: list[int] = []
         track_kid: Optional[UUID] = None
 
         if segment_template is not None:
             segment_template = copy(segment_template)
             start_number = int(segment_template.get("startNumber") or 1)
             segment_timeline = segment_template.find("SegmentTimeline")
+            segment_timescale = float(segment_template.get("timescale") or 1)
 
             for item in ("initialization", "media"):
                 value = segment_template.get(item)
                 if not value:
                     continue
                 if not re.match("^https?://", value, re.IGNORECASE):
                     if not rep_base_url:
@@ -314,53 +317,55 @@
                     RepresentationID=representation.get("id")
                 ))
                 res.raise_for_status()
                 init_data = res.content
                 track_kid = track.get_key_id(init_data)
 
             if segment_timeline is not None:
-                seg_time_list = []
                 current_time = 0
                 for s in segment_timeline.findall("S"):
                     if s.get("t"):
                         current_time = int(s.get("t"))
                     for _ in range(1 + (int(s.get("r") or 0))):
-                        seg_time_list.append(current_time)
+                        segment_durations.append(current_time)
                         current_time += int(s.get("d"))
-                seg_num_list = list(range(start_number, len(seg_time_list) + start_number))
+                seg_num_list = list(range(start_number, len(segment_durations) + start_number))
 
-                for t, n in zip(seg_time_list, seg_num_list):
+                for t, n in zip(segment_durations, seg_num_list):
                     segments.append((
                         DASH.replace_fields(
                             segment_template.get("media"),
                             Bandwidth=representation.get("bandwidth"),
                             Number=n,
                             RepresentationID=representation.get("id"),
                             Time=t
                         ), None
                     ))
             else:
                 if not period_duration:
                     raise ValueError("Duration of the Period was unable to be determined.")
                 period_duration = DASH.pt_to_sec(period_duration)
-                segment_duration = float(segment_template.get("duration"))
-                segment_timescale = float(segment_template.get("timescale") or 1)
+                segment_duration = float(segment_template.get("duration")) or 1
                 total_segments = math.ceil(period_duration / (segment_duration / segment_timescale))
 
                 for s in range(start_number, start_number + total_segments):
                     segments.append((
                         DASH.replace_fields(
                             segment_template.get("media"),
                             Bandwidth=representation.get("bandwidth"),
                             Number=s,
                             RepresentationID=representation.get("id"),
                             Time=s
                         ), None
                     ))
+                    # TODO: Should we floor/ceil/round, or is int() ok?
+                    segment_durations.append(int(segment_duration))
         elif segment_list is not None:
+            segment_timescale = float(segment_list.get("timescale") or 1)
+
             init_data = None
             initialization = segment_list.find("Initialization")
             if initialization is not None:
                 source_url = initialization.get("sourceURL")
                 if not source_url:
                     source_url = rep_base_url
                 elif not re.match("^https?://", source_url, re.IGNORECASE):
@@ -384,14 +389,15 @@
                 elif not re.match("^https?://", media_url, re.IGNORECASE):
                     media_url = urljoin(rep_base_url, f"./{media_url}")
 
                 segments.append((
                     media_url,
                     segment_url.get("mediaRange")
                 ))
+                segment_durations.append(int(segment_url.get("duration") or 1))
         elif segment_base is not None:
             media_range = None
             init_data = None
             initialization = segment_base.find("Initialization")
             if initialization is not None:
                 if initialization.get("range"):
                     init_range_header = {"Range": f"bytes={initialization.get('range')}"}
@@ -416,14 +422,18 @@
                 None
             ))
         else:
             log.error("Could not find a way to get segments from this MPD manifest.")
             log.debug(track.url)
             sys.exit(1)
 
+        # TODO: Should we floor/ceil/round, or is int() ok?
+        track.data["dash"]["timescale"] = int(segment_timescale)
+        track.data["dash"]["segment_durations"] = segment_durations
+
         if not track.drm and isinstance(track, (Video, Audio)):
             try:
                 track.drm = [Widevine.from_init_data(init_data)]
             except Widevine.Exceptions.PSSHNotFound:
                 # it might not have Widevine DRM, or might not have found the PSSH
                 log.warning("No Widevine PSSH was found for this track, is it DRM free?")
```

### Comparing `devine-3.3.2/devine/core/manifests/hls.py` & `devine-3.3.3/devine/core/manifests/hls.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 import requests
 from langcodes import Language, tag_is_valid
 from m3u8 import M3U8
 from pywidevine.cdm import Cdm as WidevineCdm
 from pywidevine.pssh import PSSH
 from requests import Session
 
+from devine.core import binaries
 from devine.core.constants import DOWNLOAD_CANCELLED, DOWNLOAD_LICENCE_ONLY, AnyTrack
 from devine.core.downloaders import requests as requests_downloader
 from devine.core.drm import DRM_T, ClearKey, Widevine
 from devine.core.events import events
 from devine.core.tracks import Audio, Subtitle, Tracks, Video
-from devine.core.utilities import get_binary_path, get_extension, is_close_match, try_ensure_utf8
+from devine.core.utilities import get_extension, is_close_match, try_ensure_utf8
 
 
 class HLS:
     def __init__(self, manifest: M3U8, session: Optional[Session] = None):
         if not manifest:
             raise ValueError("HLS manifest must be provided.")
         if not isinstance(manifest, M3U8):
@@ -251,19 +252,23 @@
 
         total_segments = len(master.segments) - len(unwanted_segments)
         progress(total=total_segments)
 
         downloader = track.downloader
 
         urls: list[dict[str, Any]] = []
+        segment_durations: list[int] = []
+
         range_offset = 0
         for segment in master.segments:
             if segment in unwanted_segments:
                 continue
 
+            segment_durations.append(int(segment.duration))
+
             if segment.byterange:
                 if downloader.__name__ == "aria2c":
                     # aria2(c) is shit and doesn't support the Range header, fallback to the requests downloader
                     downloader = requests_downloader
                 byte_range = HLS.calculate_byte_range(segment.byterange, range_offset)
                 range_offset = byte_range.split("-")[0]
             else:
@@ -272,14 +277,16 @@
             urls.append({
                 "url": urljoin(segment.base_uri, segment.uri),
                 "headers": {
                     "Range": f"bytes={byte_range}"
                 } if byte_range else {}
             })
 
+        track.data["hls"]["segment_durations"] = segment_durations
+
         segment_save_dir = save_dir / "segments"
 
         for status_update in downloader(
             urls=urls,
             output_dir=segment_save_dir,
             filename="{i:0%d}{ext}" % len(str(len(urls))),
             headers=session.headers,
@@ -552,26 +559,25 @@
     @staticmethod
     def merge_segments(segments: list[Path], save_path: Path) -> int:
         """
         Concatenate Segments by first demuxing with FFmpeg.
 
         Returns the file size of the merged file.
         """
-        ffmpeg = get_binary_path("ffmpeg")
-        if not ffmpeg:
+        if not binaries.FFMPEG:
             raise EnvironmentError("FFmpeg executable was not found but is required to merge HLS segments.")
 
         demuxer_file = segments[0].parent / "ffmpeg_concat_demuxer.txt"
         demuxer_file.write_text("\n".join([
             f"file '{segment}'"
             for segment in segments
         ]))
 
         subprocess.check_call([
-            ffmpeg, "-hide_banner",
+            binaries.FFMPEG, "-hide_banner",
             "-loglevel", "panic",
             "-f", "concat",
             "-safe", "0",
             "-i", demuxer_file,
             "-map", "0",
             "-c", "copy",
             save_path
```

### Comparing `devine-3.3.2/devine/core/proxies/basic.py` & `devine-3.3.3/devine/core/proxies/basic.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/proxies/hola.py` & `devine-3.3.3/devine/core/proxies/hola.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import random
 import re
 import subprocess
 from typing import Optional
 
+from devine.core import binaries
 from devine.core.proxies.proxy import Proxy
-from devine.core.utilities import get_binary_path
 
 
 class Hola(Proxy):
     def __init__(self):
         """
         Proxy Service using Hola's direct connections via the hola-proxy project.
         https://github.com/Snawoot/hola-proxy
         """
-        self.binary = get_binary_path("hola-proxy")
+        self.binary = binaries.HolaProxy
         if not self.binary:
             raise EnvironmentError("hola-proxy executable not found but is required for the Hola proxy provider.")
 
         self.countries = self.get_countries()
 
     def __repr__(self) -> str:
         countries = len(self.countries)
```

### Comparing `devine-3.3.2/devine/core/proxies/nordvpn.py` & `devine-3.3.3/devine/core/proxies/nordvpn.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/proxies/proxy.py` & `devine-3.3.3/devine/core/proxies/proxy.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/search_result.py` & `devine-3.3.3/devine/core/search_result.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/service.py` & `devine-3.3.3/devine/core/service.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/services.py` & `devine-3.3.3/devine/core/services.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/titles/episode.py` & `devine-3.3.3/devine/core/titles/episode.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/titles/movie.py` & `devine-3.3.3/devine/core/titles/movie.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/titles/song.py` & `devine-3.3.3/devine/core/titles/song.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/titles/title.py` & `devine-3.3.3/devine/core/titles/title.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/tracks/attachment.py` & `devine-3.3.3/devine/core/tracks/attachment.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/tracks/audio.py` & `devine-3.3.3/devine/core/tracks/audio.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/tracks/chapter.py` & `devine-3.3.3/devine/core/tracks/chapter.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/tracks/chapters.py` & `devine-3.3.3/devine/core/tracks/chapters.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/tracks/subtitle.py` & `devine-3.3.3/devine/core/tracks/subtitle.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 import re
 import subprocess
 from collections import defaultdict
 from enum import Enum
 from functools import partial
 from io import BytesIO
 from pathlib import Path
-from typing import Any, Callable, Iterable, Optional
+from typing import Any, Callable, Iterable, Optional, Union
 
 import pycaption
 import requests
 from construct import Container
 from pycaption import Caption, CaptionList, CaptionNode, WebVTTReader
 from pycaption.geometry import Layout
 from pymp4.parser import MP4
 from subtitle_filter import Subtitles
 
+from devine.core import binaries
 from devine.core.tracks.track import Track
-from devine.core.utilities import get_binary_path, try_ensure_utf8
+from devine.core.utilities import try_ensure_utf8
+from devine.core.utils.webvtt import merge_segmented_webvtt
 
 
 class Subtitle(Track):
     class Codec(str, Enum):
         SubRip = "SRT"                # https://wikipedia.org/wiki/SubRip
         SubStationAlpha = "SSA"       # https://wikipedia.org/wiki/SubStation_Alpha
         SubStationAlphav4 = "ASS"     # https://wikipedia.org/wiki/SubStation_Alpha#Advanced_SubStation_Alpha=
@@ -197,14 +199,32 @@
         if not self.path:
             return
 
         if self.codec == Subtitle.Codec.fTTML:
             self.convert(Subtitle.Codec.TimedTextMarkupLang)
         elif self.codec == Subtitle.Codec.fVTT:
             self.convert(Subtitle.Codec.WebVTT)
+        elif self.codec == Subtitle.Codec.WebVTT:
+            text = self.path.read_text("utf8")
+            if self.descriptor == Track.Descriptor.DASH:
+                text = merge_segmented_webvtt(
+                    text,
+                    segment_durations=self.data["dash"]["segment_durations"],
+                    timescale=self.data["dash"]["timescale"]
+                )
+            elif self.descriptor == Track.Descriptor.HLS:
+                text = merge_segmented_webvtt(
+                    text,
+                    segment_durations=self.data["hls"]["segment_durations"],
+                    timescale=1  # ?
+                )
+            caption_set = pycaption.WebVTTReader().read(text)
+            Subtitle.merge_same_cues(caption_set)
+            subtitle_text = pycaption.WebVTTWriter().write(caption_set)
+            self.path.write_text(subtitle_text, encoding="utf8")
 
     def convert(self, codec: Subtitle.Codec) -> Path:
         """
         Convert this Subtitle to another Format.
 
         The file path location of the Subtitle data will be kept at the same
         location but the file extension will be changed appropriately.
@@ -229,22 +249,21 @@
             raise ValueError("You must download the subtitle track first.")
 
         if self.codec == codec:
             return self.path
 
         output_path = self.path.with_suffix(f".{codec.value.lower()}")
 
-        sub_edit_executable = get_binary_path("SubtitleEdit")
-        if sub_edit_executable and self.codec not in (Subtitle.Codec.fTTML, Subtitle.Codec.fVTT):
+        if binaries.SubtitleEdit and self.codec not in (Subtitle.Codec.fTTML, Subtitle.Codec.fVTT):
             sub_edit_format = {
                 Subtitle.Codec.SubStationAlphav4: "AdvancedSubStationAlpha",
                 Subtitle.Codec.TimedTextMarkupLang: "TimedText1.0"
             }.get(codec, codec.name)
             sub_edit_args = [
-                sub_edit_executable,
+                binaries.SubtitleEdit,
                 "/Convert", self.path, sub_edit_format,
                 f"/outputfilename:{output_path.name}",
                 "/encoding:utf8"
             ]
             if codec == Subtitle.Codec.SubRip:
                 sub_edit_args.append("/ConvertColorsToDialog")
             subprocess.run(
@@ -304,22 +323,15 @@
                 caption_set = pycaption.DFXPReader().read(text)
             elif codec == Subtitle.Codec.fVTT:
                 caption_lists: dict[str, pycaption.CaptionList] = defaultdict(pycaption.CaptionList)
                 caption_list, language = Subtitle.merge_segmented_wvtt(data)
                 caption_lists[language] = caption_list
                 caption_set: pycaption.CaptionSet = pycaption.CaptionSet(caption_lists)
             elif codec == Subtitle.Codec.WebVTT:
-                text = try_ensure_utf8(data).decode("utf8")
-                # Segmented VTT when merged may have the WEBVTT headers part of the next caption
-                # if they are not separated far enough from the previous caption, hence the \n\n
-                text = text. \
-                    replace("WEBVTT", "\n\nWEBVTT"). \
-                    replace("\r", ""). \
-                    replace("\n\n\n", "\n \n\n"). \
-                    replace("\n\n<", "\n<")
+                text = Subtitle.space_webvtt_headers(data)
                 caption_set = pycaption.WebVTTReader().read(text)
             else:
                 raise ValueError(f"Unknown Subtitle format \"{codec}\"...")
         except pycaption.exceptions.CaptionReadSyntaxError as e:
             raise SyntaxError(f"A syntax error has occurred when reading the \"{codec}\" subtitle: {e}")
         except pycaption.exceptions.CaptionReadNoCaptions:
             return pycaption.CaptionSet({"en": []})
@@ -329,14 +341,35 @@
             if not caption_set.get_captions(language):
                 # noinspection PyProtectedMember
                 del caption_set._captions[language]
 
         return caption_set
 
     @staticmethod
+    def space_webvtt_headers(data: Union[str, bytes]):
+        """
+        Space out the WEBVTT Headers from Captions.
+
+        Segmented VTT when merged may have the WEBVTT headers part of the next caption
+        as they were not separated far enough from the previous caption and ended up
+        being considered as caption text rather than the header for the next segment.
+        """
+        if isinstance(data, bytes):
+            data = try_ensure_utf8(data).decode("utf8")
+        elif not isinstance(data, str):
+            raise ValueError(f"Expecting data to be a str, not {data!r}")
+
+        text = data.replace("WEBVTT", "\n\nWEBVTT").\
+            replace("\r", "").\
+            replace("\n\n\n", "\n \n\n").\
+            replace("\n\n<", "\n<")
+
+        return text
+
+    @staticmethod
     def merge_same_cues(caption_set: pycaption.CaptionSet):
         """Merge captions with the same timecodes and text as one in-place."""
         for lang in caption_set.get_languages():
             captions = caption_set.get_captions(lang)
             last_caption = None
             concurrent_captions = pycaption.CaptionList()
             merged_captions = pycaption.CaptionList()
@@ -496,25 +529,24 @@
         """
         Strip captions for hearing impaired (SDH).
         It uses SubtitleEdit if available, otherwise filter-subs.
         """
         if not self.path or not self.path.exists():
             raise ValueError("You must download the subtitle track first.")
 
-        executable = get_binary_path("SubtitleEdit")
-        if executable:
+        if binaries.SubtitleEdit:
             if self.codec == Subtitle.Codec.SubStationAlphav4:
                 output_format = "AdvancedSubStationAlpha"
             elif self.codec == Subtitle.Codec.TimedTextMarkupLang:
                 output_format = "TimedText1.0"
             else:
                 output_format = self.codec.name
             subprocess.run(
                 [
-                    executable,
+                    binaries.SubtitleEdit,
                     "/Convert", self.path, output_format,
                     "/encoding:utf8",
                     "/overwrite",
                     "/RemoveTextForHI"
                 ],
                 check=True,
                 stdout=subprocess.DEVNULL
@@ -535,28 +567,27 @@
         """
         Reverse RTL (Right to Left) Start/End on Captions.
         This can be used to fix the positioning of sentence-ending characters.
         """
         if not self.path or not self.path.exists():
             raise ValueError("You must download the subtitle track first.")
 
-        executable = get_binary_path("SubtitleEdit")
-        if not executable:
+        if not binaries.SubtitleEdit:
             raise EnvironmentError("SubtitleEdit executable not found...")
 
         if self.codec == Subtitle.Codec.SubStationAlphav4:
             output_format = "AdvancedSubStationAlpha"
         elif self.codec == Subtitle.Codec.TimedTextMarkupLang:
             output_format = "TimedText1.0"
         else:
             output_format = self.codec.name
 
         subprocess.run(
             [
-                executable,
+                binaries.SubtitleEdit,
                 "/Convert", self.path, output_format,
                 "/ReverseRtlStartEnd",
                 "/encoding:utf8",
                 "/overwrite"
             ],
             check=True,
             stdout=subprocess.DEVNULL
```

### Comparing `devine-3.3.2/devine/core/tracks/track.py` & `devine-3.3.3/devine/core/tracks/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 from typing import Any, Callable, Iterable, Optional, Union
 from uuid import UUID
 from zlib import crc32
 
 from langcodes import Language
 from requests import Session
 
+from devine.core import binaries
 from devine.core.config import config
 from devine.core.constants import DOWNLOAD_CANCELLED, DOWNLOAD_LICENCE_ONLY
 from devine.core.downloaders import aria2c, curl_impersonate, requests
 from devine.core.drm import DRM_T, Widevine
 from devine.core.events import events
-from devine.core.utilities import get_binary_path, get_boxes, try_ensure_utf8
+from devine.core.utilities import get_boxes, try_ensure_utf8
 from devine.core.utils.subprocess import ffprobe
 
 
 class Track:
     class Descriptor(Enum):
         URL = 1  # Direct URL, nothing fancy
         HLS = 2  # https://en.wikipedia.org/wiki/HTTP_Live_Streaming
@@ -466,25 +467,24 @@
 
         return init_data
 
     def repackage(self) -> None:
         if not self.path or not self.path.exists():
             raise ValueError("Cannot repackage a Track that has not been downloaded.")
 
-        executable = get_binary_path("ffmpeg")
-        if not executable:
+        if not binaries.FFMPEG:
             raise EnvironmentError("FFmpeg executable \"ffmpeg\" was not found but is required for this call.")
 
         original_path = self.path
         output_path = original_path.with_stem(f"{original_path.stem}_repack")
 
         def _ffmpeg(extra_args: list[str] = None):
             subprocess.run(
                 [
-                    executable, "-hide_banner",
+                    binaries.FFMPEG, "-hide_banner",
                     "-loglevel", "error",
                     "-i", original_path,
                     *(extra_args or []),
                     # Following are very important!
                     "-map_metadata", "-1",  # don't transfer metadata to output file
                     "-fflags", "bitexact",  # only have minimal tag data, reproducible mux
                     "-codec", "copy",
```

### Comparing `devine-3.3.2/devine/core/tracks/tracks.py` & `devine-3.3.3/devine/core/tracks/tracks.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/tracks/video.py` & `devine-3.3.3/devine/core/tracks/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 import subprocess
 from enum import Enum
 from pathlib import Path
 from typing import Any, Optional, Union
 
 from langcodes import Language
 
+from devine.core import binaries
 from devine.core.config import config
 from devine.core.tracks.subtitle import Subtitle
 from devine.core.tracks.track import Track
-from devine.core.utilities import FPS, get_binary_path, get_boxes
+from devine.core.utilities import FPS, get_boxes
 
 
 class Video(Track):
     class Codec(str, Enum):
         AVC = "H.264"
         HEVC = "H.265"
         VC1 = "VC-1"
@@ -253,28 +254,27 @@
             raise ValueError("Cannot change the color range flag on a Video that has no codec specified.")
         if self.codec not in (Video.Codec.AVC, Video.Codec.HEVC):
             raise NotImplementedError(
                 "Cannot change the color range flag on this Video as "
                 f"it's codec, {self.codec.value}, is not yet supported."
             )
 
-        executable = get_binary_path("ffmpeg")
-        if not executable:
+        if not binaries.FFMPEG:
             raise EnvironmentError("FFmpeg executable \"ffmpeg\" was not found but is required for this call.")
 
         filter_key = {
             Video.Codec.AVC: "h264_metadata",
             Video.Codec.HEVC: "hevc_metadata"
         }[self.codec]
 
         original_path = self.path
         output_path = original_path.with_stem(f"{original_path.stem}_{['limited', 'full'][range_]}_range")
 
         subprocess.run([
-            executable, "-hide_banner",
+            binaries.FFMPEG, "-hide_banner",
             "-loglevel", "panic",
             "-i", original_path,
             "-codec", "copy",
             "-bsf:v", f"{filter_key}=video_full_range_flag={range_}",
             str(output_path)
         ], check=True)
 
@@ -284,26 +284,25 @@
     def ccextractor(
         self, track_id: Any, out_path: Union[Path, str], language: Language, original: bool = False
     ) -> Optional[Subtitle]:
         """Return a TextTrack object representing CC track extracted by CCExtractor."""
         if not self.path:
             raise ValueError("You must download the track first.")
 
-        executable = get_binary_path("ccextractor", "ccextractorwin", "ccextractorwinfull")
-        if not executable:
+        if not binaries.CCExtractor:
             raise EnvironmentError("ccextractor executable was not found.")
 
         # ccextractor often fails in weird ways unless we repack
         self.repackage()
 
         out_path = Path(out_path)
 
         try:
             subprocess.run([
-                executable,
+                binaries.CCExtractor,
                 "-trim",
                 "-nobom",
                 "-noru", "-ru1",
                 "-o", out_path,
                 self.path
             ], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         except subprocess.CalledProcessError as e:
@@ -376,16 +375,15 @@
         and then re-adding SEI data (effectively a new NAL Unit with just the SEI data).
         Only bitstreams with x264 encoding information is currently supported due to the
         obscurity on the MDAT mp4 box structure. Therefore, we need to use hacky regex.
         """
         if not self.path or not self.path.exists():
             raise ValueError("Cannot clean a Track that has not been downloaded.")
 
-        executable = get_binary_path("ffmpeg")
-        if not executable:
+        if not binaries.FFMPEG:
             raise EnvironmentError("FFmpeg executable \"ffmpeg\" was not found but is required for this call.")
 
         log = logging.getLogger("x264-clean")
         log.info("Removing EIA-CC from Video Track with FFMPEG")
 
         with open(self.path, "rb") as f:
             file = f.read(60000)
@@ -398,15 +396,15 @@
         uuid = x264.group(1).hex()
         i = file.index(b"x264")
         encoding_settings = file[i: i + file[i:].index(b"\x00")].replace(b":", br"\\:").replace(b",", br"\,").decode()
 
         original_path = self.path
         cleaned_path = original_path.with_suffix(f".cleaned{original_path.suffix}")
         subprocess.run([
-            executable, "-hide_banner",
+            binaries.FFMPEG, "-hide_banner",
             "-loglevel", "panic",
             "-i", original_path,
             "-map_metadata", "-1",
             "-fflags", "bitexact",
             "-bsf:v", f"filter_units=remove_types=6,h264_metadata=sei_user_data={uuid}+{encoding_settings}",
             "-codec", "copy",
             str(cleaned_path)
```

### Comparing `devine-3.3.2/devine/core/utilities.py` & `devine-3.3.3/devine/core/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import ast
 import contextlib
 import importlib.util
 import os
 import re
-import shutil
 import socket
 import sys
 import time
 import unicodedata
 from collections import defaultdict
 from datetime import datetime
 from pathlib import Path
@@ -83,23 +82,14 @@
     spec = importlib.util.spec_from_file_location(name, path)
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
 
     return module
 
 
-def get_binary_path(*names: str) -> Optional[Path]:
-    """Find the path of the first found binary name."""
-    for name in names:
-        path = shutil.which(name)
-        if path:
-            return Path(path)
-    return None
-
-
 def sanitize_filename(filename: str, spacer: str = ".") -> str:
     """
     Sanitize a string to be filename safe.
 
     The spacer is safer to be a '.' for older DDL and p2p sharing spaces.
     This includes web-served content via direct links and such.
     """
```

### Comparing `devine-3.3.2/devine/core/utils/click_types.py` & `devine-3.3.3/devine/core/utils/click_types.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/utils/collections.py` & `devine-3.3.3/devine/core/utils/collections.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/utils/sslciphers.py` & `devine-3.3.3/devine/core/utils/sslciphers.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/utils/subprocess.py` & `devine-3.3.3/devine/core/utils/subprocess.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import json
 import subprocess
 from pathlib import Path
 from typing import Union
 
+from devine.core import binaries
+
 
 def ffprobe(uri: Union[bytes, Path]) -> dict:
     """Use ffprobe on the provided data to get stream information."""
+    if not binaries.FFProbe:
+        raise EnvironmentError("FFProbe executable \"ffprobe\" not found but is required.")
+
     args = [
-        "ffprobe",
+        binaries.FFProbe,
         "-v", "quiet",
         "-of", "json",
         "-show_streams"
     ]
     if isinstance(uri, Path):
         args.extend([
             "-f", "lavfi",
```

### Comparing `devine-3.3.2/devine/core/utils/xml.py` & `devine-3.3.3/devine/core/utils/xml.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/vault.py` & `devine-3.3.3/devine/core/vault.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/core/vaults.py` & `devine-3.3.3/devine/core/vaults.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/vaults/API.py` & `devine-3.3.3/devine/vaults/API.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/vaults/MySQL.py` & `devine-3.3.3/devine/vaults/MySQL.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/devine/vaults/SQLite.py` & `devine-3.3.3/devine/vaults/SQLite.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.2/pyproject.toml` & `devine-3.3.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "devine"
-version = "3.3.2"
+version = "3.3.3"
 description = "Modular Movie, TV, and Music Archival Software."
 license = "GPL-3.0-only"
 authors = ["rlaphoenix <rlaphoenix@pm.me>"]
 readme = "README.md"
 homepage = "https://github.com/devine-dl/devine"
 repository = "https://github.com/devine-dl/devine"
 keywords = ["python", "downloader", "drm", "widevine"]
@@ -36,15 +36,15 @@
 python = ">=3.9,<4.0"
 appdirs = "^1.4.4"
 Brotli = "^1.1.0"
 click = "^8.1.7"
 construct = "^2.8.8"
 crccheck = "^1.3.0"
 jsonpickle = "^3.0.4"
-langcodes = { extras = ["data"], version = "^3.3.0" }
+langcodes = { extras = ["data"], version = "^3.4.0" }
 lxml = "^5.2.1"
 pproxy = "^2.7.9"
 protobuf = "^4.25.3"
 pycaption = "^2.2.6"
 pycryptodomex = "^3.20.0"
 pyjwt = "^2.8.0"
 pymediainfo = "^6.1.0"
@@ -57,17 +57,15 @@
 "rlaphoenix.m3u8" = "^3.4.0"
 "ruamel.yaml" = "^0.18.6"
 sortedcontainers = "^2.4.0"
 subtitle-filter = "^1.4.9"
 Unidecode = "^1.3.8"
 urllib3 = "^2.2.1"
 chardet = "^5.2.0"
-curl-cffi = "^0.6.2"
-language-data = "^1.2.0"
-marisa-trie = "^1.1.0"
+curl-cffi = "^0.7.0b4"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^3.7.0"
 mypy = "^1.9.0"
 mypy-protobuf = "^3.6.0"
 types-protobuf = "^4.24.0.20240408"
 types-PyMySQL = "^1.1.0.1"
```

### Comparing `devine-3.3.2/PKG-INFO` & `devine-3.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devine
-Version: 3.3.2
+Version: 3.3.3
 Summary: Modular Movie, TV, and Music Archival Software.
 Home-page: https://github.com/devine-dl/devine
 License: GPL-3.0-only
 Keywords: python,downloader,drm,widevine
 Author: rlaphoenix
 Author-email: rlaphoenix@pm.me
 Requires-Python: >=3.9,<4.0
@@ -24,20 +24,18 @@
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: Unidecode (>=1.3.8,<2.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: construct (>=2.8.8,<3.0.0)
 Requires-Dist: crccheck (>=1.3.0,<2.0.0)
-Requires-Dist: curl-cffi (>=0.6.2,<0.7.0)
+Requires-Dist: curl-cffi (>=0.7.0b4,<0.8.0)
 Requires-Dist: jsonpickle (>=3.0.4,<4.0.0)
-Requires-Dist: langcodes[data] (>=3.3.0,<4.0.0)
-Requires-Dist: language-data (>=1.2.0,<2.0.0)
+Requires-Dist: langcodes[data] (>=3.4.0,<4.0.0)
 Requires-Dist: lxml (>=5.2.1,<6.0.0)
-Requires-Dist: marisa-trie (>=1.1.0,<2.0.0)
 Requires-Dist: pproxy (>=2.7.9,<3.0.0)
 Requires-Dist: protobuf (>=4.25.3,<5.0.0)
 Requires-Dist: pycaption (>=2.2.6,<3.0.0)
 Requires-Dist: pycryptodomex (>=3.20.0,<4.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: pymediainfo (>=6.1.0,<7.0.0)
 Requires-Dist: pymp4 (>=1.4.0,<2.0.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: devine Version: 3.3.2 Summary: Modular Movie, TV,
+Metadata-Version: 2.1 Name: devine Version: 3.3.3 Summary: Modular Movie, TV,
 and Music Archival Software. Home-page: https://github.com/devine-dl/devine
 License: GPL-3.0-only Keywords: python,downloader,drm,widevine Author:
 rlaphoenix Author-email: rlaphoenix@pm.me Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
@@ -10,23 +10,22 @@
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Security :: Cryptography Requires-Dist: Brotli
 (>=1.1.0,<2.0.0) Requires-Dist: PyYAML (>=6.0.1,<7.0.0) Requires-Dist:
 Unidecode (>=1.3.8,<2.0.0) Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-
 Dist: chardet (>=5.2.0,<6.0.0) Requires-Dist: click (>=8.1.7,<9.0.0) Requires-
 Dist: construct (>=2.8.8,<3.0.0) Requires-Dist: crccheck (>=1.3.0,<2.0.0)
-Requires-Dist: curl-cffi (>=0.6.2,<0.7.0) Requires-Dist: jsonpickle
-(>=3.0.4,<4.0.0) Requires-Dist: langcodes[data] (>=3.3.0,<4.0.0) Requires-Dist:
-language-data (>=1.2.0,<2.0.0) Requires-Dist: lxml (>=5.2.1,<6.0.0) Requires-
-Dist: marisa-trie (>=1.1.0,<2.0.0) Requires-Dist: pproxy (>=2.7.9,<3.0.0)
-Requires-Dist: protobuf (>=4.25.3,<5.0.0) Requires-Dist: pycaption
-(>=2.2.6,<3.0.0) Requires-Dist: pycryptodomex (>=3.20.0,<4.0.0) Requires-Dist:
-pyjwt (>=2.8.0,<3.0.0) Requires-Dist: pymediainfo (>=6.1.0,<7.0.0) Requires-
-Dist: pymp4 (>=1.4.0,<2.0.0) Requires-Dist: pymysql (>=1.1.0,<2.0.0) Requires-
-Dist: pywidevine[serve] (>=1.8.0,<2.0.0) Requires-Dist: requests[socks]
+Requires-Dist: curl-cffi (>=0.7.0b4,<0.8.0) Requires-Dist: jsonpickle
+(>=3.0.4,<4.0.0) Requires-Dist: langcodes[data] (>=3.4.0,<4.0.0) Requires-Dist:
+lxml (>=5.2.1,<6.0.0) Requires-Dist: pproxy (>=2.7.9,<3.0.0) Requires-Dist:
+protobuf (>=4.25.3,<5.0.0) Requires-Dist: pycaption (>=2.2.6,<3.0.0) Requires-
+Dist: pycryptodomex (>=3.20.0,<4.0.0) Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
+Requires-Dist: pymediainfo (>=6.1.0,<7.0.0) Requires-Dist: pymp4
+(>=1.4.0,<2.0.0) Requires-Dist: pymysql (>=1.1.0,<2.0.0) Requires-Dist:
+pywidevine[serve] (>=1.8.0,<2.0.0) Requires-Dist: requests[socks]
 (>=2.31.0,<3.0.0) Requires-Dist: rich (>=13.7.1,<14.0.0) Requires-Dist:
 rlaphoenix.m3u8 (>=3.4.0,<4.0.0) Requires-Dist: ruamel.yaml (>=0.18.6,<0.19.0)
 Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0) Requires-Dist: subtitle-filter
 (>=1.4.9,<2.0.0) Requires-Dist: urllib3 (>=2.2.1,<3.0.0) Project-URL:
 Changelog, https://github.com/devine-dl/devine/blob/master/CHANGELOG.md
 Project-URL: Discussions, https://github.com/devine-dl/devine/discussions
 Project-URL: Issues, https://github.com/devine-dl/devine/issues Project-URL:
```

