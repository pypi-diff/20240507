# Comparing `tmp/sotoki-2.0.2.tar.gz` & `tmp/sotoki-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sotoki-2.0.2.tar", last modified: Mon Oct 31 13:14:46 2022, max compression
+gzip compressed data, was "sotoki-2.1.1.tar", last modified: Tue May  7 14:51:25 2024, max compression
```

## Comparing `sotoki-2.0.2.tar` & `sotoki-2.1.1.tar`

### file list

```diff
@@ -1,222 +1,158 @@
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.102358 sotoki-2.0.2/
--rw-r--r--   0 reg        (501) staff       (20)     4007 2022-10-31 13:13:27.000000 sotoki-2.0.2/CHANGELOG.md
--rw-r--r--   0 reg        (501) staff       (20)    35141 2020-08-19 10:14:33.000000 sotoki-2.0.2/LICENSE
--rw-r--r--   0 reg        (501) staff       (20)       64 2021-05-28 11:09:10.000000 sotoki-2.0.2/MANIFEST.in
--rw-r--r--   0 reg        (501) staff       (20)     3606 2022-10-31 13:14:46.102097 sotoki-2.0.2/PKG-INFO
--rw-r--r--   0 reg        (501) staff       (20)     2425 2022-10-31 11:15:17.000000 sotoki-2.0.2/README.md
--rw-r--r--   0 reg        (501) staff       (20)      431 2022-10-31 13:00:30.000000 sotoki-2.0.2/requirements.txt
--rw-r--r--   0 reg        (501) staff       (20)       38 2022-10-31 13:14:46.102449 sotoki-2.0.2/setup.cfg
--rw-r--r--   0 reg        (501) staff       (20)     1677 2021-07-15 11:44:30.000000 sotoki-2.0.2/setup.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.012260 sotoki-2.0.2/src/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.026385 sotoki-2.0.2/src/sotoki/
--rw-r--r--   0 reg        (501) staff       (20)        6 2022-10-31 13:12:56.000000 sotoki-2.0.2/src/sotoki/VERSION
--rw-r--r--   0 reg        (501) staff       (20)        0 2021-05-19 10:33:20.000000 sotoki-2.0.2/src/sotoki/__init__.py
--rw-r--r--   0 reg        (501) staff       (20)      358 2021-05-19 10:34:49.000000 sotoki-2.0.2/src/sotoki/__main__.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.039438 sotoki-2.0.2/src/sotoki/__pycache__/
--rw-r--r--   0 reg        (501) staff       (20)      135 2021-05-19 11:49:07.000000 sotoki-2.0.2/src/sotoki/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)      135 2022-07-29 09:06:16.000000 sotoki-2.0.2/src/sotoki/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)      429 2021-05-19 11:49:07.000000 sotoki-2.0.2/src/sotoki/__pycache__/__main__.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)      451 2022-07-29 09:06:16.000000 sotoki-2.0.2/src/sotoki/__pycache__/__main__.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     5751 2022-07-26 17:32:27.000000 sotoki-2.0.2/src/sotoki/__pycache__/archives.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     5741 2022-07-29 09:06:21.000000 sotoki-2.0.2/src/sotoki/__pycache__/archives.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     5638 2022-07-26 09:15:36.000000 sotoki-2.0.2/src/sotoki/__pycache__/constants.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     5669 2022-07-29 09:06:16.000000 sotoki-2.0.2/src/sotoki/__pycache__/constants.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     6566 2022-05-01 18:33:40.000000 sotoki-2.0.2/src/sotoki/__pycache__/dependencies.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     6215 2022-10-31 13:14:26.000000 sotoki-2.0.2/src/sotoki/__pycache__/dependencies.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     8590 2021-08-30 13:26:10.000000 sotoki-2.0.2/src/sotoki/__pycache__/entrypoint.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     8626 2022-07-29 09:06:16.000000 sotoki-2.0.2/src/sotoki/__pycache__/entrypoint.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     7559 2022-07-26 15:51:30.000000 sotoki-2.0.2/src/sotoki/__pycache__/posts.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     7641 2022-07-29 09:06:31.000000 sotoki-2.0.2/src/sotoki/__pycache__/posts.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     7779 2021-08-26 15:53:51.000000 sotoki-2.0.2/src/sotoki/__pycache__/renderer.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     7769 2022-07-29 09:06:31.000000 sotoki-2.0.2/src/sotoki/__pycache__/renderer.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)    10255 2022-07-26 09:15:36.000000 sotoki-2.0.2/src/sotoki/__pycache__/scraper.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)    10385 2022-08-04 12:35:36.000000 sotoki-2.0.2/src/sotoki/__pycache__/scraper.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     4537 2022-07-26 15:51:30.000000 sotoki-2.0.2/src/sotoki/__pycache__/tags.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     4653 2022-07-29 09:06:31.000000 sotoki-2.0.2/src/sotoki/__pycache__/tags.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     4111 2022-07-26 15:51:29.000000 sotoki-2.0.2/src/sotoki/__pycache__/users.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     4177 2022-07-29 09:06:31.000000 sotoki-2.0.2/src/sotoki/__pycache__/users.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     5896 2022-07-26 17:21:12.000000 sotoki-2.0.2/src/sotoki/archives.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.039738 sotoki-2.0.2/src/sotoki/assets/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.046504 sotoki-2.0.2/src/sotoki/assets/Img/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.046800 sotoki-2.0.2/src/sotoki/assets/Img/developer-story/
--rw-r--r--   0 reg        (501) staff       (20)    28241 2021-07-29 20:59:56.000000 sotoki-2.0.2/src/sotoki/assets/Img/developer-story/timeline.svg
--rw-r--r--   0 reg        (501) staff       (20)      874 2021-07-29 21:00:05.000000 sotoki-2.0.2/src/sotoki/assets/Img/fatarrows.png
--rw-r--r--   0 reg        (501) staff       (20)    79191 2021-07-29 21:00:00.000000 sotoki-2.0.2/src/sotoki/assets/Img/favicons-sprite16-dark.png
--rw-r--r--   0 reg        (501) staff       (20)    79985 2021-07-29 21:00:00.000000 sotoki-2.0.2/src/sotoki/assets/Img/favicons-sprite16.png
--rw-r--r--   0 reg        (501) staff       (20)   251752 2021-07-29 21:00:02.000000 sotoki-2.0.2/src/sotoki/assets/Img/favicons-sprite32-dark.png
--rw-r--r--   0 reg        (501) staff       (20)   256543 2021-07-29 21:00:01.000000 sotoki-2.0.2/src/sotoki/assets/Img/favicons-sprite32.png
--rw-r--r--   0 reg        (501) staff       (20)     1636 2021-07-29 21:00:02.000000 sotoki-2.0.2/src/sotoki/assets/Img/filter-sprites.png
--rw-r--r--   0 reg        (501) staff       (20)     2421 2021-07-29 21:00:03.000000 sotoki-2.0.2/src/sotoki/assets/Img/filter-sprites.svg
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.048332 sotoki-2.0.2/src/sotoki/assets/Img/forms/
--rw-r--r--   0 reg        (501) staff       (20)      395 2021-07-29 20:59:48.000000 sotoki-2.0.2/src/sotoki/assets/Img/forms/icon-disabled.svg
--rw-r--r--   0 reg        (501) staff       (20)      260 2021-07-29 20:59:49.000000 sotoki-2.0.2/src/sotoki/assets/Img/forms/icon-error.svg
--rw-r--r--   0 reg        (501) staff       (20)      163 2021-07-29 20:59:50.000000 sotoki-2.0.2/src/sotoki/assets/Img/forms/icon-success.svg
--rw-r--r--   0 reg        (501) staff       (20)      216 2021-07-29 20:59:49.000000 sotoki-2.0.2/src/sotoki/assets/Img/forms/icon-warning.svg
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.048927 sotoki-2.0.2/src/sotoki/assets/Img/hero/
--rw-r--r--   0 reg        (501) staff       (20)     1661 2021-07-29 20:59:50.000000 sotoki-2.0.2/src/sotoki/assets/Img/hero/anonymousHeroBackground.svg
--rw-r--r--   0 reg        (501) staff       (20)      247 2021-07-29 20:59:47.000000 sotoki-2.0.2/src/sotoki/assets/Img/icon-envelope-fill-gray.png
--rw-r--r--   0 reg        (501) staff       (20)      521 2021-07-29 20:59:47.000000 sotoki-2.0.2/src/sotoki/assets/Img/icon-envelope-fill-gray.svg
--rw-r--r--   0 reg        (501) staff       (20)     6930 2021-07-29 20:59:51.000000 sotoki-2.0.2/src/sotoki/assets/Img/img-upload.png
--rw-r--r--   0 reg        (501) staff       (20)     7091 2021-07-29 21:00:04.000000 sotoki-2.0.2/src/sotoki/assets/Img/img-upload.svg
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.049910 sotoki-2.0.2/src/sotoki/assets/Img/open-graph/
--rw-r--r--   0 reg        (501) staff       (20)      562 2021-07-29 21:00:05.000000 sotoki-2.0.2/src/sotoki/assets/Img/open-graph/checkmark.png
--rw-r--r--   0 reg        (501) staff       (20)      265 2021-07-29 20:59:54.000000 sotoki-2.0.2/src/sotoki/assets/Img/progress-dots.gif
--rw-r--r--   0 reg        (501) staff       (20)    14565 2021-07-29 20:59:58.000000 sotoki-2.0.2/src/sotoki/assets/Img/share-sprite-new.png
--rw-r--r--   0 reg        (501) staff       (20)    23665 2021-07-29 20:59:59.000000 sotoki-2.0.2/src/sotoki/assets/Img/share-sprite-new.svg
--rw-r--r--   0 reg        (501) staff       (20)     5398 2021-07-29 20:59:55.000000 sotoki-2.0.2/src/sotoki/assets/Img/share-sprite.png
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.051815 sotoki-2.0.2/src/sotoki/assets/Img/unified/
--rw-r--r--   0 reg        (501) staff       (20)    20630 2021-07-29 20:59:51.000000 sotoki-2.0.2/src/sotoki/assets/Img/unified/sprites.png
--rw-r--r--   0 reg        (501) staff       (20)     7542 2021-07-29 20:59:52.000000 sotoki-2.0.2/src/sotoki/assets/Img/unified/sprites.svg
--rw-r--r--   0 reg        (501) staff       (20)    11049 2021-07-29 20:59:54.000000 sotoki-2.0.2/src/sotoki/assets/Img/unified/wmd-buttons-dark.svg
--rw-r--r--   0 reg        (501) staff       (20)    11049 2021-07-29 20:59:53.000000 sotoki-2.0.2/src/sotoki/assets/Img/unified/wmd-buttons.svg
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.052440 sotoki-2.0.2/src/sotoki/assets/Img/unifiedmeta/
--rw-r--r--   0 reg        (501) staff       (20)    10346 2021-07-29 20:59:52.000000 sotoki-2.0.2/src/sotoki/assets/Img/unifiedmeta/sprites.png
--rw-r--r--   0 reg        (501) staff       (20)    10031 2021-07-29 20:59:55.000000 sotoki-2.0.2/src/sotoki/assets/Img/unifiedmeta/sprites.svg
--rw-r--r--   0 reg        (501) staff       (20)     8999 2021-07-29 20:59:57.000000 sotoki-2.0.2/src/sotoki/assets/Img/user-profile-sprite.png
--rw-r--r--   0 reg        (501) staff       (20)    15404 2021-07-29 20:59:57.000000 sotoki-2.0.2/src/sotoki/assets/Img/user-profile-sprite.svg
--rw-r--r--   0 reg        (501) staff       (20)      255 2021-07-29 21:00:04.000000 sotoki-2.0.2/src/sotoki/assets/Img/user.svg
--rw-r--r--   0 reg        (501) staff       (20)      271 2021-06-20 12:39:51.000000 sotoki-2.0.2/src/sotoki/assets/README
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.014103 sotoki-2.0.2/src/sotoki/assets/static/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.053323 sotoki-2.0.2/src/sotoki/assets/static/css/
--rw-r--r--   0 reg        (501) staff       (20)     1147 2021-08-03 15:07:01.000000 sotoki-2.0.2/src/sotoki/assets/static/css/highlight.default.min.css
--rw-r--r--   0 reg        (501) staff       (20)     8424 2021-08-03 15:09:04.000000 sotoki-2.0.2/src/sotoki/assets/static/css/sotoki.css
--rw-r--r--   0 reg        (501) staff       (20)   403216 2021-08-03 15:07:01.000000 sotoki-2.0.2/src/sotoki/assets/static/css/stacks.css
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.054126 sotoki-2.0.2/src/sotoki/assets/static/img/
--rw-r--r--   0 reg        (501) staff       (20)      387 2022-10-31 11:18:19.000000 sotoki-2.0.2/src/sotoki/assets/static/img/external-link-ltr-icon.svg
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.062279 sotoki-2.0.2/src/sotoki/assets/static/js/
--rw-r--r--   0 reg        (501) staff       (20)    63532 2021-07-29 20:59:42.000000 sotoki-2.0.2/src/sotoki/assets/static/js/MathJax.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.062601 sotoki-2.0.2/src/sotoki/assets/static/js/config/
--rw-r--r--   0 reg        (501) staff       (20)   314739 2021-07-29 20:59:42.000000 sotoki-2.0.2/src/sotoki/assets/static/js/config/TeX-AMS_HTML-full.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.063656 sotoki-2.0.2/src/sotoki/assets/static/js/extensions/
--rw-r--r--   0 reg        (501) staff       (20)    38244 2021-07-29 20:59:43.000000 sotoki-2.0.2/src/sotoki/assets/static/js/extensions/MathMenu.js
--rw-r--r--   0 reg        (501) staff       (20)     8662 2021-07-29 20:59:43.000000 sotoki-2.0.2/src/sotoki/assets/static/js/extensions/MathZoom.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.063989 sotoki-2.0.2/src/sotoki/assets/static/js/extensions/TeX/
--rw-r--r--   0 reg        (501) staff       (20)     3913 2021-07-29 20:59:43.000000 sotoki-2.0.2/src/sotoki/assets/static/js/extensions/TeX/begingroup.js
--rw-r--r--   0 reg        (501) staff       (20)      370 2022-08-02 16:31:39.000000 sotoki-2.0.2/src/sotoki/assets/static/js/fromnow.js
--rw-r--r--   0 reg        (501) staff       (20)   108999 2021-07-29 20:59:40.000000 sotoki-2.0.2/src/sotoki/assets/static/js/highlight.min.js
--rw-r--r--   0 reg        (501) staff       (20)       21 2022-08-02 16:31:39.000000 sotoki-2.0.2/src/sotoki/assets/static/js/hljs-trigger.js
--rw-r--r--   0 reg        (501) staff       (20)     1888 2022-08-02 16:31:39.000000 sotoki-2.0.2/src/sotoki/assets/static/js/identicons.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.015183 sotoki-2.0.2/src/sotoki/assets/static/js/jax/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.014908 sotoki-2.0.2/src/sotoki/assets/static/js/jax/element/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.015003 sotoki-2.0.2/src/sotoki/assets/static/js/jax/element/mml/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.064314 sotoki-2.0.2/src/sotoki/assets/static/js/jax/element/mml/optable/
--rw-r--r--   0 reg        (501) staff       (20)     1532 2021-07-29 20:59:44.000000 sotoki-2.0.2/src/sotoki/assets/static/js/jax/element/mml/optable/BasicLatin.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.015276 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.015366 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.016038 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.064633 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.015875 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.065335 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/
--rw-r--r--   0 reg        (501) staff       (20)     2447 2021-07-29 20:59:45.000000 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/GreekItalic.js
--rw-r--r--   0 reg        (501) staff       (20)     2253 2021-07-29 20:59:44.000000 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/MathItalic.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.065990 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/
--rw-r--r--   0 reg        (501) staff       (20)     2439 2021-07-29 20:59:46.000000 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/GreekItalic.js
--rw-r--r--   0 reg        (501) staff       (20)     2245 2021-07-29 20:59:45.000000 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/MathItalic.js
--rw-r--r--   0 reg        (501) staff       (20)    38364 2021-07-29 20:59:44.000000 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/fontdata.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.066301 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/TeX/
--rw-r--r--   0 reg        (501) staff       (20)    44346 2021-07-29 20:59:46.000000 sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/TeX/fontdata.js
--rw-r--r--   0 reg        (501) staff       (20)     8907 2021-07-29 20:59:39.000000 sotoki-2.0.2/src/sotoki/assets/static/js/jdenticon.min.js
--rw-r--r--   0 reg        (501) staff       (20)      854 2022-08-02 16:31:39.000000 sotoki-2.0.2/src/sotoki/assets/static/js/mathjax-config.js
--rw-r--r--   0 reg        (501) staff       (20)    58862 2021-07-29 20:59:39.000000 sotoki-2.0.2/src/sotoki/assets/static/js/moment.min.js
--rw-r--r--   0 reg        (501) staff       (20)   519055 2021-07-29 20:59:38.000000 sotoki-2.0.2/src/sotoki/assets/static/js/stack-icons.js
--rw-r--r--   0 reg        (501) staff       (20)     3461 2022-08-04 12:35:08.000000 sotoki-2.0.2/src/sotoki/assets/static/js/tags-filter.js
--rw-r--r--   0 reg        (501) staff       (20)   794389 2021-07-29 20:59:31.000000 sotoki-2.0.2/src/sotoki/assets/static/js/tex-mml-chtml.js
--rw-r--r--   0 reg        (501) staff       (20)     5605 2021-07-29 20:59:41.000000 sotoki-2.0.2/src/sotoki/assets/static/js/webp-handler.js
--rw-r--r--   0 reg        (501) staff       (20)   343139 2021-07-29 20:59:41.000000 sotoki-2.0.2/src/sotoki/assets/static/js/webp-hero.bundle.js
--rw-r--r--   0 reg        (501) staff       (20)     7287 2021-07-29 20:59:40.000000 sotoki-2.0.2/src/sotoki/assets/static/js/webp-hero.polyfill.js
--rw-r--r--   0 reg        (501) staff       (20)     6806 2022-07-15 08:59:36.000000 sotoki-2.0.2/src/sotoki/constants.py
--rw-r--r--   0 reg        (501) staff       (20)     7885 2022-10-31 11:18:05.000000 sotoki-2.0.2/src/sotoki/dependencies.py
--rw-r--r--   0 reg        (501) staff       (20)    10754 2021-08-30 10:46:39.000000 sotoki-2.0.2/src/sotoki/entrypoint.py
--rw-r--r--   0 reg        (501) staff       (20)     3782 2021-08-26 12:08:05.000000 sotoki-2.0.2/src/sotoki/estim-size.py
--rw-r--r--   0 reg        (501) staff       (20)     9565 2022-07-26 15:50:07.000000 sotoki-2.0.2/src/sotoki/posts.py
--rw-r--r--   0 reg        (501) staff       (20)     8168 2021-08-26 15:49:34.000000 sotoki-2.0.2/src/sotoki/renderer.py
--rw-r--r--   0 reg        (501) staff       (20)    14159 2022-08-02 16:26:11.000000 sotoki-2.0.2/src/sotoki/scraper.py
--rw-r--r--   0 reg        (501) staff       (20)     4942 2022-07-26 15:50:07.000000 sotoki-2.0.2/src/sotoki/tags.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.070581 sotoki-2.0.2/src/sotoki/templates/
--rw-r--r--   0 reg        (501) staff       (20)     6196 2021-07-29 19:28:56.000000 sotoki-2.0.2/src/sotoki/templates/about.html
--rw-r--r--   0 reg        (501) staff       (20)     7535 2022-08-02 16:31:39.000000 sotoki-2.0.2/src/sotoki/templates/base.html
--rw-r--r--   0 reg        (501) staff       (20)      504 2021-07-21 16:49:24.000000 sotoki-2.0.2/src/sotoki/templates/linked_list.html
--rw-r--r--   0 reg        (501) staff       (20)     1124 2021-07-21 16:49:47.000000 sotoki-2.0.2/src/sotoki/templates/pagination.html
--rw-r--r--   0 reg        (501) staff       (20)     5750 2021-07-30 16:57:10.000000 sotoki-2.0.2/src/sotoki/templates/post_layout.html
--rw-r--r--   0 reg        (501) staff       (20)     3108 2021-07-21 17:53:11.000000 sotoki-2.0.2/src/sotoki/templates/question.html
--rw-r--r--   0 reg        (501) staff       (20)     1690 2021-07-21 16:50:26.000000 sotoki-2.0.2/src/sotoki/templates/question_list_item.html
--rw-r--r--   0 reg        (501) staff       (20)     1285 2021-07-29 19:17:54.000000 sotoki-2.0.2/src/sotoki/templates/questions.html
--rw-r--r--   0 reg        (501) staff       (20)      949 2021-07-21 17:52:24.000000 sotoki-2.0.2/src/sotoki/templates/single_comment.html
--rw-r--r--   0 reg        (501) staff       (20)     1321 2021-10-19 14:44:25.000000 sotoki-2.0.2/src/sotoki/templates/tag.html
--rw-r--r--   0 reg        (501) staff       (20)     2098 2022-08-04 09:33:25.000000 sotoki-2.0.2/src/sotoki/templates/tags.html
--rw-r--r--   0 reg        (501) staff       (20)     7175 2022-08-02 16:31:39.000000 sotoki-2.0.2/src/sotoki/templates/user.html
--rw-r--r--   0 reg        (501) staff       (20)     1818 2022-08-02 16:31:39.000000 sotoki-2.0.2/src/sotoki/templates/user_card.html
--rw-r--r--   0 reg        (501) staff       (20)     2771 2022-08-02 16:31:39.000000 sotoki-2.0.2/src/sotoki/templates/users.html
--rw-r--r--   0 reg        (501) staff       (20)     4691 2022-07-26 15:50:07.000000 sotoki-2.0.2/src/sotoki/users.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.078027 sotoki-2.0.2/src/sotoki/utils/
--rw-r--r--   0 reg        (501) staff       (20)        0 2021-07-15 09:01:44.000000 sotoki-2.0.2/src/sotoki/utils/__init__.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.091470 sotoki-2.0.2/src/sotoki/utils/__pycache__/
--rw-r--r--   0 reg        (501) staff       (20)      141 2021-07-15 09:07:13.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)      141 2022-07-29 09:06:17.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)    25602 2022-07-26 15:51:35.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/database.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     5200 2022-05-17 13:20:43.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/executor.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     5290 2022-07-29 09:06:37.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/executor.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     2119 2022-07-26 09:15:37.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/generator.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     2189 2022-07-29 09:06:31.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/generator.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)    10556 2022-07-26 15:51:30.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/html.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)    10459 2022-08-04 12:35:36.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/html.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     9116 2022-05-17 13:25:17.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/imager.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     9206 2022-07-29 09:06:37.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/imager.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     4045 2021-08-28 19:55:57.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/misc.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     4169 2022-07-29 09:06:21.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/misc.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     6293 2021-06-21 10:55:25.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/paginator.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     6291 2022-07-29 09:06:31.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/paginator.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)    16341 2021-07-29 11:56:40.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/preparation.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)    16638 2022-07-29 09:06:30.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/preparation.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     5317 2021-08-09 14:38:15.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/progress.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     5341 2022-07-29 09:06:35.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/progress.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)      941 2021-07-15 09:07:14.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/s3.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)      933 2022-07-29 09:06:30.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/s3.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     1564 2021-06-24 08:49:52.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/sevenzip.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     1556 2022-07-29 09:06:21.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/sevenzip.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     4223 2022-07-26 16:42:35.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/shared.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     4225 2022-10-31 13:01:49.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/shared.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     2449 2022-05-17 13:25:05.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/sites.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     2449 2022-07-29 09:06:17.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/sites.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)      468 2021-06-21 10:55:25.000000 sotoki-2.0.2/src/sotoki/utils/__pycache__/system.cpython-38.pyc
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.094960 sotoki-2.0.2/src/sotoki/utils/database/
--rw-r--r--   0 reg        (501) staff       (20)      219 2022-07-26 17:31:29.000000 sotoki-2.0.2/src/sotoki/utils/database/__init__.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.101628 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/
--rw-r--r--   0 reg        (501) staff       (20)      378 2022-07-26 17:32:33.000000 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)      378 2022-07-29 09:06:37.000000 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     3775 2022-07-26 17:32:33.000000 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     3779 2022-07-29 09:06:37.000000 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     5648 2022-07-26 17:32:33.000000 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/posts.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     5643 2022-07-29 09:06:37.000000 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/posts.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     7081 2022-07-26 16:44:38.000000 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/redis.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     7083 2022-07-26 17:32:33.000000 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/redisdb.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     7083 2022-07-29 09:06:37.000000 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/redisdb.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     6126 2022-07-26 17:32:33.000000 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/tags.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     6212 2022-07-29 09:06:37.000000 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/tags.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     4195 2022-07-26 17:32:33.000000 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/users.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     4275 2022-07-29 09:06:37.000000 sotoki-2.0.2/src/sotoki/utils/database/__pycache__/users.cpython-39.pyc
--rw-r--r--   0 reg        (501) staff       (20)     3009 2022-07-26 17:21:12.000000 sotoki-2.0.2/src/sotoki/utils/database/common.py
--rw-r--r--   0 reg        (501) staff       (20)     6553 2022-07-26 17:21:12.000000 sotoki-2.0.2/src/sotoki/utils/database/posts.py
--rw-r--r--   0 reg        (501) staff       (20)     6479 2022-07-26 17:21:12.000000 sotoki-2.0.2/src/sotoki/utils/database/redisdb.py
--rw-r--r--   0 reg        (501) staff       (20)     5639 2022-07-26 17:21:12.000000 sotoki-2.0.2/src/sotoki/utils/database/tags.py
--rw-r--r--   0 reg        (501) staff       (20)     4298 2022-07-26 17:21:12.000000 sotoki-2.0.2/src/sotoki/utils/database/users.py
--rw-r--r--   0 reg        (501) staff       (20)     5628 2022-05-17 13:20:21.000000 sotoki-2.0.2/src/sotoki/utils/executor.py
--rw-r--r--   0 reg        (501) staff       (20)     1791 2022-07-15 08:59:36.000000 sotoki-2.0.2/src/sotoki/utils/generator.py
--rw-r--r--   0 reg        (501) staff       (20)    17306 2022-08-02 16:31:39.000000 sotoki-2.0.2/src/sotoki/utils/html.py
--rw-r--r--   0 reg        (501) staff       (20)    10753 2022-05-17 13:22:30.000000 sotoki-2.0.2/src/sotoki/utils/imager.py
--rw-r--r--   0 reg        (501) staff       (20)     4205 2021-08-26 18:13:19.000000 sotoki-2.0.2/src/sotoki/utils/misc.py
--rw-r--r--   0 reg        (501) staff       (20)     5880 2021-06-20 12:39:51.000000 sotoki-2.0.2/src/sotoki/utils/paginator.py
--rw-r--r--   0 reg        (501) staff       (20)    21684 2021-07-29 11:55:59.000000 sotoki-2.0.2/src/sotoki/utils/preparation.py
--rw-r--r--   0 reg        (501) staff       (20)     5843 2021-08-09 12:17:56.000000 sotoki-2.0.2/src/sotoki/utils/progress.py
--rw-r--r--   0 reg        (501) staff       (20)      899 2021-07-15 09:01:44.000000 sotoki-2.0.2/src/sotoki/utils/s3.py
--rw-r--r--   0 reg        (501) staff       (20)     1476 2021-06-23 15:20:22.000000 sotoki-2.0.2/src/sotoki/utils/sevenzip.py
--rw-r--r--   0 reg        (501) staff       (20)     3812 2022-10-31 11:15:13.000000 sotoki-2.0.2/src/sotoki/utils/shared.py
--rw-r--r--   0 reg        (501) staff       (20)     2303 2022-05-17 13:23:13.000000 sotoki-2.0.2/src/sotoki/utils/sites.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-31 13:14:46.029031 sotoki-2.0.2/src/sotoki.egg-info/
--rw-r--r--   0 reg        (501) staff       (20)     3606 2022-10-31 13:14:45.000000 sotoki-2.0.2/src/sotoki.egg-info/PKG-INFO
--rw-r--r--   0 reg        (501) staff       (20)     7902 2022-10-31 13:14:45.000000 sotoki-2.0.2/src/sotoki.egg-info/SOURCES.txt
--rw-r--r--   0 reg        (501) staff       (20)        1 2022-10-31 13:14:45.000000 sotoki-2.0.2/src/sotoki.egg-info/dependency_links.txt
--rw-r--r--   0 reg        (501) staff       (20)       97 2022-10-31 13:14:45.000000 sotoki-2.0.2/src/sotoki.egg-info/entry_points.txt
--rw-r--r--   0 reg        (501) staff       (20)        1 2022-05-01 18:33:57.000000 sotoki-2.0.2/src/sotoki.egg-info/not-zip-safe
--rw-r--r--   0 reg        (501) staff       (20)      431 2022-10-31 13:14:45.000000 sotoki-2.0.2/src/sotoki.egg-info/requires.txt
--rw-r--r--   0 reg        (501) staff       (20)        7 2022-10-31 13:14:45.000000 sotoki-2.0.2/src/sotoki.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.583782 sotoki-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-07 14:51:08.000000 sotoki-2.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-07 14:51:08.000000 sotoki-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 14:51:08.000000 sotoki-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-07 14:51:25.583782 sotoki-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-07 14:51:08.000000 sotoki-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-07 14:51:08.000000 sotoki-2.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:51:25.583782 sotoki-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-07 14:51:08.000000 sotoki-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.559781 sotoki-2.1.1/src/sotoki/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.563781 sotoki-2.1.1/src/sotoki/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 14:51:20.000000 sotoki-2.1.1/src/sotoki/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-07 14:51:20.000000 sotoki-2.1.1/src/sotoki/__pycache__/dependencies.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/archives.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.563781 sotoki-2.1.1/src/sotoki/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/developer-story/
+-rw-r--r--   0 runner    (1001) docker     (127)    28241 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/developer-story/timeline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki/assets/Img/fatarrows.png
+-rw-r--r--   0 runner    (1001) docker     (127)    88992 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/favicons-sprite16-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90236 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/favicons-sprite16.png
+-rw-r--r--   0 runner    (1001) docker     (127)   277754 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/favicons-sprite32-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)   283322 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/favicons-sprite32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/filter-sprites.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/filter-sprites.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/Img/forms/icon-disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/Img/forms/icon-error.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/forms/icon-success.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/Img/forms/icon-warning.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/hero/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/hero/anonymousHeroBackground.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/Img/icon-envelope-fill-gray.png
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/Img/icon-envelope-fill-gray.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/img-upload.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/img-upload.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/open-graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki/assets/Img/open-graph/checkmark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/progress-dots.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/share-sprite-new.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23665 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/share-sprite-new.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/share-sprite.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/unified/
+-rw-r--r--   0 runner    (1001) docker     (127)    20630 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/unified/sprites.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/unified/sprites.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/unified/wmd-buttons-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/unified/wmd-buttons.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/Img/unifiedmeta/
+-rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/unifiedmeta/sprites.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-07 14:51:23.000000 sotoki-2.1.1/src/sotoki/assets/Img/unifiedmeta/sprites.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/user-profile-sprite.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15404 2024-05-07 14:51:24.000000 sotoki-2.1.1/src/sotoki/assets/Img/user-profile-sprite.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki/assets/Img/user.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.567782 sotoki-2.1.1/src/sotoki/assets/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/css/highlight.default.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/css/sotoki.css
+-rw-r--r--   0 runner    (1001) docker     (127)   828990 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/css/stacks.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.571781 sotoki-2.1.1/src/sotoki/assets/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/img/external-link-ltr-icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    63532 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/MathJax.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/config/
+-rw-r--r--   0 runner    (1001) docker     (127)   314739 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/config/TeX-AMS_HTML-full.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)    38244 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/extensions/MathMenu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/extensions/MathZoom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/extensions/TeX/
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/extensions/TeX/begingroup.js
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/js/fromnow.js
+-rw-r--r--   0 runner    (1001) docker     (127)   108999 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/js/hljs-trigger.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/js/identicons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/element/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/element/mml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/jax/element/mml/optable/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/element/mml/optable/BasicLatin.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.555781 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/GreekItalic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/MathItalic.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/GreekItalic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/MathItalic.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38364 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/fontdata.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.575782 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/TeX/
+-rw-r--r--   0 runner    (1001) docker     (127)    44346 2024-05-07 14:51:22.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/TeX/fontdata.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/jdenticon.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/js/mathjax-config.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58890 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/moment.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   519055 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/stack-icons.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/assets/static/js/tags-filter.js
+-rw-r--r--   0 runner    (1001) docker     (127)   794389 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/tex-mml-chtml.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/webp-handler.js
+-rw-r--r--   0 runner    (1001) docker     (127)   343139 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/webp-hero.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-07 14:51:21.000000 sotoki-2.1.1/src/sotoki/assets/static/js/webp-hero.polyfill.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10919 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.579782 sotoki-2.1.1/src/sotoki/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/about.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/linked_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/post_layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/question.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/question_list_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/questions.html
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/single_comment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/tags.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/user_card.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/templates/users.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.579782 sotoki-2.1.1/src/sotoki/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.583782 sotoki-2.1.1/src/sotoki/utils/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/database/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/database/posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/database/redisdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/database/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/database/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22583 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/preparation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/sevenzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-07 14:51:08.000000 sotoki-2.1.1/src/sotoki/utils/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:51:25.583782 sotoki-2.1.1/src/sotoki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:51:25.000000 sotoki-2.1.1/src/sotoki.egg-info/top_level.txt
```

### Comparing `sotoki-2.0.2/CHANGELOG.md` & `sotoki-2.1.1/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,48 @@
 ## Changelog
 
 All notable changes to this project are documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) (as of version 2.0.1).
 
+## [2.1.1] - 2024-05-07
+
+## Fixed
+
+- Adapt to upstream XML format changes (#305)
+- Add continuous delivery to Pypi (#303)
+
+## [2.1.0] - 2024-03-28
+
+## Added
+
+- Redirection from `/questions/{questionId}` to the question page (#277)
+
+## Changed
+
+- ZIM Tags now include `_videos:no;_details:no` and conditionaly include `_pictures:no` (#278)
+- Default filename now uses `nopic` instead of `all` if using `--without-images` (#278)
+- Multi-language domains now handled as such:
+  - `Language` metadata to be set to `eng,xxx` (xxx being the second language)
+  - `Name` metadata to be like "{domain}_mul_{variant}"
+  - Filename metadata to match `Name`
+- Using zimscraperlib 3.3
+- Changed default publisher metadata from 'Kiwix' to 'openZIM'
+- `description` metadata is now limited to 80 chars, full description goes to the `long_description` (#290)
+
+## Fixed
+
+- Multilanguage ZIM are not perfectly handled (#259)
+- Incorrect image displayed (#284) 
+- Markdown text formatting is not rendered (#286)
+- Harmonize default publisher to openZIM (#291)
+- Docker image: align redis binaries with Python distribution (#294)
+- Issue with xml.sax.saxutils (#298)
+
 ## [2.0.2] - 2022-10-31
 
 ### Changed
 
 - Fixed language-code-looking project codes setting incorrect Language (`ell`, `or`, `vi`)
 - Fixed `--name` parameter not being used to set Name nor filename (#267)
 - Sax parser now explicitly closed after use
```

### Comparing `sotoki-2.0.2/LICENSE` & `sotoki-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/PKG-INFO` & `sotoki-2.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,68 @@
-Metadata-Version: 2.1
-Name: sotoki
-Version: 2.0.2
-Summary: Turn StackExchange dumps into ZIM files for offline usage
-Home-page: https://github.com/openzim/sotoki
-Author: Kiwix
-Author-email: contact+dev@kiwix.org
-License: GPLv3+
-Description: Sotoki
-        ======
-        
-        `Sotoki` (*Stack Overflow to Kiwix*) is an
-        [openZIM](https://github.com/openzim) scraper to create offline
-        versions of [Stack Exchange](https://stackexchange.com) websites such
-        as [Stack Overflow](https://stackoverflow.com/).
-        
-        It is based on Stack Exchange's Data Dumps hosted by [The Internet
-        Archive](https://archive.org/download/stackexchange/).
-        
-        [![CodeFactor](https://www.codefactor.io/repository/github/openzim/sotoki/badge)](https://www.codefactor.io/repository/github/openzim/sotoki)
-        [![Docker](https://img.shields.io/docker/v/openzim/sotoki?label=docker&sort=semver)](https://hub.docker.com/r/openzim/sotoki)
-        [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-        [![PyPI version shields.io](https://img.shields.io/pypi/v/sotoki.svg)](https://pypi.org/project/sotoki/)
-        
-        ## Usage
-        
-        `Sotoki` works off a `domain` that you must provide. That is the
-        domain-name of the stackexchange website you want to scrape. Run
-        `sotoki --list-all` to get a list of those
-        
-        ### Docker
-        
-        ```bash
-        docker run -v my_dir:/output openzim/sotoki sotoki --help
-        ```
-        
-        ### Installation
-        
-        `sotoki` is a Python3 software. If you are not using the
-        [Docker](https://hub.docker.com/r/openzim/sotoki/) image, you are advised to use it in a
-        virtual environment to avoid installing software dependencies on your
-        system.
-        
-        ```sh
-        python3 -m venv ./env  # creates a virtual python environment in ./env folder
-        ./env/bin/pip install -U pip  # upgrade pip (package manager). recommended
-        ./env/bin/pip install -U sotoki  # install/upgrade sotoki inside virtualenv
-        
-        # direct access to in-virtualenv sotoki binary, without shell-attachment
-        ./env/bin/sotoki --help
-        # alias or link it for convenience
-        sudo ln -s $(pwd)/env/bin/sotoki /usr/local/bin/
-        
-        # alternatively, attach virtualenv to shell
-        source env/bin/activate
-        sotoki --help
-        deactivate  # unloads virtualenv from shell
-        ```
-        
-        ## Developers
-        
-        Anybody is welcome to improve the Sotoki.
-        
-        To run Sotoki off the git repository, you'll need to download a few
-        external dependencies that we pack in Python releases. Just run
-        `python src/sotoki/dependencies.py`.
-        
-        See `requirements.txt` for the list of python dependencies.
-        
-        ## Users
-        
-        You don't have to make your own ZIM files of Stack Exchange's Web 
-        sites. Updated ZIM files are built on a regular basis for all 
-        of them. Look at https://library.kiwix.org/?category=stack_exchange
-        to download them.
-        
-Keywords: kiwix zim offline stackechange stackoverflow
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Sotoki
+======
+
+`Sotoki` (*Stack Overflow to Kiwix*) is an
+[openZIM](https://github.com/openzim) scraper to create offline
+versions of [Stack Exchange](https://stackexchange.com) websites such
+as [Stack Overflow](https://stackoverflow.com/).
+
+It is based on Stack Exchange's Data Dumps hosted by [The Internet
+Archive](https://archive.org/download/stackexchange/).
+
+[![CodeFactor](https://www.codefactor.io/repository/github/openzim/sotoki/badge)](https://www.codefactor.io/repository/github/openzim/sotoki)
+[![Docker](https://ghcr-badge.deta.dev/openzim/sotoki/latest_tag?label=docker)](https://ghcr.io/openzim/sotoki)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/sotoki.svg)](https://pypi.org/project/sotoki/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sotoki.svg)](https://pypi.org/project/sotoki)
+
+## Usage
+
+`Sotoki` works off a `domain` that you must provide. That is the
+domain-name of the stackexchange website you want to scrape. Run
+`sotoki --list-all` to get a list of those
+
+### Docker
+
+```bash
+docker run -v my_dir:/output ghcr.io/openzim/sotoki sotoki --help
+```
+
+### Installation
+
+`sotoki` is a Python3 software. If you are not using the
+[Docker](https://ghcr.io/openzim/sotoki/) image, you are advised to use it in a
+virtual environment to avoid installing software dependencies on your
+system.
+
+```sh
+python3 -m venv ./env  # creates a virtual python environment in ./env folder
+./env/bin/pip install -U pip  # upgrade pip (package manager). recommended
+./env/bin/pip install -U sotoki  # install/upgrade sotoki inside virtualenv
+
+# direct access to in-virtualenv sotoki binary, without shell-attachment
+./env/bin/sotoki --help
+# alias or link it for convenience
+sudo ln -s $(pwd)/env/bin/sotoki /usr/local/bin/
+
+# alternatively, attach virtualenv to shell
+source env/bin/activate
+sotoki --help
+deactivate  # unloads virtualenv from shell
+```
+
+## Developers
+
+Anybody is welcome to improve the Sotoki.
+
+To run Sotoki off the git repository, you'll need to download a few
+external dependencies that we pack in Python releases. Just run
+`python src/sotoki/dependencies.py`.
+
+See `requirements.txt` for the list of python dependencies.
+
+## Users
+
+You don't have to make your own ZIM files of Stack Exchange's Web 
+sites. Updated ZIM files are built on a regular basis for all 
+of them. Look at https://library.kiwix.org/?category=stack_exchange
+to download them.
```

### Comparing `sotoki-2.0.2/setup.py` & `sotoki-2.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # vim: ai ts=4 sts=4 et sw=4 nu
 
 import sys
 import pathlib
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
 
 root_dir = pathlib.Path(__file__).parent
 
 # download assets dependencies before packing
 sys.path = [str(root_dir.joinpath("src").resolve())] + sys.path
 from sotoki.dependencies import main as download_deps
 
@@ -27,15 +27,15 @@
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="Kiwix",
     author_email="contact+dev@kiwix.org",
     url="https://github.com/openzim/sotoki",
     keywords="kiwix zim offline stackechange stackoverflow",
     license="GPLv3+",
-    packages=find_packages("src"),
+    packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         line.strip()
         for line in read("requirements.txt").splitlines()
         if not line.strip().startswith("#")
     ],
     zip_safe=False,
```

### Comparing `sotoki-2.0.2/src/sotoki/__pycache__/dependencies.cpython-38.pyc` & `sotoki-2.1.1/src/sotoki/__pycache__/dependencies.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Aug  3 14:45:23 2021 UTC, .py size: 8101 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,411 +1,403 @@
-00000000: 550d 0d0a 0000 0000 8356 0961 a51f 0000  U........V.a....
+00000000: 550d 0d0a 0000 0000 dc3f 3a66 cd1e 0000  U........?:f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0036 0000 0040 0000 0073 a600 0000 6400  .6...@...s....d.
+00000020: 0035 0000 0040 0000 0073 a400 0000 6400  .5...@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6405 6406 6407 6408 6409  ..d.d.d.d.d.d.d.
 00000050: 640a 640b 640c 640d 640e 640f 6410 6411  d.d.d.d.d.d.d.d.
 00000060: 6412 6413 6414 6415 6416 6417 6418 6419  d.d.d.d.d.d.d.d.
 00000070: 641a 641b 641c 641d 641e 641f 6420 6421  d.d.d.d.d.d.d d!
 00000080: 6422 6423 6424 6425 6426 6427 6428 6429  d"d#d$d%d&d'd(d)
 00000090: 642a 642b 642c 642d 642e 642f 6430 6431  d*d+d,d-d.d/d0d1
-000000a0: 6432 6433 6434 6435 6436 6437 6438 6736  d2d3d4d5d6d7d8g6
-000000b0: 5a03 6439 643a 8400 5a04 643b 643c 8400  Z.d9d:..Z.d;d<..
-000000c0: 5a05 6506 643d 6b02 72a2 6505 8300 0100  Z.e.d=k.r.e.....
-000000d0: 6401 5300 293e e900 0000 004e 2901 da0b  d.S.)>.....N)...
-000000e0: 7374 7265 616d 5f66 696c 6529 027a 1573  stream_file).z.s
-000000f0: 7461 7469 632f 6373 732f 7374 6163 6b73  tatic/css/stacks
-00000100: 2e63 7373 7a38 6874 7470 733a 2f2f 6364  .cssz8https://cd
-00000110: 6e2e 7373 7461 7469 632e 6e65 742f 5368  n.sstatic.net/Sh
-00000120: 6172 6564 2f73 7461 636b 732e 6373 733f  ared/stacks.css?
-00000130: 763d 6361 3533 3139 6534 3963 3633 2902  v=ca5319e49c63).
-00000140: 7a1a 7374 6174 6963 2f6a 732f 7465 782d  z.static/js/tex-
-00000150: 6d6d 6c2d 6368 746d 6c2e 6a73 7a3f 6874  mml-chtml.jsz?ht
-00000160: 7470 733a 2f2f 6364 6e2e 6a73 6465 6c69  tps://cdn.jsdeli
-00000170: 7672 2e6e 6574 2f6e 706d 2f6d 6174 686a  vr.net/npm/mathj
-00000180: 6178 4033 2e31 2e33 2f65 7335 2f74 6578  ax@3.1.3/es5/tex
-00000190: 2d6d 6d6c 2d63 6874 6d6c 2e6a 7329 027a  -mml-chtml.js).z
-000001a0: 1873 7461 7469 632f 6a73 2f73 7461 636b  .static/js/stack
-000001b0: 2d69 636f 6e73 2e6a 737a 4368 7474 7073  -icons.jszChttps
-000001c0: 3a2f 2f75 6e70 6b67 2e63 6f6d 2f40 7374  ://unpkg.com/@st
-000001d0: 6163 6b6f 7665 7266 6c6f 772f 7374 6163  ackoverflow/stac
-000001e0: 6b73 2d69 636f 6e73 4032 2e32 302e 302f  ks-icons@2.20.0/
-000001f0: 6275 696c 642f 696e 6465 782e 6a73 2902  build/index.js).
-00000200: 7a17 7374 6174 6963 2f6a 732f 6d6f 6d65  z.static/js/mome
-00000210: 6e74 2e6d 696e 2e6a 737a 2c68 7474 7073  nt.min.jsz,https
-00000220: 3a2f 2f6d 6f6d 656e 746a 732e 636f 6d2f  ://momentjs.com/
-00000230: 646f 776e 6c6f 6164 732f 6d6f 6d65 6e74  downloads/moment
-00000240: 2e6d 696e 2e6a 7329 027a 1a73 7461 7469  .min.js).z.stati
-00000250: 632f 6a73 2f6a 6465 6e74 6963 6f6e 2e6d  c/js/jdenticon.m
-00000260: 696e 2e6a 737a 4f68 7474 7073 3a2f 2f72  in.jszOhttps://r
-00000270: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000280: 7465 6e74 2e63 6f6d 2f64 6d65 7374 6572  tent.com/dmester
-00000290: 2f6a 6465 6e74 6963 6f6e 2f33 2e31 2e30  /jdenticon/3.1.0
-000002a0: 2f64 6973 742f 6a64 656e 7469 636f 6e2e  /dist/jdenticon.
-000002b0: 6d69 6e2e 6a73 2902 7a24 7374 6174 6963  min.js).z$static
-000002c0: 2f63 7373 2f68 6967 686c 6967 6874 2e64  /css/highlight.d
-000002d0: 6566 6175 6c74 2e6d 696e 2e63 7373 7a51  efault.min.csszQ
-000002e0: 6874 7470 733a 2f2f 6364 6e6a 732e 636c  https://cdnjs.cl
-000002f0: 6f75 6466 6c61 7265 2e63 6f6d 2f61 6a61  oudflare.com/aja
-00000300: 782f 6c69 6273 2f68 6967 686c 6967 6874  x/libs/highlight
-00000310: 2e6a 732f 3131 2e31 2e30 2f73 7479 6c65  .js/11.1.0/style
-00000320: 732f 6465 6661 756c 742e 6d69 6e2e 6373  s/default.min.cs
-00000330: 7329 027a 1a73 7461 7469 632f 6a73 2f68  s).z.static/js/h
-00000340: 6967 686c 6967 6874 2e6d 696e 2e6a 737a  ighlight.min.jsz
-00000350: 4b68 7474 7073 3a2f 2f63 646e 6a73 2e63  Khttps://cdnjs.c
-00000360: 6c6f 7564 666c 6172 652e 636f 6d2f 616a  loudflare.com/aj
-00000370: 6178 2f6c 6962 732f 6869 6768 6c69 6768  ax/libs/highligh
-00000380: 742e 6a73 2f31 312e 312e 302f 6869 6768  t.js/11.1.0/high
-00000390: 6c69 6768 742e 6d69 6e2e 6a73 2902 7a1f  light.min.js).z.
-000003a0: 7374 6174 6963 2f6a 732f 7765 6270 2d68  static/js/webp-h
-000003b0: 6572 6f2e 706f 6c79 6669 6c6c 2e6a 737a  ero.polyfill.jsz
-000003c0: 3e68 7474 7073 3a2f 2f75 6e70 6b67 2e63  >https://unpkg.c
-000003d0: 6f6d 2f77 6562 702d 6865 726f 4030 2e30  om/webp-hero@0.0
-000003e0: 2e30 2d64 6576 2e32 372f 6469 7374 2d63  .0-dev.27/dist-c
-000003f0: 6a73 2f70 6f6c 7966 696c 6c73 2e6a 7329  js/polyfills.js)
-00000400: 027a 1d73 7461 7469 632f 6a73 2f77 6562  .z.static/js/web
-00000410: 702d 6865 726f 2e62 756e 646c 652e 6a73  p-hero.bundle.js
-00000420: 7a45 6874 7470 733a 2f2f 756e 706b 672e  zEhttps://unpkg.
-00000430: 636f 6d2f 7765 6270 2d68 6572 6f40 302e  com/webp-hero@0.
-00000440: 302e 302d 6465 762e 3237 2f64 6973 742d  0.0-dev.27/dist-
-00000450: 636a 732f 7765 6270 2d68 6572 6f2e 6275  cjs/webp-hero.bu
-00000460: 6e64 6c65 2e6a 7329 027a 1973 7461 7469  ndle.js).z.stati
-00000470: 632f 6a73 2f77 6562 702d 6861 6e64 6c65  c/js/webp-handle
-00000480: 722e 6a73 7a87 6874 7470 733a 2f2f 6769  r.jsz.https://gi
-00000490: 7374 2e67 6974 6875 6275 7365 7263 6f6e  st.githubusercon
-000004a0: 7465 6e74 2e63 6f6d 2f72 6761 7564 696e  tent.com/rgaudin
-000004b0: 2f36 3062 6239 6363 3666 3138 3761 6464  /60bb9cc6f187add
-000004c0: 3530 3635 3834 3235 3830 3238 6238 6565  506584258028b8ee
-000004d0: 312f 7261 772f 3964 3537 3562 3865 3235  1/raw/9d575b8e25
-000004e0: 6436 3765 6564 3261 3963 3961 3931 6433  d67eed2a9c9a91d3
-000004f0: 6530 3533 6130 3036 3264 3266 6337 2f77  e053a0062d2fc7/w
-00000500: 6562 2d68 616e 646c 6572 2e6a 7329 027a  eb-handler.js).z
-00000510: 2573 7461 7469 632f 696d 672f 6578 7465  %static/img/exte
-00000520: 726e 616c 2d6c 696e 6b2d 6c74 722d 6963  rnal-link-ltr-ic
-00000530: 6f6e 2e73 7667 7a60 6874 7470 733a 2f2f  on.svgz`https://
-00000540: 6672 2e77 696b 6970 6564 6961 2e6f 7267  fr.wikipedia.org
-00000550: 2f77 2f73 6b69 6e73 2f56 6563 746f 722f  /w/skins/Vector/
-00000560: 7265 736f 7572 6365 732f 636f 6d6d 6f6e  resources/common
-00000570: 2f69 6d61 6765 732f 6578 7465 726e 616c  /images/external
-00000580: 2d6c 696e 6b2d 6c74 722d 6963 6f6e 2e73  -link-ltr-icon.s
-00000590: 7667 3f34 3865 3534 2902 7a14 7374 6174  vg?48e54).z.stat
-000005a0: 6963 2f6a 732f 4d61 7468 4a61 782e 6a73  ic/js/MathJax.js
-000005b0: 7a58 6874 7470 733a 2f2f 6364 6e6a 732e  zXhttps://cdnjs.
-000005c0: 636c 6f75 6466 6c61 7265 2e63 6f6d 2f61  cloudflare.com/a
-000005d0: 6a61 782f 6c69 6273 2f6d 6174 686a 6178  jax/libs/mathjax
-000005e0: 2f32 2e37 2e35 2f4d 6174 684a 6178 2e6a  /2.7.5/MathJax.j
-000005f0: 733f 636f 6e66 6967 3d54 6558 2d41 4d53  s?config=TeX-AMS
-00000600: 5f48 544d 4c2d 6675 6c6c 2902 7a25 7374  _HTML-full).z%st
-00000610: 6174 6963 2f6a 732f 636f 6e66 6967 2f54  atic/js/config/T
-00000620: 6558 2d41 4d53 5f48 544d 4c2d 6675 6c6c  eX-AMS_HTML-full
-00000630: 2e6a 737a 5868 7474 7073 3a2f 2f63 646e  .jszXhttps://cdn
-00000640: 6a73 2e63 6c6f 7564 666c 6172 652e 636f  js.cloudflare.co
-00000650: 6d2f 616a 6178 2f6c 6962 732f 6d61 7468  m/ajax/libs/math
-00000660: 6a61 782f 322e 372e 352f 636f 6e66 6967  jax/2.7.5/config
-00000670: 2f54 6558 2d41 4d53 5f48 544d 4c2d 6675  /TeX-AMS_HTML-fu
-00000680: 6c6c 2e6a 733f 563d 322e 372e 3529 027a  ll.js?V=2.7.5).z
-00000690: 2073 7461 7469 632f 6a73 2f65 7874 656e   static/js/exten
-000006a0: 7369 6f6e 732f 4d61 7468 4d65 6e75 2e6a  sions/MathMenu.j
-000006b0: 737a 5368 7474 7073 3a2f 2f63 646e 6a73  szShttps://cdnjs
-000006c0: 2e63 6c6f 7564 666c 6172 652e 636f 6d2f  .cloudflare.com/
-000006d0: 616a 6178 2f6c 6962 732f 6d61 7468 6a61  ajax/libs/mathja
-000006e0: 782f 322e 372e 352f 6578 7465 6e73 696f  x/2.7.5/extensio
-000006f0: 6e73 2f4d 6174 684d 656e 752e 6a73 3f56  ns/MathMenu.js?V
-00000700: 3d32 2e37 2e35 2902 7a20 7374 6174 6963  =2.7.5).z static
-00000710: 2f6a 732f 6578 7465 6e73 696f 6e73 2f4d  /js/extensions/M
-00000720: 6174 685a 6f6f 6d2e 6a73 7a53 6874 7470  athZoom.jszShttp
-00000730: 733a 2f2f 6364 6e6a 732e 636c 6f75 6466  s://cdnjs.cloudf
-00000740: 6c61 7265 2e63 6f6d 2f61 6a61 782f 6c69  lare.com/ajax/li
-00000750: 6273 2f6d 6174 686a 6178 2f32 2e37 2e35  bs/mathjax/2.7.5
-00000760: 2f65 7874 656e 7369 6f6e 732f 4d61 7468  /extensions/Math
-00000770: 5a6f 6f6d 2e6a 733f 563d 322e 372e 3529  Zoom.js?V=2.7.5)
-00000780: 027a 2673 7461 7469 632f 6a73 2f65 7874  .z&static/js/ext
-00000790: 656e 7369 6f6e 732f 5465 582f 6265 6769  ensions/TeX/begi
-000007a0: 6e67 726f 7570 2e6a 737a 5968 7474 7073  ngroup.jszYhttps
-000007b0: 3a2f 2f63 646e 6a73 2e63 6c6f 7564 666c  ://cdnjs.cloudfl
-000007c0: 6172 652e 636f 6d2f 616a 6178 2f6c 6962  are.com/ajax/lib
-000007d0: 732f 6d61 7468 6a61 782f 322e 372e 352f  s/mathjax/2.7.5/
-000007e0: 6578 7465 6e73 696f 6e73 2f54 6558 2f62  extensions/TeX/b
-000007f0: 6567 696e 6772 6f75 702e 6a73 3f56 3d32  egingroup.js?V=2
-00000800: 2e37 2e35 2902 7a34 7374 6174 6963 2f6a  .7.5).z4static/j
-00000810: 732f 6a61 782f 6f75 7470 7574 2f48 544d  s/jax/output/HTM
-00000820: 4c2d 4353 532f 666f 6e74 732f 5354 4958  L-CSS/fonts/STIX
-00000830: 2f66 6f6e 7464 6174 612e 6a73 7a67 6874  /fontdata.jszght
-00000840: 7470 733a 2f2f 6364 6e6a 732e 636c 6f75  tps://cdnjs.clou
-00000850: 6466 6c61 7265 2e63 6f6d 2f61 6a61 782f  dflare.com/ajax/
-00000860: 6c69 6273 2f6d 6174 686a 6178 2f32 2e37  libs/mathjax/2.7
-00000870: 2e35 2f6a 6178 2f6f 7574 7075 742f 4854  .5/jax/output/HT
-00000880: 4d4c 2d43 5353 2f66 6f6e 7473 2f53 5449  ML-CSS/fonts/STI
-00000890: 582f 666f 6e74 6461 7461 2e6a 733f 563d  X/fontdata.js?V=
-000008a0: 322e 372e 3529 027a 2f73 7461 7469 632f  2.7.5).z/static/
-000008b0: 6a73 2f6a 6178 2f65 6c65 6d65 6e74 2f6d  js/jax/element/m
-000008c0: 6d6c 2f6f 7074 6162 6c65 2f42 6173 6963  ml/optable/Basic
-000008d0: 4c61 7469 6e2e 6a73 7a62 6874 7470 733a  Latin.jszbhttps:
-000008e0: 2f2f 6364 6e6a 732e 636c 6f75 6466 6c61  //cdnjs.cloudfla
-000008f0: 7265 2e63 6f6d 2f61 6a61 782f 6c69 6273  re.com/ajax/libs
-00000900: 2f6d 6174 686a 6178 2f32 2e37 2e35 2f6a  /mathjax/2.7.5/j
-00000910: 6178 2f65 6c65 6d65 6e74 2f6d 6d6c 2f6f  ax/element/mml/o
-00000920: 7074 6162 6c65 2f42 6173 6963 4c61 7469  ptable/BasicLati
-00000930: 6e2e 6a73 3f56 3d32 2e37 2e35 2902 7a45  n.js?V=2.7.5).zE
-00000940: 7374 6174 6963 2f6a 732f 6a61 782f 6f75  static/js/jax/ou
-00000950: 7470 7574 2f48 544d 4c2d 4353 532f 666f  tput/HTML-CSS/fo
-00000960: 6e74 732f 5354 4958 2f47 656e 6572 616c  nts/STIX/General
-00000970: 2f49 7461 6c69 632f 4d61 7468 4974 616c  /Italic/MathItal
-00000980: 6963 2e6a 737a 7868 7474 7073 3a2f 2f63  ic.jszxhttps://c
-00000990: 646e 6a73 2e63 6c6f 7564 666c 6172 652e  dnjs.cloudflare.
-000009a0: 636f 6d2f 616a 6178 2f6c 6962 732f 6d61  com/ajax/libs/ma
-000009b0: 7468 6a61 782f 322e 372e 352f 6a61 782f  thjax/2.7.5/jax/
-000009c0: 6f75 7470 7574 2f48 544d 4c2d 4353 532f  output/HTML-CSS/
-000009d0: 666f 6e74 732f 5354 4958 2f47 656e 6572  fonts/STIX/Gener
-000009e0: 616c 2f49 7461 6c69 632f 4d61 7468 4974  al/Italic/MathIt
-000009f0: 616c 6963 2e6a 733f 563d 322e 372e 3529  alic.js?V=2.7.5)
-00000a00: 027a 4673 7461 7469 632f 6a73 2f6a 6178  .zFstatic/js/jax
-00000a10: 2f6f 7574 7075 742f 4854 4d4c 2d43 5353  /output/HTML-CSS
-00000a20: 2f66 6f6e 7473 2f53 5449 582f 4765 6e65  /fonts/STIX/Gene
-00000a30: 7261 6c2f 5265 6775 6c61 722f 4d61 7468  ral/Regular/Math
-00000a40: 4974 616c 6963 2e6a 737a 7968 7474 7073  Italic.jszyhttps
-00000a50: 3a2f 2f63 646e 6a73 2e63 6c6f 7564 666c  ://cdnjs.cloudfl
-00000a60: 6172 652e 636f 6d2f 616a 6178 2f6c 6962  are.com/ajax/lib
-00000a70: 732f 6d61 7468 6a61 782f 322e 372e 352f  s/mathjax/2.7.5/
-00000a80: 6a61 782f 6f75 7470 7574 2f48 544d 4c2d  jax/output/HTML-
-00000a90: 4353 532f 666f 6e74 732f 5354 4958 2f47  CSS/fonts/STIX/G
-00000aa0: 656e 6572 616c 2f52 6567 756c 6172 2f4d  eneral/Regular/M
-00000ab0: 6174 6849 7461 6c69 632e 6a73 3f56 3d32  athItalic.js?V=2
-00000ac0: 2e37 2e35 2902 7a46 7374 6174 6963 2f6a  .7.5).zFstatic/j
-00000ad0: 732f 6a61 782f 6f75 7470 7574 2f48 544d  s/jax/output/HTM
-00000ae0: 4c2d 4353 532f 666f 6e74 732f 5354 4958  L-CSS/fonts/STIX
-00000af0: 2f47 656e 6572 616c 2f49 7461 6c69 632f  /General/Italic/
-00000b00: 4772 6565 6b49 7461 6c69 632e 6a73 7a79  GreekItalic.jszy
-00000b10: 6874 7470 733a 2f2f 6364 6e6a 732e 636c  https://cdnjs.cl
-00000b20: 6f75 6466 6c61 7265 2e63 6f6d 2f61 6a61  oudflare.com/aja
-00000b30: 782f 6c69 6273 2f6d 6174 686a 6178 2f32  x/libs/mathjax/2
-00000b40: 2e37 2e35 2f6a 6178 2f6f 7574 7075 742f  .7.5/jax/output/
-00000b50: 4854 4d4c 2d43 5353 2f66 6f6e 7473 2f53  HTML-CSS/fonts/S
-00000b60: 5449 582f 4765 6e65 7261 6c2f 4974 616c  TIX/General/Ital
-00000b70: 6963 2f47 7265 656b 4974 616c 6963 2e6a  ic/GreekItalic.j
-00000b80: 733f 563d 322e 372e 3529 027a 4773 7461  s?V=2.7.5).zGsta
-00000b90: 7469 632f 6a73 2f6a 6178 2f6f 7574 7075  tic/js/jax/outpu
-00000ba0: 742f 4854 4d4c 2d43 5353 2f66 6f6e 7473  t/HTML-CSS/fonts
-00000bb0: 2f53 5449 582f 4765 6e65 7261 6c2f 5265  /STIX/General/Re
-00000bc0: 6775 6c61 722f 4772 6565 6b49 7461 6c69  gular/GreekItali
-00000bd0: 632e 6a73 7a7a 6874 7470 733a 2f2f 6364  c.jszzhttps://cd
-00000be0: 6e6a 732e 636c 6f75 6466 6c61 7265 2e63  njs.cloudflare.c
-00000bf0: 6f6d 2f61 6a61 782f 6c69 6273 2f6d 6174  om/ajax/libs/mat
-00000c00: 686a 6178 2f32 2e37 2e35 2f6a 6178 2f6f  hjax/2.7.5/jax/o
-00000c10: 7574 7075 742f 4854 4d4c 2d43 5353 2f66  utput/HTML-CSS/f
-00000c20: 6f6e 7473 2f53 5449 582f 4765 6e65 7261  onts/STIX/Genera
-00000c30: 6c2f 5265 6775 6c61 722f 4772 6565 6b49  l/Regular/GreekI
-00000c40: 7461 6c69 632e 6a73 3f56 3d32 2e37 2e35  talic.js?V=2.7.5
-00000c50: 2902 7a33 7374 6174 6963 2f6a 732f 6a61  ).z3static/js/ja
-00000c60: 782f 6f75 7470 7574 2f48 544d 4c2d 4353  x/output/HTML-CS
-00000c70: 532f 666f 6e74 732f 5465 582f 666f 6e74  S/fonts/TeX/font
-00000c80: 6461 7461 2e6a 737a 6668 7474 7073 3a2f  data.jszfhttps:/
-00000c90: 2f63 646e 6a73 2e63 6c6f 7564 666c 6172  /cdnjs.cloudflar
-00000ca0: 652e 636f 6d2f 616a 6178 2f6c 6962 732f  e.com/ajax/libs/
-00000cb0: 6d61 7468 6a61 782f 322e 372e 352f 6a61  mathjax/2.7.5/ja
-00000cc0: 782f 6f75 7470 7574 2f48 544d 4c2d 4353  x/output/HTML-CS
-00000cd0: 532f 666f 6e74 732f 5465 582f 666f 6e74  S/fonts/TeX/font
-00000ce0: 6461 7461 2e6a 733f 563d 322e 372e 3529  data.js?V=2.7.5)
-00000cf0: 027a 1f49 6d67 2f69 636f 6e2d 656e 7665  .z.Img/icon-enve
-00000d00: 6c6f 7065 2d66 696c 6c2d 6772 6179 2e70  lope-fill-gray.p
-00000d10: 6e67 7a37 6874 7470 733a 2f2f 6364 6e2e  ngz7https://cdn.
-00000d20: 7373 7461 7469 632e 6e65 742f 496d 672f  sstatic.net/Img/
-00000d30: 6963 6f6e 2d65 6e76 656c 6f70 652d 6669  icon-envelope-fi
-00000d40: 6c6c 2d67 7261 792e 706e 6729 027a 1f49  ll-gray.png).z.I
-00000d50: 6d67 2f69 636f 6e2d 656e 7665 6c6f 7065  mg/icon-envelope
-00000d60: 2d66 696c 6c2d 6772 6179 2e73 7667 7a37  -fill-gray.svgz7
-00000d70: 6874 7470 733a 2f2f 6364 6e2e 7373 7461  https://cdn.ssta
-00000d80: 7469 632e 6e65 742f 496d 672f 6963 6f6e  tic.net/Img/icon
-00000d90: 2d65 6e76 656c 6f70 652d 6669 6c6c 2d67  -envelope-fill-g
-00000da0: 7261 792e 7376 6729 027a 1b49 6d67 2f66  ray.svg).z.Img/f
-00000db0: 6f72 6d73 2f69 636f 6e2d 6469 7361 626c  orms/icon-disabl
-00000dc0: 6564 2e73 7667 7a33 6874 7470 733a 2f2f  ed.svgz3https://
-00000dd0: 6364 6e2e 7373 7461 7469 632e 6e65 742f  cdn.sstatic.net/
-00000de0: 496d 672f 666f 726d 732f 6963 6f6e 2d64  Img/forms/icon-d
-00000df0: 6973 6162 6c65 642e 7376 6729 027a 1a49  isabled.svg).z.I
-00000e00: 6d67 2f66 6f72 6d73 2f69 636f 6e2d 7761  mg/forms/icon-wa
-00000e10: 726e 696e 672e 7376 677a 3268 7474 7073  rning.svgz2https
-00000e20: 3a2f 2f63 646e 2e73 7374 6174 6963 2e6e  ://cdn.sstatic.n
-00000e30: 6574 2f49 6d67 2f66 6f72 6d73 2f69 636f  et/Img/forms/ico
-00000e40: 6e2d 7761 726e 696e 672e 7376 6729 027a  n-warning.svg).z
-00000e50: 1849 6d67 2f66 6f72 6d73 2f69 636f 6e2d  .Img/forms/icon-
-00000e60: 6572 726f 722e 7376 677a 3068 7474 7073  error.svgz0https
-00000e70: 3a2f 2f63 646e 2e73 7374 6174 6963 2e6e  ://cdn.sstatic.n
-00000e80: 6574 2f49 6d67 2f66 6f72 6d73 2f69 636f  et/Img/forms/ico
-00000e90: 6e2d 6572 726f 722e 7376 6729 027a 1a49  n-error.svg).z.I
-00000ea0: 6d67 2f66 6f72 6d73 2f69 636f 6e2d 7375  mg/forms/icon-su
-00000eb0: 6363 6573 732e 7376 677a 3268 7474 7073  ccess.svgz2https
-00000ec0: 3a2f 2f63 646e 2e73 7374 6174 6963 2e6e  ://cdn.sstatic.n
-00000ed0: 6574 2f49 6d67 2f66 6f72 6d73 2f69 636f  et/Img/forms/ico
-00000ee0: 6e2d 7375 6363 6573 732e 7376 6729 027a  n-success.svg).z
-00000ef0: 2449 6d67 2f68 6572 6f2f 616e 6f6e 796d  $Img/hero/anonym
-00000f00: 6f75 7348 6572 6f42 6163 6b67 726f 756e  ousHeroBackgroun
-00000f10: 642e 7376 677a 3c68 7474 7073 3a2f 2f63  d.svgz<https://c
-00000f20: 646e 2e73 7374 6174 6963 2e6e 6574 2f49  dn.sstatic.net/I
-00000f30: 6d67 2f68 6572 6f2f 616e 6f6e 796d 6f75  mg/hero/anonymou
-00000f40: 7348 6572 6f42 6163 6b67 726f 756e 642e  sHeroBackground.
-00000f50: 7376 6729 027a 1249 6d67 2f69 6d67 2d75  svg).z.Img/img-u
-00000f60: 706c 6f61 642e 706e 677a 2a68 7474 7073  pload.pngz*https
-00000f70: 3a2f 2f63 646e 2e73 7374 6174 6963 2e6e  ://cdn.sstatic.n
-00000f80: 6574 2f49 6d67 2f69 6d67 2d75 706c 6f61  et/Img/img-uploa
-00000f90: 642e 706e 6729 027a 1749 6d67 2f75 6e69  d.png).z.Img/uni
-00000fa0: 6669 6564 2f73 7072 6974 6573 2e70 6e67  fied/sprites.png
-00000fb0: 7a2f 6874 7470 733a 2f2f 6364 6e2e 7373  z/https://cdn.ss
-00000fc0: 7461 7469 632e 6e65 742f 496d 672f 756e  tatic.net/Img/un
-00000fd0: 6966 6965 642f 7370 7269 7465 732e 706e  ified/sprites.pn
-00000fe0: 6729 027a 1749 6d67 2f75 6e69 6669 6564  g).z.Img/unified
-00000ff0: 2f73 7072 6974 6573 2e73 7667 7a2f 6874  /sprites.svgz/ht
-00001000: 7470 733a 2f2f 6364 6e2e 7373 7461 7469  tps://cdn.sstati
-00001010: 632e 6e65 742f 496d 672f 756e 6966 6965  c.net/Img/unifie
-00001020: 642f 7370 7269 7465 732e 7376 6729 027a  d/sprites.svg).z
-00001030: 1b49 6d67 2f75 6e69 6669 6564 6d65 7461  .Img/unifiedmeta
-00001040: 2f73 7072 6974 6573 2e70 6e67 7a33 6874  /sprites.pngz3ht
-00001050: 7470 733a 2f2f 6364 6e2e 7373 7461 7469  tps://cdn.sstati
-00001060: 632e 6e65 742f 496d 672f 756e 6966 6965  c.net/Img/unifie
-00001070: 646d 6574 612f 7370 7269 7465 732e 706e  dmeta/sprites.pn
-00001080: 6729 027a 1b49 6d67 2f75 6e69 6669 6564  g).z.Img/unified
-00001090: 2f77 6d64 2d62 7574 746f 6e73 2e73 7667  /wmd-buttons.svg
-000010a0: 7a33 6874 7470 733a 2f2f 6364 6e2e 7373  z3https://cdn.ss
-000010b0: 7461 7469 632e 6e65 742f 496d 672f 756e  tatic.net/Img/un
-000010c0: 6966 6965 642f 776d 642d 6275 7474 6f6e  ified/wmd-button
-000010d0: 732e 7376 6729 027a 2049 6d67 2f75 6e69  s.svg).z Img/uni
-000010e0: 6669 6564 2f77 6d64 2d62 7574 746f 6e73  fied/wmd-buttons
-000010f0: 2d64 6172 6b2e 7376 677a 3868 7474 7073  -dark.svgz8https
-00001100: 3a2f 2f63 646e 2e73 7374 6174 6963 2e6e  ://cdn.sstatic.n
-00001110: 6574 2f49 6d67 2f75 6e69 6669 6564 2f77  et/Img/unified/w
-00001120: 6d64 2d62 7574 746f 6e73 2d64 6172 6b2e  md-buttons-dark.
-00001130: 7376 6729 027a 1549 6d67 2f70 726f 6772  svg).z.Img/progr
-00001140: 6573 732d 646f 7473 2e67 6966 7a2d 6874  ess-dots.gifz-ht
-00001150: 7470 733a 2f2f 6364 6e2e 7373 7461 7469  tps://cdn.sstati
-00001160: 632e 6e65 742f 496d 672f 7072 6f67 7265  c.net/Img/progre
-00001170: 7373 2d64 6f74 732e 6769 6629 027a 1449  ss-dots.gif).z.I
-00001180: 6d67 2f73 6861 7265 2d73 7072 6974 652e  mg/share-sprite.
-00001190: 706e 677a 2c68 7474 7073 3a2f 2f63 646e  pngz,https://cdn
-000011a0: 2e73 7374 6174 6963 2e6e 6574 2f49 6d67  .sstatic.net/Img
-000011b0: 2f73 6861 7265 2d73 7072 6974 652e 706e  /share-sprite.pn
-000011c0: 6729 027a 1b49 6d67 2f75 6e69 6669 6564  g).z.Img/unified
-000011d0: 6d65 7461 2f73 7072 6974 6573 2e73 7667  meta/sprites.svg
-000011e0: 7a33 6874 7470 733a 2f2f 6364 6e2e 7373  z3https://cdn.ss
-000011f0: 7461 7469 632e 6e65 742f 496d 672f 756e  tatic.net/Img/un
-00001200: 6966 6965 646d 6574 612f 7370 7269 7465  ifiedmeta/sprite
-00001210: 732e 7376 6729 027a 2049 6d67 2f64 6576  s.svg).z Img/dev
-00001220: 656c 6f70 6572 2d73 746f 7279 2f74 696d  eloper-story/tim
-00001230: 656c 696e 652e 7376 677a 3868 7474 7073  eline.svgz8https
-00001240: 3a2f 2f63 646e 2e73 7374 6174 6963 2e6e  ://cdn.sstatic.n
-00001250: 6574 2f49 6d67 2f64 6576 656c 6f70 6572  et/Img/developer
-00001260: 2d73 746f 7279 2f74 696d 656c 696e 652e  -story/timeline.
-00001270: 7376 6729 027a 1b49 6d67 2f75 7365 722d  svg).z.Img/user-
-00001280: 7072 6f66 696c 652d 7370 7269 7465 2e70  profile-sprite.p
-00001290: 6e67 7a33 6874 7470 733a 2f2f 6364 6e2e  ngz3https://cdn.
-000012a0: 7373 7461 7469 632e 6e65 742f 496d 672f  sstatic.net/Img/
-000012b0: 7573 6572 2d70 726f 6669 6c65 2d73 7072  user-profile-spr
-000012c0: 6974 652e 706e 6729 027a 1b49 6d67 2f75  ite.png).z.Img/u
-000012d0: 7365 722d 7072 6f66 696c 652d 7370 7269  ser-profile-spri
-000012e0: 7465 2e73 7667 7a33 6874 7470 733a 2f2f  te.svgz3https://
-000012f0: 6364 6e2e 7373 7461 7469 632e 6e65 742f  cdn.sstatic.net/
-00001300: 496d 672f 7573 6572 2d70 726f 6669 6c65  Img/user-profile
-00001310: 2d73 7072 6974 652e 7376 6729 027a 1849  -sprite.svg).z.I
-00001320: 6d67 2f73 6861 7265 2d73 7072 6974 652d  mg/share-sprite-
-00001330: 6e65 772e 706e 677a 3068 7474 7073 3a2f  new.pngz0https:/
-00001340: 2f63 646e 2e73 7374 6174 6963 2e6e 6574  /cdn.sstatic.net
-00001350: 2f49 6d67 2f73 6861 7265 2d73 7072 6974  /Img/share-sprit
-00001360: 652d 6e65 772e 706e 6729 027a 1849 6d67  e-new.png).z.Img
-00001370: 2f73 6861 7265 2d73 7072 6974 652d 6e65  /share-sprite-ne
-00001380: 772e 7376 677a 3068 7474 7073 3a2f 2f63  w.svgz0https://c
-00001390: 646e 2e73 7374 6174 6963 2e6e 6574 2f49  dn.sstatic.net/I
-000013a0: 6d67 2f73 6861 7265 2d73 7072 6974 652d  mg/share-sprite-
-000013b0: 6e65 772e 7376 6729 027a 1949 6d67 2f66  new.svg).z.Img/f
-000013c0: 6176 6963 6f6e 732d 7370 7269 7465 3136  avicons-sprite16
-000013d0: 2e70 6e67 7a31 6874 7470 733a 2f2f 6364  .pngz1https://cd
-000013e0: 6e2e 7373 7461 7469 632e 6e65 742f 496d  n.sstatic.net/Im
-000013f0: 672f 6661 7669 636f 6e73 2d73 7072 6974  g/favicons-sprit
-00001400: 6531 362e 706e 6729 027a 1e49 6d67 2f66  e16.png).z.Img/f
-00001410: 6176 6963 6f6e 732d 7370 7269 7465 3136  avicons-sprite16
-00001420: 2d64 6172 6b2e 706e 677a 3668 7474 7073  -dark.pngz6https
-00001430: 3a2f 2f63 646e 2e73 7374 6174 6963 2e6e  ://cdn.sstatic.n
-00001440: 6574 2f49 6d67 2f66 6176 6963 6f6e 732d  et/Img/favicons-
-00001450: 7370 7269 7465 3136 2d64 6172 6b2e 706e  sprite16-dark.pn
-00001460: 6729 027a 1949 6d67 2f66 6176 6963 6f6e  g).z.Img/favicon
-00001470: 732d 7370 7269 7465 3332 2e70 6e67 7a31  s-sprite32.pngz1
-00001480: 6874 7470 733a 2f2f 6364 6e2e 7373 7461  https://cdn.ssta
-00001490: 7469 632e 6e65 742f 496d 672f 6661 7669  tic.net/Img/favi
-000014a0: 636f 6e73 2d73 7072 6974 6533 322e 706e  cons-sprite32.pn
-000014b0: 6729 027a 1e49 6d67 2f66 6176 6963 6f6e  g).z.Img/favicon
-000014c0: 732d 7370 7269 7465 3332 2d64 6172 6b2e  s-sprite32-dark.
-000014d0: 706e 677a 3668 7474 7073 3a2f 2f63 646e  pngz6https://cdn
-000014e0: 2e73 7374 6174 6963 2e6e 6574 2f49 6d67  .sstatic.net/Img
-000014f0: 2f66 6176 6963 6f6e 732d 7370 7269 7465  /favicons-sprite
-00001500: 3332 2d64 6172 6b2e 706e 6729 027a 1649  32-dark.png).z.I
-00001510: 6d67 2f66 696c 7465 722d 7370 7269 7465  mg/filter-sprite
-00001520: 732e 706e 677a 2e68 7474 7073 3a2f 2f63  s.pngz.https://c
-00001530: 646e 2e73 7374 6174 6963 2e6e 6574 2f49  dn.sstatic.net/I
-00001540: 6d67 2f66 696c 7465 722d 7370 7269 7465  mg/filter-sprite
-00001550: 732e 706e 6729 027a 1649 6d67 2f66 696c  s.png).z.Img/fil
-00001560: 7465 722d 7370 7269 7465 732e 7376 677a  ter-sprites.svgz
-00001570: 2e68 7474 7073 3a2f 2f63 646e 2e73 7374  .https://cdn.sst
-00001580: 6174 6963 2e6e 6574 2f49 6d67 2f66 696c  atic.net/Img/fil
-00001590: 7465 722d 7370 7269 7465 732e 7376 6729  ter-sprites.svg)
-000015a0: 027a 1249 6d67 2f69 6d67 2d75 706c 6f61  .z.Img/img-uploa
-000015b0: 642e 7376 677a 2a68 7474 7073 3a2f 2f63  d.svgz*https://c
-000015c0: 646e 2e73 7374 6174 6963 2e6e 6574 2f49  dn.sstatic.net/I
-000015d0: 6d67 2f69 6d67 2d75 706c 6f61 642e 7376  mg/img-upload.sv
-000015e0: 6729 027a 0c49 6d67 2f75 7365 722e 7376  g).z.Img/user.sv
-000015f0: 677a 2468 7474 7073 3a2f 2f63 646e 2e73  gz$https://cdn.s
-00001600: 7374 6174 6963 2e6e 6574 2f49 6d67 2f75  static.net/Img/u
-00001610: 7365 722e 7376 6729 027a 1149 6d67 2f66  ser.svg).z.Img/f
-00001620: 6174 6172 726f 7773 2e70 6e67 7a29 6874  atarrows.pngz)ht
-00001630: 7470 733a 2f2f 6364 6e2e 7373 7461 7469  tps://cdn.sstati
-00001640: 632e 6e65 742f 496d 672f 6661 7461 7272  c.net/Img/fatarr
-00001650: 6f77 732e 706e 6729 027a 1c49 6d67 2f6f  ows.png).z.Img/o
-00001660: 7065 6e2d 6772 6170 682f 6368 6563 6b6d  pen-graph/checkm
-00001670: 6172 6b2e 706e 677a 3468 7474 7073 3a2f  ark.pngz4https:/
-00001680: 2f63 646e 2e73 7374 6174 6963 2e6e 6574  /cdn.sstatic.net
-00001690: 2f49 6d67 2f6f 7065 6e2d 6772 6170 682f  /Img/open-graph/
-000016a0: 6368 6563 6b6d 6172 6b2e 706e 6763 0100  checkmark.pngc..
-000016b0: 0000 0000 0000 0000 0000 0400 0000 0600  ................
-000016c0: 0000 4300 0000 7360 0000 0074 0044 005d  ..C...s`...t.D.]
-000016d0: 565c 027d 017d 027c 00a0 017c 01a1 017d  V\.}.}.|...|...}
-000016e0: 037c 03a0 02a1 0072 2071 047c 036a 03a0  .|.....r q.|.j..
-000016f0: 02a1 0073 3a7c 036a 036a 0464 0164 0164  ...s:|.j.j.d.d.d
-00001700: 028d 0201 0074 0564 037c 029b 0064 047c  .....t.d.|...d.|
-00001710: 039b 009d 0483 0101 0074 067c 027c 0364  .........t.|.|.d
-00001720: 058d 0201 0071 0464 0053 0029 064e 5429  .....q.d.S.).NT)
-00001730: 02da 0865 7869 7374 5f6f 6bda 0770 6172  ...exist_ok..par
-00001740: 656e 7473 7a0c 446f 776e 6c6f 6164 696e  entsz.Downloadin
-00001750: 6720 7a06 2069 6e74 6f20 2902 da03 7572  g z. into )...ur
-00001760: 6c5a 0566 7061 7468 2907 da06 4153 5345  lZ.fpath)...ASSE
-00001770: 5453 da08 6a6f 696e 7061 7468 da06 6578  TS..joinpath..ex
-00001780: 6973 7473 da06 7061 7265 6e74 da05 6d6b  ists..parent..mk
-00001790: 6469 72da 0570 7269 6e74 7202 0000 0029  dir..printr....)
-000017a0: 04da 0563 6163 6865 da04 7061 7468 da06  ...cache..path..
-000017b0: 736f 7572 6365 da06 7461 7267 6574 a900  source..target..
-000017c0: 7210 0000 00fa 302f 5573 6572 732f 7265  r.....0/Users/re
-000017d0: 672f 7372 632f 736f 746f 6b69 2f73 7263  g/src/sotoki/src
-000017e0: 2f73 6f74 6f6b 692f 6465 7065 6e64 656e  /sotoki/dependen
-000017f0: 6369 6573 2e70 79da 0e67 6574 5f61 6c6c  cies.py..get_all
-00001800: 5f61 7373 6574 73d2 0000 0073 1000 0000  _assets....s....
-00001810: 0002 0c01 0a01 0801 0202 0a01 1001 1401  ................
-00001820: 7212 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00001830: 0000 0000 0000 0400 0000 4300 0000 731a  ..........C...s.
-00001840: 0000 0074 0074 01a0 0274 03a1 016a 04a0  ...t.t...t...j..
-00001850: 0564 01a1 0183 0101 0064 0053 0029 024e  .d.......d.S.).N
-00001860: 5a06 6173 7365 7473 2906 7212 0000 00da  Z.assets).r.....
-00001870: 0770 6174 686c 6962 da04 5061 7468 da08  .pathlib..Path..
-00001880: 5f5f 6669 6c65 5f5f 7209 0000 0072 0700  __file__r....r..
-00001890: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
-000018a0: 0072 1100 0000 da04 6d61 696e df00 0000  .r......main....
-000018b0: 7302 0000 0000 0172 1600 0000 da08 5f5f  s......r......__
-000018c0: 6d61 696e 5f5f 2907 7213 0000 005a 167a  main__).r....Z.z
-000018d0: 696d 7363 7261 7065 726c 6962 2e64 6f77  imscraperlib.dow
-000018e0: 6e6c 6f61 6472 0200 0000 7206 0000 0072  nloadr....r....r
-000018f0: 1200 0000 7216 0000 00da 085f 5f6e 616d  ....r......__nam
-00001900: 655f 5f72 1000 0000 7210 0000 0072 1000  e__r....r....r..
-00001910: 0000 7211 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00001920: 3e04 0000 0073 7c00 0000 0802 0c04 0204  >....s|.........
-00001930: 0204 0204 0201 0205 0205 0205 0204 0204  ................
-00001940: 0206 0206 0205 0205 0205 0205 0205 0205  ................
-00001950: 0205 0205 0205 0205 0205 0209 0204 0204  ................
-00001960: 0204 0204 0201 0204 0204 0201 0204 0204  ................
-00001970: 0204 0204 0204 0201 0201 0204 0204 0204  ................
-00001980: 0204 0201 0201 0201 0204 0201 0204 0201  ................
-00001990: 0201 0201 0201 0201 0280 00be 047f 004a  ...............J
-000019a0: 080d 0804 0801                           ......
+000000a0: 6432 6433 6434 6435 6436 6437 6735 5a03  d2d3d4d5d6d7g5Z.
+000000b0: 6438 6439 8400 5a04 643a 643b 8400 5a05  d8d9..Z.d:d;..Z.
+000000c0: 6506 643c 6b02 72a0 6505 8300 0100 6401  e.d<k.r.e.....d.
+000000d0: 5300 293d e900 0000 004e 2901 da0b 7374  S.)=.....N)...st
+000000e0: 7265 616d 5f66 696c 6529 027a 1573 7461  ream_file).z.sta
+000000f0: 7469 632f 6373 732f 7374 6163 6b73 2e63  tic/css/stacks.c
+00000100: 7373 7a38 6874 7470 733a 2f2f 6364 6e2e  ssz8https://cdn.
+00000110: 7373 7461 7469 632e 6e65 742f 5368 6172  sstatic.net/Shar
+00000120: 6564 2f73 7461 636b 732e 6373 733f 763d  ed/stacks.css?v=
+00000130: 6361 3533 3139 6534 3963 3633 2902 7a1a  ca5319e49c63).z.
+00000140: 7374 6174 6963 2f6a 732f 7465 782d 6d6d  static/js/tex-mm
+00000150: 6c2d 6368 746d 6c2e 6a73 7a3f 6874 7470  l-chtml.jsz?http
+00000160: 733a 2f2f 6364 6e2e 6a73 6465 6c69 7672  s://cdn.jsdelivr
+00000170: 2e6e 6574 2f6e 706d 2f6d 6174 686a 6178  .net/npm/mathjax
+00000180: 4033 2e31 2e33 2f65 7335 2f74 6578 2d6d  @3.1.3/es5/tex-m
+00000190: 6d6c 2d63 6874 6d6c 2e6a 7329 027a 1873  ml-chtml.js).z.s
+000001a0: 7461 7469 632f 6a73 2f73 7461 636b 2d69  tatic/js/stack-i
+000001b0: 636f 6e73 2e6a 737a 4368 7474 7073 3a2f  cons.jszChttps:/
+000001c0: 2f75 6e70 6b67 2e63 6f6d 2f40 7374 6163  /unpkg.com/@stac
+000001d0: 6b6f 7665 7266 6c6f 772f 7374 6163 6b73  koverflow/stacks
+000001e0: 2d69 636f 6e73 4032 2e32 302e 302f 6275  -icons@2.20.0/bu
+000001f0: 696c 642f 696e 6465 782e 6a73 2902 7a17  ild/index.js).z.
+00000200: 7374 6174 6963 2f6a 732f 6d6f 6d65 6e74  static/js/moment
+00000210: 2e6d 696e 2e6a 737a 2c68 7474 7073 3a2f  .min.jsz,https:/
+00000220: 2f6d 6f6d 656e 746a 732e 636f 6d2f 646f  /momentjs.com/do
+00000230: 776e 6c6f 6164 732f 6d6f 6d65 6e74 2e6d  wnloads/moment.m
+00000240: 696e 2e6a 7329 027a 1a73 7461 7469 632f  in.js).z.static/
+00000250: 6a73 2f6a 6465 6e74 6963 6f6e 2e6d 696e  js/jdenticon.min
+00000260: 2e6a 737a 4f68 7474 7073 3a2f 2f72 6177  .jszOhttps://raw
+00000270: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000280: 6e74 2e63 6f6d 2f64 6d65 7374 6572 2f6a  nt.com/dmester/j
+00000290: 6465 6e74 6963 6f6e 2f33 2e31 2e30 2f64  denticon/3.1.0/d
+000002a0: 6973 742f 6a64 656e 7469 636f 6e2e 6d69  ist/jdenticon.mi
+000002b0: 6e2e 6a73 2902 7a24 7374 6174 6963 2f63  n.js).z$static/c
+000002c0: 7373 2f68 6967 686c 6967 6874 2e64 6566  ss/highlight.def
+000002d0: 6175 6c74 2e6d 696e 2e63 7373 7a51 6874  ault.min.csszQht
+000002e0: 7470 733a 2f2f 6364 6e6a 732e 636c 6f75  tps://cdnjs.clou
+000002f0: 6466 6c61 7265 2e63 6f6d 2f61 6a61 782f  dflare.com/ajax/
+00000300: 6c69 6273 2f68 6967 686c 6967 6874 2e6a  libs/highlight.j
+00000310: 732f 3131 2e31 2e30 2f73 7479 6c65 732f  s/11.1.0/styles/
+00000320: 6465 6661 756c 742e 6d69 6e2e 6373 7329  default.min.css)
+00000330: 027a 1a73 7461 7469 632f 6a73 2f68 6967  .z.static/js/hig
+00000340: 686c 6967 6874 2e6d 696e 2e6a 737a 4b68  hlight.min.jszKh
+00000350: 7474 7073 3a2f 2f63 646e 6a73 2e63 6c6f  ttps://cdnjs.clo
+00000360: 7564 666c 6172 652e 636f 6d2f 616a 6178  udflare.com/ajax
+00000370: 2f6c 6962 732f 6869 6768 6c69 6768 742e  /libs/highlight.
+00000380: 6a73 2f31 312e 312e 302f 6869 6768 6c69  js/11.1.0/highli
+00000390: 6768 742e 6d69 6e2e 6a73 2902 7a1f 7374  ght.min.js).z.st
+000003a0: 6174 6963 2f6a 732f 7765 6270 2d68 6572  atic/js/webp-her
+000003b0: 6f2e 706f 6c79 6669 6c6c 2e6a 737a 3e68  o.polyfill.jsz>h
+000003c0: 7474 7073 3a2f 2f75 6e70 6b67 2e63 6f6d  ttps://unpkg.com
+000003d0: 2f77 6562 702d 6865 726f 4030 2e30 2e30  /webp-hero@0.0.0
+000003e0: 2d64 6576 2e32 372f 6469 7374 2d63 6a73  -dev.27/dist-cjs
+000003f0: 2f70 6f6c 7966 696c 6c73 2e6a 7329 027a  /polyfills.js).z
+00000400: 1d73 7461 7469 632f 6a73 2f77 6562 702d  .static/js/webp-
+00000410: 6865 726f 2e62 756e 646c 652e 6a73 7a45  hero.bundle.jszE
+00000420: 6874 7470 733a 2f2f 756e 706b 672e 636f  https://unpkg.co
+00000430: 6d2f 7765 6270 2d68 6572 6f40 302e 302e  m/webp-hero@0.0.
+00000440: 302d 6465 762e 3237 2f64 6973 742d 636a  0-dev.27/dist-cj
+00000450: 732f 7765 6270 2d68 6572 6f2e 6275 6e64  s/webp-hero.bund
+00000460: 6c65 2e6a 7329 027a 1973 7461 7469 632f  le.js).z.static/
+00000470: 6a73 2f77 6562 702d 6861 6e64 6c65 722e  js/webp-handler.
+00000480: 6a73 7a87 6874 7470 733a 2f2f 6769 7374  jsz.https://gist
+00000490: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000004a0: 6e74 2e63 6f6d 2f72 6761 7564 696e 2f36  nt.com/rgaudin/6
+000004b0: 3062 6239 6363 3666 3138 3761 6464 3530  0bb9cc6f187add50
+000004c0: 3635 3834 3235 3830 3238 6238 6565 312f  6584258028b8ee1/
+000004d0: 7261 772f 3964 3537 3562 3865 3235 6436  raw/9d575b8e25d6
+000004e0: 3765 6564 3261 3963 3961 3931 6433 6530  7eed2a9c9a91d3e0
+000004f0: 3533 6130 3036 3264 3266 6337 2f77 6562  53a0062d2fc7/web
+00000500: 2d68 616e 646c 6572 2e6a 7329 027a 1473  -handler.js).z.s
+00000510: 7461 7469 632f 6a73 2f4d 6174 684a 6178  tatic/js/MathJax
+00000520: 2e6a 737a 5868 7474 7073 3a2f 2f63 646e  .jszXhttps://cdn
+00000530: 6a73 2e63 6c6f 7564 666c 6172 652e 636f  js.cloudflare.co
+00000540: 6d2f 616a 6178 2f6c 6962 732f 6d61 7468  m/ajax/libs/math
+00000550: 6a61 782f 322e 372e 352f 4d61 7468 4a61  jax/2.7.5/MathJa
+00000560: 782e 6a73 3f63 6f6e 6669 673d 5465 582d  x.js?config=TeX-
+00000570: 414d 535f 4854 4d4c 2d66 756c 6c29 027a  AMS_HTML-full).z
+00000580: 2573 7461 7469 632f 6a73 2f63 6f6e 6669  %static/js/confi
+00000590: 672f 5465 582d 414d 535f 4854 4d4c 2d66  g/TeX-AMS_HTML-f
+000005a0: 756c 6c2e 6a73 7a58 6874 7470 733a 2f2f  ull.jszXhttps://
+000005b0: 6364 6e6a 732e 636c 6f75 6466 6c61 7265  cdnjs.cloudflare
+000005c0: 2e63 6f6d 2f61 6a61 782f 6c69 6273 2f6d  .com/ajax/libs/m
+000005d0: 6174 686a 6178 2f32 2e37 2e35 2f63 6f6e  athjax/2.7.5/con
+000005e0: 6669 672f 5465 582d 414d 535f 4854 4d4c  fig/TeX-AMS_HTML
+000005f0: 2d66 756c 6c2e 6a73 3f56 3d32 2e37 2e35  -full.js?V=2.7.5
+00000600: 2902 7a20 7374 6174 6963 2f6a 732f 6578  ).z static/js/ex
+00000610: 7465 6e73 696f 6e73 2f4d 6174 684d 656e  tensions/MathMen
+00000620: 752e 6a73 7a53 6874 7470 733a 2f2f 6364  u.jszShttps://cd
+00000630: 6e6a 732e 636c 6f75 6466 6c61 7265 2e63  njs.cloudflare.c
+00000640: 6f6d 2f61 6a61 782f 6c69 6273 2f6d 6174  om/ajax/libs/mat
+00000650: 686a 6178 2f32 2e37 2e35 2f65 7874 656e  hjax/2.7.5/exten
+00000660: 7369 6f6e 732f 4d61 7468 4d65 6e75 2e6a  sions/MathMenu.j
+00000670: 733f 563d 322e 372e 3529 027a 2073 7461  s?V=2.7.5).z sta
+00000680: 7469 632f 6a73 2f65 7874 656e 7369 6f6e  tic/js/extension
+00000690: 732f 4d61 7468 5a6f 6f6d 2e6a 737a 5368  s/MathZoom.jszSh
+000006a0: 7474 7073 3a2f 2f63 646e 6a73 2e63 6c6f  ttps://cdnjs.clo
+000006b0: 7564 666c 6172 652e 636f 6d2f 616a 6178  udflare.com/ajax
+000006c0: 2f6c 6962 732f 6d61 7468 6a61 782f 322e  /libs/mathjax/2.
+000006d0: 372e 352f 6578 7465 6e73 696f 6e73 2f4d  7.5/extensions/M
+000006e0: 6174 685a 6f6f 6d2e 6a73 3f56 3d32 2e37  athZoom.js?V=2.7
+000006f0: 2e35 2902 7a26 7374 6174 6963 2f6a 732f  .5).z&static/js/
+00000700: 6578 7465 6e73 696f 6e73 2f54 6558 2f62  extensions/TeX/b
+00000710: 6567 696e 6772 6f75 702e 6a73 7a59 6874  egingroup.jszYht
+00000720: 7470 733a 2f2f 6364 6e6a 732e 636c 6f75  tps://cdnjs.clou
+00000730: 6466 6c61 7265 2e63 6f6d 2f61 6a61 782f  dflare.com/ajax/
+00000740: 6c69 6273 2f6d 6174 686a 6178 2f32 2e37  libs/mathjax/2.7
+00000750: 2e35 2f65 7874 656e 7369 6f6e 732f 5465  .5/extensions/Te
+00000760: 582f 6265 6769 6e67 726f 7570 2e6a 733f  X/begingroup.js?
+00000770: 563d 322e 372e 3529 027a 3473 7461 7469  V=2.7.5).z4stati
+00000780: 632f 6a73 2f6a 6178 2f6f 7574 7075 742f  c/js/jax/output/
+00000790: 4854 4d4c 2d43 5353 2f66 6f6e 7473 2f53  HTML-CSS/fonts/S
+000007a0: 5449 582f 666f 6e74 6461 7461 2e6a 737a  TIX/fontdata.jsz
+000007b0: 6768 7474 7073 3a2f 2f63 646e 6a73 2e63  ghttps://cdnjs.c
+000007c0: 6c6f 7564 666c 6172 652e 636f 6d2f 616a  loudflare.com/aj
+000007d0: 6178 2f6c 6962 732f 6d61 7468 6a61 782f  ax/libs/mathjax/
+000007e0: 322e 372e 352f 6a61 782f 6f75 7470 7574  2.7.5/jax/output
+000007f0: 2f48 544d 4c2d 4353 532f 666f 6e74 732f  /HTML-CSS/fonts/
+00000800: 5354 4958 2f66 6f6e 7464 6174 612e 6a73  STIX/fontdata.js
+00000810: 3f56 3d32 2e37 2e35 2902 7a2f 7374 6174  ?V=2.7.5).z/stat
+00000820: 6963 2f6a 732f 6a61 782f 656c 656d 656e  ic/js/jax/elemen
+00000830: 742f 6d6d 6c2f 6f70 7461 626c 652f 4261  t/mml/optable/Ba
+00000840: 7369 634c 6174 696e 2e6a 737a 6268 7474  sicLatin.jszbhtt
+00000850: 7073 3a2f 2f63 646e 6a73 2e63 6c6f 7564  ps://cdnjs.cloud
+00000860: 666c 6172 652e 636f 6d2f 616a 6178 2f6c  flare.com/ajax/l
+00000870: 6962 732f 6d61 7468 6a61 782f 322e 372e  ibs/mathjax/2.7.
+00000880: 352f 6a61 782f 656c 656d 656e 742f 6d6d  5/jax/element/mm
+00000890: 6c2f 6f70 7461 626c 652f 4261 7369 634c  l/optable/BasicL
+000008a0: 6174 696e 2e6a 733f 563d 322e 372e 3529  atin.js?V=2.7.5)
+000008b0: 027a 4573 7461 7469 632f 6a73 2f6a 6178  .zEstatic/js/jax
+000008c0: 2f6f 7574 7075 742f 4854 4d4c 2d43 5353  /output/HTML-CSS
+000008d0: 2f66 6f6e 7473 2f53 5449 582f 4765 6e65  /fonts/STIX/Gene
+000008e0: 7261 6c2f 4974 616c 6963 2f4d 6174 6849  ral/Italic/MathI
+000008f0: 7461 6c69 632e 6a73 7a78 6874 7470 733a  talic.jszxhttps:
+00000900: 2f2f 6364 6e6a 732e 636c 6f75 6466 6c61  //cdnjs.cloudfla
+00000910: 7265 2e63 6f6d 2f61 6a61 782f 6c69 6273  re.com/ajax/libs
+00000920: 2f6d 6174 686a 6178 2f32 2e37 2e35 2f6a  /mathjax/2.7.5/j
+00000930: 6178 2f6f 7574 7075 742f 4854 4d4c 2d43  ax/output/HTML-C
+00000940: 5353 2f66 6f6e 7473 2f53 5449 582f 4765  SS/fonts/STIX/Ge
+00000950: 6e65 7261 6c2f 4974 616c 6963 2f4d 6174  neral/Italic/Mat
+00000960: 6849 7461 6c69 632e 6a73 3f56 3d32 2e37  hItalic.js?V=2.7
+00000970: 2e35 2902 7a46 7374 6174 6963 2f6a 732f  .5).zFstatic/js/
+00000980: 6a61 782f 6f75 7470 7574 2f48 544d 4c2d  jax/output/HTML-
+00000990: 4353 532f 666f 6e74 732f 5354 4958 2f47  CSS/fonts/STIX/G
+000009a0: 656e 6572 616c 2f52 6567 756c 6172 2f4d  eneral/Regular/M
+000009b0: 6174 6849 7461 6c69 632e 6a73 7a79 6874  athItalic.jszyht
+000009c0: 7470 733a 2f2f 6364 6e6a 732e 636c 6f75  tps://cdnjs.clou
+000009d0: 6466 6c61 7265 2e63 6f6d 2f61 6a61 782f  dflare.com/ajax/
+000009e0: 6c69 6273 2f6d 6174 686a 6178 2f32 2e37  libs/mathjax/2.7
+000009f0: 2e35 2f6a 6178 2f6f 7574 7075 742f 4854  .5/jax/output/HT
+00000a00: 4d4c 2d43 5353 2f66 6f6e 7473 2f53 5449  ML-CSS/fonts/STI
+00000a10: 582f 4765 6e65 7261 6c2f 5265 6775 6c61  X/General/Regula
+00000a20: 722f 4d61 7468 4974 616c 6963 2e6a 733f  r/MathItalic.js?
+00000a30: 563d 322e 372e 3529 027a 4673 7461 7469  V=2.7.5).zFstati
+00000a40: 632f 6a73 2f6a 6178 2f6f 7574 7075 742f  c/js/jax/output/
+00000a50: 4854 4d4c 2d43 5353 2f66 6f6e 7473 2f53  HTML-CSS/fonts/S
+00000a60: 5449 582f 4765 6e65 7261 6c2f 4974 616c  TIX/General/Ital
+00000a70: 6963 2f47 7265 656b 4974 616c 6963 2e6a  ic/GreekItalic.j
+00000a80: 737a 7968 7474 7073 3a2f 2f63 646e 6a73  szyhttps://cdnjs
+00000a90: 2e63 6c6f 7564 666c 6172 652e 636f 6d2f  .cloudflare.com/
+00000aa0: 616a 6178 2f6c 6962 732f 6d61 7468 6a61  ajax/libs/mathja
+00000ab0: 782f 322e 372e 352f 6a61 782f 6f75 7470  x/2.7.5/jax/outp
+00000ac0: 7574 2f48 544d 4c2d 4353 532f 666f 6e74  ut/HTML-CSS/font
+00000ad0: 732f 5354 4958 2f47 656e 6572 616c 2f49  s/STIX/General/I
+00000ae0: 7461 6c69 632f 4772 6565 6b49 7461 6c69  talic/GreekItali
+00000af0: 632e 6a73 3f56 3d32 2e37 2e35 2902 7a47  c.js?V=2.7.5).zG
+00000b00: 7374 6174 6963 2f6a 732f 6a61 782f 6f75  static/js/jax/ou
+00000b10: 7470 7574 2f48 544d 4c2d 4353 532f 666f  tput/HTML-CSS/fo
+00000b20: 6e74 732f 5354 4958 2f47 656e 6572 616c  nts/STIX/General
+00000b30: 2f52 6567 756c 6172 2f47 7265 656b 4974  /Regular/GreekIt
+00000b40: 616c 6963 2e6a 737a 7a68 7474 7073 3a2f  alic.jszzhttps:/
+00000b50: 2f63 646e 6a73 2e63 6c6f 7564 666c 6172  /cdnjs.cloudflar
+00000b60: 652e 636f 6d2f 616a 6178 2f6c 6962 732f  e.com/ajax/libs/
+00000b70: 6d61 7468 6a61 782f 322e 372e 352f 6a61  mathjax/2.7.5/ja
+00000b80: 782f 6f75 7470 7574 2f48 544d 4c2d 4353  x/output/HTML-CS
+00000b90: 532f 666f 6e74 732f 5354 4958 2f47 656e  S/fonts/STIX/Gen
+00000ba0: 6572 616c 2f52 6567 756c 6172 2f47 7265  eral/Regular/Gre
+00000bb0: 656b 4974 616c 6963 2e6a 733f 563d 322e  ekItalic.js?V=2.
+00000bc0: 372e 3529 027a 3373 7461 7469 632f 6a73  7.5).z3static/js
+00000bd0: 2f6a 6178 2f6f 7574 7075 742f 4854 4d4c  /jax/output/HTML
+00000be0: 2d43 5353 2f66 6f6e 7473 2f54 6558 2f66  -CSS/fonts/TeX/f
+00000bf0: 6f6e 7464 6174 612e 6a73 7a66 6874 7470  ontdata.jszfhttp
+00000c00: 733a 2f2f 6364 6e6a 732e 636c 6f75 6466  s://cdnjs.cloudf
+00000c10: 6c61 7265 2e63 6f6d 2f61 6a61 782f 6c69  lare.com/ajax/li
+00000c20: 6273 2f6d 6174 686a 6178 2f32 2e37 2e35  bs/mathjax/2.7.5
+00000c30: 2f6a 6178 2f6f 7574 7075 742f 4854 4d4c  /jax/output/HTML
+00000c40: 2d43 5353 2f66 6f6e 7473 2f54 6558 2f66  -CSS/fonts/TeX/f
+00000c50: 6f6e 7464 6174 612e 6a73 3f56 3d32 2e37  ontdata.js?V=2.7
+00000c60: 2e35 2902 7a1f 496d 672f 6963 6f6e 2d65  .5).z.Img/icon-e
+00000c70: 6e76 656c 6f70 652d 6669 6c6c 2d67 7261  nvelope-fill-gra
+00000c80: 792e 706e 677a 3768 7474 7073 3a2f 2f63  y.pngz7https://c
+00000c90: 646e 2e73 7374 6174 6963 2e6e 6574 2f49  dn.sstatic.net/I
+00000ca0: 6d67 2f69 636f 6e2d 656e 7665 6c6f 7065  mg/icon-envelope
+00000cb0: 2d66 696c 6c2d 6772 6179 2e70 6e67 2902  -fill-gray.png).
+00000cc0: 7a1f 496d 672f 6963 6f6e 2d65 6e76 656c  z.Img/icon-envel
+00000cd0: 6f70 652d 6669 6c6c 2d67 7261 792e 7376  ope-fill-gray.sv
+00000ce0: 677a 3768 7474 7073 3a2f 2f63 646e 2e73  gz7https://cdn.s
+00000cf0: 7374 6174 6963 2e6e 6574 2f49 6d67 2f69  static.net/Img/i
+00000d00: 636f 6e2d 656e 7665 6c6f 7065 2d66 696c  con-envelope-fil
+00000d10: 6c2d 6772 6179 2e73 7667 2902 7a1b 496d  l-gray.svg).z.Im
+00000d20: 672f 666f 726d 732f 6963 6f6e 2d64 6973  g/forms/icon-dis
+00000d30: 6162 6c65 642e 7376 677a 3368 7474 7073  abled.svgz3https
+00000d40: 3a2f 2f63 646e 2e73 7374 6174 6963 2e6e  ://cdn.sstatic.n
+00000d50: 6574 2f49 6d67 2f66 6f72 6d73 2f69 636f  et/Img/forms/ico
+00000d60: 6e2d 6469 7361 626c 6564 2e73 7667 2902  n-disabled.svg).
+00000d70: 7a1a 496d 672f 666f 726d 732f 6963 6f6e  z.Img/forms/icon
+00000d80: 2d77 6172 6e69 6e67 2e73 7667 7a32 6874  -warning.svgz2ht
+00000d90: 7470 733a 2f2f 6364 6e2e 7373 7461 7469  tps://cdn.sstati
+00000da0: 632e 6e65 742f 496d 672f 666f 726d 732f  c.net/Img/forms/
+00000db0: 6963 6f6e 2d77 6172 6e69 6e67 2e73 7667  icon-warning.svg
+00000dc0: 2902 7a18 496d 672f 666f 726d 732f 6963  ).z.Img/forms/ic
+00000dd0: 6f6e 2d65 7272 6f72 2e73 7667 7a30 6874  on-error.svgz0ht
+00000de0: 7470 733a 2f2f 6364 6e2e 7373 7461 7469  tps://cdn.sstati
+00000df0: 632e 6e65 742f 496d 672f 666f 726d 732f  c.net/Img/forms/
+00000e00: 6963 6f6e 2d65 7272 6f72 2e73 7667 2902  icon-error.svg).
+00000e10: 7a1a 496d 672f 666f 726d 732f 6963 6f6e  z.Img/forms/icon
+00000e20: 2d73 7563 6365 7373 2e73 7667 7a32 6874  -success.svgz2ht
+00000e30: 7470 733a 2f2f 6364 6e2e 7373 7461 7469  tps://cdn.sstati
+00000e40: 632e 6e65 742f 496d 672f 666f 726d 732f  c.net/Img/forms/
+00000e50: 6963 6f6e 2d73 7563 6365 7373 2e73 7667  icon-success.svg
+00000e60: 2902 7a24 496d 672f 6865 726f 2f61 6e6f  ).z$Img/hero/ano
+00000e70: 6e79 6d6f 7573 4865 726f 4261 636b 6772  nymousHeroBackgr
+00000e80: 6f75 6e64 2e73 7667 7a3c 6874 7470 733a  ound.svgz<https:
+00000e90: 2f2f 6364 6e2e 7373 7461 7469 632e 6e65  //cdn.sstatic.ne
+00000ea0: 742f 496d 672f 6865 726f 2f61 6e6f 6e79  t/Img/hero/anony
+00000eb0: 6d6f 7573 4865 726f 4261 636b 6772 6f75  mousHeroBackgrou
+00000ec0: 6e64 2e73 7667 2902 7a12 496d 672f 696d  nd.svg).z.Img/im
+00000ed0: 672d 7570 6c6f 6164 2e70 6e67 7a2a 6874  g-upload.pngz*ht
+00000ee0: 7470 733a 2f2f 6364 6e2e 7373 7461 7469  tps://cdn.sstati
+00000ef0: 632e 6e65 742f 496d 672f 696d 672d 7570  c.net/Img/img-up
+00000f00: 6c6f 6164 2e70 6e67 2902 7a17 496d 672f  load.png).z.Img/
+00000f10: 756e 6966 6965 642f 7370 7269 7465 732e  unified/sprites.
+00000f20: 706e 677a 2f68 7474 7073 3a2f 2f63 646e  pngz/https://cdn
+00000f30: 2e73 7374 6174 6963 2e6e 6574 2f49 6d67  .sstatic.net/Img
+00000f40: 2f75 6e69 6669 6564 2f73 7072 6974 6573  /unified/sprites
+00000f50: 2e70 6e67 2902 7a17 496d 672f 756e 6966  .png).z.Img/unif
+00000f60: 6965 642f 7370 7269 7465 732e 7376 677a  ied/sprites.svgz
+00000f70: 2f68 7474 7073 3a2f 2f63 646e 2e73 7374  /https://cdn.sst
+00000f80: 6174 6963 2e6e 6574 2f49 6d67 2f75 6e69  atic.net/Img/uni
+00000f90: 6669 6564 2f73 7072 6974 6573 2e73 7667  fied/sprites.svg
+00000fa0: 2902 7a1b 496d 672f 756e 6966 6965 646d  ).z.Img/unifiedm
+00000fb0: 6574 612f 7370 7269 7465 732e 706e 677a  eta/sprites.pngz
+00000fc0: 3368 7474 7073 3a2f 2f63 646e 2e73 7374  3https://cdn.sst
+00000fd0: 6174 6963 2e6e 6574 2f49 6d67 2f75 6e69  atic.net/Img/uni
+00000fe0: 6669 6564 6d65 7461 2f73 7072 6974 6573  fiedmeta/sprites
+00000ff0: 2e70 6e67 2902 7a1b 496d 672f 756e 6966  .png).z.Img/unif
+00001000: 6965 642f 776d 642d 6275 7474 6f6e 732e  ied/wmd-buttons.
+00001010: 7376 677a 3368 7474 7073 3a2f 2f63 646e  svgz3https://cdn
+00001020: 2e73 7374 6174 6963 2e6e 6574 2f49 6d67  .sstatic.net/Img
+00001030: 2f75 6e69 6669 6564 2f77 6d64 2d62 7574  /unified/wmd-but
+00001040: 746f 6e73 2e73 7667 2902 7a20 496d 672f  tons.svg).z Img/
+00001050: 756e 6966 6965 642f 776d 642d 6275 7474  unified/wmd-butt
+00001060: 6f6e 732d 6461 726b 2e73 7667 7a38 6874  ons-dark.svgz8ht
+00001070: 7470 733a 2f2f 6364 6e2e 7373 7461 7469  tps://cdn.sstati
+00001080: 632e 6e65 742f 496d 672f 756e 6966 6965  c.net/Img/unifie
+00001090: 642f 776d 642d 6275 7474 6f6e 732d 6461  d/wmd-buttons-da
+000010a0: 726b 2e73 7667 2902 7a15 496d 672f 7072  rk.svg).z.Img/pr
+000010b0: 6f67 7265 7373 2d64 6f74 732e 6769 667a  ogress-dots.gifz
+000010c0: 2d68 7474 7073 3a2f 2f63 646e 2e73 7374  -https://cdn.sst
+000010d0: 6174 6963 2e6e 6574 2f49 6d67 2f70 726f  atic.net/Img/pro
+000010e0: 6772 6573 732d 646f 7473 2e67 6966 2902  gress-dots.gif).
+000010f0: 7a14 496d 672f 7368 6172 652d 7370 7269  z.Img/share-spri
+00001100: 7465 2e70 6e67 7a2c 6874 7470 733a 2f2f  te.pngz,https://
+00001110: 6364 6e2e 7373 7461 7469 632e 6e65 742f  cdn.sstatic.net/
+00001120: 496d 672f 7368 6172 652d 7370 7269 7465  Img/share-sprite
+00001130: 2e70 6e67 2902 7a1b 496d 672f 756e 6966  .png).z.Img/unif
+00001140: 6965 646d 6574 612f 7370 7269 7465 732e  iedmeta/sprites.
+00001150: 7376 677a 3368 7474 7073 3a2f 2f63 646e  svgz3https://cdn
+00001160: 2e73 7374 6174 6963 2e6e 6574 2f49 6d67  .sstatic.net/Img
+00001170: 2f75 6e69 6669 6564 6d65 7461 2f73 7072  /unifiedmeta/spr
+00001180: 6974 6573 2e73 7667 2902 7a20 496d 672f  ites.svg).z Img/
+00001190: 6465 7665 6c6f 7065 722d 7374 6f72 792f  developer-story/
+000011a0: 7469 6d65 6c69 6e65 2e73 7667 7a38 6874  timeline.svgz8ht
+000011b0: 7470 733a 2f2f 6364 6e2e 7373 7461 7469  tps://cdn.sstati
+000011c0: 632e 6e65 742f 496d 672f 6465 7665 6c6f  c.net/Img/develo
+000011d0: 7065 722d 7374 6f72 792f 7469 6d65 6c69  per-story/timeli
+000011e0: 6e65 2e73 7667 2902 7a1b 496d 672f 7573  ne.svg).z.Img/us
+000011f0: 6572 2d70 726f 6669 6c65 2d73 7072 6974  er-profile-sprit
+00001200: 652e 706e 677a 3368 7474 7073 3a2f 2f63  e.pngz3https://c
+00001210: 646e 2e73 7374 6174 6963 2e6e 6574 2f49  dn.sstatic.net/I
+00001220: 6d67 2f75 7365 722d 7072 6f66 696c 652d  mg/user-profile-
+00001230: 7370 7269 7465 2e70 6e67 2902 7a1b 496d  sprite.png).z.Im
+00001240: 672f 7573 6572 2d70 726f 6669 6c65 2d73  g/user-profile-s
+00001250: 7072 6974 652e 7376 677a 3368 7474 7073  prite.svgz3https
+00001260: 3a2f 2f63 646e 2e73 7374 6174 6963 2e6e  ://cdn.sstatic.n
+00001270: 6574 2f49 6d67 2f75 7365 722d 7072 6f66  et/Img/user-prof
+00001280: 696c 652d 7370 7269 7465 2e73 7667 2902  ile-sprite.svg).
+00001290: 7a18 496d 672f 7368 6172 652d 7370 7269  z.Img/share-spri
+000012a0: 7465 2d6e 6577 2e70 6e67 7a30 6874 7470  te-new.pngz0http
+000012b0: 733a 2f2f 6364 6e2e 7373 7461 7469 632e  s://cdn.sstatic.
+000012c0: 6e65 742f 496d 672f 7368 6172 652d 7370  net/Img/share-sp
+000012d0: 7269 7465 2d6e 6577 2e70 6e67 2902 7a18  rite-new.png).z.
+000012e0: 496d 672f 7368 6172 652d 7370 7269 7465  Img/share-sprite
+000012f0: 2d6e 6577 2e73 7667 7a30 6874 7470 733a  -new.svgz0https:
+00001300: 2f2f 6364 6e2e 7373 7461 7469 632e 6e65  //cdn.sstatic.ne
+00001310: 742f 496d 672f 7368 6172 652d 7370 7269  t/Img/share-spri
+00001320: 7465 2d6e 6577 2e73 7667 2902 7a19 496d  te-new.svg).z.Im
+00001330: 672f 6661 7669 636f 6e73 2d73 7072 6974  g/favicons-sprit
+00001340: 6531 362e 706e 677a 3168 7474 7073 3a2f  e16.pngz1https:/
+00001350: 2f63 646e 2e73 7374 6174 6963 2e6e 6574  /cdn.sstatic.net
+00001360: 2f49 6d67 2f66 6176 6963 6f6e 732d 7370  /Img/favicons-sp
+00001370: 7269 7465 3136 2e70 6e67 2902 7a1e 496d  rite16.png).z.Im
+00001380: 672f 6661 7669 636f 6e73 2d73 7072 6974  g/favicons-sprit
+00001390: 6531 362d 6461 726b 2e70 6e67 7a36 6874  e16-dark.pngz6ht
+000013a0: 7470 733a 2f2f 6364 6e2e 7373 7461 7469  tps://cdn.sstati
+000013b0: 632e 6e65 742f 496d 672f 6661 7669 636f  c.net/Img/favico
+000013c0: 6e73 2d73 7072 6974 6531 362d 6461 726b  ns-sprite16-dark
+000013d0: 2e70 6e67 2902 7a19 496d 672f 6661 7669  .png).z.Img/favi
+000013e0: 636f 6e73 2d73 7072 6974 6533 322e 706e  cons-sprite32.pn
+000013f0: 677a 3168 7474 7073 3a2f 2f63 646e 2e73  gz1https://cdn.s
+00001400: 7374 6174 6963 2e6e 6574 2f49 6d67 2f66  static.net/Img/f
+00001410: 6176 6963 6f6e 732d 7370 7269 7465 3332  avicons-sprite32
+00001420: 2e70 6e67 2902 7a1e 496d 672f 6661 7669  .png).z.Img/favi
+00001430: 636f 6e73 2d73 7072 6974 6533 322d 6461  cons-sprite32-da
+00001440: 726b 2e70 6e67 7a36 6874 7470 733a 2f2f  rk.pngz6https://
+00001450: 6364 6e2e 7373 7461 7469 632e 6e65 742f  cdn.sstatic.net/
+00001460: 496d 672f 6661 7669 636f 6e73 2d73 7072  Img/favicons-spr
+00001470: 6974 6533 322d 6461 726b 2e70 6e67 2902  ite32-dark.png).
+00001480: 7a16 496d 672f 6669 6c74 6572 2d73 7072  z.Img/filter-spr
+00001490: 6974 6573 2e70 6e67 7a2e 6874 7470 733a  ites.pngz.https:
+000014a0: 2f2f 6364 6e2e 7373 7461 7469 632e 6e65  //cdn.sstatic.ne
+000014b0: 742f 496d 672f 6669 6c74 6572 2d73 7072  t/Img/filter-spr
+000014c0: 6974 6573 2e70 6e67 2902 7a16 496d 672f  ites.png).z.Img/
+000014d0: 6669 6c74 6572 2d73 7072 6974 6573 2e73  filter-sprites.s
+000014e0: 7667 7a2e 6874 7470 733a 2f2f 6364 6e2e  vgz.https://cdn.
+000014f0: 7373 7461 7469 632e 6e65 742f 496d 672f  sstatic.net/Img/
+00001500: 6669 6c74 6572 2d73 7072 6974 6573 2e73  filter-sprites.s
+00001510: 7667 2902 7a12 496d 672f 696d 672d 7570  vg).z.Img/img-up
+00001520: 6c6f 6164 2e73 7667 7a2a 6874 7470 733a  load.svgz*https:
+00001530: 2f2f 6364 6e2e 7373 7461 7469 632e 6e65  //cdn.sstatic.ne
+00001540: 742f 496d 672f 696d 672d 7570 6c6f 6164  t/Img/img-upload
+00001550: 2e73 7667 2902 7a0c 496d 672f 7573 6572  .svg).z.Img/user
+00001560: 2e73 7667 7a24 6874 7470 733a 2f2f 6364  .svgz$https://cd
+00001570: 6e2e 7373 7461 7469 632e 6e65 742f 496d  n.sstatic.net/Im
+00001580: 672f 7573 6572 2e73 7667 2902 7a11 496d  g/user.svg).z.Im
+00001590: 672f 6661 7461 7272 6f77 732e 706e 677a  g/fatarrows.pngz
+000015a0: 2968 7474 7073 3a2f 2f63 646e 2e73 7374  )https://cdn.sst
+000015b0: 6174 6963 2e6e 6574 2f49 6d67 2f66 6174  atic.net/Img/fat
+000015c0: 6172 726f 7773 2e70 6e67 2902 7a1c 496d  arrows.png).z.Im
+000015d0: 672f 6f70 656e 2d67 7261 7068 2f63 6865  g/open-graph/che
+000015e0: 636b 6d61 726b 2e70 6e67 7a34 6874 7470  ckmark.pngz4http
+000015f0: 733a 2f2f 6364 6e2e 7373 7461 7469 632e  s://cdn.sstatic.
+00001600: 6e65 742f 496d 672f 6f70 656e 2d67 7261  net/Img/open-gra
+00001610: 7068 2f63 6865 636b 6d61 726b 2e70 6e67  ph/checkmark.png
+00001620: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00001630: 0006 0000 0043 0000 0073 6000 0000 7400  .....C...s`...t.
+00001640: 4400 5d56 5c02 7d01 7d02 7c00 a001 7c01  D.]V\.}.}.|...|.
+00001650: a101 7d03 7c03 a002 a100 7220 7104 7c03  ..}.|.....r q.|.
+00001660: 6a03 a002 a100 733a 7c03 6a03 6a04 6401  j.....s:|.j.j.d.
+00001670: 6401 6402 8d02 0100 7405 6403 7c02 9b00  d.d.....t.d.|...
+00001680: 6404 7c03 9b00 9d04 8301 0100 7406 7c02  d.|.........t.|.
+00001690: 7c03 6405 8d02 0100 7104 6400 5300 2906  |.d.....q.d.S.).
+000016a0: 4e54 2902 da08 6578 6973 745f 6f6b da07  NT)...exist_ok..
+000016b0: 7061 7265 6e74 737a 0c44 6f77 6e6c 6f61  parentsz.Downloa
+000016c0: 6469 6e67 207a 0620 696e 746f 2029 02da  ding z. into )..
+000016d0: 0375 726c 5a05 6670 6174 6829 07da 0641  .urlZ.fpath)...A
+000016e0: 5353 4554 53da 086a 6f69 6e70 6174 68da  SSETS..joinpath.
+000016f0: 0665 7869 7374 73da 0670 6172 656e 74da  .exists..parent.
+00001700: 056d 6b64 6972 da05 7072 696e 7472 0200  .mkdir..printr..
+00001710: 0000 2904 da05 6361 6368 65da 0470 6174  ..)...cache..pat
+00001720: 68da 0673 6f75 7263 65da 0674 6172 6765  h..source..targe
+00001730: 74a9 0072 1000 0000 fa3a 2f68 6f6d 652f  t..r.....:/home/
+00001740: 7275 6e6e 6572 2f77 6f72 6b2f 736f 746f  runner/work/soto
+00001750: 6b69 2f73 6f74 6f6b 692f 7372 632f 736f  ki/sotoki/src/so
+00001760: 746f 6b69 2f64 6570 656e 6465 6e63 6965  toki/dependencie
+00001770: 732e 7079 da0e 6765 745f 616c 6c5f 6173  s.py..get_all_as
+00001780: 7365 7473 cc00 0000 7310 0000 0000 020c  sets....s.......
+00001790: 010a 0108 0102 020a 0110 0114 0172 1200  .............r..
+000017a0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000017b0: 0000 0004 0000 0043 0000 0073 1a00 0000  .......C...s....
+000017c0: 7400 7401 a002 7403 a101 6a04 a005 6401  t.t...t...j...d.
+000017d0: a101 8301 0100 6400 5300 2902 4e5a 0661  ......d.S.).NZ.a
+000017e0: 7373 6574 7329 0672 1200 0000 da07 7061  ssets).r......pa
+000017f0: 7468 6c69 62da 0450 6174 68da 085f 5f66  thlib..Path..__f
+00001800: 696c 655f 5f72 0900 0000 7207 0000 0072  ile__r....r....r
+00001810: 1000 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
+00001820: 0000 00da 046d 6169 6ed9 0000 0073 0200  .....main....s..
+00001830: 0000 0001 7216 0000 00da 085f 5f6d 6169  ....r......__mai
+00001840: 6e5f 5f29 0772 1300 0000 5a16 7a69 6d73  n__).r....Z.zims
+00001850: 6372 6170 6572 6c69 622e 646f 776e 6c6f  craperlib.downlo
+00001860: 6164 7202 0000 0072 0600 0000 7212 0000  adr....r....r...
+00001870: 0072 1600 0000 da08 5f5f 6e61 6d65 5f5f  .r......__name__
+00001880: 7210 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
+00001890: 1100 0000 da08 3c6d 6f64 756c 653e 0400  ......<module>..
+000018a0: 0000 737a 0000 0008 020c 0402 0402 0402  ..sz............
+000018b0: 0402 0102 0502 0502 0502 0402 0402 0602  ................
+000018c0: 0502 0502 0502 0502 0502 0502 0502 0502  ................
+000018d0: 0502 0502 0502 0902 0402 0402 0402 0402  ................
+000018e0: 0102 0402 0402 0102 0402 0402 0402 0402  ................
+000018f0: 0402 0102 0102 0402 0402 0402 0402 0102  ................
+00001900: 0102 0102 0402 0102 0402 0102 0102 0102  ................
+00001910: 0102 0102 8000 c404 7f00 4408 0d08 0408  ..........D.....
+00001920: 01                                       .
```

### Comparing `sotoki-2.0.2/src/sotoki/archives.py` & `sotoki-2.1.1/src/sotoki/archives.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from .utils.shared import Global, logger
 from .utils.misc import has_binary
 from .utils.sevenzip import extract_7z
 from .utils.preparation import (
     merge_users_with_badges,
     merge_posts_with_answers_comments,
+    reencode_file,
 )
 
 
 class ArchiveManager:
     """Handle retrieval and processing of StackExchange dump files
 
     Each website is available as a single 7z archive
@@ -85,17 +86,21 @@
 
             logger.info(f"Extracting {fpath.name}")
             extract_7z(fpath, self.build_dir, delete_src=self.delete_src)
             Global.progresser.update(incr=1)
 
             # remove other files from ark that we won't need
             for fp in self.build_dir.iterdir():
-                if fp.suffix == ".xml" and fp.stem not in self.dump_parts:
+                if fp.suffix != ".xml" or fp.stem not in self.dump_parts:
                     fp.unlink()
 
+            # reencode xml files
+            for fp in self.build_dir.iterdir():
+                reencode_file(fp)
+
         futures = {}
         executor = cf.ThreadPoolExecutor(max_workers=len(self.archives))
 
         for ark in self.archives:
             url = f"{self.mirror}/{ark.name}"
             kwargs = {"url": url, "fpath": ark}
             future = executor.submit(_run, **kwargs)
```

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/developer-story/timeline.svg` & `sotoki-2.1.1/src/sotoki/assets/Img/developer-story/timeline.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/fatarrows.png` & `sotoki-2.1.1/src/sotoki/assets/Img/fatarrows.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/filter-sprites.png` & `sotoki-2.1.1/src/sotoki/assets/Img/filter-sprites.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/filter-sprites.svg` & `sotoki-2.1.1/src/sotoki/assets/Img/filter-sprites.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/hero/anonymousHeroBackground.svg` & `sotoki-2.1.1/src/sotoki/assets/Img/hero/anonymousHeroBackground.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/icon-envelope-fill-gray.svg` & `sotoki-2.1.1/src/sotoki/assets/Img/icon-envelope-fill-gray.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/img-upload.png` & `sotoki-2.1.1/src/sotoki/assets/Img/img-upload.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/img-upload.svg` & `sotoki-2.1.1/src/sotoki/assets/Img/img-upload.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/open-graph/checkmark.png` & `sotoki-2.1.1/src/sotoki/assets/Img/open-graph/checkmark.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/share-sprite-new.png` & `sotoki-2.1.1/src/sotoki/assets/Img/share-sprite-new.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/share-sprite-new.svg` & `sotoki-2.1.1/src/sotoki/assets/Img/share-sprite-new.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/share-sprite.png` & `sotoki-2.1.1/src/sotoki/assets/Img/share-sprite.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/unified/sprites.png` & `sotoki-2.1.1/src/sotoki/assets/Img/unified/sprites.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/unified/sprites.svg` & `sotoki-2.1.1/src/sotoki/assets/Img/unified/sprites.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/unified/wmd-buttons-dark.svg` & `sotoki-2.1.1/src/sotoki/assets/Img/unified/wmd-buttons-dark.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/unified/wmd-buttons.svg` & `sotoki-2.1.1/src/sotoki/assets/Img/unified/wmd-buttons.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/unifiedmeta/sprites.png` & `sotoki-2.1.1/src/sotoki/assets/Img/unifiedmeta/sprites.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/unifiedmeta/sprites.svg` & `sotoki-2.1.1/src/sotoki/assets/Img/unifiedmeta/sprites.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/user-profile-sprite.png` & `sotoki-2.1.1/src/sotoki/assets/Img/user-profile-sprite.png`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/Img/user-profile-sprite.svg` & `sotoki-2.1.1/src/sotoki/assets/Img/user-profile-sprite.svg`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/css/highlight.default.min.css` & `sotoki-2.1.1/src/sotoki/assets/static/css/highlight.default.min.css`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/css/sotoki.css` & `sotoki-2.1.1/src/sotoki/assets/static/css/sotoki.css`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/MathJax.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/MathJax.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/config/TeX-AMS_HTML-full.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/config/TeX-AMS_HTML-full.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/extensions/MathMenu.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/extensions/MathMenu.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/extensions/MathZoom.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/extensions/MathZoom.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/extensions/TeX/begingroup.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/extensions/TeX/begingroup.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/highlight.min.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/identicons.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/identicons.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/jax/element/mml/optable/BasicLatin.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/jax/element/mml/optable/BasicLatin.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/GreekItalic.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/GreekItalic.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/MathItalic.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Italic/MathItalic.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/GreekItalic.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/GreekItalic.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/MathItalic.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/General/Regular/MathItalic.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/fontdata.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/STIX/fontdata.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/TeX/fontdata.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/jax/output/HTML-CSS/fonts/TeX/fontdata.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/jdenticon.min.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/jdenticon.min.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/mathjax-config.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/mathjax-config.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/moment.min.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/moment.min.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,63 +1,63 @@
 ! function(e, t) {
     "object" == typeof exports && "undefined" != typeof module ? module.exports = t() : "function" == typeof define && define.amd ? define(t) : e.moment = t()
 }(this, function() {
     "use strict";
-    var e, i;
+    var H;
 
-    function f() {
-        return e.apply(null, arguments)
+    function _() {
+        return H.apply(null, arguments)
     }
 
-    function o(e) {
+    function y(e) {
         return e instanceof Array || "[object Array]" === Object.prototype.toString.call(e)
     }
 
-    function u(e) {
+    function F(e) {
         return null != e && "[object Object]" === Object.prototype.toString.call(e)
     }
 
-    function m(e, t) {
+    function c(e, t) {
         return Object.prototype.hasOwnProperty.call(e, t)
     }
 
-    function l(e) {
+    function L(e) {
         if (Object.getOwnPropertyNames) return 0 === Object.getOwnPropertyNames(e).length;
         for (var t in e)
-            if (m(e, t)) return;
+            if (c(e, t)) return;
         return 1
     }
 
-    function r(e) {
+    function g(e) {
         return void 0 === e
     }
 
-    function h(e) {
+    function w(e) {
         return "number" == typeof e || "[object Number]" === Object.prototype.toString.call(e)
     }
 
-    function a(e) {
+    function V(e) {
         return e instanceof Date || "[object Date]" === Object.prototype.toString.call(e)
     }
 
-    function d(e, t) {
-        for (var n = [], s = 0; s < e.length; ++s) n.push(t(e[s], s));
+    function G(e, t) {
+        for (var n = [], s = e.length, i = 0; i < s; ++i) n.push(t(e[i], i));
         return n
     }
 
-    function c(e, t) {
-        for (var n in t) m(t, n) && (e[n] = t[n]);
-        return m(t, "toString") && (e.toString = t.toString), m(t, "valueOf") && (e.valueOf = t.valueOf), e
+    function E(e, t) {
+        for (var n in t) c(t, n) && (e[n] = t[n]);
+        return c(t, "toString") && (e.toString = t.toString), c(t, "valueOf") && (e.valueOf = t.valueOf), e
     }
 
-    function _(e, t, n, s) {
-        return xt(e, t, n, s, !0).utc()
+    function l(e, t, n, s) {
+        return Wt(e, t, n, s, !0).utc()
     }
 
-    function y(e) {
+    function p(e) {
         return null == e._pf && (e._pf = {
             empty: !1,
             unusedTokens: [],
             unusedInput: [],
             overflow: -2,
             charsLeftOver: 0,
             nullInput: !1,
@@ -70,439 +70,536 @@
             era: null,
             meridiem: null,
             rfc2822: !1,
             weekdayMismatch: !1
         }), e._pf
     }
 
-    function g(e) {
-        if (null == e._isValid) {
-            var t = y(e),
-                n = i.call(t.parsedDateParts, function(e) {
-                    return null != e
-                }),
-                s = !isNaN(e._d.getTime()) && t.overflow < 0 && !t.empty && !t.invalidEra && !t.invalidMonth && !t.invalidWeekday && !t.weekdayMismatch && !t.nullInput && !t.invalidFormat && !t.userInvalidated && (!t.meridiem || t.meridiem && n);
-            if (e._strict && (s = s && 0 === t.charsLeftOver && 0 === t.unusedTokens.length && void 0 === t.bigHour), null != Object.isFrozen && Object.isFrozen(e)) return s;
-            e._isValid = s
-        }
-        return e._isValid
+    function A(e) {
+        var t, n, s = e._d && !isNaN(e._d.getTime());
+        return s && (t = p(e), n = j.call(t.parsedDateParts, function(e) {
+            return null != e
+        }), s = t.overflow < 0 && !t.empty && !t.invalidEra && !t.invalidMonth && !t.invalidWeekday && !t.weekdayMismatch && !t.nullInput && !t.invalidFormat && !t.userInvalidated && (!t.meridiem || t.meridiem && n), e._strict) && (s = s && 0 === t.charsLeftOver && 0 === t.unusedTokens.length && void 0 === t.bigHour), null != Object.isFrozen && Object.isFrozen(e) ? s : (e._isValid = s, e._isValid)
     }
 
-    function w(e) {
-        var t = _(NaN);
-        return null != e ? c(y(t), e) : y(t).userInvalidated = !0, t
+    function I(e) {
+        var t = l(NaN);
+        return null != e ? E(p(t), e) : p(t).userInvalidated = !0, t
     }
-    i = Array.prototype.some ? Array.prototype.some : function(e) {
-        for (var t = Object(this), n = t.length >>> 0, s = 0; s < n; s++)
-            if (s in t && e.call(this, t[s], s, t)) return !0;
-        return !1
-    };
-    var p = f.momentProperties = [],
-        t = !1;
+    var j = Array.prototype.some || function(e) {
+            for (var t = Object(this), n = t.length >>> 0, s = 0; s < n; s++)
+                if (s in t && e.call(this, t[s], s, t)) return !0;
+            return !1
+        },
+        Z = _.momentProperties = [],
+        z = !1;
 
-    function v(e, t) {
-        var n, s, i;
-        if (r(t._isAMomentObject) || (e._isAMomentObject = t._isAMomentObject), r(t._i) || (e._i = t._i), r(t._f) || (e._f = t._f), r(t._l) || (e._l = t._l), r(t._strict) || (e._strict = t._strict), r(t._tzm) || (e._tzm = t._tzm), r(t._isUTC) || (e._isUTC = t._isUTC), r(t._offset) || (e._offset = t._offset), r(t._pf) || (e._pf = y(t)), r(t._locale) || (e._locale = t._locale), 0 < p.length)
-            for (n = 0; n < p.length; n++) r(i = t[s = p[n]]) || (e[s] = i);
+    function q(e, t) {
+        var n, s, i, r = Z.length;
+        if (g(t._isAMomentObject) || (e._isAMomentObject = t._isAMomentObject), g(t._i) || (e._i = t._i), g(t._f) || (e._f = t._f), g(t._l) || (e._l = t._l), g(t._strict) || (e._strict = t._strict), g(t._tzm) || (e._tzm = t._tzm), g(t._isUTC) || (e._isUTC = t._isUTC), g(t._offset) || (e._offset = t._offset), g(t._pf) || (e._pf = p(t)), g(t._locale) || (e._locale = t._locale), 0 < r)
+            for (n = 0; n < r; n++) g(i = t[s = Z[n]]) || (e[s] = i);
         return e
     }
 
-    function k(e) {
-        v(this, e), this._d = new Date(null != e._d ? e._d.getTime() : NaN), this.isValid() || (this._d = new Date(NaN)), !1 === t && (t = !0, f.updateOffset(this), t = !1)
+    function $(e) {
+        q(this, e), this._d = new Date(null != e._d ? e._d.getTime() : NaN), this.isValid() || (this._d = new Date(NaN)), !1 === z && (z = !0, _.updateOffset(this), z = !1)
     }
 
-    function M(e) {
-        return e instanceof k || null != e && null != e._isAMomentObject
+    function k(e) {
+        return e instanceof $ || null != e && null != e._isAMomentObject
     }
 
-    function D(e) {
-        !1 === f.suppressDeprecationWarnings && "undefined" != typeof console && console.warn && console.warn("Deprecation warning: " + e)
+    function B(e) {
+        !1 === _.suppressDeprecationWarnings && "undefined" != typeof console && console.warn && console.warn("Deprecation warning: " + e)
     }
 
-    function n(i, r) {
-        var a = !0;
-        return c(function() {
-            if (null != f.deprecationHandler && f.deprecationHandler(null, i), a) {
-                for (var e, t, n = [], s = 0; s < arguments.length; s++) {
-                    if (e = "", "object" == typeof arguments[s]) {
-                        for (t in e += "\n[" + s + "] ", arguments[0]) m(arguments[0], t) && (e += t + ": " + arguments[0][t] + ", ");
+    function e(r, a) {
+        var o = !0;
+        return E(function() {
+            if (null != _.deprecationHandler && _.deprecationHandler(null, r), o) {
+                for (var e, t, n = [], s = arguments.length, i = 0; i < s; i++) {
+                    if (e = "", "object" == typeof arguments[i]) {
+                        for (t in e += "\n[" + i + "] ", arguments[0]) c(arguments[0], t) && (e += t + ": " + arguments[0][t] + ", ");
                         e = e.slice(0, -2)
-                    } else e = arguments[s];
+                    } else e = arguments[i];
                     n.push(e)
                 }
-                D(i + "\nArguments: " + Array.prototype.slice.call(n).join("") + "\n" + (new Error).stack), a = !1
+                B(r + "\nArguments: " + Array.prototype.slice.call(n).join("") + "\n" + (new Error).stack), o = !1
             }
-            return r.apply(this, arguments)
-        }, r)
+            return a.apply(this, arguments)
+        }, a)
     }
-    var s, S = {};
+    var J = {};
 
-    function Y(e, t) {
-        null != f.deprecationHandler && f.deprecationHandler(e, t), S[e] || (D(t), S[e] = !0)
+    function Q(e, t) {
+        null != _.deprecationHandler && _.deprecationHandler(e, t), J[e] || (B(t), J[e] = !0)
     }
 
-    function O(e) {
+    function a(e) {
         return "undefined" != typeof Function && e instanceof Function || "[object Function]" === Object.prototype.toString.call(e)
     }
 
-    function b(e, t) {
-        var n, s = c({}, e);
-        for (n in t) m(t, n) && (u(e[n]) && u(t[n]) ? (s[n] = {}, c(s[n], e[n]), c(s[n], t[n])) : null != t[n] ? s[n] = t[n] : delete s[n]);
-        for (n in e) m(e, n) && !m(t, n) && u(e[n]) && (s[n] = c({}, s[n]));
+    function X(e, t) {
+        var n, s = E({}, e);
+        for (n in t) c(t, n) && (F(e[n]) && F(t[n]) ? (s[n] = {}, E(s[n], e[n]), E(s[n], t[n])) : null != t[n] ? s[n] = t[n] : delete s[n]);
+        for (n in e) c(e, n) && !c(t, n) && F(e[n]) && (s[n] = E({}, s[n]));
         return s
     }
 
-    function x(e) {
+    function K(e) {
         null != e && this.set(e)
     }
-    f.suppressDeprecationWarnings = !1, f.deprecationHandler = null, s = Object.keys ? Object.keys : function(e) {
+    _.suppressDeprecationWarnings = !1, _.deprecationHandler = null;
+    var ee = Object.keys || function(e) {
         var t, n = [];
-        for (t in e) m(e, t) && n.push(t);
+        for (t in e) c(e, t) && n.push(t);
         return n
     };
 
-    function T(e, t, n) {
-        var s = "" + Math.abs(e),
-            i = t - s.length;
-        return (0 <= e ? n ? "+" : "" : "-") + Math.pow(10, Math.max(0, i)).toString().substr(1) + s
-    }
-    var N = /(\[[^\[]*\])|(\\)?([Hh]mm(ss)?|Mo|MM?M?M?|Do|DDDo|DD?D?D?|ddd?d?|do?|w[o|w]?|W[o|W]?|Qo?|N{1,5}|YYYYYY|YYYYY|YYYY|YY|y{2,4}|yo?|gg(ggg?)?|GG(GGG?)?|e|E|a|A|hh?|HH?|kk?|mm?|ss?|S{1,9}|x|X|zz?|ZZ?|.)/g,
-        P = /(\[[^\[]*\])|(\\)?(LTS|LT|LL?L?L?|l{1,4})/g,
-        R = {},
-        W = {};
+    function r(e, t, n) {
+        var s = "" + Math.abs(e);
+        return (0 <= e ? n ? "+" : "" : "-") + Math.pow(10, Math.max(0, t - s.length)).toString().substr(1) + s
+    }
+    var te = /(\[[^\[]*\])|(\\)?([Hh]mm(ss)?|Mo|MM?M?M?|Do|DDDo|DD?D?D?|ddd?d?|do?|w[o|w]?|W[o|W]?|Qo?|N{1,5}|YYYYYY|YYYYY|YYYY|YY|y{2,4}|yo?|gg(ggg?)?|GG(GGG?)?|e|E|a|A|hh?|HH?|kk?|mm?|ss?|S{1,9}|x|X|zz?|ZZ?|.)/g,
+        ne = /(\[[^\[]*\])|(\\)?(LTS|LT|LL?L?L?|l{1,4})/g,
+        se = {},
+        ie = {};
 
-    function C(e, t, n, s) {
+    function s(e, t, n, s) {
         var i = "string" == typeof s ? function() {
             return this[s]()
         } : s;
-        e && (W[e] = i), t && (W[t[0]] = function() {
-            return T(i.apply(this, arguments), t[1], t[2])
-        }), n && (W[n] = function() {
+        e && (ie[e] = i), t && (ie[t[0]] = function() {
+            return r(i.apply(this, arguments), t[1], t[2])
+        }), n && (ie[n] = function() {
             return this.localeData().ordinal(i.apply(this, arguments), e)
         })
     }
 
-    function U(e, t) {
-        return e.isValid() ? (t = H(t, e.localeData()), R[t] = R[t] || function(s) {
-            for (var e, i = s.match(N), t = 0, r = i.length; t < r; t++) W[i[t]] ? i[t] = W[i[t]] : i[t] = (e = i[t]).match(/\[[\s\S]/) ? e.replace(/^\[|\]$/g, "") : e.replace(/\\/g, "");
+    function re(e, t) {
+        return e.isValid() ? (t = ae(t, e.localeData()), se[t] = se[t] || function(s) {
+            for (var e, i = s.match(te), t = 0, r = i.length; t < r; t++) ie[i[t]] ? i[t] = ie[i[t]] : i[t] = (e = i[t]).match(/\[[\s\S]/) ? e.replace(/^\[|\]$/g, "") : e.replace(/\\/g, "");
             return function(e) {
-                for (var t = "", n = 0; n < r; n++) t += O(i[n]) ? i[n].call(e, s) : i[n];
+                for (var t = "", n = 0; n < r; n++) t += a(i[n]) ? i[n].call(e, s) : i[n];
                 return t
             }
-        }(t), R[t](e)) : e.localeData().invalidDate()
+        }(t), se[t](e)) : e.localeData().invalidDate()
     }
 
-    function H(e, t) {
+    function ae(e, t) {
         var n = 5;
 
         function s(e) {
             return t.longDateFormat(e) || e
         }
-        for (P.lastIndex = 0; 0 <= n && P.test(e);) e = e.replace(P, s), P.lastIndex = 0, --n;
+        for (ne.lastIndex = 0; 0 <= n && ne.test(e);) e = e.replace(ne, s), ne.lastIndex = 0, --n;
         return e
     }
-    var F = {};
-
-    function L(e, t) {
-        var n = e.toLowerCase();
-        F[n] = F[n + "s"] = F[t] = e
-    }
+    var oe = {
+        D: "date",
+        dates: "date",
+        date: "date",
+        d: "day",
+        days: "day",
+        day: "day",
+        e: "weekday",
+        weekdays: "weekday",
+        weekday: "weekday",
+        E: "isoWeekday",
+        isoweekdays: "isoWeekday",
+        isoweekday: "isoWeekday",
+        DDD: "dayOfYear",
+        dayofyears: "dayOfYear",
+        dayofyear: "dayOfYear",
+        h: "hour",
+        hours: "hour",
+        hour: "hour",
+        ms: "millisecond",
+        milliseconds: "millisecond",
+        millisecond: "millisecond",
+        m: "minute",
+        minutes: "minute",
+        minute: "minute",
+        M: "month",
+        months: "month",
+        month: "month",
+        Q: "quarter",
+        quarters: "quarter",
+        quarter: "quarter",
+        s: "second",
+        seconds: "second",
+        second: "second",
+        gg: "weekYear",
+        weekyears: "weekYear",
+        weekyear: "weekYear",
+        GG: "isoWeekYear",
+        isoweekyears: "isoWeekYear",
+        isoweekyear: "isoWeekYear",
+        w: "week",
+        weeks: "week",
+        week: "week",
+        W: "isoWeek",
+        isoweeks: "isoWeek",
+        isoweek: "isoWeek",
+        y: "year",
+        years: "year",
+        year: "year"
+    };
 
-    function V(e) {
-        return "string" == typeof e ? F[e] || F[e.toLowerCase()] : void 0
+    function o(e) {
+        return "string" == typeof e ? oe[e] || oe[e.toLowerCase()] : void 0
     }
 
-    function G(e) {
+    function ue(e) {
         var t, n, s = {};
-        for (n in e) m(e, n) && (t = V(n)) && (s[t] = e[n]);
+        for (n in e) c(e, n) && (t = o(n)) && (s[t] = e[n]);
         return s
     }
-    var E = {};
+    var le = {
+        date: 9,
+        day: 11,
+        weekday: 11,
+        isoWeekday: 11,
+        dayOfYear: 4,
+        hour: 13,
+        millisecond: 16,
+        minute: 14,
+        month: 8,
+        quarter: 7,
+        second: 15,
+        weekYear: 1,
+        isoWeekYear: 1,
+        week: 5,
+        isoWeek: 5,
+        year: 1
+    };
+    var de = /\d/,
+        t = /\d\d/,
+        he = /\d{3}/,
+        ce = /\d{4}/,
+        fe = /[+-]?\d{6}/,
+        n = /\d\d?/,
+        me = /\d\d\d\d?/,
+        _e = /\d\d\d\d\d\d?/,
+        ye = /\d{1,3}/,
+        ge = /\d{1,4}/,
+        we = /[+-]?\d{1,6}/,
+        pe = /\d+/,
+        ke = /[+-]?\d+/,
+        Me = /Z|[+-]\d\d:?\d\d/gi,
+        ve = /Z|[+-]\d\d(?::?\d\d)?/gi,
+        i = /[0-9]{0,256}['a-z\u00A0-\u05FF\u0700-\uD7FF\uF900-\uFDCF\uFDF0-\uFF07\uFF10-\uFFEF]{1,256}|[\u0600-\u06FF\/]{1,256}(\s*?[\u0600-\u06FF]{1,256}){1,2}/i,
+        u = /^[1-9]\d?/,
+        d = /^([1-9]\d|\d)/;
 
-    function A(e, t) {
-        E[e] = t
+    function h(e, n, s) {
+        Ye[e] = a(n) ? n : function(e, t) {
+            return e && s ? s : n
+        }
     }
 
-    function j(e) {
-        return e % 4 == 0 && e % 100 != 0 || e % 400 == 0
+    function De(e, t) {
+        return c(Ye, e) ? Ye[e](t._strict, t._locale) : new RegExp(f(e.replace("\\", "").replace(/\\(\[)|\\(\])|\[([^\]\[]*)\]|\\(.)/g, function(e, t, n, s, i) {
+            return t || n || s || i
+        })))
     }
 
-    function I(e) {
-        return e < 0 ? Math.ceil(e) || 0 : Math.floor(e)
+    function f(e) {
+        return e.replace(/[-\/\\^$*+?.()|[\]{}]/g, "\\$&")
     }
 
-    function Z(e) {
-        var t = +e,
-            n = 0;
-        return 0 != t && isFinite(t) && (n = I(t)), n
+    function m(e) {
+        return e < 0 ? Math.ceil(e) || 0 : Math.floor(e)
     }
 
-    function z(t, n) {
-        return function(e) {
-            return null != e ? (q(this, t, e), f.updateOffset(this, n), this) : $(this, t)
-        }
+    function M(e) {
+        var e = +e,
+            t = 0;
+        return t = 0 != e && isFinite(e) ? m(e) : t
+    }
+    var Ye = {},
+        Se = {};
+
+    function v(e, n) {
+        var t, s, i = n;
+        for ("string" == typeof e && (e = [e]), w(n) && (i = function(e, t) {
+                t[n] = M(e)
+            }), s = e.length, t = 0; t < s; t++) Se[e[t]] = i
     }
 
-    function $(e, t) {
-        return e.isValid() ? e._d["get" + (e._isUTC ? "UTC" : "") + t]() : NaN
+    function Oe(e, i) {
+        v(e, function(e, t, n, s) {
+            n._w = n._w || {}, i(e, n._w, n, s)
+        })
     }
 
-    function q(e, t, n) {
-        e.isValid() && !isNaN(n) && ("FullYear" === t && j(e.year()) && 1 === e.month() && 29 === e.date() ? (n = Z(n), e._d["set" + (e._isUTC ? "UTC" : "") + t](n, e.month(), xe(n, e.month()))) : e._d["set" + (e._isUTC ? "UTC" : "") + t](n))
-    }
-    var B, J = /\d/,
-        Q = /\d\d/,
-        X = /\d{3}/,
-        K = /\d{4}/,
-        ee = /[+-]?\d{6}/,
-        te = /\d\d?/,
-        ne = /\d\d\d\d?/,
-        se = /\d\d\d\d\d\d?/,
-        ie = /\d{1,3}/,
-        re = /\d{1,4}/,
-        ae = /[+-]?\d{1,6}/,
-        oe = /\d+/,
-        ue = /[+-]?\d+/,
-        le = /Z|[+-]\d\d:?\d\d/gi,
-        he = /Z|[+-]\d\d(?::?\d\d)?/gi,
-        de = /[0-9]{0,256}['a-z\u00A0-\u05FF\u0700-\uD7FF\uF900-\uFDCF\uFDF0-\uFF07\uFF10-\uFFEF]{1,256}|[\u0600-\u06FF\/]{1,256}(\s*?[\u0600-\u06FF]{1,256}){1,2}/i;
-
-    function ce(e, n, s) {
-        B[e] = O(n) ? n : function(e, t) {
-            return e && s ? s : n
-        }
+    function be(e) {
+        return e % 4 == 0 && e % 100 != 0 || e % 400 == 0
     }
+    var D = 0,
+        Y = 1,
+        S = 2,
+        O = 3,
+        b = 4,
+        T = 5,
+        Te = 6,
+        xe = 7,
+        Ne = 8;
 
-    function fe(e, t) {
-        return m(B, e) ? B[e](t._strict, t._locale) : new RegExp(me(e.replace("\\", "").replace(/\\(\[)|\\(\])|\[([^\]\[]*)\]|\\(.)/g, function(e, t, n, s, i) {
-            return t || n || s || i
-        })))
+    function We(e) {
+        return be(e) ? 366 : 365
     }
+    s("Y", 0, 0, function() {
+        var e = this.year();
+        return e <= 9999 ? r(e, 4) : "+" + e
+    }), s(0, ["YY", 2], 0, function() {
+        return this.year() % 100
+    }), s(0, ["YYYY", 4], 0, "year"), s(0, ["YYYYY", 5], 0, "year"), s(0, ["YYYYYY", 6, !0], 0, "year"), h("Y", ke), h("YY", n, t), h("YYYY", ge, ce), h("YYYYY", we, fe), h("YYYYYY", we, fe), v(["YYYYY", "YYYYYY"], D), v("YYYY", function(e, t) {
+        t[D] = 2 === e.length ? _.parseTwoDigitYear(e) : M(e)
+    }), v("YY", function(e, t) {
+        t[D] = _.parseTwoDigitYear(e)
+    }), v("Y", function(e, t) {
+        t[D] = parseInt(e, 10)
+    }), _.parseTwoDigitYear = function(e) {
+        return M(e) + (68 < M(e) ? 1900 : 2e3)
+    };
+    var x, Pe = Re("FullYear", !0);
 
-    function me(e) {
-        return e.replace(/[-\/\\^$*+?.()|[\]{}]/g, "\\$&")
+    function Re(t, n) {
+        return function(e) {
+            return null != e ? (Ue(this, t, e), _.updateOffset(this, n), this) : Ce(this, t)
+        }
     }
-    B = {};
-    var _e = {};
 
-    function ye(e, n) {
-        var t, s = n;
-        for ("string" == typeof e && (e = [e]), h(n) && (s = function(e, t) {
-                t[n] = Z(e)
-            }), t = 0; t < e.length; t++) _e[e[t]] = s
+    function Ce(e, t) {
+        if (!e.isValid()) return NaN;
+        var n = e._d,
+            s = e._isUTC;
+        switch (t) {
+            case "Milliseconds":
+                return s ? n.getUTCMilliseconds() : n.getMilliseconds();
+            case "Seconds":
+                return s ? n.getUTCSeconds() : n.getSeconds();
+            case "Minutes":
+                return s ? n.getUTCMinutes() : n.getMinutes();
+            case "Hours":
+                return s ? n.getUTCHours() : n.getHours();
+            case "Date":
+                return s ? n.getUTCDate() : n.getDate();
+            case "Day":
+                return s ? n.getUTCDay() : n.getDay();
+            case "Month":
+                return s ? n.getUTCMonth() : n.getMonth();
+            case "FullYear":
+                return s ? n.getUTCFullYear() : n.getFullYear();
+            default:
+                return NaN
+        }
     }
 
-    function ge(e, i) {
-        ye(e, function(e, t, n, s) {
-            n._w = n._w || {}, i(e, n._w, n, s)
-        })
+    function Ue(e, t, n) {
+        var s, i, r;
+        if (e.isValid() && !isNaN(n)) {
+            switch (s = e._d, i = e._isUTC, t) {
+                case "Milliseconds":
+                    return i ? s.setUTCMilliseconds(n) : s.setMilliseconds(n);
+                case "Seconds":
+                    return i ? s.setUTCSeconds(n) : s.setSeconds(n);
+                case "Minutes":
+                    return i ? s.setUTCMinutes(n) : s.setMinutes(n);
+                case "Hours":
+                    return i ? s.setUTCHours(n) : s.setHours(n);
+                case "Date":
+                    return i ? s.setUTCDate(n) : s.setDate(n);
+                case "FullYear":
+                    break;
+                default:
+                    return
+            }
+            t = n, r = e.month(), e = 29 !== (e = e.date()) || 1 !== r || be(t) ? e : 28, i ? s.setUTCFullYear(t, r, e) : s.setFullYear(t, r, e)
+        }
     }
-    var we, pe = 0,
-        ve = 1,
-        ke = 2,
-        Me = 3,
-        De = 4,
-        Se = 5,
-        Ye = 6,
-        Oe = 7,
-        be = 8;
-
-    function xe(e, t) {
-        if (isNaN(e) || isNaN(t)) return NaN;
-        var n, s = (t % (n = 12) + n) % n;
-        return e += (t - s) / 12, 1 == s ? j(e) ? 29 : 28 : 31 - s % 7 % 2
+
+    function He(e, t) {
+        var n;
+        return isNaN(e) || isNaN(t) ? NaN : (n = (t % (n = 12) + n) % n, e += (t - n) / 12, 1 == n ? be(e) ? 29 : 28 : 31 - n % 7 % 2)
     }
-    we = Array.prototype.indexOf ? Array.prototype.indexOf : function(e) {
+    x = Array.prototype.indexOf || function(e) {
         for (var t = 0; t < this.length; ++t)
             if (this[t] === e) return t;
         return -1
-    }, C("M", ["MM", 2], "Mo", function() {
+    }, s("M", ["MM", 2], "Mo", function() {
         return this.month() + 1
-    }), C("MMM", 0, 0, function(e) {
+    }), s("MMM", 0, 0, function(e) {
         return this.localeData().monthsShort(this, e)
-    }), C("MMMM", 0, 0, function(e) {
+    }), s("MMMM", 0, 0, function(e) {
         return this.localeData().months(this, e)
-    }), L("month", "M"), A("month", 8), ce("M", te), ce("MM", te, Q), ce("MMM", function(e, t) {
+    }), h("M", n, u), h("MM", n, t), h("MMM", function(e, t) {
         return t.monthsShortRegex(e)
-    }), ce("MMMM", function(e, t) {
+    }), h("MMMM", function(e, t) {
         return t.monthsRegex(e)
-    }), ye(["M", "MM"], function(e, t) {
-        t[ve] = Z(e) - 1
-    }), ye(["MMM", "MMMM"], function(e, t, n, s) {
-        var i = n._locale.monthsParse(e, s, n._strict);
-        null != i ? t[ve] = i : y(n).invalidMonth = e
+    }), v(["M", "MM"], function(e, t) {
+        t[Y] = M(e) - 1
+    }), v(["MMM", "MMMM"], function(e, t, n, s) {
+        s = n._locale.monthsParse(e, s, n._strict);
+        null != s ? t[Y] = s : p(n).invalidMonth = e
     });
-    var Te = "January_February_March_April_May_June_July_August_September_October_November_December".split("_"),
-        Ne = "Jan_Feb_Mar_Apr_May_Jun_Jul_Aug_Sep_Oct_Nov_Dec".split("_"),
-        Pe = /D[oD]?(\[[^\[\]]*\]|\s)+MMMM?/,
-        Re = de,
-        We = de;
+    var Fe = "January_February_March_April_May_June_July_August_September_October_November_December".split("_"),
+        Le = "Jan_Feb_Mar_Apr_May_Jun_Jul_Aug_Sep_Oct_Nov_Dec".split("_"),
+        Ve = /D[oD]?(\[[^\[\]]*\]|\s)+MMMM?/,
+        Ge = i,
+        Ee = i;
 
-    function Ce(e, t) {
-        var n;
-        if (!e.isValid()) return e;
-        if ("string" == typeof t)
-            if (/^\d+$/.test(t)) t = Z(t);
-            else if (!h(t = e.localeData().monthsParse(t))) return e;
-        return n = Math.min(e.date(), xe(e.year(), t)), e._d["set" + (e._isUTC ? "UTC" : "") + "Month"](t, n), e
+    function Ae(e, t) {
+        if (e.isValid()) {
+            if ("string" == typeof t)
+                if (/^\d+$/.test(t)) t = M(t);
+                else if (!w(t = e.localeData().monthsParse(t))) return;
+            var n = (n = e.date()) < 29 ? n : Math.min(n, He(e.year(), t));
+            e._isUTC ? e._d.setUTCMonth(t, n) : e._d.setMonth(t, n)
+        }
     }
 
-    function Ue(e) {
-        return null != e ? (Ce(this, e), f.updateOffset(this, !0), this) : $(this, "Month")
+    function Ie(e) {
+        return null != e ? (Ae(this, e), _.updateOffset(this, !0), this) : Ce(this, "Month")
     }
 
-    function He() {
+    function je() {
         function e(e, t) {
             return t.length - e.length
         }
-        for (var t, n = [], s = [], i = [], r = 0; r < 12; r++) t = _([2e3, r]), n.push(this.monthsShort(t, "")), s.push(this.months(t, "")), i.push(this.months(t, "")), i.push(this.monthsShort(t, ""));
-        for (n.sort(e), s.sort(e), i.sort(e), r = 0; r < 12; r++) n[r] = me(n[r]), s[r] = me(s[r]);
-        for (r = 0; r < 24; r++) i[r] = me(i[r]);
-        this._monthsRegex = new RegExp("^(" + i.join("|") + ")", "i"), this._monthsShortRegex = this._monthsRegex, this._monthsStrictRegex = new RegExp("^(" + s.join("|") + ")", "i"), this._monthsShortStrictRegex = new RegExp("^(" + n.join("|") + ")", "i")
+        for (var t, n, s = [], i = [], r = [], a = 0; a < 12; a++) n = l([2e3, a]), t = f(this.monthsShort(n, "")), n = f(this.months(n, "")), s.push(t), i.push(n), r.push(n), r.push(t);
+        s.sort(e), i.sort(e), r.sort(e), this._monthsRegex = new RegExp("^(" + r.join("|") + ")", "i"), this._monthsShortRegex = this._monthsRegex, this._monthsStrictRegex = new RegExp("^(" + i.join("|") + ")", "i"), this._monthsShortStrictRegex = new RegExp("^(" + s.join("|") + ")", "i")
     }
 
-    function Fe(e) {
-        return j(e) ? 366 : 365
+    function Ze(e, t, n, s, i, r, a) {
+        var o;
+        return e < 100 && 0 <= e ? (o = new Date(e + 400, t, n, s, i, r, a), isFinite(o.getFullYear()) && o.setFullYear(e)) : o = new Date(e, t, n, s, i, r, a), o
     }
-    C("Y", 0, 0, function() {
-        var e = this.year();
-        return e <= 9999 ? T(e, 4) : "+" + e
-    }), C(0, ["YY", 2], 0, function() {
-        return this.year() % 100
-    }), C(0, ["YYYY", 4], 0, "year"), C(0, ["YYYYY", 5], 0, "year"), C(0, ["YYYYYY", 6, !0], 0, "year"), L("year", "y"), A("year", 1), ce("Y", ue), ce("YY", te, Q), ce("YYYY", re, K), ce("YYYYY", ae, ee), ce("YYYYYY", ae, ee), ye(["YYYYY", "YYYYYY"], pe), ye("YYYY", function(e, t) {
-        t[pe] = 2 === e.length ? f.parseTwoDigitYear(e) : Z(e)
-    }), ye("YY", function(e, t) {
-        t[pe] = f.parseTwoDigitYear(e)
-    }), ye("Y", function(e, t) {
-        t[pe] = parseInt(e, 10)
-    }), f.parseTwoDigitYear = function(e) {
-        return Z(e) + (68 < Z(e) ? 1900 : 2e3)
-    };
-    var Le = z("FullYear", !0);
 
-    function Ve(e) {
-        var t, n;
-        return e < 100 && 0 <= e ? ((n = Array.prototype.slice.call(arguments))[0] = e + 400, t = new Date(Date.UTC.apply(null, n)), isFinite(t.getUTCFullYear()) && t.setUTCFullYear(e)) : t = new Date(Date.UTC.apply(null, arguments)), t
+    function ze(e) {
+        var t;
+        return e < 100 && 0 <= e ? ((t = Array.prototype.slice.call(arguments))[0] = e + 400, t = new Date(Date.UTC.apply(null, t)), isFinite(t.getUTCFullYear()) && t.setUTCFullYear(e)) : t = new Date(Date.UTC.apply(null, arguments)), t
     }
 
-    function Ge(e, t, n) {
-        var s = 7 + t - n;
-        return s - (7 + Ve(e, 0, s).getUTCDay() - t) % 7 - 1
+    function qe(e, t, n) {
+        n = 7 + t - n;
+        return n - (7 + ze(e, 0, n).getUTCDay() - t) % 7 - 1
     }
 
-    function Ee(e, t, n, s, i) {
-        var r, a = 1 + 7 * (t - 1) + (7 + n - s) % 7 + Ge(e, s, i),
-            o = a <= 0 ? Fe(r = e - 1) + a : a > Fe(e) ? (r = e + 1, a - Fe(e)) : (r = e, a);
+    function $e(e, t, n, s, i) {
+        var r, t = 1 + 7 * (t - 1) + (7 + n - s) % 7 + qe(e, s, i),
+            n = t <= 0 ? We(r = e - 1) + t : t > We(e) ? (r = e + 1, t - We(e)) : (r = e, t);
         return {
             year: r,
-            dayOfYear: o
+            dayOfYear: n
         }
     }
 
-    function Ae(e, t, n) {
-        var s, i, r = Ge(e.year(), t, n),
-            a = Math.floor((e.dayOfYear() - r - 1) / 7) + 1;
-        return a < 1 ? s = a + je(i = e.year() - 1, t, n) : a > je(e.year(), t, n) ? (s = a - je(e.year(), t, n), i = e.year() + 1) : (i = e.year(), s = a), {
+    function Be(e, t, n) {
+        var s, i, r = qe(e.year(), t, n),
+            r = Math.floor((e.dayOfYear() - r - 1) / 7) + 1;
+        return r < 1 ? s = r + N(i = e.year() - 1, t, n) : r > N(e.year(), t, n) ? (s = r - N(e.year(), t, n), i = e.year() + 1) : (i = e.year(), s = r), {
             week: s,
             year: i
         }
     }
 
-    function je(e, t, n) {
-        var s = Ge(e, t, n),
-            i = Ge(e + 1, t, n);
-        return (Fe(e) - s + i) / 7
+    function N(e, t, n) {
+        var s = qe(e, t, n),
+            t = qe(e + 1, t, n);
+        return (We(e) - s + t) / 7
     }
-    C("w", ["ww", 2], "wo", "week"), C("W", ["WW", 2], "Wo", "isoWeek"), L("week", "w"), L("isoWeek", "W"), A("week", 5), A("isoWeek", 5), ce("w", te), ce("ww", te, Q), ce("W", te), ce("WW", te, Q), ge(["w", "ww", "W", "WW"], function(e, t, n, s) {
-        t[s.substr(0, 1)] = Z(e)
+    s("w", ["ww", 2], "wo", "week"), s("W", ["WW", 2], "Wo", "isoWeek"), h("w", n, u), h("ww", n, t), h("W", n, u), h("WW", n, t), Oe(["w", "ww", "W", "WW"], function(e, t, n, s) {
+        t[s.substr(0, 1)] = M(e)
     });
 
-    function Ie(e, t) {
+    function Je(e, t) {
         return e.slice(t, 7).concat(e.slice(0, t))
     }
-    C("d", 0, "do", "day"), C("dd", 0, 0, function(e) {
+    s("d", 0, "do", "day"), s("dd", 0, 0, function(e) {
         return this.localeData().weekdaysMin(this, e)
-    }), C("ddd", 0, 0, function(e) {
+    }), s("ddd", 0, 0, function(e) {
         return this.localeData().weekdaysShort(this, e)
-    }), C("dddd", 0, 0, function(e) {
+    }), s("dddd", 0, 0, function(e) {
         return this.localeData().weekdays(this, e)
-    }), C("e", 0, 0, "weekday"), C("E", 0, 0, "isoWeekday"), L("day", "d"), L("weekday", "e"), L("isoWeekday", "E"), A("day", 11), A("weekday", 11), A("isoWeekday", 11), ce("d", te), ce("e", te), ce("E", te), ce("dd", function(e, t) {
+    }), s("e", 0, 0, "weekday"), s("E", 0, 0, "isoWeekday"), h("d", n), h("e", n), h("E", n), h("dd", function(e, t) {
         return t.weekdaysMinRegex(e)
-    }), ce("ddd", function(e, t) {
+    }), h("ddd", function(e, t) {
         return t.weekdaysShortRegex(e)
-    }), ce("dddd", function(e, t) {
+    }), h("dddd", function(e, t) {
         return t.weekdaysRegex(e)
-    }), ge(["dd", "ddd", "dddd"], function(e, t, n, s) {
-        var i = n._locale.weekdaysParse(e, s, n._strict);
-        null != i ? t.d = i : y(n).invalidWeekday = e
-    }), ge(["d", "e", "E"], function(e, t, n, s) {
-        t[s] = Z(e)
+    }), Oe(["dd", "ddd", "dddd"], function(e, t, n, s) {
+        s = n._locale.weekdaysParse(e, s, n._strict);
+        null != s ? t.d = s : p(n).invalidWeekday = e
+    }), Oe(["d", "e", "E"], function(e, t, n, s) {
+        t[s] = M(e)
     });
-    var Ze = "Sunday_Monday_Tuesday_Wednesday_Thursday_Friday_Saturday".split("_"),
-        ze = "Sun_Mon_Tue_Wed_Thu_Fri_Sat".split("_"),
-        $e = "Su_Mo_Tu_We_Th_Fr_Sa".split("_"),
-        qe = de,
-        Be = de,
-        Je = de;
+    var Qe = "Sunday_Monday_Tuesday_Wednesday_Thursday_Friday_Saturday".split("_"),
+        Xe = "Sun_Mon_Tue_Wed_Thu_Fri_Sat".split("_"),
+        Ke = "Su_Mo_Tu_We_Th_Fr_Sa".split("_"),
+        et = i,
+        tt = i,
+        nt = i;
 
-    function Qe() {
+    function st() {
         function e(e, t) {
             return t.length - e.length
         }
-        for (var t, n, s, i, r = [], a = [], o = [], u = [], l = 0; l < 7; l++) t = _([2e3, 1]).day(l), n = me(this.weekdaysMin(t, "")), s = me(this.weekdaysShort(t, "")), i = me(this.weekdays(t, "")), r.push(n), a.push(s), o.push(i), u.push(n), u.push(s), u.push(i);
-        r.sort(e), a.sort(e), o.sort(e), u.sort(e), this._weekdaysRegex = new RegExp("^(" + u.join("|") + ")", "i"), this._weekdaysShortRegex = this._weekdaysRegex, this._weekdaysMinRegex = this._weekdaysRegex, this._weekdaysStrictRegex = new RegExp("^(" + o.join("|") + ")", "i"), this._weekdaysShortStrictRegex = new RegExp("^(" + a.join("|") + ")", "i"), this._weekdaysMinStrictRegex = new RegExp("^(" + r.join("|") + ")", "i")
+        for (var t, n, s, i = [], r = [], a = [], o = [], u = 0; u < 7; u++) s = l([2e3, 1]).day(u), t = f(this.weekdaysMin(s, "")), n = f(this.weekdaysShort(s, "")), s = f(this.weekdays(s, "")), i.push(t), r.push(n), a.push(s), o.push(t), o.push(n), o.push(s);
+        i.sort(e), r.sort(e), a.sort(e), o.sort(e), this._weekdaysRegex = new RegExp("^(" + o.join("|") + ")", "i"), this._weekdaysShortRegex = this._weekdaysRegex, this._weekdaysMinRegex = this._weekdaysRegex, this._weekdaysStrictRegex = new RegExp("^(" + a.join("|") + ")", "i"), this._weekdaysShortStrictRegex = new RegExp("^(" + r.join("|") + ")", "i"), this._weekdaysMinStrictRegex = new RegExp("^(" + i.join("|") + ")", "i")
     }
 
-    function Xe() {
+    function it() {
         return this.hours() % 12 || 12
     }
 
-    function Ke(e, t) {
-        C(e, 0, 0, function() {
+    function rt(e, t) {
+        s(e, 0, 0, function() {
             return this.localeData().meridiem(this.hours(), this.minutes(), t)
         })
     }
 
-    function et(e, t) {
+    function at(e, t) {
         return t._meridiemParse
     }
-    C("H", ["HH", 2], 0, "hour"), C("h", ["hh", 2], 0, Xe), C("k", ["kk", 2], 0, function() {
+    s("H", ["HH", 2], 0, "hour"), s("h", ["hh", 2], 0, it), s("k", ["kk", 2], 0, function() {
         return this.hours() || 24
-    }), C("hmm", 0, 0, function() {
-        return "" + Xe.apply(this) + T(this.minutes(), 2)
-    }), C("hmmss", 0, 0, function() {
-        return "" + Xe.apply(this) + T(this.minutes(), 2) + T(this.seconds(), 2)
-    }), C("Hmm", 0, 0, function() {
-        return "" + this.hours() + T(this.minutes(), 2)
-    }), C("Hmmss", 0, 0, function() {
-        return "" + this.hours() + T(this.minutes(), 2) + T(this.seconds(), 2)
-    }), Ke("a", !0), Ke("A", !1), L("hour", "h"), A("hour", 13), ce("a", et), ce("A", et), ce("H", te), ce("h", te), ce("k", te), ce("HH", te, Q), ce("hh", te, Q), ce("kk", te, Q), ce("hmm", ne), ce("hmmss", se), ce("Hmm", ne), ce("Hmmss", se), ye(["H", "HH"], Me), ye(["k", "kk"], function(e, t, n) {
-        var s = Z(e);
-        t[Me] = 24 === s ? 0 : s
-    }), ye(["a", "A"], function(e, t, n) {
+    }), s("hmm", 0, 0, function() {
+        return "" + it.apply(this) + r(this.minutes(), 2)
+    }), s("hmmss", 0, 0, function() {
+        return "" + it.apply(this) + r(this.minutes(), 2) + r(this.seconds(), 2)
+    }), s("Hmm", 0, 0, function() {
+        return "" + this.hours() + r(this.minutes(), 2)
+    }), s("Hmmss", 0, 0, function() {
+        return "" + this.hours() + r(this.minutes(), 2) + r(this.seconds(), 2)
+    }), rt("a", !0), rt("A", !1), h("a", at), h("A", at), h("H", n, d), h("h", n, u), h("k", n, u), h("HH", n, t), h("hh", n, t), h("kk", n, t), h("hmm", me), h("hmmss", _e), h("Hmm", me), h("Hmmss", _e), v(["H", "HH"], O), v(["k", "kk"], function(e, t, n) {
+        e = M(e);
+        t[O] = 24 === e ? 0 : e
+    }), v(["a", "A"], function(e, t, n) {
         n._isPm = n._locale.isPM(e), n._meridiem = e
-    }), ye(["h", "hh"], function(e, t, n) {
-        t[Me] = Z(e), y(n).bigHour = !0
-    }), ye("hmm", function(e, t, n) {
+    }), v(["h", "hh"], function(e, t, n) {
+        t[O] = M(e), p(n).bigHour = !0
+    }), v("hmm", function(e, t, n) {
         var s = e.length - 2;
-        t[Me] = Z(e.substr(0, s)), t[De] = Z(e.substr(s)), y(n).bigHour = !0
-    }), ye("hmmss", function(e, t, n) {
+        t[O] = M(e.substr(0, s)), t[b] = M(e.substr(s)), p(n).bigHour = !0
+    }), v("hmmss", function(e, t, n) {
         var s = e.length - 4,
             i = e.length - 2;
-        t[Me] = Z(e.substr(0, s)), t[De] = Z(e.substr(s, 2)), t[Se] = Z(e.substr(i)), y(n).bigHour = !0
-    }), ye("Hmm", function(e, t, n) {
+        t[O] = M(e.substr(0, s)), t[b] = M(e.substr(s, 2)), t[T] = M(e.substr(i)), p(n).bigHour = !0
+    }), v("Hmm", function(e, t, n) {
         var s = e.length - 2;
-        t[Me] = Z(e.substr(0, s)), t[De] = Z(e.substr(s))
-    }), ye("Hmmss", function(e, t, n) {
+        t[O] = M(e.substr(0, s)), t[b] = M(e.substr(s))
+    }), v("Hmmss", function(e, t, n) {
         var s = e.length - 4,
             i = e.length - 2;
-        t[Me] = Z(e.substr(0, s)), t[De] = Z(e.substr(s, 2)), t[Se] = Z(e.substr(i))
+        t[O] = M(e.substr(0, s)), t[b] = M(e.substr(s, 2)), t[T] = M(e.substr(i))
     });
-    var tt = z("Hours", !0);
-    var nt, st = {
+    i = Re("Hours", !0);
+    var ot, ut = {
             calendar: {
                 sameDay: "[Today at] LT",
                 nextDay: "[Tomorrow at] LT",
                 nextWeek: "dddd [at] LT",
                 lastDay: "[Yesterday at] LT",
                 lastWeek: "[Last] dddd [at] LT",
                 sameElse: "L"
@@ -532,563 +629,550 @@
                 w: "a week",
                 ww: "%d weeks",
                 M: "a month",
                 MM: "%d months",
                 y: "a year",
                 yy: "%d years"
             },
-            months: Te,
-            monthsShort: Ne,
+            months: Fe,
+            monthsShort: Le,
             week: {
                 dow: 0,
                 doy: 6
             },
-            weekdays: Ze,
-            weekdaysMin: $e,
-            weekdaysShort: ze,
+            weekdays: Qe,
+            weekdaysMin: Ke,
+            weekdaysShort: Xe,
             meridiemParse: /[ap]\.?m?\.?/i
         },
-        it = {},
-        rt = {};
+        W = {},
+        lt = {};
 
-    function at(e) {
-        return e ? e.toLowerCase().replace("_", "-") : e
+    function dt(e) {
+        return e && e.toLowerCase().replace("_", "-")
     }
 
-    function ot(e) {
+    function ht(e) {
         for (var t, n, s, i, r = 0; r < e.length;) {
-            for (t = (i = at(e[r]).split("-")).length, n = (n = at(e[r + 1])) ? n.split("-") : null; 0 < t;) {
-                if (s = ut(i.slice(0, t).join("-"))) return s;
+            for (t = (i = dt(e[r]).split("-")).length, n = (n = dt(e[r + 1])) ? n.split("-") : null; 0 < t;) {
+                if (s = ct(i.slice(0, t).join("-"))) return s;
                 if (n && n.length >= t && function(e, t) {
                         for (var n = Math.min(e.length, t.length), s = 0; s < n; s += 1)
                             if (e[s] !== t[s]) return s;
                         return n
                     }(i, n) >= t - 1) break;
                 t--
             }
             r++
         }
-        return nt
+        return ot
     }
 
-    function ut(t) {
-        var e;
-        if (void 0 === it[t] && "undefined" != typeof module && module && module.exports) try {
-            e = nt._abbr, require("./locale/" + t), lt(e)
+    function ct(t) {
+        var e, n;
+        if (void 0 === W[t] && "undefined" != typeof module && module && module.exports && (n = t) && n.match("^[^/\\\\]*$")) try {
+            e = ot._abbr, require("./locale/" + t), ft(e)
         } catch (e) {
-            it[t] = null
+            W[t] = null
         }
-        return it[t]
+        return W[t]
     }
 
-    function lt(e, t) {
-        var n;
-        return e && ((n = r(t) ? dt(e) : ht(e, t)) ? nt = n : "undefined" != typeof console && console.warn && console.warn("Locale " + e + " not found. Did you forget to load it?")), nt._abbr
+    function ft(e, t) {
+        return e && ((t = g(t) ? P(e) : mt(e, t)) ? ot = t : "undefined" != typeof console && console.warn && console.warn("Locale " + e + " not found. Did you forget to load it?")), ot._abbr
     }
 
-    function ht(e, t) {
-        if (null === t) return delete it[e], null;
-        var n, s = st;
-        if (t.abbr = e, null != it[e]) Y("defineLocaleOverride", "use moment.updateLocale(localeName, config) to change an existing locale. moment.defineLocale(localeName, config) should only be used for creating a new locale See http://momentjs.com/guides/#/warnings/define-locale/ for more info."), s = it[e]._config;
+    function mt(e, t) {
+        if (null === t) return delete W[e], null;
+        var n, s = ut;
+        if (t.abbr = e, null != W[e]) Q("defineLocaleOverride", "use moment.updateLocale(localeName, config) to change an existing locale. moment.defineLocale(localeName, config) should only be used for creating a new locale See http://momentjs.com/guides/#/warnings/define-locale/ for more info."), s = W[e]._config;
         else if (null != t.parentLocale)
-            if (null != it[t.parentLocale]) s = it[t.parentLocale]._config;
+            if (null != W[t.parentLocale]) s = W[t.parentLocale]._config;
             else {
-                if (null == (n = ut(t.parentLocale))) return rt[t.parentLocale] || (rt[t.parentLocale] = []), rt[t.parentLocale].push({
+                if (null == (n = ct(t.parentLocale))) return lt[t.parentLocale] || (lt[t.parentLocale] = []), lt[t.parentLocale].push({
                     name: e,
                     config: t
                 }), null;
                 s = n._config
-            } return it[e] = new x(b(s, t)), rt[e] && rt[e].forEach(function(e) {
-            ht(e.name, e.config)
-        }), lt(e), it[e]
+            } return W[e] = new K(X(s, t)), lt[e] && lt[e].forEach(function(e) {
+            mt(e.name, e.config)
+        }), ft(e), W[e]
     }
 
-    function dt(e) {
+    function P(e) {
         var t;
-        if (e && e._locale && e._locale._abbr && (e = e._locale._abbr), !e) return nt;
-        if (!o(e)) {
-            if (t = ut(e)) return t;
+        if (!(e = e && e._locale && e._locale._abbr ? e._locale._abbr : e)) return ot;
+        if (!y(e)) {
+            if (t = ct(e)) return t;
             e = [e]
         }
-        return ot(e)
+        return ht(e)
     }
 
-    function ct(e) {
-        var t, n = e._a;
-        return n && -2 === y(e).overflow && (t = n[ve] < 0 || 11 < n[ve] ? ve : n[ke] < 1 || n[ke] > xe(n[pe], n[ve]) ? ke : n[Me] < 0 || 24 < n[Me] || 24 === n[Me] && (0 !== n[De] || 0 !== n[Se] || 0 !== n[Ye]) ? Me : n[De] < 0 || 59 < n[De] ? De : n[Se] < 0 || 59 < n[Se] ? Se : n[Ye] < 0 || 999 < n[Ye] ? Ye : -1, y(e)._overflowDayOfYear && (t < pe || ke < t) && (t = ke), y(e)._overflowWeeks && -1 === t && (t = Oe), y(e)._overflowWeekday && -1 === t && (t = be), y(e).overflow = t), e
+    function _t(e) {
+        var t = e._a;
+        return t && -2 === p(e).overflow && (t = t[Y] < 0 || 11 < t[Y] ? Y : t[S] < 1 || t[S] > He(t[D], t[Y]) ? S : t[O] < 0 || 24 < t[O] || 24 === t[O] && (0 !== t[b] || 0 !== t[T] || 0 !== t[Te]) ? O : t[b] < 0 || 59 < t[b] ? b : t[T] < 0 || 59 < t[T] ? T : t[Te] < 0 || 999 < t[Te] ? Te : -1, p(e)._overflowDayOfYear && (t < D || S < t) && (t = S), p(e)._overflowWeeks && -1 === t && (t = xe), p(e)._overflowWeekday && -1 === t && (t = Ne), p(e).overflow = t), e
     }
-    var ft = /^\s*((?:[+-]\d{6}|\d{4})-(?:\d\d-\d\d|W\d\d-\d|W\d\d|\d\d\d|\d\d))(?:(T| )(\d\d(?::\d\d(?::\d\d(?:[.,]\d+)?)?)?)([+-]\d\d(?::?\d\d)?|\s*Z)?)?$/,
-        mt = /^\s*((?:[+-]\d{6}|\d{4})(?:\d\d\d\d|W\d\d\d|W\d\d|\d\d\d|\d\d|))(?:(T| )(\d\d(?:\d\d(?:\d\d(?:[.,]\d+)?)?)?)([+-]\d\d(?::?\d\d)?|\s*Z)?)?$/,
-        _t = /Z|[+-]\d\d(?::?\d\d)?/,
-        yt = [
+    var yt = /^\s*((?:[+-]\d{6}|\d{4})-(?:\d\d-\d\d|W\d\d-\d|W\d\d|\d\d\d|\d\d))(?:(T| )(\d\d(?::\d\d(?::\d\d(?:[.,]\d+)?)?)?)([+-]\d\d(?::?\d\d)?|\s*Z)?)?$/,
+        gt = /^\s*((?:[+-]\d{6}|\d{4})(?:\d\d\d\d|W\d\d\d|W\d\d|\d\d\d|\d\d|))(?:(T| )(\d\d(?:\d\d(?:\d\d(?:[.,]\d+)?)?)?)([+-]\d\d(?::?\d\d)?|\s*Z)?)?$/,
+        wt = /Z|[+-]\d\d(?::?\d\d)?/,
+        pt = [
             ["YYYYYY-MM-DD", /[+-]\d{6}-\d\d-\d\d/],
             ["YYYY-MM-DD", /\d{4}-\d\d-\d\d/],
             ["GGGG-[W]WW-E", /\d{4}-W\d\d-\d/],
             ["GGGG-[W]WW", /\d{4}-W\d\d/, !1],
             ["YYYY-DDD", /\d{4}-\d{3}/],
             ["YYYY-MM", /\d{4}-\d\d/, !1],
             ["YYYYYYMMDD", /[+-]\d{10}/],
             ["YYYYMMDD", /\d{8}/],
             ["GGGG[W]WWE", /\d{4}W\d{3}/],
             ["GGGG[W]WW", /\d{4}W\d{2}/, !1],
             ["YYYYDDD", /\d{7}/],
             ["YYYYMM", /\d{6}/, !1],
             ["YYYY", /\d{4}/, !1]
         ],
-        gt = [
+        kt = [
             ["HH:mm:ss.SSSS", /\d\d:\d\d:\d\d\.\d+/],
             ["HH:mm:ss,SSSS", /\d\d:\d\d:\d\d,\d+/],
             ["HH:mm:ss", /\d\d:\d\d:\d\d/],
             ["HH:mm", /\d\d:\d\d/],
             ["HHmmss.SSSS", /\d\d\d\d\d\d\.\d+/],
             ["HHmmss,SSSS", /\d\d\d\d\d\d,\d+/],
             ["HHmmss", /\d\d\d\d\d\d/],
             ["HHmm", /\d\d\d\d/],
             ["HH", /\d\d/]
         ],
-        wt = /^\/?Date\((-?\d+)/i,
-        pt = /^(?:(Mon|Tue|Wed|Thu|Fri|Sat|Sun),?\s)?(\d{1,2})\s(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)\s(\d{2,4})\s(\d\d):(\d\d)(?::(\d\d))?\s(?:(UT|GMT|[ECMP][SD]T)|([Zz])|([+-]\d{4}))$/,
-        vt = {
+        Mt = /^\/?Date\((-?\d+)/i,
+        vt = /^(?:(Mon|Tue|Wed|Thu|Fri|Sat|Sun),?\s)?(\d{1,2})\s(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)\s(\d{2,4})\s(\d\d):(\d\d)(?::(\d\d))?\s(?:(UT|GMT|[ECMP][SD]T)|([Zz])|([+-]\d{4}))$/,
+        Dt = {
             UT: 0,
             GMT: 0,
             EDT: -240,
             EST: -300,
             CDT: -300,
             CST: -360,
             MDT: -360,
             MST: -420,
             PDT: -420,
             PST: -480
         };
 
-    function kt(e) {
+    function Yt(e) {
         var t, n, s, i, r, a, o = e._i,
-            u = ft.exec(o) || mt.exec(o);
+            u = yt.exec(o) || gt.exec(o),
+            o = pt.length,
+            l = kt.length;
         if (u) {
-            for (y(e).iso = !0, t = 0, n = yt.length; t < n; t++)
-                if (yt[t][1].exec(u[1])) {
-                    i = yt[t][0], s = !1 !== yt[t][2];
+            for (p(e).iso = !0, t = 0, n = o; t < n; t++)
+                if (pt[t][1].exec(u[1])) {
+                    i = pt[t][0], s = !1 !== pt[t][2];
                     break
-                } if (null == i) return void(e._isValid = !1);
-            if (u[3]) {
-                for (t = 0, n = gt.length; t < n; t++)
-                    if (gt[t][1].exec(u[3])) {
-                        r = (u[2] || " ") + gt[t][0];
-                        break
-                    } if (null == r) return void(e._isValid = !1)
-            }
-            if (!s && null != r) return void(e._isValid = !1);
-            if (u[4]) {
-                if (!_t.exec(u[4])) return void(e._isValid = !1);
-                a = "Z"
+                } if (null == i) e._isValid = !1;
+            else {
+                if (u[3]) {
+                    for (t = 0, n = l; t < n; t++)
+                        if (kt[t][1].exec(u[3])) {
+                            r = (u[2] || " ") + kt[t][0];
+                            break
+                        } if (null == r) return void(e._isValid = !1)
+                }
+                if (s || null == r) {
+                    if (u[4]) {
+                        if (!wt.exec(u[4])) return void(e._isValid = !1);
+                        a = "Z"
+                    }
+                    e._f = i + (r || "") + (a || ""), xt(e)
+                } else e._isValid = !1
             }
-            e._f = i + (r || "") + (a || ""), Ot(e)
         } else e._isValid = !1
     }
 
-    function Mt(e, t, n, s, i, r) {
-        var a = [function(e) {
-            var t = parseInt(e, 10);
+    function St(e, t, n, s, i, r) {
+        e = [function(e) {
+            e = parseInt(e, 10);
             {
-                if (t <= 49) return 2e3 + t;
-                if (t <= 999) return 1900 + t
+                if (e <= 49) return 2e3 + e;
+                if (e <= 999) return 1900 + e
             }
-            return t
-        }(e), Ne.indexOf(t), parseInt(n, 10), parseInt(s, 10), parseInt(i, 10)];
-        return r && a.push(parseInt(r, 10)), a
-    }
-
-    function Dt(e) {
-        var t, n, s, i, r = pt.exec(e._i.replace(/\([^)]*\)|[\n\t]/g, " ").replace(/(\s\s+)/g, " ").replace(/^\s\s*/, "").replace(/\s\s*$/, ""));
-        if (r) {
-            if (t = Mt(r[4], r[3], r[2], r[5], r[6], r[7]), n = r[1], s = t, i = e, n && ze.indexOf(n) !== new Date(s[0], s[1], s[2]).getDay() && (y(i).weekdayMismatch = !0, !void(i._isValid = !1))) return;
-            e._a = t, e._tzm = function(e, t, n) {
-                if (e) return vt[e];
-                if (t) return 0;
-                var s = parseInt(n, 10),
-                    i = s % 100;
-                return 60 * ((s - i) / 100) + i
-            }(r[8], r[9], r[10]), e._d = Ve.apply(null, e._a), e._d.setUTCMinutes(e._d.getUTCMinutes() - e._tzm), y(e).rfc2822 = !0
-        } else e._isValid = !1
+            return e
+        }(e), Le.indexOf(t), parseInt(n, 10), parseInt(s, 10), parseInt(i, 10)];
+        return r && e.push(parseInt(r, 10)), e
+    }
+
+    function Ot(e) {
+        var t, n, s = vt.exec(e._i.replace(/\([^()]*\)|[\n\t]/g, " ").replace(/(\s\s+)/g, " ").replace(/^\s\s*/, "").replace(/\s\s*$/, ""));
+        s ? (t = St(s[4], s[3], s[2], s[5], s[6], s[7]), function(e, t, n) {
+            if (!e || Xe.indexOf(e) === new Date(t[0], t[1], t[2]).getDay()) return 1;
+            p(n).weekdayMismatch = !0, n._isValid = !1
+        }(s[1], t, e) && (e._a = t, e._tzm = (t = s[8], n = s[9], s = s[10], t ? Dt[t] : n ? 0 : 60 * (((t = parseInt(s, 10)) - (n = t % 100)) / 100) + n), e._d = ze.apply(null, e._a), e._d.setUTCMinutes(e._d.getUTCMinutes() - e._tzm), p(e).rfc2822 = !0)) : e._isValid = !1
     }
 
-    function St(e, t, n) {
+    function bt(e, t, n) {
         return null != e ? e : null != t ? t : n
     }
 
-    function Yt(e) {
-        var t, n, s, i, r, a, o, u = [];
+    function Tt(e) {
+        var t, n, s, i, r, a, o, u, l, d, h, c = [];
         if (!e._d) {
-            for (a = e, o = new Date(f.now()), s = a._useUTC ? [o.getUTCFullYear(), o.getUTCMonth(), o.getUTCDate()] : [o.getFullYear(), o.getMonth(), o.getDate()], e._w && null == e._a[ke] && null == e._a[ve] && function(e) {
-                    var t, n, s, i, r, a, o, u, l;
-                    null != (t = e._w).GG || null != t.W || null != t.E ? (r = 1, a = 4, n = St(t.GG, e._a[pe], Ae(Tt(), 1, 4).year), s = St(t.W, 1), ((i = St(t.E, 1)) < 1 || 7 < i) && (u = !0)) : (r = e._locale._week.dow, a = e._locale._week.doy, l = Ae(Tt(), r, a), n = St(t.gg, e._a[pe], l.year), s = St(t.w, l.week), null != t.d ? ((i = t.d) < 0 || 6 < i) && (u = !0) : null != t.e ? (i = t.e + r, (t.e < 0 || 6 < t.e) && (u = !0)) : i = r);
-                    s < 1 || s > je(n, r, a) ? y(e)._overflowWeeks = !0 : null != u ? y(e)._overflowWeekday = !0 : (o = Ee(n, s, i, r, a), e._a[pe] = o.year, e._dayOfYear = o.dayOfYear)
-                }(e), null != e._dayOfYear && (r = St(e._a[pe], s[pe]), (e._dayOfYear > Fe(r) || 0 === e._dayOfYear) && (y(e)._overflowDayOfYear = !0), n = Ve(r, 0, e._dayOfYear), e._a[ve] = n.getUTCMonth(), e._a[ke] = n.getUTCDate()), t = 0; t < 3 && null == e._a[t]; ++t) e._a[t] = u[t] = s[t];
-            for (; t < 7; t++) e._a[t] = u[t] = null == e._a[t] ? 2 === t ? 1 : 0 : e._a[t];
-            24 === e._a[Me] && 0 === e._a[De] && 0 === e._a[Se] && 0 === e._a[Ye] && (e._nextDay = !0, e._a[Me] = 0), e._d = (e._useUTC ? Ve : function(e, t, n, s, i, r, a) {
-                var o;
-                return e < 100 && 0 <= e ? (o = new Date(e + 400, t, n, s, i, r, a), isFinite(o.getFullYear()) && o.setFullYear(e)) : o = new Date(e, t, n, s, i, r, a), o
-            }).apply(null, u), i = e._useUTC ? e._d.getUTCDay() : e._d.getDay(), null != e._tzm && e._d.setUTCMinutes(e._d.getUTCMinutes() - e._tzm), e._nextDay && (e._a[Me] = 24), e._w && void 0 !== e._w.d && e._w.d !== i && (y(e).weekdayMismatch = !0)
+            for (s = e, i = new Date(_.now()), n = s._useUTC ? [i.getUTCFullYear(), i.getUTCMonth(), i.getUTCDate()] : [i.getFullYear(), i.getMonth(), i.getDate()], e._w && null == e._a[S] && null == e._a[Y] && (null != (i = (s = e)._w).GG || null != i.W || null != i.E ? (u = 1, l = 4, r = bt(i.GG, s._a[D], Be(R(), 1, 4).year), a = bt(i.W, 1), ((o = bt(i.E, 1)) < 1 || 7 < o) && (d = !0)) : (u = s._locale._week.dow, l = s._locale._week.doy, h = Be(R(), u, l), r = bt(i.gg, s._a[D], h.year), a = bt(i.w, h.week), null != i.d ? ((o = i.d) < 0 || 6 < o) && (d = !0) : null != i.e ? (o = i.e + u, (i.e < 0 || 6 < i.e) && (d = !0)) : o = u), a < 1 || a > N(r, u, l) ? p(s)._overflowWeeks = !0 : null != d ? p(s)._overflowWeekday = !0 : (h = $e(r, a, o, u, l), s._a[D] = h.year, s._dayOfYear = h.dayOfYear)), null != e._dayOfYear && (i = bt(e._a[D], n[D]), (e._dayOfYear > We(i) || 0 === e._dayOfYear) && (p(e)._overflowDayOfYear = !0), d = ze(i, 0, e._dayOfYear), e._a[Y] = d.getUTCMonth(), e._a[S] = d.getUTCDate()), t = 0; t < 3 && null == e._a[t]; ++t) e._a[t] = c[t] = n[t];
+            for (; t < 7; t++) e._a[t] = c[t] = null == e._a[t] ? 2 === t ? 1 : 0 : e._a[t];
+            24 === e._a[O] && 0 === e._a[b] && 0 === e._a[T] && 0 === e._a[Te] && (e._nextDay = !0, e._a[O] = 0), e._d = (e._useUTC ? ze : Ze).apply(null, c), r = e._useUTC ? e._d.getUTCDay() : e._d.getDay(), null != e._tzm && e._d.setUTCMinutes(e._d.getUTCMinutes() - e._tzm), e._nextDay && (e._a[O] = 24), e._w && void 0 !== e._w.d && e._w.d !== r && (p(e).weekdayMismatch = !0)
         }
     }
 
-    function Ot(e) {
-        if (e._f !== f.ISO_8601)
-            if (e._f !== f.RFC_2822) {
-                e._a = [], y(e).empty = !0;
-                for (var t, n, s, i, r, a, o, u = "" + e._i, l = u.length, h = 0, d = H(e._f, e._locale).match(N) || [], c = 0; c < d.length; c++) n = d[c], (t = (u.match(fe(n, e)) || [])[0]) && (0 < (s = u.substr(0, u.indexOf(t))).length && y(e).unusedInput.push(s), u = u.slice(u.indexOf(t) + t.length), h += t.length), W[n] ? (t ? y(e).empty = !1 : y(e).unusedTokens.push(n), r = n, o = e, null != (a = t) && m(_e, r) && _e[r](a, o._a, o, r)) : e._strict && !t && y(e).unusedTokens.push(n);
-                y(e).charsLeftOver = l - h, 0 < u.length && y(e).unusedInput.push(u), e._a[Me] <= 12 && !0 === y(e).bigHour && 0 < e._a[Me] && (y(e).bigHour = void 0), y(e).parsedDateParts = e._a.slice(0), y(e).meridiem = e._meridiem, e._a[Me] = function(e, t, n) {
-                    var s;
-                    if (null == n) return t;
-                    return null != e.meridiemHour ? e.meridiemHour(t, n) : (null != e.isPM && ((s = e.isPM(n)) && t < 12 && (t += 12), s || 12 !== t || (t = 0)), t)
-                }(e._locale, e._a[Me], e._meridiem), null !== (i = y(e).era) && (e._a[pe] = e._locale.erasConvertYear(i, e._a[pe])), Yt(e), ct(e)
-            } else Dt(e);
-        else kt(e)
-    }
-
-    function bt(e) {
-        var t, n, s = e._i,
-            i = e._f;
-        return e._locale = e._locale || dt(e._l), null === s || void 0 === i && "" === s ? w({
+    function xt(e) {
+        if (e._f === _.ISO_8601) Yt(e);
+        else if (e._f === _.RFC_2822) Ot(e);
+        else {
+            e._a = [], p(e).empty = !0;
+            for (var t, n, s, i, r, a = "" + e._i, o = a.length, u = 0, l = ae(e._f, e._locale).match(te) || [], d = l.length, h = 0; h < d; h++) n = l[h], (t = (a.match(De(n, e)) || [])[0]) && (0 < (s = a.substr(0, a.indexOf(t))).length && p(e).unusedInput.push(s), a = a.slice(a.indexOf(t) + t.length), u += t.length), ie[n] ? (t ? p(e).empty = !1 : p(e).unusedTokens.push(n), s = n, r = e, null != (i = t) && c(Se, s) && Se[s](i, r._a, r, s)) : e._strict && !t && p(e).unusedTokens.push(n);
+            p(e).charsLeftOver = o - u, 0 < a.length && p(e).unusedInput.push(a), e._a[O] <= 12 && !0 === p(e).bigHour && 0 < e._a[O] && (p(e).bigHour = void 0), p(e).parsedDateParts = e._a.slice(0), p(e).meridiem = e._meridiem, e._a[O] = function(e, t, n) {
+                if (null == n) return t;
+                return null != e.meridiemHour ? e.meridiemHour(t, n) : null != e.isPM ? ((e = e.isPM(n)) && t < 12 && (t += 12), t = e || 12 !== t ? t : 0) : t
+            }(e._locale, e._a[O], e._meridiem), null !== (o = p(e).era) && (e._a[D] = e._locale.erasConvertYear(o, e._a[D])), Tt(e), _t(e)
+        }
+    }
+
+    function Nt(e) {
+        var t, n, s, i = e._i,
+            r = e._f;
+        if (e._locale = e._locale || P(e._l), null === i || void 0 === r && "" === i) return I({
             nullInput: !0
-        }) : ("string" == typeof s && (e._i = s = e._locale.preparse(s)), M(s) ? new k(ct(s)) : (a(s) ? e._d = s : o(i) ? function(e) {
-            var t, n, s, i, r, a, o = !1;
-            if (0 === e._f.length) return y(e).invalidFormat = !0, e._d = new Date(NaN);
-            for (i = 0; i < e._f.length; i++) r = 0, a = !1, t = v({}, e), null != e._useUTC && (t._useUTC = e._useUTC), t._f = e._f[i], Ot(t), g(t) && (a = !0), r += y(t).charsLeftOver, r += 10 * y(t).unusedTokens.length, y(t).score = r, o ? r < s && (s = r, n = t) : (null == s || r < s || a) && (s = r, n = t, a && (o = !0));
-            c(e, n || t)
-        }(e) : i ? Ot(e) : r(n = (t = e)._i) ? t._d = new Date(f.now()) : a(n) ? t._d = new Date(n.valueOf()) : "string" == typeof n ? function(e) {
-            var t = wt.exec(e._i);
-            null === t ? (kt(e), !1 === e._isValid && (delete e._isValid, Dt(e), !1 === e._isValid && (delete e._isValid, e._strict ? e._isValid = !1 : f.createFromInputFallback(e)))) : e._d = new Date(+t[1])
-        }(t) : o(n) ? (t._a = d(n.slice(0), function(e) {
+        });
+        if ("string" == typeof i && (e._i = i = e._locale.preparse(i)), k(i)) return new $(_t(i));
+        if (V(i)) e._d = i;
+        else if (y(r)) {
+            var a, o, u, l, d, h, c = e,
+                f = !1,
+                m = c._f.length;
+            if (0 === m) p(c).invalidFormat = !0, c._d = new Date(NaN);
+            else {
+                for (l = 0; l < m; l++) d = 0, h = !1, a = q({}, c), null != c._useUTC && (a._useUTC = c._useUTC), a._f = c._f[l], xt(a), A(a) && (h = !0), d = (d += p(a).charsLeftOver) + 10 * p(a).unusedTokens.length, p(a).score = d, f ? d < u && (u = d, o = a) : (null == u || d < u || h) && (u = d, o = a, h) && (f = !0);
+                E(c, o || a)
+            }
+        } else if (r) xt(e);
+        else if (g(r = (i = e)._i)) i._d = new Date(_.now());
+        else V(r) ? i._d = new Date(r.valueOf()) : "string" == typeof r ? (n = i, null !== (t = Mt.exec(n._i)) ? n._d = new Date(+t[1]) : (Yt(n), !1 === n._isValid && (delete n._isValid, Ot(n), !1 === n._isValid) && (delete n._isValid, n._strict ? n._isValid = !1 : _.createFromInputFallback(n)))) : y(r) ? (i._a = G(r.slice(0), function(e) {
             return parseInt(e, 10)
-        }), Yt(t)) : u(n) ? function(e) {
-            var t, n;
-            e._d || (n = void 0 === (t = G(e._i)).day ? t.date : t.day, e._a = d([t.year, t.month, n, t.hour, t.minute, t.second, t.millisecond], function(e) {
-                return e && parseInt(e, 10)
-            }), Yt(e))
-        }(t) : h(n) ? t._d = new Date(n) : f.createFromInputFallback(t), g(e) || (e._d = null), e))
+        }), Tt(i)) : F(r) ? (t = i)._d || (s = void 0 === (n = ue(t._i)).day ? n.date : n.day, t._a = G([n.year, n.month, s, n.hour, n.minute, n.second, n.millisecond], function(e) {
+            return e && parseInt(e, 10)
+        }), Tt(t)) : w(r) ? i._d = new Date(r) : _.createFromInputFallback(i);
+        return A(e) || (e._d = null), e
     }
 
-    function xt(e, t, n, s, i) {
-        var r, a = {};
-        return !0 !== t && !1 !== t || (s = t, t = void 0), !0 !== n && !1 !== n || (s = n, n = void 0), (u(e) && l(e) || o(e) && 0 === e.length) && (e = void 0), a._isAMomentObject = !0, a._useUTC = a._isUTC = i, a._l = n, a._i = e, a._f = t, a._strict = s, (r = new k(ct(bt(a))))._nextDay && (r.add(1, "d"), r._nextDay = void 0), r
+    function Wt(e, t, n, s, i) {
+        var r = {};
+        return !0 !== t && !1 !== t || (s = t, t = void 0), !0 !== n && !1 !== n || (s = n, n = void 0), (F(e) && L(e) || y(e) && 0 === e.length) && (e = void 0), r._isAMomentObject = !0, r._useUTC = r._isUTC = i, r._l = n, r._i = e, r._f = t, r._strict = s, (i = new $(_t(Nt(i = r))))._nextDay && (i.add(1, "d"), i._nextDay = void 0), i
     }
 
-    function Tt(e, t, n, s) {
-        return xt(e, t, n, s, !1)
+    function R(e, t, n, s) {
+        return Wt(e, t, n, s, !1)
     }
-    f.createFromInputFallback = n("value provided is not in a recognized RFC2822 or ISO format. moment construction falls back to js Date(), which is not reliable across all browsers and versions. Non RFC2822/ISO date formats are discouraged. Please refer to http://momentjs.com/guides/#/warnings/js-date/ for more info.", function(e) {
+    _.createFromInputFallback = e("value provided is not in a recognized RFC2822 or ISO format. moment construction falls back to js Date(), which is not reliable across all browsers and versions. Non RFC2822/ISO date formats are discouraged. Please refer to http://momentjs.com/guides/#/warnings/js-date/ for more info.", function(e) {
         e._d = new Date(e._i + (e._useUTC ? " UTC" : ""))
-    }), f.ISO_8601 = function() {}, f.RFC_2822 = function() {};
-    var Nt = n("moment().min is deprecated, use moment.max instead. http://momentjs.com/guides/#/warnings/min-max/", function() {
-            var e = Tt.apply(null, arguments);
-            return this.isValid() && e.isValid() ? e < this ? this : e : w()
-        }),
-        Pt = n("moment().max is deprecated, use moment.min instead. http://momentjs.com/guides/#/warnings/min-max/", function() {
-            var e = Tt.apply(null, arguments);
-            return this.isValid() && e.isValid() ? this < e ? this : e : w()
-        });
+    }), _.ISO_8601 = function() {}, _.RFC_2822 = function() {};
+    me = e("moment().min is deprecated, use moment.max instead. http://momentjs.com/guides/#/warnings/min-max/", function() {
+        var e = R.apply(null, arguments);
+        return this.isValid() && e.isValid() ? e < this ? this : e : I()
+    }), _e = e("moment().max is deprecated, use moment.min instead. http://momentjs.com/guides/#/warnings/min-max/", function() {
+        var e = R.apply(null, arguments);
+        return this.isValid() && e.isValid() ? this < e ? this : e : I()
+    });
 
-    function Rt(e, t) {
+    function Pt(e, t) {
         var n, s;
-        if (1 === t.length && o(t[0]) && (t = t[0]), !t.length) return Tt();
+        if (!(t = 1 === t.length && y(t[0]) ? t[0] : t).length) return R();
         for (n = t[0], s = 1; s < t.length; ++s) t[s].isValid() && !t[s][e](n) || (n = t[s]);
         return n
     }
-    var Wt = ["year", "quarter", "month", "week", "day", "hour", "minute", "second", "millisecond"];
+    var Rt = ["year", "quarter", "month", "week", "day", "hour", "minute", "second", "millisecond"];
 
     function Ct(e) {
-        var t = G(e),
-            n = t.year || 0,
-            s = t.quarter || 0,
-            i = t.month || 0,
-            r = t.week || t.isoWeek || 0,
-            a = t.day || 0,
-            o = t.hour || 0,
-            u = t.minute || 0,
-            l = t.second || 0,
-            h = t.millisecond || 0;
+        var e = ue(e),
+            t = e.year || 0,
+            n = e.quarter || 0,
+            s = e.month || 0,
+            i = e.week || e.isoWeek || 0,
+            r = e.day || 0,
+            a = e.hour || 0,
+            o = e.minute || 0,
+            u = e.second || 0,
+            l = e.millisecond || 0;
         this._isValid = function(e) {
-            var t, n, s = !1;
+            var t, n, s = !1,
+                i = Rt.length;
             for (t in e)
-                if (m(e, t) && (-1 === we.call(Wt, t) || null != e[t] && isNaN(e[t]))) return !1;
-            for (n = 0; n < Wt.length; ++n)
-                if (e[Wt[n]]) {
+                if (c(e, t) && (-1 === x.call(Rt, t) || null != e[t] && isNaN(e[t]))) return !1;
+            for (n = 0; n < i; ++n)
+                if (e[Rt[n]]) {
                     if (s) return !1;
-                    parseFloat(e[Wt[n]]) !== Z(e[Wt[n]]) && (s = !0)
+                    parseFloat(e[Rt[n]]) !== M(e[Rt[n]]) && (s = !0)
                 } return !0
-        }(t), this._milliseconds = +h + 1e3 * l + 6e4 * u + 1e3 * o * 60 * 60, this._days = +a + 7 * r, this._months = +i + 3 * s + 12 * n, this._data = {}, this._locale = dt(), this._bubble()
+        }(e), this._milliseconds = +l + 1e3 * u + 6e4 * o + 1e3 * a * 60 * 60, this._days = +r + 7 * i, this._months = +s + 3 * n + 12 * t, this._data = {}, this._locale = P(), this._bubble()
     }
 
     function Ut(e) {
         return e instanceof Ct
     }
 
     function Ht(e) {
         return e < 0 ? -1 * Math.round(-1 * e) : Math.round(e)
     }
 
     function Ft(e, n) {
-        C(e, 0, 0, function() {
+        s(e, 0, 0, function() {
             var e = this.utcOffset(),
                 t = "+";
-            return e < 0 && (e = -e, t = "-"), t + T(~~(e / 60), 2) + n + T(~~e % 60, 2)
+            return e < 0 && (e = -e, t = "-"), t + r(~~(e / 60), 2) + n + r(~~e % 60, 2)
         })
     }
-    Ft("Z", ":"), Ft("ZZ", ""), ce("Z", he), ce("ZZ", he), ye(["Z", "ZZ"], function(e, t, n) {
-        n._useUTC = !0, n._tzm = Vt(he, e)
+    Ft("Z", ":"), Ft("ZZ", ""), h("Z", ve), h("ZZ", ve), v(["Z", "ZZ"], function(e, t, n) {
+        n._useUTC = !0, n._tzm = Vt(ve, e)
     });
     var Lt = /([\+\-]|\d\d)/gi;
 
     function Vt(e, t) {
-        var n, s, i = (t || "").match(e);
-        return null === i ? null : 0 === (s = 60 * (n = ((i[i.length - 1] || []) + "").match(Lt) || ["-", 0, 0])[1] + Z(n[2])) ? 0 : "+" === n[0] ? s : -s
+        var t = (t || "").match(e);
+        return null === t ? null : 0 === (t = 60 * (e = ((t[t.length - 1] || []) + "").match(Lt) || ["-", 0, 0])[1] + M(e[2])) ? 0 : "+" === e[0] ? t : -t
     }
 
     function Gt(e, t) {
-        var n, s;
-        return t._isUTC ? (n = t.clone(), s = (M(e) || a(e) ? e.valueOf() : Tt(e).valueOf()) - n.valueOf(), n._d.setTime(n._d.valueOf() + s), f.updateOffset(n, !1), n) : Tt(e).local()
+        var n;
+        return t._isUTC ? (t = t.clone(), n = (k(e) || V(e) ? e : R(e)).valueOf() - t.valueOf(), t._d.setTime(t._d.valueOf() + n), _.updateOffset(t, !1), t) : R(e).local()
     }
 
     function Et(e) {
         return -Math.round(e._d.getTimezoneOffset())
     }
 
     function At() {
-        return !!this.isValid() && (this._isUTC && 0 === this._offset)
+        return !!this.isValid() && this._isUTC && 0 === this._offset
     }
-    f.updateOffset = function() {};
-    var jt = /^(-|\+)?(?:(\d*)[. ])?(\d+):(\d+)(?::(\d+)(\.\d*)?)?$/,
-        It = /^(-|\+)?P(?:([-+]?[0-9,.]*)Y)?(?:([-+]?[0-9,.]*)M)?(?:([-+]?[0-9,.]*)W)?(?:([-+]?[0-9,.]*)D)?(?:T(?:([-+]?[0-9,.]*)H)?(?:([-+]?[0-9,.]*)M)?(?:([-+]?[0-9,.]*)S)?)?$/;
-
-    function Zt(e, t) {
-        var n, s, i, r = e,
-            a = null;
-        return Ut(e) ? r = {
+    _.updateOffset = function() {};
+    var It = /^(-|\+)?(?:(\d*)[. ])?(\d+):(\d+)(?::(\d+)(\.\d*)?)?$/,
+        jt = /^(-|\+)?P(?:([-+]?[0-9,.]*)Y)?(?:([-+]?[0-9,.]*)M)?(?:([-+]?[0-9,.]*)W)?(?:([-+]?[0-9,.]*)D)?(?:T(?:([-+]?[0-9,.]*)H)?(?:([-+]?[0-9,.]*)M)?(?:([-+]?[0-9,.]*)S)?)?$/;
+
+    function C(e, t) {
+        var n, s = e;
+        return Ut(e) ? s = {
             ms: e._milliseconds,
             d: e._days,
             M: e._months
-        } : h(e) || !isNaN(+e) ? (r = {}, t ? r[t] = +e : r.milliseconds = +e) : (a = jt.exec(e)) ? (n = "-" === a[1] ? -1 : 1, r = {
+        } : w(e) || !isNaN(+e) ? (s = {}, t ? s[t] = +e : s.milliseconds = +e) : (t = It.exec(e)) ? (n = "-" === t[1] ? -1 : 1, s = {
             y: 0,
-            d: Z(a[ke]) * n,
-            h: Z(a[Me]) * n,
-            m: Z(a[De]) * n,
-            s: Z(a[Se]) * n,
-            ms: Z(Ht(1e3 * a[Ye])) * n
-        }) : (a = It.exec(e)) ? (n = "-" === a[1] ? -1 : 1, r = {
-            y: zt(a[2], n),
-            M: zt(a[3], n),
-            w: zt(a[4], n),
-            d: zt(a[5], n),
-            h: zt(a[6], n),
-            m: zt(a[7], n),
-            s: zt(a[8], n)
-        }) : null == r ? r = {} : "object" == typeof r && ("from" in r || "to" in r) && (i = function(e, t) {
+            d: M(t[S]) * n,
+            h: M(t[O]) * n,
+            m: M(t[b]) * n,
+            s: M(t[T]) * n,
+            ms: M(Ht(1e3 * t[Te])) * n
+        }) : (t = jt.exec(e)) ? (n = "-" === t[1] ? -1 : 1, s = {
+            y: Zt(t[2], n),
+            M: Zt(t[3], n),
+            w: Zt(t[4], n),
+            d: Zt(t[5], n),
+            h: Zt(t[6], n),
+            m: Zt(t[7], n),
+            s: Zt(t[8], n)
+        }) : null == s ? s = {} : "object" == typeof s && ("from" in s || "to" in s) && (t = function(e, t) {
             var n;
             if (!e.isValid() || !t.isValid()) return {
                 milliseconds: 0,
                 months: 0
             };
-            t = Gt(t, e), e.isBefore(t) ? n = $t(e, t) : ((n = $t(t, e)).milliseconds = -n.milliseconds, n.months = -n.months);
+            t = Gt(t, e), e.isBefore(t) ? n = zt(e, t) : ((n = zt(t, e)).milliseconds = -n.milliseconds, n.months = -n.months);
             return n
-        }(Tt(r.from), Tt(r.to)), (r = {}).ms = i.milliseconds, r.M = i.months), s = new Ct(r), Ut(e) && m(e, "_locale") && (s._locale = e._locale), Ut(e) && m(e, "_isValid") && (s._isValid = e._isValid), s
+        }(R(s.from), R(s.to)), (s = {}).ms = t.milliseconds, s.M = t.months), n = new Ct(s), Ut(e) && c(e, "_locale") && (n._locale = e._locale), Ut(e) && c(e, "_isValid") && (n._isValid = e._isValid), n
     }
 
-    function zt(e, t) {
-        var n = e && parseFloat(e.replace(",", "."));
-        return (isNaN(n) ? 0 : n) * t
+    function Zt(e, t) {
+        e = e && parseFloat(e.replace(",", "."));
+        return (isNaN(e) ? 0 : e) * t
     }
 
-    function $t(e, t) {
+    function zt(e, t) {
         var n = {};
-        return n.months = t.month() - e.month() + 12 * (t.year() - e.year()), e.clone().add(n.months, "M").isAfter(t) && --n.months, n.milliseconds = t - e.clone().add(n.months, "M"), n
+        return n.months = t.month() - e.month() + 12 * (t.year() - e.year()), e.clone().add(n.months, "M").isAfter(t) && --n.months, n.milliseconds = +t - +e.clone().add(n.months, "M"), n
     }
 
     function qt(s, i) {
         return function(e, t) {
             var n;
-            return null === t || isNaN(+t) || (Y(i, "moment()." + i + "(period, number) is deprecated. Please use moment()." + i + "(number, period). See http://momentjs.com/guides/#/warnings/add-inverted-param/ for more info."), n = e, e = t, t = n), Bt(this, Zt(e, t), s), this
+            return null === t || isNaN(+t) || (Q(i, "moment()." + i + "(period, number) is deprecated. Please use moment()." + i + "(number, period). See http://momentjs.com/guides/#/warnings/add-inverted-param/ for more info."), n = e, e = t, t = n), $t(this, C(e, t), s), this
         }
     }
 
-    function Bt(e, t, n, s) {
+    function $t(e, t, n, s) {
         var i = t._milliseconds,
             r = Ht(t._days),
-            a = Ht(t._months);
-        e.isValid() && (s = null == s || s, a && Ce(e, $(e, "Month") + a * n), r && q(e, "Date", $(e, "Date") + r * n), i && e._d.setTime(e._d.valueOf() + i * n), s && f.updateOffset(e, r || a))
+            t = Ht(t._months);
+        e.isValid() && (s = null == s || s, t && Ae(e, Ce(e, "Month") + t * n), r && Ue(e, "Date", Ce(e, "Date") + r * n), i && e._d.setTime(e._d.valueOf() + i * n), s) && _.updateOffset(e, r || t)
     }
-    Zt.fn = Ct.prototype, Zt.invalid = function() {
-        return Zt(NaN)
+    C.fn = Ct.prototype, C.invalid = function() {
+        return C(NaN)
     };
-    var Jt = qt(1, "add"),
-        Qt = qt(-1, "subtract");
+    Fe = qt(1, "add"), Qe = qt(-1, "subtract");
 
-    function Xt(e) {
+    function Bt(e) {
         return "string" == typeof e || e instanceof String
     }
 
-    function Kt(e) {
-        return M(e) || a(e) || Xt(e) || h(e) || function(t) {
-            var e = o(t),
+    function Jt(e) {
+        return k(e) || V(e) || Bt(e) || w(e) || function(t) {
+            var e = y(t),
                 n = !1;
             e && (n = 0 === t.filter(function(e) {
-                return !h(e) && Xt(t)
+                return !w(e) && Bt(t)
             }).length);
             return e && n
         }(e) || function(e) {
-            var t, n, s = u(e) && !l(e),
+            var t, n, s = F(e) && !L(e),
                 i = !1,
-                r = ["years", "year", "y", "months", "month", "M", "days", "day", "d", "dates", "date", "D", "hours", "hour", "h", "minutes", "minute", "m", "seconds", "second", "s", "milliseconds", "millisecond", "ms"];
-            for (t = 0; t < r.length; t += 1) n = r[t], i = i || m(e, n);
+                r = ["years", "year", "y", "months", "month", "M", "days", "day", "d", "dates", "date", "D", "hours", "hour", "h", "minutes", "minute", "m", "seconds", "second", "s", "milliseconds", "millisecond", "ms"],
+                a = r.length;
+            for (t = 0; t < a; t += 1) n = r[t], i = i || c(e, n);
             return s && i
         }(e) || null == e
     }
 
-    function en(e, t) {
-        if (e.date() < t.date()) return -en(t, e);
-        var n = 12 * (t.year() - e.year()) + (t.month() - e.month()),
-            s = e.clone().add(n, "months"),
-            i = t - s < 0 ? (t - s) / (s - e.clone().add(n - 1, "months")) : (t - s) / (e.clone().add(1 + n, "months") - s);
-        return -(n + i) || 0
+    function Qt(e, t) {
+        var n, s;
+        return e.date() < t.date() ? -Qt(t, e) : -((n = 12 * (t.year() - e.year()) + (t.month() - e.month())) + (t - (s = e.clone().add(n, "months")) < 0 ? (t - s) / (s - e.clone().add(n - 1, "months")) : (t - s) / (e.clone().add(1 + n, "months") - s))) || 0
     }
 
-    function tn(e) {
-        var t;
-        return void 0 === e ? this._locale._abbr : (null != (t = dt(e)) && (this._locale = t), this)
+    function Xt(e) {
+        return void 0 === e ? this._locale._abbr : (null != (e = P(e)) && (this._locale = e), this)
     }
-    f.defaultFormat = "YYYY-MM-DDTHH:mm:ssZ", f.defaultFormatUtc = "YYYY-MM-DDTHH:mm:ss[Z]";
-    var nn = n("moment().lang() is deprecated. Instead, use moment().localeData() to get the language configuration. Use moment().locale() to change languages.", function(e) {
+    _.defaultFormat = "YYYY-MM-DDTHH:mm:ssZ", _.defaultFormatUtc = "YYYY-MM-DDTHH:mm:ss[Z]";
+    Ke = e("moment().lang() is deprecated. Instead, use moment().localeData() to get the language configuration. Use moment().locale() to change languages.", function(e) {
         return void 0 === e ? this.localeData() : this.locale(e)
     });
 
-    function sn() {
+    function Kt() {
         return this._locale
     }
-    var rn = 126227808e5;
+    var en = 126227808e5;
 
-    function an(e, t) {
+    function tn(e, t) {
         return (e % t + t) % t
     }
 
-    function on(e, t, n) {
-        return e < 100 && 0 <= e ? new Date(e + 400, t, n) - rn : new Date(e, t, n).valueOf()
+    function nn(e, t, n) {
+        return e < 100 && 0 <= e ? new Date(e + 400, t, n) - en : new Date(e, t, n).valueOf()
     }
 
-    function un(e, t, n) {
-        return e < 100 && 0 <= e ? Date.UTC(e + 400, t, n) - rn : Date.UTC(e, t, n)
+    function sn(e, t, n) {
+        return e < 100 && 0 <= e ? Date.UTC(e + 400, t, n) - en : Date.UTC(e, t, n)
     }
 
-    function ln(e, t) {
+    function rn(e, t) {
         return t.erasAbbrRegex(e)
     }
 
-    function hn() {
-        for (var e = [], t = [], n = [], s = [], i = this.eras(), r = 0, a = i.length; r < a; ++r) t.push(me(i[r].name)), e.push(me(i[r].abbr)), n.push(me(i[r].narrow)), s.push(me(i[r].name)), s.push(me(i[r].abbr)), s.push(me(i[r].narrow));
-        this._erasRegex = new RegExp("^(" + s.join("|") + ")", "i"), this._erasNameRegex = new RegExp("^(" + t.join("|") + ")", "i"), this._erasAbbrRegex = new RegExp("^(" + e.join("|") + ")", "i"), this._erasNarrowRegex = new RegExp("^(" + n.join("|") + ")", "i")
+    function an() {
+        for (var e, t, n, s = [], i = [], r = [], a = [], o = this.eras(), u = 0, l = o.length; u < l; ++u) e = f(o[u].name), t = f(o[u].abbr), n = f(o[u].narrow), i.push(e), s.push(t), r.push(n), a.push(e), a.push(t), a.push(n);
+        this._erasRegex = new RegExp("^(" + a.join("|") + ")", "i"), this._erasNameRegex = new RegExp("^(" + i.join("|") + ")", "i"), this._erasAbbrRegex = new RegExp("^(" + s.join("|") + ")", "i"), this._erasNarrowRegex = new RegExp("^(" + r.join("|") + ")", "i")
     }
 
-    function dn(e, t) {
-        C(0, [e, e.length], 0, t)
+    function on(e, t) {
+        s(0, [e, e.length], 0, t)
     }
 
-    function cn(e, t, n, s, i) {
+    function un(e, t, n, s, i) {
         var r;
-        return null == e ? Ae(this, s, i).year : ((r = je(e, s, i)) < t && (t = r), function(e, t, n, s, i) {
-            var r = Ee(e, t, n, s, i),
-                a = Ve(r.year, 0, r.dayOfYear);
-            return this.year(a.getUTCFullYear()), this.month(a.getUTCMonth()), this.date(a.getUTCDate()), this
-        }.call(this, e, t, n, s, i))
+        return null == e ? Be(this, s, i).year : (r = N(e, s, i), function(e, t, n, s, i) {
+            e = $e(e, t, n, s, i), t = ze(e.year, 0, e.dayOfYear);
+            return this.year(t.getUTCFullYear()), this.month(t.getUTCMonth()), this.date(t.getUTCDate()), this
+        }.call(this, e, t = r < t ? r : t, n, s, i))
     }
-    C("N", 0, 0, "eraAbbr"), C("NN", 0, 0, "eraAbbr"), C("NNN", 0, 0, "eraAbbr"), C("NNNN", 0, 0, "eraName"), C("NNNNN", 0, 0, "eraNarrow"), C("y", ["y", 1], "yo", "eraYear"), C("y", ["yy", 2], 0, "eraYear"), C("y", ["yyy", 3], 0, "eraYear"), C("y", ["yyyy", 4], 0, "eraYear"), ce("N", ln), ce("NN", ln), ce("NNN", ln), ce("NNNN", function(e, t) {
+    s("N", 0, 0, "eraAbbr"), s("NN", 0, 0, "eraAbbr"), s("NNN", 0, 0, "eraAbbr"), s("NNNN", 0, 0, "eraName"), s("NNNNN", 0, 0, "eraNarrow"), s("y", ["y", 1], "yo", "eraYear"), s("y", ["yy", 2], 0, "eraYear"), s("y", ["yyy", 3], 0, "eraYear"), s("y", ["yyyy", 4], 0, "eraYear"), h("N", rn), h("NN", rn), h("NNN", rn), h("NNNN", function(e, t) {
         return t.erasNameRegex(e)
-    }), ce("NNNNN", function(e, t) {
+    }), h("NNNNN", function(e, t) {
         return t.erasNarrowRegex(e)
-    }), ye(["N", "NN", "NNN", "NNNN", "NNNNN"], function(e, t, n, s) {
-        var i = n._locale.erasParse(e, s, n._strict);
-        i ? y(n).era = i : y(n).invalidEra = e
-    }), ce("y", oe), ce("yy", oe), ce("yyy", oe), ce("yyyy", oe), ce("yo", function(e, t) {
-        return t._eraYearOrdinalRegex || oe
-    }), ye(["y", "yy", "yyy", "yyyy"], pe), ye(["yo"], function(e, t, n, s) {
+    }), v(["N", "NN", "NNN", "NNNN", "NNNNN"], function(e, t, n, s) {
+        s = n._locale.erasParse(e, s, n._strict);
+        s ? p(n).era = s : p(n).invalidEra = e
+    }), h("y", pe), h("yy", pe), h("yyy", pe), h("yyyy", pe), h("yo", function(e, t) {
+        return t._eraYearOrdinalRegex || pe
+    }), v(["y", "yy", "yyy", "yyyy"], D), v(["yo"], function(e, t, n, s) {
         var i;
-        n._locale._eraYearOrdinalRegex && (i = e.match(n._locale._eraYearOrdinalRegex)), n._locale.eraYearOrdinalParse ? t[pe] = n._locale.eraYearOrdinalParse(e, i) : t[pe] = parseInt(e, 10)
-    }), C(0, ["gg", 2], 0, function() {
+        n._locale._eraYearOrdinalRegex && (i = e.match(n._locale._eraYearOrdinalRegex)), n._locale.eraYearOrdinalParse ? t[D] = n._locale.eraYearOrdinalParse(e, i) : t[D] = parseInt(e, 10)
+    }), s(0, ["gg", 2], 0, function() {
         return this.weekYear() % 100
-    }), C(0, ["GG", 2], 0, function() {
+    }), s(0, ["GG", 2], 0, function() {
         return this.isoWeekYear() % 100
-    }), dn("gggg", "weekYear"), dn("ggggg", "weekYear"), dn("GGGG", "isoWeekYear"), dn("GGGGG", "isoWeekYear"), L("weekYear", "gg"), L("isoWeekYear", "GG"), A("weekYear", 1), A("isoWeekYear", 1), ce("G", ue), ce("g", ue), ce("GG", te, Q), ce("gg", te, Q), ce("GGGG", re, K), ce("gggg", re, K), ce("GGGGG", ae, ee), ce("ggggg", ae, ee), ge(["gggg", "ggggg", "GGGG", "GGGGG"], function(e, t, n, s) {
-        t[s.substr(0, 2)] = Z(e)
-    }), ge(["gg", "GG"], function(e, t, n, s) {
-        t[s] = f.parseTwoDigitYear(e)
-    }), C("Q", 0, "Qo", "quarter"), L("quarter", "Q"), A("quarter", 7), ce("Q", J), ye("Q", function(e, t) {
-        t[ve] = 3 * (Z(e) - 1)
-    }), C("D", ["DD", 2], "Do", "date"), L("date", "D"), A("date", 9), ce("D", te), ce("DD", te, Q), ce("Do", function(e, t) {
+    }), on("gggg", "weekYear"), on("ggggg", "weekYear"), on("GGGG", "isoWeekYear"), on("GGGGG", "isoWeekYear"), h("G", ke), h("g", ke), h("GG", n, t), h("gg", n, t), h("GGGG", ge, ce), h("gggg", ge, ce), h("GGGGG", we, fe), h("ggggg", we, fe), Oe(["gggg", "ggggg", "GGGG", "GGGGG"], function(e, t, n, s) {
+        t[s.substr(0, 2)] = M(e)
+    }), Oe(["gg", "GG"], function(e, t, n, s) {
+        t[s] = _.parseTwoDigitYear(e)
+    }), s("Q", 0, "Qo", "quarter"), h("Q", de), v("Q", function(e, t) {
+        t[Y] = 3 * (M(e) - 1)
+    }), s("D", ["DD", 2], "Do", "date"), h("D", n, u), h("DD", n, t), h("Do", function(e, t) {
         return e ? t._dayOfMonthOrdinalParse || t._ordinalParse : t._dayOfMonthOrdinalParseLenient
-    }), ye(["D", "DD"], ke), ye("Do", function(e, t) {
-        t[ke] = Z(e.match(te)[0])
+    }), v(["D", "DD"], S), v("Do", function(e, t) {
+        t[S] = M(e.match(n)[0])
     });
-    var fn = z("Date", !0);
-    C("DDD", ["DDDD", 3], "DDDo", "dayOfYear"), L("dayOfYear", "DDD"), A("dayOfYear", 4), ce("DDD", ie), ce("DDDD", X), ye(["DDD", "DDDD"], function(e, t, n) {
-        n._dayOfYear = Z(e)
-    }), C("m", ["mm", 2], 0, "minute"), L("minute", "m"), A("minute", 14), ce("m", te), ce("mm", te, Q), ye(["m", "mm"], De);
-    var mn = z("Minutes", !1);
-    C("s", ["ss", 2], 0, "second"), L("second", "s"), A("second", 15), ce("s", te), ce("ss", te, Q), ye(["s", "ss"], Se);
-    var _n, yn, gn = z("Seconds", !1);
-    for (C("S", 0, 0, function() {
+    ge = Re("Date", !0);
+    s("DDD", ["DDDD", 3], "DDDo", "dayOfYear"), h("DDD", ye), h("DDDD", he), v(["DDD", "DDDD"], function(e, t, n) {
+        n._dayOfYear = M(e)
+    }), s("m", ["mm", 2], 0, "minute"), h("m", n, d), h("mm", n, t), v(["m", "mm"], b);
+    var ln, ce = Re("Minutes", !1),
+        we = (s("s", ["ss", 2], 0, "second"), h("s", n, d), h("ss", n, t), v(["s", "ss"], T), Re("Seconds", !1));
+    for (s("S", 0, 0, function() {
             return ~~(this.millisecond() / 100)
-        }), C(0, ["SS", 2], 0, function() {
+        }), s(0, ["SS", 2], 0, function() {
             return ~~(this.millisecond() / 10)
-        }), C(0, ["SSS", 3], 0, "millisecond"), C(0, ["SSSS", 4], 0, function() {
+        }), s(0, ["SSS", 3], 0, "millisecond"), s(0, ["SSSS", 4], 0, function() {
             return 10 * this.millisecond()
-        }), C(0, ["SSSSS", 5], 0, function() {
+        }), s(0, ["SSSSS", 5], 0, function() {
             return 100 * this.millisecond()
-        }), C(0, ["SSSSSS", 6], 0, function() {
+        }), s(0, ["SSSSSS", 6], 0, function() {
             return 1e3 * this.millisecond()
-        }), C(0, ["SSSSSSS", 7], 0, function() {
+        }), s(0, ["SSSSSSS", 7], 0, function() {
             return 1e4 * this.millisecond()
-        }), C(0, ["SSSSSSSS", 8], 0, function() {
+        }), s(0, ["SSSSSSSS", 8], 0, function() {
             return 1e5 * this.millisecond()
-        }), C(0, ["SSSSSSSSS", 9], 0, function() {
+        }), s(0, ["SSSSSSSSS", 9], 0, function() {
             return 1e6 * this.millisecond()
-        }), L("millisecond", "ms"), A("millisecond", 16), ce("S", ie, J), ce("SS", ie, Q), ce("SSS", ie, X), _n = "SSSS"; _n.length <= 9; _n += "S") ce(_n, oe);
+        }), h("S", ye, de), h("SS", ye, t), h("SSS", ye, he), ln = "SSSS"; ln.length <= 9; ln += "S") h(ln, pe);
 
-    function wn(e, t) {
-        t[Ye] = Z(1e3 * ("0." + e))
+    function dn(e, t) {
+        t[Te] = M(1e3 * ("0." + e))
     }
-    for (_n = "S"; _n.length <= 9; _n += "S") ye(_n, wn);
-    yn = z("Milliseconds", !1), C("z", 0, 0, "zoneAbbr"), C("zz", 0, 0, "zoneName");
-    var pn = k.prototype;
+    for (ln = "S"; ln.length <= 9; ln += "S") v(ln, dn);
+    fe = Re("Milliseconds", !1), s("z", 0, 0, "zoneAbbr"), s("zz", 0, 0, "zoneName");
+    u = $.prototype;
 
-    function vn(e) {
+    function hn(e) {
         return e
     }
-    pn.add = Jt, pn.calendar = function(e, t) {
-        1 === arguments.length && (arguments[0] ? Kt(arguments[0]) ? (e = arguments[0], t = void 0) : function(e) {
-            for (var t = u(e) && !l(e), n = !1, s = ["sameDay", "nextDay", "lastDay", "nextWeek", "lastWeek", "sameElse"], i = 0; i < s.length; i += 1) n = n || m(e, s[i]);
+    u.add = Fe, u.calendar = function(e, t) {
+        1 === arguments.length && (arguments[0] ? Jt(arguments[0]) ? (e = arguments[0], t = void 0) : function(e) {
+            for (var t = F(e) && !L(e), n = !1, s = ["sameDay", "nextDay", "lastDay", "nextWeek", "lastWeek", "sameElse"], i = 0; i < s.length; i += 1) n = n || c(e, s[i]);
             return t && n
         }(arguments[0]) && (t = arguments[0], e = void 0) : t = e = void 0);
-        var n = e || Tt(),
-            s = Gt(n, this).startOf("day"),
-            i = f.calendarFormat(this, s) || "sameElse",
-            r = t && (O(t[i]) ? t[i].call(this, n) : t[i]);
-        return this.format(r || this.localeData().calendar(i, this, Tt(n)))
-    }, pn.clone = function() {
-        return new k(this)
-    }, pn.diff = function(e, t, n) {
+        var e = e || R(),
+            n = Gt(e, this).startOf("day"),
+            n = _.calendarFormat(this, n) || "sameElse",
+            t = t && (a(t[n]) ? t[n].call(this, e) : t[n]);
+        return this.format(t || this.localeData().calendar(n, this, R(e)))
+    }, u.clone = function() {
+        return new $(this)
+    }, u.diff = function(e, t, n) {
         var s, i, r;
         if (!this.isValid()) return NaN;
         if (!(s = Gt(e, this)).isValid()) return NaN;
-        switch (i = 6e4 * (s.utcOffset() - this.utcOffset()), t = V(t)) {
+        switch (i = 6e4 * (s.utcOffset() - this.utcOffset()), t = o(t)) {
             case "year":
-                r = en(this, s) / 12;
+                r = Qt(this, s) / 12;
                 break;
             case "month":
-                r = en(this, s);
+                r = Qt(this, s);
                 break;
             case "quarter":
-                r = en(this, s) / 3;
+                r = Qt(this, s) / 3;
                 break;
             case "second":
                 r = (this - s) / 1e3;
                 break;
             case "minute":
                 r = (this - s) / 6e4;
                 break;
@@ -1100,349 +1184,336 @@
                 break;
             case "week":
                 r = (this - s - i) / 6048e5;
                 break;
             default:
                 r = this - s
         }
-        return n ? r : I(r)
-    }, pn.endOf = function(e) {
+        return n ? r : m(r)
+    }, u.endOf = function(e) {
         var t, n;
-        if (void 0 === (e = V(e)) || "millisecond" === e || !this.isValid()) return this;
-        switch (n = this._isUTC ? un : on, e) {
-            case "year":
-                t = n(this.year() + 1, 0, 1) - 1;
-                break;
-            case "quarter":
-                t = n(this.year(), this.month() - this.month() % 3 + 3, 1) - 1;
-                break;
-            case "month":
-                t = n(this.year(), this.month() + 1, 1) - 1;
-                break;
-            case "week":
-                t = n(this.year(), this.month(), this.date() - this.weekday() + 7) - 1;
-                break;
-            case "isoWeek":
-                t = n(this.year(), this.month(), this.date() - (this.isoWeekday() - 1) + 7) - 1;
-                break;
-            case "day":
-            case "date":
-                t = n(this.year(), this.month(), this.date() + 1) - 1;
-                break;
-            case "hour":
-                t = this._d.valueOf(), t += 36e5 - an(t + (this._isUTC ? 0 : 6e4 * this.utcOffset()), 36e5) - 1;
-                break;
-            case "minute":
-                t = this._d.valueOf(), t += 6e4 - an(t, 6e4) - 1;
-                break;
-            case "second":
-                t = this._d.valueOf(), t += 1e3 - an(t, 1e3) - 1;
-                break
+        if (void 0 !== (e = o(e)) && "millisecond" !== e && this.isValid()) {
+            switch (n = this._isUTC ? sn : nn, e) {
+                case "year":
+                    t = n(this.year() + 1, 0, 1) - 1;
+                    break;
+                case "quarter":
+                    t = n(this.year(), this.month() - this.month() % 3 + 3, 1) - 1;
+                    break;
+                case "month":
+                    t = n(this.year(), this.month() + 1, 1) - 1;
+                    break;
+                case "week":
+                    t = n(this.year(), this.month(), this.date() - this.weekday() + 7) - 1;
+                    break;
+                case "isoWeek":
+                    t = n(this.year(), this.month(), this.date() - (this.isoWeekday() - 1) + 7) - 1;
+                    break;
+                case "day":
+                case "date":
+                    t = n(this.year(), this.month(), this.date() + 1) - 1;
+                    break;
+                case "hour":
+                    t = this._d.valueOf(), t += 36e5 - tn(t + (this._isUTC ? 0 : 6e4 * this.utcOffset()), 36e5) - 1;
+                    break;
+                case "minute":
+                    t = this._d.valueOf(), t += 6e4 - tn(t, 6e4) - 1;
+                    break;
+                case "second":
+                    t = this._d.valueOf(), t += 1e3 - tn(t, 1e3) - 1;
+                    break
+            }
+            this._d.setTime(t), _.updateOffset(this, !0)
         }
-        return this._d.setTime(t), f.updateOffset(this, !0), this
-    }, pn.format = function(e) {
-        e = e || (this.isUtc() ? f.defaultFormatUtc : f.defaultFormat);
-        var t = U(this, e);
-        return this.localeData().postformat(t)
-    }, pn.from = function(e, t) {
-        return this.isValid() && (M(e) && e.isValid() || Tt(e).isValid()) ? Zt({
+        return this
+    }, u.format = function(e) {
+        return e = e || (this.isUtc() ? _.defaultFormatUtc : _.defaultFormat), e = re(this, e), this.localeData().postformat(e)
+    }, u.from = function(e, t) {
+        return this.isValid() && (k(e) && e.isValid() || R(e).isValid()) ? C({
             to: this,
             from: e
         }).locale(this.locale()).humanize(!t) : this.localeData().invalidDate()
-    }, pn.fromNow = function(e) {
-        return this.from(Tt(), e)
-    }, pn.to = function(e, t) {
-        return this.isValid() && (M(e) && e.isValid() || Tt(e).isValid()) ? Zt({
+    }, u.fromNow = function(e) {
+        return this.from(R(), e)
+    }, u.to = function(e, t) {
+        return this.isValid() && (k(e) && e.isValid() || R(e).isValid()) ? C({
             from: this,
             to: e
         }).locale(this.locale()).humanize(!t) : this.localeData().invalidDate()
-    }, pn.toNow = function(e) {
-        return this.to(Tt(), e)
-    }, pn.get = function(e) {
-        return O(this[e = V(e)]) ? this[e]() : this
-    }, pn.invalidAt = function() {
-        return y(this).overflow
-    }, pn.isAfter = function(e, t) {
-        var n = M(e) ? e : Tt(e);
-        return !(!this.isValid() || !n.isValid()) && ("millisecond" === (t = V(t) || "millisecond") ? this.valueOf() > n.valueOf() : n.valueOf() < this.clone().startOf(t).valueOf())
-    }, pn.isBefore = function(e, t) {
-        var n = M(e) ? e : Tt(e);
-        return !(!this.isValid() || !n.isValid()) && ("millisecond" === (t = V(t) || "millisecond") ? this.valueOf() < n.valueOf() : this.clone().endOf(t).valueOf() < n.valueOf())
-    }, pn.isBetween = function(e, t, n, s) {
-        var i = M(e) ? e : Tt(e),
-            r = M(t) ? t : Tt(t);
-        return !!(this.isValid() && i.isValid() && r.isValid()) && (("(" === (s = s || "()")[0] ? this.isAfter(i, n) : !this.isBefore(i, n)) && (")" === s[1] ? this.isBefore(r, n) : !this.isAfter(r, n)))
-    }, pn.isSame = function(e, t) {
-        var n, s = M(e) ? e : Tt(e);
-        return !(!this.isValid() || !s.isValid()) && ("millisecond" === (t = V(t) || "millisecond") ? this.valueOf() === s.valueOf() : (n = s.valueOf(), this.clone().startOf(t).valueOf() <= n && n <= this.clone().endOf(t).valueOf()))
-    }, pn.isSameOrAfter = function(e, t) {
+    }, u.toNow = function(e) {
+        return this.to(R(), e)
+    }, u.get = function(e) {
+        return a(this[e = o(e)]) ? this[e]() : this
+    }, u.invalidAt = function() {
+        return p(this).overflow
+    }, u.isAfter = function(e, t) {
+        return e = k(e) ? e : R(e), !(!this.isValid() || !e.isValid()) && ("millisecond" === (t = o(t) || "millisecond") ? this.valueOf() > e.valueOf() : e.valueOf() < this.clone().startOf(t).valueOf())
+    }, u.isBefore = function(e, t) {
+        return e = k(e) ? e : R(e), !(!this.isValid() || !e.isValid()) && ("millisecond" === (t = o(t) || "millisecond") ? this.valueOf() < e.valueOf() : this.clone().endOf(t).valueOf() < e.valueOf())
+    }, u.isBetween = function(e, t, n, s) {
+        return e = k(e) ? e : R(e), t = k(t) ? t : R(t), !!(this.isValid() && e.isValid() && t.isValid()) && ("(" === (s = s || "()")[0] ? this.isAfter(e, n) : !this.isBefore(e, n)) && (")" === s[1] ? this.isBefore(t, n) : !this.isAfter(t, n))
+    }, u.isSame = function(e, t) {
+        var e = k(e) ? e : R(e);
+        return !(!this.isValid() || !e.isValid()) && ("millisecond" === (t = o(t) || "millisecond") ? this.valueOf() === e.valueOf() : (e = e.valueOf(), this.clone().startOf(t).valueOf() <= e && e <= this.clone().endOf(t).valueOf()))
+    }, u.isSameOrAfter = function(e, t) {
         return this.isSame(e, t) || this.isAfter(e, t)
-    }, pn.isSameOrBefore = function(e, t) {
+    }, u.isSameOrBefore = function(e, t) {
         return this.isSame(e, t) || this.isBefore(e, t)
-    }, pn.isValid = function() {
-        return g(this)
-    }, pn.lang = nn, pn.locale = tn, pn.localeData = sn, pn.max = Pt, pn.min = Nt, pn.parsingFlags = function() {
-        return c({}, y(this))
-    }, pn.set = function(e, t) {
+    }, u.isValid = function() {
+        return A(this)
+    }, u.lang = Ke, u.locale = Xt, u.localeData = Kt, u.max = _e, u.min = me, u.parsingFlags = function() {
+        return E({}, p(this))
+    }, u.set = function(e, t) {
         if ("object" == typeof e)
             for (var n = function(e) {
                     var t, n = [];
-                    for (t in e) m(e, t) && n.push({
+                    for (t in e) c(e, t) && n.push({
                         unit: t,
-                        priority: E[t]
+                        priority: le[t]
                     });
                     return n.sort(function(e, t) {
                         return e.priority - t.priority
                     }), n
-                }(e = G(e)), s = 0; s < n.length; s++) this[n[s].unit](e[n[s].unit]);
-        else if (O(this[e = V(e)])) return this[e](t);
+                }(e = ue(e)), s = n.length, i = 0; i < s; i++) this[n[i].unit](e[n[i].unit]);
+        else if (a(this[e = o(e)])) return this[e](t);
         return this
-    }, pn.startOf = function(e) {
+    }, u.startOf = function(e) {
         var t, n;
-        if (void 0 === (e = V(e)) || "millisecond" === e || !this.isValid()) return this;
-        switch (n = this._isUTC ? un : on, e) {
-            case "year":
-                t = n(this.year(), 0, 1);
-                break;
-            case "quarter":
-                t = n(this.year(), this.month() - this.month() % 3, 1);
-                break;
-            case "month":
-                t = n(this.year(), this.month(), 1);
-                break;
-            case "week":
-                t = n(this.year(), this.month(), this.date() - this.weekday());
-                break;
-            case "isoWeek":
-                t = n(this.year(), this.month(), this.date() - (this.isoWeekday() - 1));
-                break;
-            case "day":
-            case "date":
-                t = n(this.year(), this.month(), this.date());
-                break;
-            case "hour":
-                t = this._d.valueOf(), t -= an(t + (this._isUTC ? 0 : 6e4 * this.utcOffset()), 36e5);
-                break;
-            case "minute":
-                t = this._d.valueOf(), t -= an(t, 6e4);
-                break;
-            case "second":
-                t = this._d.valueOf(), t -= an(t, 1e3);
-                break
+        if (void 0 !== (e = o(e)) && "millisecond" !== e && this.isValid()) {
+            switch (n = this._isUTC ? sn : nn, e) {
+                case "year":
+                    t = n(this.year(), 0, 1);
+                    break;
+                case "quarter":
+                    t = n(this.year(), this.month() - this.month() % 3, 1);
+                    break;
+                case "month":
+                    t = n(this.year(), this.month(), 1);
+                    break;
+                case "week":
+                    t = n(this.year(), this.month(), this.date() - this.weekday());
+                    break;
+                case "isoWeek":
+                    t = n(this.year(), this.month(), this.date() - (this.isoWeekday() - 1));
+                    break;
+                case "day":
+                case "date":
+                    t = n(this.year(), this.month(), this.date());
+                    break;
+                case "hour":
+                    t = this._d.valueOf(), t -= tn(t + (this._isUTC ? 0 : 6e4 * this.utcOffset()), 36e5);
+                    break;
+                case "minute":
+                    t = this._d.valueOf(), t -= tn(t, 6e4);
+                    break;
+                case "second":
+                    t = this._d.valueOf(), t -= tn(t, 1e3);
+                    break
+            }
+            this._d.setTime(t), _.updateOffset(this, !0)
         }
-        return this._d.setTime(t), f.updateOffset(this, !0), this
-    }, pn.subtract = Qt, pn.toArray = function() {
+        return this
+    }, u.subtract = Qe, u.toArray = function() {
         var e = this;
         return [e.year(), e.month(), e.date(), e.hour(), e.minute(), e.second(), e.millisecond()]
-    }, pn.toObject = function() {
+    }, u.toObject = function() {
         var e = this;
         return {
             years: e.year(),
             months: e.month(),
             date: e.date(),
             hours: e.hours(),
             minutes: e.minutes(),
             seconds: e.seconds(),
             milliseconds: e.milliseconds()
         }
-    }, pn.toDate = function() {
+    }, u.toDate = function() {
         return new Date(this.valueOf())
-    }, pn.toISOString = function(e) {
-        if (!this.isValid()) return null;
-        var t = !0 !== e,
-            n = t ? this.clone().utc() : this;
-        return n.year() < 0 || 9999 < n.year() ? U(n, t ? "YYYYYY-MM-DD[T]HH:mm:ss.SSS[Z]" : "YYYYYY-MM-DD[T]HH:mm:ss.SSSZ") : O(Date.prototype.toISOString) ? t ? this.toDate().toISOString() : new Date(this.valueOf() + 60 * this.utcOffset() * 1e3).toISOString().replace("Z", U(n, "Z")) : U(n, t ? "YYYY-MM-DD[T]HH:mm:ss.SSS[Z]" : "YYYY-MM-DD[T]HH:mm:ss.SSSZ")
-    }, pn.inspect = function() {
-        if (!this.isValid()) return "moment.invalid(/* " + this._i + " */)";
-        var e, t, n, s = "moment",
-            i = "";
-        return this.isLocal() || (s = 0 === this.utcOffset() ? "moment.utc" : "moment.parseZone", i = "Z"), e = "[" + s + '("]', t = 0 <= this.year() && this.year() <= 9999 ? "YYYY" : "YYYYYY", n = i + '[")]', this.format(e + t + "-MM-DD[T]HH:mm:ss.SSS" + n)
-    }, "undefined" != typeof Symbol && null != Symbol.for && (pn[Symbol.for("nodejs.util.inspect.custom")] = function() {
+    }, u.toISOString = function(e) {
+        var t;
+        return this.isValid() ? (t = (e = !0 !== e) ? this.clone().utc() : this).year() < 0 || 9999 < t.year() ? re(t, e ? "YYYYYY-MM-DD[T]HH:mm:ss.SSS[Z]" : "YYYYYY-MM-DD[T]HH:mm:ss.SSSZ") : a(Date.prototype.toISOString) ? e ? this.toDate().toISOString() : new Date(this.valueOf() + 60 * this.utcOffset() * 1e3).toISOString().replace("Z", re(t, "Z")) : re(t, e ? "YYYY-MM-DD[T]HH:mm:ss.SSS[Z]" : "YYYY-MM-DD[T]HH:mm:ss.SSSZ") : null
+    }, u.inspect = function() {
+        var e, t, n;
+        return this.isValid() ? (t = "moment", e = "", this.isLocal() || (t = 0 === this.utcOffset() ? "moment.utc" : "moment.parseZone", e = "Z"), t = "[" + t + '("]', n = 0 <= this.year() && this.year() <= 9999 ? "YYYY" : "YYYYYY", this.format(t + n + "-MM-DD[T]HH:mm:ss.SSS" + (e + '[")]'))) : "moment.invalid(/* " + this._i + " */)"
+    }, "undefined" != typeof Symbol && null != Symbol.for && (u[Symbol.for("nodejs.util.inspect.custom")] = function() {
         return "Moment<" + this.format() + ">"
-    }), pn.toJSON = function() {
+    }), u.toJSON = function() {
         return this.isValid() ? this.toISOString() : null
-    }, pn.toString = function() {
+    }, u.toString = function() {
         return this.clone().locale("en").format("ddd MMM DD YYYY HH:mm:ss [GMT]ZZ")
-    }, pn.unix = function() {
+    }, u.unix = function() {
         return Math.floor(this.valueOf() / 1e3)
-    }, pn.valueOf = function() {
+    }, u.valueOf = function() {
         return this._d.valueOf() - 6e4 * (this._offset || 0)
-    }, pn.creationData = function() {
+    }, u.creationData = function() {
         return {
             input: this._i,
             format: this._f,
             locale: this._locale,
             isUTC: this._isUTC,
             strict: this._strict
         }
-    }, pn.eraName = function() {
+    }, u.eraName = function() {
         for (var e, t = this.localeData().eras(), n = 0, s = t.length; n < s; ++n) {
             if (e = this.clone().startOf("day").valueOf(), t[n].since <= e && e <= t[n].until) return t[n].name;
             if (t[n].until <= e && e <= t[n].since) return t[n].name
         }
         return ""
-    }, pn.eraNarrow = function() {
+    }, u.eraNarrow = function() {
         for (var e, t = this.localeData().eras(), n = 0, s = t.length; n < s; ++n) {
             if (e = this.clone().startOf("day").valueOf(), t[n].since <= e && e <= t[n].until) return t[n].narrow;
             if (t[n].until <= e && e <= t[n].since) return t[n].narrow
         }
         return ""
-    }, pn.eraAbbr = function() {
+    }, u.eraAbbr = function() {
         for (var e, t = this.localeData().eras(), n = 0, s = t.length; n < s; ++n) {
             if (e = this.clone().startOf("day").valueOf(), t[n].since <= e && e <= t[n].until) return t[n].abbr;
             if (t[n].until <= e && e <= t[n].since) return t[n].abbr
         }
         return ""
-    }, pn.eraYear = function() {
+    }, u.eraYear = function() {
         for (var e, t, n = this.localeData().eras(), s = 0, i = n.length; s < i; ++s)
-            if (e = n[s].since <= n[s].until ? 1 : -1, t = this.clone().startOf("day").valueOf(), n[s].since <= t && t <= n[s].until || n[s].until <= t && t <= n[s].since) return (this.year() - f(n[s].since).year()) * e + n[s].offset;
+            if (e = n[s].since <= n[s].until ? 1 : -1, t = this.clone().startOf("day").valueOf(), n[s].since <= t && t <= n[s].until || n[s].until <= t && t <= n[s].since) return (this.year() - _(n[s].since).year()) * e + n[s].offset;
         return this.year()
-    }, pn.year = Le, pn.isLeapYear = function() {
-        return j(this.year())
-    }, pn.weekYear = function(e) {
-        return cn.call(this, e, this.week(), this.weekday(), this.localeData()._week.dow, this.localeData()._week.doy)
-    }, pn.isoWeekYear = function(e) {
-        return cn.call(this, e, this.isoWeek(), this.isoWeekday(), 1, 4)
-    }, pn.quarter = pn.quarters = function(e) {
+    }, u.year = Pe, u.isLeapYear = function() {
+        return be(this.year())
+    }, u.weekYear = function(e) {
+        return un.call(this, e, this.week(), this.weekday() + this.localeData()._week.dow, this.localeData()._week.dow, this.localeData()._week.doy)
+    }, u.isoWeekYear = function(e) {
+        return un.call(this, e, this.isoWeek(), this.isoWeekday(), 1, 4)
+    }, u.quarter = u.quarters = function(e) {
         return null == e ? Math.ceil((this.month() + 1) / 3) : this.month(3 * (e - 1) + this.month() % 3)
-    }, pn.month = Ue, pn.daysInMonth = function() {
-        return xe(this.year(), this.month())
-    }, pn.week = pn.weeks = function(e) {
+    }, u.month = Ie, u.daysInMonth = function() {
+        return He(this.year(), this.month())
+    }, u.week = u.weeks = function(e) {
         var t = this.localeData().week(this);
         return null == e ? t : this.add(7 * (e - t), "d")
-    }, pn.isoWeek = pn.isoWeeks = function(e) {
-        var t = Ae(this, 1, 4).week;
+    }, u.isoWeek = u.isoWeeks = function(e) {
+        var t = Be(this, 1, 4).week;
         return null == e ? t : this.add(7 * (e - t), "d")
-    }, pn.weeksInYear = function() {
+    }, u.weeksInYear = function() {
         var e = this.localeData()._week;
-        return je(this.year(), e.dow, e.doy)
-    }, pn.weeksInWeekYear = function() {
+        return N(this.year(), e.dow, e.doy)
+    }, u.weeksInWeekYear = function() {
         var e = this.localeData()._week;
-        return je(this.weekYear(), e.dow, e.doy)
-    }, pn.isoWeeksInYear = function() {
-        return je(this.year(), 1, 4)
-    }, pn.isoWeeksInISOWeekYear = function() {
-        return je(this.isoWeekYear(), 1, 4)
-    }, pn.date = fn, pn.day = pn.days = function(e) {
-        if (!this.isValid()) return null != e ? this : NaN;
-        var t, n, s = this._isUTC ? this._d.getUTCDay() : this._d.getDay();
-        return null != e ? (t = e, n = this.localeData(), e = "string" != typeof t ? t : isNaN(t) ? "number" == typeof(t = n.weekdaysParse(t)) ? t : null : parseInt(t, 10), this.add(e - s, "d")) : s
-    }, pn.weekday = function(e) {
-        if (!this.isValid()) return null != e ? this : NaN;
-        var t = (this.day() + 7 - this.localeData()._week.dow) % 7;
-        return null == e ? t : this.add(e - t, "d")
-    }, pn.isoWeekday = function(e) {
-        if (!this.isValid()) return null != e ? this : NaN;
-        if (null == e) return this.day() || 7;
-        var t, n, s = (t = e, n = this.localeData(), "string" == typeof t ? n.weekdaysParse(t) % 7 || 7 : isNaN(t) ? null : t);
-        return this.day(this.day() % 7 ? s : s - 7)
-    }, pn.dayOfYear = function(e) {
+        return N(this.weekYear(), e.dow, e.doy)
+    }, u.isoWeeksInYear = function() {
+        return N(this.year(), 1, 4)
+    }, u.isoWeeksInISOWeekYear = function() {
+        return N(this.isoWeekYear(), 1, 4)
+    }, u.date = ge, u.day = u.days = function(e) {
+        var t, n, s;
+        return this.isValid() ? (t = Ce(this, "Day"), null != e ? (n = e, s = this.localeData(), e = "string" != typeof n ? n : isNaN(n) ? "number" == typeof(n = s.weekdaysParse(n)) ? n : null : parseInt(n, 10), this.add(e - t, "d")) : t) : null != e ? this : NaN
+    }, u.weekday = function(e) {
+        var t;
+        return this.isValid() ? (t = (this.day() + 7 - this.localeData()._week.dow) % 7, null == e ? t : this.add(e - t, "d")) : null != e ? this : NaN
+    }, u.isoWeekday = function(e) {
+        var t, n;
+        return this.isValid() ? null != e ? (t = e, n = this.localeData(), n = "string" == typeof t ? n.weekdaysParse(t) % 7 || 7 : isNaN(t) ? null : t, this.day(this.day() % 7 ? n : n - 7)) : this.day() || 7 : null != e ? this : NaN
+    }, u.dayOfYear = function(e) {
         var t = Math.round((this.clone().startOf("day") - this.clone().startOf("year")) / 864e5) + 1;
         return null == e ? t : this.add(e - t, "d")
-    }, pn.hour = pn.hours = tt, pn.minute = pn.minutes = mn, pn.second = pn.seconds = gn, pn.millisecond = pn.milliseconds = yn, pn.utcOffset = function(e, t, n) {
+    }, u.hour = u.hours = i, u.minute = u.minutes = ce, u.second = u.seconds = we, u.millisecond = u.milliseconds = fe, u.utcOffset = function(e, t, n) {
         var s, i = this._offset || 0;
         if (!this.isValid()) return null != e ? this : NaN;
         if (null == e) return this._isUTC ? i : Et(this);
         if ("string" == typeof e) {
-            if (null === (e = Vt(he, e))) return this
+            if (null === (e = Vt(ve, e))) return this
         } else Math.abs(e) < 16 && !n && (e *= 60);
-        return !this._isUTC && t && (s = Et(this)), this._offset = e, this._isUTC = !0, null != s && this.add(s, "m"), i !== e && (!t || this._changeInProgress ? Bt(this, Zt(e - i, "m"), 1, !1) : this._changeInProgress || (this._changeInProgress = !0, f.updateOffset(this, !0), this._changeInProgress = null)), this
-    }, pn.utc = function(e) {
+        return !this._isUTC && t && (s = Et(this)), this._offset = e, this._isUTC = !0, null != s && this.add(s, "m"), i !== e && (!t || this._changeInProgress ? $t(this, C(e - i, "m"), 1, !1) : this._changeInProgress || (this._changeInProgress = !0, _.updateOffset(this, !0), this._changeInProgress = null)), this
+    }, u.utc = function(e) {
         return this.utcOffset(0, e)
-    }, pn.local = function(e) {
-        return this._isUTC && (this.utcOffset(0, e), this._isUTC = !1, e && this.subtract(Et(this), "m")), this
-    }, pn.parseZone = function() {
+    }, u.local = function(e) {
+        return this._isUTC && (this.utcOffset(0, e), this._isUTC = !1, e) && this.subtract(Et(this), "m"), this
+    }, u.parseZone = function() {
         var e;
-        return null != this._tzm ? this.utcOffset(this._tzm, !1, !0) : "string" == typeof this._i && (null != (e = Vt(le, this._i)) ? this.utcOffset(e) : this.utcOffset(0, !0)), this
-    }, pn.hasAlignedHourOffset = function(e) {
-        return !!this.isValid() && (e = e ? Tt(e).utcOffset() : 0, (this.utcOffset() - e) % 60 == 0)
-    }, pn.isDST = function() {
+        return null != this._tzm ? this.utcOffset(this._tzm, !1, !0) : "string" == typeof this._i && (null != (e = Vt(Me, this._i)) ? this.utcOffset(e) : this.utcOffset(0, !0)), this
+    }, u.hasAlignedHourOffset = function(e) {
+        return !!this.isValid() && (e = e ? R(e).utcOffset() : 0, (this.utcOffset() - e) % 60 == 0)
+    }, u.isDST = function() {
         return this.utcOffset() > this.clone().month(0).utcOffset() || this.utcOffset() > this.clone().month(5).utcOffset()
-    }, pn.isLocal = function() {
+    }, u.isLocal = function() {
         return !!this.isValid() && !this._isUTC
-    }, pn.isUtcOffset = function() {
+    }, u.isUtcOffset = function() {
         return !!this.isValid() && this._isUTC
-    }, pn.isUtc = At, pn.isUTC = At, pn.zoneAbbr = function() {
+    }, u.isUtc = At, u.isUTC = At, u.zoneAbbr = function() {
         return this._isUTC ? "UTC" : ""
-    }, pn.zoneName = function() {
+    }, u.zoneName = function() {
         return this._isUTC ? "Coordinated Universal Time" : ""
-    }, pn.dates = n("dates accessor is deprecated. Use date instead.", fn), pn.months = n("months accessor is deprecated. Use month instead", Ue), pn.years = n("years accessor is deprecated. Use year instead", Le), pn.zone = n("moment().zone is deprecated, use moment().utcOffset instead. http://momentjs.com/guides/#/warnings/zone/", function(e, t) {
-        return null != e ? ("string" != typeof e && (e = -e), this.utcOffset(e, t), this) : -this.utcOffset()
-    }), pn.isDSTShifted = n("isDSTShifted is deprecated. See http://momentjs.com/guides/#/warnings/dst-shifted/ for more information", function() {
-        if (!r(this._isDSTShifted)) return this._isDSTShifted;
-        var e, t = {};
-        return v(t, this), (t = bt(t))._a ? (e = (t._isUTC ? _ : Tt)(t._a), this._isDSTShifted = this.isValid() && 0 < function(e, t, n) {
-            for (var s = Math.min(e.length, t.length), i = Math.abs(e.length - t.length), r = 0, a = 0; a < s; a++)(n && e[a] !== t[a] || !n && Z(e[a]) !== Z(t[a])) && r++;
+    }, u.dates = e("dates accessor is deprecated. Use date instead.", ge), u.months = e("months accessor is deprecated. Use month instead", Ie), u.years = e("years accessor is deprecated. Use year instead", Pe), u.zone = e("moment().zone is deprecated, use moment().utcOffset instead. http://momentjs.com/guides/#/warnings/zone/", function(e, t) {
+        return null != e ? (this.utcOffset(e = "string" != typeof e ? -e : e, t), this) : -this.utcOffset()
+    }), u.isDSTShifted = e("isDSTShifted is deprecated. See http://momentjs.com/guides/#/warnings/dst-shifted/ for more information", function() {
+        var e, t;
+        return g(this._isDSTShifted) && (q(e = {}, this), (e = Nt(e))._a ? (t = (e._isUTC ? l : R)(e._a), this._isDSTShifted = this.isValid() && 0 < function(e, t, n) {
+            for (var s = Math.min(e.length, t.length), i = Math.abs(e.length - t.length), r = 0, a = 0; a < s; a++)(n && e[a] !== t[a] || !n && M(e[a]) !== M(t[a])) && r++;
             return r + i
-        }(t._a, e.toArray())) : this._isDSTShifted = !1, this._isDSTShifted
+        }(e._a, t.toArray())) : this._isDSTShifted = !1), this._isDSTShifted
     });
-    var kn = x.prototype;
+    d = K.prototype;
 
-    function Mn(e, t, n, s) {
-        var i = dt(),
-            r = _().set(s, t);
-        return i[n](r, e)
+    function cn(e, t, n, s) {
+        var i = P(),
+            s = l().set(s, t);
+        return i[n](s, e)
     }
 
-    function Dn(e, t, n) {
-        if (h(e) && (t = e, e = void 0), e = e || "", null != t) return Mn(e, t, n, "month");
-        for (var s = [], i = 0; i < 12; i++) s[i] = Mn(e, i, n, "month");
+    function fn(e, t, n) {
+        if (w(e) && (t = e, e = void 0), e = e || "", null != t) return cn(e, t, n, "month");
+        for (var s = [], i = 0; i < 12; i++) s[i] = cn(e, i, n, "month");
         return s
     }
 
-    function Sn(e, t, n, s) {
-        t = ("boolean" == typeof e ? h(t) && (n = t, t = void 0) : (t = e, e = !1, h(n = t) && (n = t, t = void 0)), t || "");
-        var i, r = dt(),
+    function mn(e, t, n, s) {
+        t = ("boolean" == typeof e ? w(t) && (n = t, t = void 0) : (t = e, e = !1, w(n = t) && (n = t, t = void 0)), t || "");
+        var i, r = P(),
             a = e ? r._week.dow : 0,
             o = [];
-        if (null != n) return Mn(t, (n + a) % 7, s, "day");
-        for (i = 0; i < 7; i++) o[i] = Mn(t, (i + a) % 7, s, "day");
+        if (null != n) return cn(t, (n + a) % 7, s, "day");
+        for (i = 0; i < 7; i++) o[i] = cn(t, (i + a) % 7, s, "day");
         return o
     }
-    kn.calendar = function(e, t, n) {
-        var s = this._calendar[e] || this._calendar.sameElse;
-        return O(s) ? s.call(t, n) : s
-    }, kn.longDateFormat = function(e) {
+    d.calendar = function(e, t, n) {
+        return a(e = this._calendar[e] || this._calendar.sameElse) ? e.call(t, n) : e
+    }, d.longDateFormat = function(e) {
         var t = this._longDateFormat[e],
             n = this._longDateFormat[e.toUpperCase()];
-        return t || !n ? t : (this._longDateFormat[e] = n.match(N).map(function(e) {
+        return t || !n ? t : (this._longDateFormat[e] = n.match(te).map(function(e) {
             return "MMMM" === e || "MM" === e || "DD" === e || "dddd" === e ? e.slice(1) : e
         }).join(""), this._longDateFormat[e])
-    }, kn.invalidDate = function() {
+    }, d.invalidDate = function() {
         return this._invalidDate
-    }, kn.ordinal = function(e) {
+    }, d.ordinal = function(e) {
         return this._ordinal.replace("%d", e)
-    }, kn.preparse = vn, kn.postformat = vn, kn.relativeTime = function(e, t, n, s) {
+    }, d.preparse = hn, d.postformat = hn, d.relativeTime = function(e, t, n, s) {
         var i = this._relativeTime[n];
-        return O(i) ? i(e, t, n, s) : i.replace(/%d/i, e)
-    }, kn.pastFuture = function(e, t) {
-        var n = this._relativeTime[0 < e ? "future" : "past"];
-        return O(n) ? n(t) : n.replace(/%s/i, t)
-    }, kn.set = function(e) {
+        return a(i) ? i(e, t, n, s) : i.replace(/%d/i, e)
+    }, d.pastFuture = function(e, t) {
+        return a(e = this._relativeTime[0 < e ? "future" : "past"]) ? e(t) : e.replace(/%s/i, t)
+    }, d.set = function(e) {
         var t, n;
-        for (n in e) m(e, n) && (O(t = e[n]) ? this[n] = t : this["_" + n] = t);
+        for (n in e) c(e, n) && (a(t = e[n]) ? this[n] = t : this["_" + n] = t);
         this._config = e, this._dayOfMonthOrdinalParseLenient = new RegExp((this._dayOfMonthOrdinalParse.source || this._ordinalParse.source) + "|" + /\d{1,2}/.source)
-    }, kn.eras = function(e, t) {
-        for (var n, s = this._eras || dt("en")._eras, i = 0, r = s.length; i < r; ++i) {
+    }, d.eras = function(e, t) {
+        for (var n, s = this._eras || P("en")._eras, i = 0, r = s.length; i < r; ++i) {
             switch (typeof s[i].since) {
                 case "string":
-                    n = f(s[i].since).startOf("day"), s[i].since = n.valueOf();
+                    n = _(s[i].since).startOf("day"), s[i].since = n.valueOf();
                     break
             }
             switch (typeof s[i].until) {
                 case "undefined":
                     s[i].until = 1 / 0;
                     break;
                 case "string":
-                    n = f(s[i].until).startOf("day").valueOf(), s[i].until = n.valueOf();
+                    n = _(s[i].until).startOf("day").valueOf(), s[i].until = n.valueOf();
                     break
             }
         }
         return s
-    }, kn.erasParse = function(e, t, n) {
+    }, d.erasParse = function(e, t, n) {
         var s, i, r, a, o, u = this.eras();
         for (e = e.toUpperCase(), s = 0, i = u.length; s < i; ++s)
             if (r = u[s].name.toUpperCase(), a = u[s].abbr.toUpperCase(), o = u[s].narrow.toUpperCase(), n) switch (t) {
                 case "N":
                 case "NN":
                 case "NNN":
                     if (a === e) return u[s];
@@ -1450,82 +1521,81 @@
                 case "NNNN":
                     if (r === e) return u[s];
                     break;
                 case "NNNNN":
                     if (o === e) return u[s];
                     break
             } else if (0 <= [r, a, o].indexOf(e)) return u[s]
-    }, kn.erasConvertYear = function(e, t) {
+    }, d.erasConvertYear = function(e, t) {
         var n = e.since <= e.until ? 1 : -1;
-        return void 0 === t ? f(e.since).year() : f(e.since).year() + (t - e.offset) * n
-    }, kn.erasAbbrRegex = function(e) {
-        return m(this, "_erasAbbrRegex") || hn.call(this), e ? this._erasAbbrRegex : this._erasRegex
-    }, kn.erasNameRegex = function(e) {
-        return m(this, "_erasNameRegex") || hn.call(this), e ? this._erasNameRegex : this._erasRegex
-    }, kn.erasNarrowRegex = function(e) {
-        return m(this, "_erasNarrowRegex") || hn.call(this), e ? this._erasNarrowRegex : this._erasRegex
-    }, kn.months = function(e, t) {
-        return e ? o(this._months) ? this._months[e.month()] : this._months[(this._months.isFormat || Pe).test(t) ? "format" : "standalone"][e.month()] : o(this._months) ? this._months : this._months.standalone
-    }, kn.monthsShort = function(e, t) {
-        return e ? o(this._monthsShort) ? this._monthsShort[e.month()] : this._monthsShort[Pe.test(t) ? "format" : "standalone"][e.month()] : o(this._monthsShort) ? this._monthsShort : this._monthsShort.standalone
-    }, kn.monthsParse = function(e, t, n) {
-        var s, i, r;
+        return void 0 === t ? _(e.since).year() : _(e.since).year() + (t - e.offset) * n
+    }, d.erasAbbrRegex = function(e) {
+        return c(this, "_erasAbbrRegex") || an.call(this), e ? this._erasAbbrRegex : this._erasRegex
+    }, d.erasNameRegex = function(e) {
+        return c(this, "_erasNameRegex") || an.call(this), e ? this._erasNameRegex : this._erasRegex
+    }, d.erasNarrowRegex = function(e) {
+        return c(this, "_erasNarrowRegex") || an.call(this), e ? this._erasNarrowRegex : this._erasRegex
+    }, d.months = function(e, t) {
+        return e ? (y(this._months) ? this._months : this._months[(this._months.isFormat || Ve).test(t) ? "format" : "standalone"])[e.month()] : y(this._months) ? this._months : this._months.standalone
+    }, d.monthsShort = function(e, t) {
+        return e ? (y(this._monthsShort) ? this._monthsShort : this._monthsShort[Ve.test(t) ? "format" : "standalone"])[e.month()] : y(this._monthsShort) ? this._monthsShort : this._monthsShort.standalone
+    }, d.monthsParse = function(e, t, n) {
+        var s, i;
         if (this._monthsParseExact) return function(e, t, n) {
-            var s, i, r, a = e.toLocaleLowerCase();
+            var s, i, r, e = e.toLocaleLowerCase();
             if (!this._monthsParse)
-                for (this._monthsParse = [], this._longMonthsParse = [], this._shortMonthsParse = [], s = 0; s < 12; ++s) r = _([2e3, s]), this._shortMonthsParse[s] = this.monthsShort(r, "").toLocaleLowerCase(), this._longMonthsParse[s] = this.months(r, "").toLocaleLowerCase();
-            return n ? "MMM" === t ? -1 !== (i = we.call(this._shortMonthsParse, a)) ? i : null : -1 !== (i = we.call(this._longMonthsParse, a)) ? i : null : "MMM" === t ? -1 !== (i = we.call(this._shortMonthsParse, a)) || -1 !== (i = we.call(this._longMonthsParse, a)) ? i : null : -1 !== (i = we.call(this._longMonthsParse, a)) || -1 !== (i = we.call(this._shortMonthsParse, a)) ? i : null
+                for (this._monthsParse = [], this._longMonthsParse = [], this._shortMonthsParse = [], s = 0; s < 12; ++s) r = l([2e3, s]), this._shortMonthsParse[s] = this.monthsShort(r, "").toLocaleLowerCase(), this._longMonthsParse[s] = this.months(r, "").toLocaleLowerCase();
+            return n ? "MMM" === t ? -1 !== (i = x.call(this._shortMonthsParse, e)) ? i : null : -1 !== (i = x.call(this._longMonthsParse, e)) ? i : null : "MMM" === t ? -1 !== (i = x.call(this._shortMonthsParse, e)) || -1 !== (i = x.call(this._longMonthsParse, e)) ? i : null : -1 !== (i = x.call(this._longMonthsParse, e)) || -1 !== (i = x.call(this._shortMonthsParse, e)) ? i : null
         }.call(this, e, t, n);
         for (this._monthsParse || (this._monthsParse = [], this._longMonthsParse = [], this._shortMonthsParse = []), s = 0; s < 12; s++) {
-            if (i = _([2e3, s]), n && !this._longMonthsParse[s] && (this._longMonthsParse[s] = new RegExp("^" + this.months(i, "").replace(".", "") + "$", "i"), this._shortMonthsParse[s] = new RegExp("^" + this.monthsShort(i, "").replace(".", "") + "$", "i")), n || this._monthsParse[s] || (r = "^" + this.months(i, "") + "|^" + this.monthsShort(i, ""), this._monthsParse[s] = new RegExp(r.replace(".", ""), "i")), n && "MMMM" === t && this._longMonthsParse[s].test(e)) return s;
+            if (i = l([2e3, s]), n && !this._longMonthsParse[s] && (this._longMonthsParse[s] = new RegExp("^" + this.months(i, "").replace(".", "") + "$", "i"), this._shortMonthsParse[s] = new RegExp("^" + this.monthsShort(i, "").replace(".", "") + "$", "i")), n || this._monthsParse[s] || (i = "^" + this.months(i, "") + "|^" + this.monthsShort(i, ""), this._monthsParse[s] = new RegExp(i.replace(".", ""), "i")), n && "MMMM" === t && this._longMonthsParse[s].test(e)) return s;
             if (n && "MMM" === t && this._shortMonthsParse[s].test(e)) return s;
             if (!n && this._monthsParse[s].test(e)) return s
         }
-    }, kn.monthsRegex = function(e) {
-        return this._monthsParseExact ? (m(this, "_monthsRegex") || He.call(this), e ? this._monthsStrictRegex : this._monthsRegex) : (m(this, "_monthsRegex") || (this._monthsRegex = We), this._monthsStrictRegex && e ? this._monthsStrictRegex : this._monthsRegex)
-    }, kn.monthsShortRegex = function(e) {
-        return this._monthsParseExact ? (m(this, "_monthsRegex") || He.call(this), e ? this._monthsShortStrictRegex : this._monthsShortRegex) : (m(this, "_monthsShortRegex") || (this._monthsShortRegex = Re), this._monthsShortStrictRegex && e ? this._monthsShortStrictRegex : this._monthsShortRegex)
-    }, kn.week = function(e) {
-        return Ae(e, this._week.dow, this._week.doy).week
-    }, kn.firstDayOfYear = function() {
+    }, d.monthsRegex = function(e) {
+        return this._monthsParseExact ? (c(this, "_monthsRegex") || je.call(this), e ? this._monthsStrictRegex : this._monthsRegex) : (c(this, "_monthsRegex") || (this._monthsRegex = Ee), this._monthsStrictRegex && e ? this._monthsStrictRegex : this._monthsRegex)
+    }, d.monthsShortRegex = function(e) {
+        return this._monthsParseExact ? (c(this, "_monthsRegex") || je.call(this), e ? this._monthsShortStrictRegex : this._monthsShortRegex) : (c(this, "_monthsShortRegex") || (this._monthsShortRegex = Ge), this._monthsShortStrictRegex && e ? this._monthsShortStrictRegex : this._monthsShortRegex)
+    }, d.week = function(e) {
+        return Be(e, this._week.dow, this._week.doy).week
+    }, d.firstDayOfYear = function() {
         return this._week.doy
-    }, kn.firstDayOfWeek = function() {
+    }, d.firstDayOfWeek = function() {
         return this._week.dow
-    }, kn.weekdays = function(e, t) {
-        var n = o(this._weekdays) ? this._weekdays : this._weekdays[e && !0 !== e && this._weekdays.isFormat.test(t) ? "format" : "standalone"];
-        return !0 === e ? Ie(n, this._week.dow) : e ? n[e.day()] : n
-    }, kn.weekdaysMin = function(e) {
-        return !0 === e ? Ie(this._weekdaysMin, this._week.dow) : e ? this._weekdaysMin[e.day()] : this._weekdaysMin
-    }, kn.weekdaysShort = function(e) {
-        return !0 === e ? Ie(this._weekdaysShort, this._week.dow) : e ? this._weekdaysShort[e.day()] : this._weekdaysShort
-    }, kn.weekdaysParse = function(e, t, n) {
-        var s, i, r;
+    }, d.weekdays = function(e, t) {
+        return t = y(this._weekdays) ? this._weekdays : this._weekdays[e && !0 !== e && this._weekdays.isFormat.test(t) ? "format" : "standalone"], !0 === e ? Je(t, this._week.dow) : e ? t[e.day()] : t
+    }, d.weekdaysMin = function(e) {
+        return !0 === e ? Je(this._weekdaysMin, this._week.dow) : e ? this._weekdaysMin[e.day()] : this._weekdaysMin
+    }, d.weekdaysShort = function(e) {
+        return !0 === e ? Je(this._weekdaysShort, this._week.dow) : e ? this._weekdaysShort[e.day()] : this._weekdaysShort
+    }, d.weekdaysParse = function(e, t, n) {
+        var s, i;
         if (this._weekdaysParseExact) return function(e, t, n) {
-            var s, i, r, a = e.toLocaleLowerCase();
+            var s, i, r, e = e.toLocaleLowerCase();
             if (!this._weekdaysParse)
-                for (this._weekdaysParse = [], this._shortWeekdaysParse = [], this._minWeekdaysParse = [], s = 0; s < 7; ++s) r = _([2e3, 1]).day(s), this._minWeekdaysParse[s] = this.weekdaysMin(r, "").toLocaleLowerCase(), this._shortWeekdaysParse[s] = this.weekdaysShort(r, "").toLocaleLowerCase(), this._weekdaysParse[s] = this.weekdays(r, "").toLocaleLowerCase();
-            return n ? "dddd" === t ? -1 !== (i = we.call(this._weekdaysParse, a)) ? i : null : "ddd" === t ? -1 !== (i = we.call(this._shortWeekdaysParse, a)) ? i : null : -1 !== (i = we.call(this._minWeekdaysParse, a)) ? i : null : "dddd" === t ? -1 !== (i = we.call(this._weekdaysParse, a)) || -1 !== (i = we.call(this._shortWeekdaysParse, a)) || -1 !== (i = we.call(this._minWeekdaysParse, a)) ? i : null : "ddd" === t ? -1 !== (i = we.call(this._shortWeekdaysParse, a)) || -1 !== (i = we.call(this._weekdaysParse, a)) || -1 !== (i = we.call(this._minWeekdaysParse, a)) ? i : null : -1 !== (i = we.call(this._minWeekdaysParse, a)) || -1 !== (i = we.call(this._weekdaysParse, a)) || -1 !== (i = we.call(this._shortWeekdaysParse, a)) ? i : null
+                for (this._weekdaysParse = [], this._shortWeekdaysParse = [], this._minWeekdaysParse = [], s = 0; s < 7; ++s) r = l([2e3, 1]).day(s), this._minWeekdaysParse[s] = this.weekdaysMin(r, "").toLocaleLowerCase(), this._shortWeekdaysParse[s] = this.weekdaysShort(r, "").toLocaleLowerCase(), this._weekdaysParse[s] = this.weekdays(r, "").toLocaleLowerCase();
+            return n ? "dddd" === t ? -1 !== (i = x.call(this._weekdaysParse, e)) ? i : null : "ddd" === t ? -1 !== (i = x.call(this._shortWeekdaysParse, e)) ? i : null : -1 !== (i = x.call(this._minWeekdaysParse, e)) ? i : null : "dddd" === t ? -1 !== (i = x.call(this._weekdaysParse, e)) || -1 !== (i = x.call(this._shortWeekdaysParse, e)) || -1 !== (i = x.call(this._minWeekdaysParse, e)) ? i : null : "ddd" === t ? -1 !== (i = x.call(this._shortWeekdaysParse, e)) || -1 !== (i = x.call(this._weekdaysParse, e)) || -1 !== (i = x.call(this._minWeekdaysParse, e)) ? i : null : -1 !== (i = x.call(this._minWeekdaysParse, e)) || -1 !== (i = x.call(this._weekdaysParse, e)) || -1 !== (i = x.call(this._shortWeekdaysParse, e)) ? i : null
         }.call(this, e, t, n);
         for (this._weekdaysParse || (this._weekdaysParse = [], this._minWeekdaysParse = [], this._shortWeekdaysParse = [], this._fullWeekdaysParse = []), s = 0; s < 7; s++) {
-            if (i = _([2e3, 1]).day(s), n && !this._fullWeekdaysParse[s] && (this._fullWeekdaysParse[s] = new RegExp("^" + this.weekdays(i, "").replace(".", "\\.?") + "$", "i"), this._shortWeekdaysParse[s] = new RegExp("^" + this.weekdaysShort(i, "").replace(".", "\\.?") + "$", "i"), this._minWeekdaysParse[s] = new RegExp("^" + this.weekdaysMin(i, "").replace(".", "\\.?") + "$", "i")), this._weekdaysParse[s] || (r = "^" + this.weekdays(i, "") + "|^" + this.weekdaysShort(i, "") + "|^" + this.weekdaysMin(i, ""), this._weekdaysParse[s] = new RegExp(r.replace(".", ""), "i")), n && "dddd" === t && this._fullWeekdaysParse[s].test(e)) return s;
+            if (i = l([2e3, 1]).day(s), n && !this._fullWeekdaysParse[s] && (this._fullWeekdaysParse[s] = new RegExp("^" + this.weekdays(i, "").replace(".", "\\.?") + "$", "i"), this._shortWeekdaysParse[s] = new RegExp("^" + this.weekdaysShort(i, "").replace(".", "\\.?") + "$", "i"), this._minWeekdaysParse[s] = new RegExp("^" + this.weekdaysMin(i, "").replace(".", "\\.?") + "$", "i")), this._weekdaysParse[s] || (i = "^" + this.weekdays(i, "") + "|^" + this.weekdaysShort(i, "") + "|^" + this.weekdaysMin(i, ""), this._weekdaysParse[s] = new RegExp(i.replace(".", ""), "i")), n && "dddd" === t && this._fullWeekdaysParse[s].test(e)) return s;
             if (n && "ddd" === t && this._shortWeekdaysParse[s].test(e)) return s;
             if (n && "dd" === t && this._minWeekdaysParse[s].test(e)) return s;
             if (!n && this._weekdaysParse[s].test(e)) return s
         }
-    }, kn.weekdaysRegex = function(e) {
-        return this._weekdaysParseExact ? (m(this, "_weekdaysRegex") || Qe.call(this), e ? this._weekdaysStrictRegex : this._weekdaysRegex) : (m(this, "_weekdaysRegex") || (this._weekdaysRegex = qe), this._weekdaysStrictRegex && e ? this._weekdaysStrictRegex : this._weekdaysRegex)
-    }, kn.weekdaysShortRegex = function(e) {
-        return this._weekdaysParseExact ? (m(this, "_weekdaysRegex") || Qe.call(this), e ? this._weekdaysShortStrictRegex : this._weekdaysShortRegex) : (m(this, "_weekdaysShortRegex") || (this._weekdaysShortRegex = Be), this._weekdaysShortStrictRegex && e ? this._weekdaysShortStrictRegex : this._weekdaysShortRegex)
-    }, kn.weekdaysMinRegex = function(e) {
-        return this._weekdaysParseExact ? (m(this, "_weekdaysRegex") || Qe.call(this), e ? this._weekdaysMinStrictRegex : this._weekdaysMinRegex) : (m(this, "_weekdaysMinRegex") || (this._weekdaysMinRegex = Je), this._weekdaysMinStrictRegex && e ? this._weekdaysMinStrictRegex : this._weekdaysMinRegex)
-    }, kn.isPM = function(e) {
+    }, d.weekdaysRegex = function(e) {
+        return this._weekdaysParseExact ? (c(this, "_weekdaysRegex") || st.call(this), e ? this._weekdaysStrictRegex : this._weekdaysRegex) : (c(this, "_weekdaysRegex") || (this._weekdaysRegex = et), this._weekdaysStrictRegex && e ? this._weekdaysStrictRegex : this._weekdaysRegex)
+    }, d.weekdaysShortRegex = function(e) {
+        return this._weekdaysParseExact ? (c(this, "_weekdaysRegex") || st.call(this), e ? this._weekdaysShortStrictRegex : this._weekdaysShortRegex) : (c(this, "_weekdaysShortRegex") || (this._weekdaysShortRegex = tt), this._weekdaysShortStrictRegex && e ? this._weekdaysShortStrictRegex : this._weekdaysShortRegex)
+    }, d.weekdaysMinRegex = function(e) {
+        return this._weekdaysParseExact ? (c(this, "_weekdaysRegex") || st.call(this), e ? this._weekdaysMinStrictRegex : this._weekdaysMinRegex) : (c(this, "_weekdaysMinRegex") || (this._weekdaysMinRegex = nt), this._weekdaysMinStrictRegex && e ? this._weekdaysMinStrictRegex : this._weekdaysMinRegex)
+    }, d.isPM = function(e) {
         return "p" === (e + "").toLowerCase().charAt(0)
-    }, kn.meridiem = function(e, t, n) {
+    }, d.meridiem = function(e, t, n) {
         return 11 < e ? n ? "pm" : "PM" : n ? "am" : "AM"
-    }, lt("en", {
+    }, ft("en", {
         eras: [{
             since: "0001-01-01",
             until: 1 / 0,
             offset: 1,
             name: "Anno Domini",
             narrow: "AD",
             abbr: "AD"
@@ -1536,124 +1606,112 @@
             name: "Before Christ",
             narrow: "BC",
             abbr: "BC"
         }],
         dayOfMonthOrdinalParse: /\d{1,2}(th|st|nd|rd)/,
         ordinal: function(e) {
             var t = e % 10;
-            return e + (1 === Z(e % 100 / 10) ? "th" : 1 == t ? "st" : 2 == t ? "nd" : 3 == t ? "rd" : "th")
+            return e + (1 === M(e % 100 / 10) ? "th" : 1 == t ? "st" : 2 == t ? "nd" : 3 == t ? "rd" : "th")
         }
-    }), f.lang = n("moment.lang is deprecated. Use moment.locale instead.", lt), f.langData = n("moment.langData is deprecated. Use moment.localeData instead.", dt);
-    var Yn = Math.abs;
+    }), _.lang = e("moment.lang is deprecated. Use moment.locale instead.", ft), _.langData = e("moment.langData is deprecated. Use moment.localeData instead.", P);
+    var _n = Math.abs;
 
-    function On(e, t, n, s) {
-        var i = Zt(t, n);
-        return e._milliseconds += s * i._milliseconds, e._days += s * i._days, e._months += s * i._months, e._bubble()
+    function yn(e, t, n, s) {
+        t = C(t, n);
+        return e._milliseconds += s * t._milliseconds, e._days += s * t._days, e._months += s * t._months, e._bubble()
     }
 
-    function bn(e) {
+    function gn(e) {
         return e < 0 ? Math.floor(e) : Math.ceil(e)
     }
 
-    function xn(e) {
+    function wn(e) {
         return 4800 * e / 146097
     }
 
-    function Tn(e) {
+    function pn(e) {
         return 146097 * e / 4800
     }
 
-    function Nn(e) {
+    function kn(e) {
         return function() {
             return this.as(e)
         }
     }
-    var Pn = Nn("ms"),
-        Rn = Nn("s"),
-        Wn = Nn("m"),
-        Cn = Nn("h"),
-        Un = Nn("d"),
-        Hn = Nn("w"),
-        Fn = Nn("M"),
-        Ln = Nn("Q"),
-        Vn = Nn("y");
+    de = kn("ms"), t = kn("s"), ye = kn("m"), he = kn("h"), Fe = kn("d"), _e = kn("w"), me = kn("M"), Qe = kn("Q"), i = kn("y"), ce = de;
 
-    function Gn(e) {
+    function Mn(e) {
         return function() {
             return this.isValid() ? this._data[e] : NaN
         }
     }
-    var En = Gn("milliseconds"),
-        An = Gn("seconds"),
-        jn = Gn("minutes"),
-        In = Gn("hours"),
-        Zn = Gn("days"),
-        zn = Gn("months"),
-        $n = Gn("years");
-    var qn = Math.round,
-        Bn = {
+    var we = Mn("milliseconds"),
+        fe = Mn("seconds"),
+        ge = Mn("minutes"),
+        Pe = Mn("hours"),
+        d = Mn("days"),
+        vn = Mn("months"),
+        Dn = Mn("years");
+    var Yn = Math.round,
+        Sn = {
             ss: 44,
             s: 45,
             m: 45,
             h: 22,
             d: 26,
             w: null,
             M: 11
         };
 
-    function Jn(e, t, n, s) {
-        var i = Zt(e).abs(),
-            r = qn(i.as("s")),
-            a = qn(i.as("m")),
-            o = qn(i.as("h")),
-            u = qn(i.as("d")),
-            l = qn(i.as("M")),
-            h = qn(i.as("w")),
-            d = qn(i.as("y")),
-            c = (r <= n.ss ? ["s", r] : r < n.s && ["ss", r]) || a <= 1 && ["m"] || a < n.m && ["mm", a] || o <= 1 && ["h"] || o < n.h && ["hh", o] || u <= 1 && ["d"] || u < n.d && ["dd", u];
-        return null != n.w && (c = c || h <= 1 && ["w"] || h < n.w && ["ww", h]), (c = c || l <= 1 && ["M"] || l < n.M && ["MM", l] || d <= 1 && ["y"] || ["yy", d])[2] = t, c[3] = 0 < +e, c[4] = s,
+    function On(e, t, n, s) {
+        var i = C(e).abs(),
+            r = Yn(i.as("s")),
+            a = Yn(i.as("m")),
+            o = Yn(i.as("h")),
+            u = Yn(i.as("d")),
+            l = Yn(i.as("M")),
+            d = Yn(i.as("w")),
+            i = Yn(i.as("y")),
+            r = (r <= n.ss ? ["s", r] : r < n.s && ["ss", r]) || (a <= 1 ? ["m"] : a < n.m && ["mm", a]) || (o <= 1 ? ["h"] : o < n.h && ["hh", o]) || (u <= 1 ? ["d"] : u < n.d && ["dd", u]);
+        return (r = (r = null != n.w ? r || (d <= 1 ? ["w"] : d < n.w && ["ww", d]) : r) || (l <= 1 ? ["M"] : l < n.M && ["MM", l]) || (i <= 1 ? ["y"] : ["yy", i]))[2] = t, r[3] = 0 < +e, r[4] = s,
             function(e, t, n, s, i) {
                 return i.relativeTime(t || 1, !!n, e, s)
-            }.apply(null, c)
+            }.apply(null, r)
     }
-    var Qn = Math.abs;
+    var bn = Math.abs;
 
-    function Xn(e) {
+    function Tn(e) {
         return (0 < e) - (e < 0) || +e
     }
 
-    function Kn() {
-        if (!this.isValid()) return this.localeData().invalidDate();
-        var e, t, n, s, i, r, a, o, u = Qn(this._milliseconds) / 1e3,
-            l = Qn(this._days),
-            h = Qn(this._months),
-            d = this.asSeconds();
-        return d ? (e = I(u / 60), t = I(e / 60), u %= 60, e %= 60, n = I(h / 12), h %= 12, s = u ? u.toFixed(3).replace(/\.?0+$/, "") : "", i = d < 0 ? "-" : "", r = Xn(this._months) !== Xn(d) ? "-" : "", a = Xn(this._days) !== Xn(d) ? "-" : "", o = Xn(this._milliseconds) !== Xn(d) ? "-" : "", i + "P" + (n ? r + n + "Y" : "") + (h ? r + h + "M" : "") + (l ? a + l + "D" : "") + (t || e || u ? "T" : "") + (t ? o + t + "H" : "") + (e ? o + e + "M" : "") + (u ? o + s + "S" : "")) : "P0D"
+    function xn() {
+        var e, t, n, s, i, r, a, o, u, l, d;
+        return this.isValid() ? (e = bn(this._milliseconds) / 1e3, t = bn(this._days), n = bn(this._months), (o = this.asSeconds()) ? (s = m(e / 60), i = m(s / 60), e %= 60, s %= 60, r = m(n / 12), n %= 12, a = e ? e.toFixed(3).replace(/\.?0+$/, "") : "", u = Tn(this._months) !== Tn(o) ? "-" : "", l = Tn(this._days) !== Tn(o) ? "-" : "", d = Tn(this._milliseconds) !== Tn(o) ? "-" : "", (o < 0 ? "-" : "") + "P" + (r ? u + r + "Y" : "") + (n ? u + n + "M" : "") + (t ? l + t + "D" : "") + (i || s || e ? "T" : "") + (i ? d + i + "H" : "") + (s ? d + s + "M" : "") + (e ? d + a + "S" : "")) : "P0D") : this.localeData().invalidDate()
     }
-    var es = Ct.prototype;
-    return es.isValid = function() {
+    var U = Ct.prototype;
+    return U.isValid = function() {
         return this._isValid
-    }, es.abs = function() {
+    }, U.abs = function() {
         var e = this._data;
-        return this._milliseconds = Yn(this._milliseconds), this._days = Yn(this._days), this._months = Yn(this._months), e.milliseconds = Yn(e.milliseconds), e.seconds = Yn(e.seconds), e.minutes = Yn(e.minutes), e.hours = Yn(e.hours), e.months = Yn(e.months), e.years = Yn(e.years), this
-    }, es.add = function(e, t) {
-        return On(this, e, t, 1)
-    }, es.subtract = function(e, t) {
-        return On(this, e, t, -1)
-    }, es.as = function(e) {
+        return this._milliseconds = _n(this._milliseconds), this._days = _n(this._days), this._months = _n(this._months), e.milliseconds = _n(e.milliseconds), e.seconds = _n(e.seconds), e.minutes = _n(e.minutes), e.hours = _n(e.hours), e.months = _n(e.months), e.years = _n(e.years), this
+    }, U.add = function(e, t) {
+        return yn(this, e, t, 1)
+    }, U.subtract = function(e, t) {
+        return yn(this, e, t, -1)
+    }, U.as = function(e) {
         if (!this.isValid()) return NaN;
         var t, n, s = this._milliseconds;
-        if ("month" === (e = V(e)) || "quarter" === e || "year" === e) switch (t = this._days + s / 864e5, n = this._months + xn(t), e) {
+        if ("month" === (e = o(e)) || "quarter" === e || "year" === e) switch (t = this._days + s / 864e5, n = this._months + wn(t), e) {
             case "month":
                 return n;
             case "quarter":
                 return n / 3;
             case "year":
                 return n / 12
-        } else switch (t = this._days + Math.round(Tn(this._months)), e) {
+        } else switch (t = this._days + Math.round(pn(this._months)), e) {
             case "week":
                 return t / 7 + s / 6048e5;
             case "day":
                 return t + s / 864e5;
             case "hour":
                 return 24 * t + s / 36e5;
             case "minute":
@@ -1661,75 +1719,70 @@
             case "second":
                 return 86400 * t + s / 1e3;
             case "millisecond":
                 return Math.floor(864e5 * t) + s;
             default:
                 throw new Error("Unknown unit " + e)
         }
-    }, es.asMilliseconds = Pn, es.asSeconds = Rn, es.asMinutes = Wn, es.asHours = Cn, es.asDays = Un, es.asWeeks = Hn, es.asMonths = Fn, es.asQuarters = Ln, es.asYears = Vn, es.valueOf = function() {
-        return this.isValid() ? this._milliseconds + 864e5 * this._days + this._months % 12 * 2592e6 + 31536e6 * Z(this._months / 12) : NaN
-    }, es._bubble = function() {
-        var e, t, n, s, i, r = this._milliseconds,
-            a = this._days,
-            o = this._months,
-            u = this._data;
-        return 0 <= r && 0 <= a && 0 <= o || r <= 0 && a <= 0 && o <= 0 || (r += 864e5 * bn(Tn(o) + a), o = a = 0), u.milliseconds = r % 1e3, e = I(r / 1e3), u.seconds = e % 60, t = I(e / 60), u.minutes = t % 60, n = I(t / 60), u.hours = n % 24, a += I(n / 24), o += i = I(xn(a)), a -= bn(Tn(i)), s = I(o / 12), o %= 12, u.days = a, u.months = o, u.years = s, this
-    }, es.clone = function() {
-        return Zt(this)
-    }, es.get = function(e) {
-        return e = V(e), this.isValid() ? this[e + "s"]() : NaN
-    }, es.milliseconds = En, es.seconds = An, es.minutes = jn, es.hours = In, es.days = Zn, es.weeks = function() {
-        return I(this.days() / 7)
-    }, es.months = zn, es.years = $n, es.humanize = function(e, t) {
-        if (!this.isValid()) return this.localeData().invalidDate();
-        var n, s, i = !1,
-            r = Bn;
-        return "object" == typeof e && (t = e, e = !1), "boolean" == typeof e && (i = e), "object" == typeof t && (r = Object.assign({}, Bn, t), null != t.s && null == t.ss && (r.ss = t.s - 1)), n = this.localeData(), s = Jn(this, !i, r, n), i && (s = n.pastFuture(+this, s)), n.postformat(s)
-    }, es.toISOString = Kn, es.toString = Kn, es.toJSON = Kn, es.locale = tn, es.localeData = sn, es.toIsoString = n("toIsoString() is deprecated. Please use toISOString() instead (notice the capitals)", Kn), es.lang = nn, C("X", 0, 0, "unix"), C("x", 0, 0, "valueOf"), ce("x", ue), ce("X", /[+-]?\d+(\.\d{1,3})?/), ye("X", function(e, t, n) {
+    }, U.asMilliseconds = de, U.asSeconds = t, U.asMinutes = ye, U.asHours = he, U.asDays = Fe, U.asWeeks = _e, U.asMonths = me, U.asQuarters = Qe, U.asYears = i, U.valueOf = ce, U._bubble = function() {
+        var e = this._milliseconds,
+            t = this._days,
+            n = this._months,
+            s = this._data;
+        return 0 <= e && 0 <= t && 0 <= n || e <= 0 && t <= 0 && n <= 0 || (e += 864e5 * gn(pn(n) + t), n = t = 0), s.milliseconds = e % 1e3, e = m(e / 1e3), s.seconds = e % 60, e = m(e / 60), s.minutes = e % 60, e = m(e / 60), s.hours = e % 24, t += m(e / 24), n += e = m(wn(t)), t -= gn(pn(e)), e = m(n / 12), n %= 12, s.days = t, s.months = n, s.years = e, this
+    }, U.clone = function() {
+        return C(this)
+    }, U.get = function(e) {
+        return e = o(e), this.isValid() ? this[e + "s"]() : NaN
+    }, U.milliseconds = we, U.seconds = fe, U.minutes = ge, U.hours = Pe, U.days = d, U.weeks = function() {
+        return m(this.days() / 7)
+    }, U.months = vn, U.years = Dn, U.humanize = function(e, t) {
+        var n, s;
+        return this.isValid() ? (n = !1, s = Sn, "object" == typeof e && (t = e, e = !1), "boolean" == typeof e && (n = e), "object" == typeof t && (s = Object.assign({}, Sn, t), null != t.s) && null == t.ss && (s.ss = t.s - 1), e = this.localeData(), t = On(this, !n, s, e), n && (t = e.pastFuture(+this, t)), e.postformat(t)) : this.localeData().invalidDate()
+    }, U.toISOString = xn, U.toString = xn, U.toJSON = xn, U.locale = Xt, U.localeData = Kt, U.toIsoString = e("toIsoString() is deprecated. Please use toISOString() instead (notice the capitals)", xn), U.lang = Ke, s("X", 0, 0, "unix"), s("x", 0, 0, "valueOf"), h("x", ke), h("X", /[+-]?\d+(\.\d{1,3})?/), v("X", function(e, t, n) {
         n._d = new Date(1e3 * parseFloat(e))
-    }), ye("x", function(e, t, n) {
-        n._d = new Date(Z(e))
-    }), f.version = "2.29.1", e = Tt, f.fn = pn, f.min = function() {
-        return Rt("isBefore", [].slice.call(arguments, 0))
-    }, f.max = function() {
-        return Rt("isAfter", [].slice.call(arguments, 0))
-    }, f.now = function() {
+    }), v("x", function(e, t, n) {
+        n._d = new Date(M(e))
+    }), _.version = "2.30.1", H = R, _.fn = u, _.min = function() {
+        return Pt("isBefore", [].slice.call(arguments, 0))
+    }, _.max = function() {
+        return Pt("isAfter", [].slice.call(arguments, 0))
+    }, _.now = function() {
         return Date.now ? Date.now() : +new Date
-    }, f.utc = _, f.unix = function(e) {
-        return Tt(1e3 * e)
-    }, f.months = function(e, t) {
-        return Dn(e, t, "months")
-    }, f.isDate = a, f.locale = lt, f.invalid = w, f.duration = Zt, f.isMoment = M, f.weekdays = function(e, t, n) {
-        return Sn(e, t, n, "weekdays")
-    }, f.parseZone = function() {
-        return Tt.apply(null, arguments).parseZone()
-    }, f.localeData = dt, f.isDuration = Ut, f.monthsShort = function(e, t) {
-        return Dn(e, t, "monthsShort")
-    }, f.weekdaysMin = function(e, t, n) {
-        return Sn(e, t, n, "weekdaysMin")
-    }, f.defineLocale = ht, f.updateLocale = function(e, t) {
-        var n, s, i;
-        return null != t ? (i = st, null != it[e] && null != it[e].parentLocale ? it[e].set(b(it[e]._config, t)) : (null != (s = ut(e)) && (i = s._config), t = b(i, t), null == s && (t.abbr = e), (n = new x(t)).parentLocale = it[e], it[e] = n), lt(e)) : null != it[e] && (null != it[e].parentLocale ? (it[e] = it[e].parentLocale, e === lt() && lt(e)) : null != it[e] && delete it[e]), it[e]
-    }, f.locales = function() {
-        return s(it)
-    }, f.weekdaysShort = function(e, t, n) {
-        return Sn(e, t, n, "weekdaysShort")
-    }, f.normalizeUnits = V, f.relativeTimeRounding = function(e) {
-        return void 0 === e ? qn : "function" == typeof e && (qn = e, !0)
-    }, f.relativeTimeThreshold = function(e, t) {
-        return void 0 !== Bn[e] && (void 0 === t ? Bn[e] : (Bn[e] = t, "s" === e && (Bn.ss = t - 1), !0))
-    }, f.calendarFormat = function(e, t) {
-        var n = e.diff(t, "days", !0);
-        return n < -6 ? "sameElse" : n < -1 ? "lastWeek" : n < 0 ? "lastDay" : n < 1 ? "sameDay" : n < 2 ? "nextDay" : n < 7 ? "nextWeek" : "sameElse"
-    }, f.prototype = pn, f.HTML5_FMT = {
+    }, _.utc = l, _.unix = function(e) {
+        return R(1e3 * e)
+    }, _.months = function(e, t) {
+        return fn(e, t, "months")
+    }, _.isDate = V, _.locale = ft, _.invalid = I, _.duration = C, _.isMoment = k, _.weekdays = function(e, t, n) {
+        return mn(e, t, n, "weekdays")
+    }, _.parseZone = function() {
+        return R.apply(null, arguments).parseZone()
+    }, _.localeData = P, _.isDuration = Ut, _.monthsShort = function(e, t) {
+        return fn(e, t, "monthsShort")
+    }, _.weekdaysMin = function(e, t, n) {
+        return mn(e, t, n, "weekdaysMin")
+    }, _.defineLocale = mt, _.updateLocale = function(e, t) {
+        var n, s;
+        return null != t ? (s = ut, null != W[e] && null != W[e].parentLocale ? W[e].set(X(W[e]._config, t)) : (t = X(s = null != (n = ct(e)) ? n._config : s, t), null == n && (t.abbr = e), (s = new K(t)).parentLocale = W[e], W[e] = s), ft(e)) : null != W[e] && (null != W[e].parentLocale ? (W[e] = W[e].parentLocale, e === ft() && ft(e)) : null != W[e] && delete W[e]), W[e]
+    }, _.locales = function() {
+        return ee(W)
+    }, _.weekdaysShort = function(e, t, n) {
+        return mn(e, t, n, "weekdaysShort")
+    }, _.normalizeUnits = o, _.relativeTimeRounding = function(e) {
+        return void 0 === e ? Yn : "function" == typeof e && (Yn = e, !0)
+    }, _.relativeTimeThreshold = function(e, t) {
+        return void 0 !== Sn[e] && (void 0 === t ? Sn[e] : (Sn[e] = t, "s" === e && (Sn.ss = t - 1), !0))
+    }, _.calendarFormat = function(e, t) {
+        return (e = e.diff(t, "days", !0)) < -6 ? "sameElse" : e < -1 ? "lastWeek" : e < 0 ? "lastDay" : e < 1 ? "sameDay" : e < 2 ? "nextDay" : e < 7 ? "nextWeek" : "sameElse"
+    }, _.prototype = u, _.HTML5_FMT = {
         DATETIME_LOCAL: "YYYY-MM-DDTHH:mm",
         DATETIME_LOCAL_SECONDS: "YYYY-MM-DDTHH:mm:ss",
         DATETIME_LOCAL_MS: "YYYY-MM-DDTHH:mm:ss.SSS",
         DATE: "YYYY-MM-DD",
         TIME: "HH:mm",
         TIME_SECONDS: "HH:mm:ss",
         TIME_MS: "HH:mm:ss.SSS",
         WEEK: "GGGG-[W]WW",
         MONTH: "YYYY-MM"
-    }, f
+    }, _
 });
 //# sourceMappingURL=moment.min.js.map
```

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/stack-icons.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/stack-icons.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/tags-filter.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/tags-filter.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/tex-mml-chtml.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/tex-mml-chtml.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/webp-handler.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/webp-handler.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/webp-hero.bundle.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/webp-hero.bundle.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/assets/static/js/webp-hero.polyfill.js` & `sotoki-2.1.1/src/sotoki/assets/static/js/webp-hero.polyfill.js`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/constants.py` & `sotoki-2.1.1/src/sotoki/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 
 import os
 import pathlib
 import datetime
 import re
 import tempfile
 import urllib.parse
-from typing import Optional, List
+from typing import Optional, List, Tuple
 from dataclasses import dataclass, field
 
 import requests
 from zimscraperlib.i18n import get_language_details, NotFound
 
 ROOT_DIR = pathlib.Path(__file__).parent
 NAME = ROOT_DIR.name
 
 with open(ROOT_DIR.joinpath("VERSION"), "r") as fh:
     VERSION = fh.read().strip()
 
 UTF8 = "utf-8"
+UTF16LE = "utf-16-le"
 SCRAPER = f"{NAME} {VERSION}"
 USER_AGENT = (
     f"{NAME}/{VERSION} (https://github.com/openzim/sotoki; "
     f"contact+crawl@kiwix.org) requests/{requests.__version__}"
 )
 DOWNLOAD_ROOT = "https://archive.org/download/stackexchange"
 # some domains have changed names overtime but SE's Sites.xml still reference old Url
@@ -43,15 +44,17 @@
 NB_QUESTIONS_PAGES = 100
 NB_PAGINATED_QUESTIONS = NB_QUESTIONS_PER_PAGE * NB_QUESTIONS_PAGES
 NB_USERS_PER_PAGE = 36
 NB_USERS_PAGES = 100
 NB_PAGINATED_USERS = NB_USERS_PER_PAGE * NB_USERS_PAGES
 
 
-def lang_for_domain(domain):
+def langs_for_domain(domain: str) -> Tuple[List[str], List[str]]:
+    """(ISO-639-1 lang codes, ISO-639-3 lang codes) for a domain"""
+    iso_langs_1, iso_langs_3 = ["en"], ["eng"]
     match = re.match(r"^(?P<lang>[a-z]+)\.(stackexchange|stackoverflow)\.com$", domain)
     if match:
         so_code = match.groupdict()["lang"]
         if so_code not in (
             "meta",
             "diy",
             "sqa",
@@ -60,48 +63,52 @@
             "tex",
             "law",
             "ham",
             "gis",
             "ell",
             "or",
             "vi",
+            "cs",
         ):
             try:
                 lang = get_language_details(so_code)
                 if not lang["iso-639-1"] or not lang["iso-639-3"]:
                     raise NotFound("Might be an abbreviation")
-                return lang["iso-639-1"], lang["iso-639-3"]
+                iso_langs_1.append(lang["iso-639-1"])
+                iso_langs_3.append(lang["iso-639-3"])
             except NotFound:
                 ...
-    return "en", "eng"
+    return iso_langs_1, iso_langs_3
 
 
 @dataclass
 class Sotoconf:
     required = [
         "domain",
         "name",
         "output_dir",
         "keep_build_dir",
         "nb_threads",
     ]
 
     domain: str
-    _redis_url: str
+    redis_url: str
 
     # zim params
     name: str
     title: Optional[str] = ""
     description: Optional[str] = ""
+    long_description: Optional[str] = ""
     author: Optional[str] = ""
     publisher: Optional[str] = ""
     fname: Optional[str] = ""
     tag: List[str] = field(default_factory=list)
-    iso_lang_1: str = "en"  # ISO-639-1
-    iso_lang_3: str = "eng"  # ISO-639-3
+    flavour: Optional[str] = ""
+    iso_langs_1: List[str] = field(default_factory=list)  # ISO-639-1
+    iso_langs_3: List[str] = field(default_factory=list)  # ISO-639-3
 
     # customization
     favicon: Optional[str] = ""
 
     # filesystem
     _output_dir: Optional[str] = "."
     _tmp_dir: Optional[str] = "."
@@ -136,14 +143,18 @@
     dump_date: Optional[datetime.date] = datetime.date.today()
     open_shell: Optional[bool] = False
     skip_tags_meta: Optional[bool] = False
     skip_questions_meta: Optional[bool] = False
     skip_users: Optional[bool] = False
 
     @property
+    def tags(self):
+        return list(set(self.tag))
+
+    @property
     def s3_url(self):
         return self.s3_url_with_credentials
 
     @property
     def is_stackO(self):
         return self.domain == "stackoverflow.com"
 
@@ -180,16 +191,18 @@
                 self.censor_words_list,
             )
         )
 
     def __post_init__(self):
         self.dump_domain = self.domain  # dumps are named after unfixed domains
         self.domain = FIXED_DOMAINS.get(self.domain, self.domain)
-        self.iso_lang_1, self.iso_lang_3 = lang_for_domain(self.domain)
-        self.name = self.name or f"{self.domain}_{self.iso_lang_1}_all"
+        self.iso_langs_1, self.iso_langs_3 = langs_for_domain(self.domain)
+        self.flavour = "nopic" if self.without_images else "all"
+        lang_in_name = self.iso_langs_1[0] if len(self.iso_langs_1) == 1 else "mul"
+        self.name = self.name or f"{self.domain}_{lang_in_name}_{self.flavour}"
         self.output_dir = pathlib.Path(self._output_dir).expanduser().resolve()
         self.output_dir.mkdir(parents=True, exist_ok=True)
         self.tmp_dir = pathlib.Path(self._tmp_dir).expanduser().resolve()
         if self.tmp_dir:
             self.tmp_dir.mkdir(parents=True, exist_ok=True)
         if self.build_dir_is_tmp_dir:
             self.build_dir = self.tmp_dir
@@ -197,17 +210,27 @@
             self.build_dir = pathlib.Path(
                 tempfile.mkdtemp(prefix=f"{self.domain}_", dir=self.tmp_dir)
             )
         if self.stats_filename:
             self.stats_filename = pathlib.Path(self.stats_filename).expanduser()
             self.stats_filename.parent.mkdir(parents=True, exist_ok=True)
 
-        self.redis_url = urllib.parse.urlparse(self._redis_url)
-        if self.redis_url and self.redis_url.scheme not in ("unix", "redis"):
+        redis_url = urllib.parse.urlparse(self.redis_url)
+        if redis_url and redis_url.scheme not in ("unix", "redis"):
             raise ValueError(
-                f"Unknown scheme `{self.redis_url.scheme}` for redis. "
+                f"Unknown scheme `{redis_url.scheme}` for redis. "
                 "Use redis:// or unix://"
             )
 
+        self.tag += [
+            "_category:stack_exchange",
+            "stack_exchange",
+            "_videos:no",
+            "_details:no",
+        ]
+
+        if self.without_images:
+            self.tag.append("_pictures:no")
+
         # shell implies debug
         if self.open_shell:
             self.debug = True
```

### Comparing `sotoki-2.0.2/src/sotoki/dependencies.py` & `sotoki-2.1.1/src/sotoki/dependencies.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/entrypoint.py` & `sotoki-2.1.1/src/sotoki/entrypoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,14 +93,19 @@
         help="Custom title for your ZIM. Site name otherwise",
     )
 
     metadata.add_argument(
         "--description",
         help="Custom description for your ZIM. Site tagline otherwise",
     )
+    metadata.add_argument(
+        "--long-description",
+        help="Custom long description for your ZIM, defaults to description if description is too long",
+        required=False,
+    )
 
     metadata.add_argument(
         "--favicon",
         help="URL/path for Zim Illustration. Site square logo otherwise",
     )
 
     metadata.add_argument(
@@ -108,16 +113,15 @@
         help="Name of content creator. “Stack Exchange” otherwise",
         dest="author",
     )
 
     metadata.add_argument(
         "-p",
         "--publisher",
-        help="Custom publisher name (ZIM metadata). “OpenZIM” otherwise",
-        default="Kiwix",
+        help="Custom publisher name (ZIM metadata). “openZIM” otherwise"
     )
     metadata.add_argument(
         "--tag",
         help="Add tag to the ZIM file. "
         "category:stack_exchange and stack_exchange added automatically",
         default=["_category:stack_exchange", "stack_exchange"],
         action="append",
@@ -229,15 +233,15 @@
 
     advanced.add_argument(
         "--redis-url",
         help="Redis URL to use as database. "
         "Must be redis://user?:pass?@host:port/dbnum. "
         "Use unix:///path/to/redis.sock?db=dbnum for sockets",
         default="redis://localhost:6379",
-        dest="_redis_url",
+        dest="redis_url",
     )
 
     advanced.add_argument(
         "--debug", help="Enable verbose output", action="store_true", default=False
     )
 
     advanced.add_argument(
```

### Comparing `sotoki-2.0.2/src/sotoki/posts.py` & `sotoki-2.1.1/src/sotoki/posts.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,17 @@
         # opening comments of a question
         if name == "comment":
             _user_to_set(self.post["users_ids"], "UserId")
             return
 
         # opening answers of a question
         if name == "answer":  # a answer
+            # ignore deleted answers
+            if "DeletionDate" in attrs:
+                return
             _user_to_set(self.post["users_ids"], "OwnerUserId")
             _user_to_set(self.post["users_ids"], "LastEditorUserId")
             self.post["nb_answers"] += 1
 
     def endElement(self, name):
 
         if name == "post":
@@ -87,14 +90,18 @@
         self.database.record_questions_stats(
             nb_answers=self.nb_answers,
             nb_answered=self.nb_answered,
             nb_accepted=self.nb_accepted,
         )
 
     def processor(self, item):
+        # ignore deleted posts
+        if "DeletionDate" in item:
+            self.release()
+            return
         # skip post without answers ; maybe?
         if self.conf.without_unanswered and not item["nb_answers"]:
             self.release()
             return
 
         harmonize_post(item)
 
@@ -161,14 +168,16 @@
             self.currently_in = "post/answers"
             self.comments = []
             self.answers = []
             return
 
         # an answer
         if name == "answer":
+            if "DeletionDate" in attrs:
+                return
             self.answers.append(dict(attrs.items()))
             return
 
         # opening comments of an answer
         if name == "comments" and self.currently_in == "post/answers":
             self.currently_in = "post/answers/comments"
             self.comments = []
@@ -237,28 +246,36 @@
         self.fpath = self.conf.build_dir / "posts_complete.xml"
 
     def processor(self, item):
         post = item
         if self.conf.without_unanswered and not post["answers"]:
             self.release()
             return
+        # ignore deleted posts
+        if "DeletionDate" in item:
+            self.release()
+            return
         harmonize_post(post)
 
         path = f'questions/{post["Id"]}/{get_slug_for(post["Title"])}'
         # prepare post page outside Lock to prevent dead-lock on image discovery
         post_page = self.renderer.get_question(post)
         with self.lock:
             self.creator.add_item_for(
                 path=path,
                 title=self.rewriter.rewrite_string(post.get("Title")),
                 content=post_page,
                 mimetype="text/html",
                 is_front=True,
                 callback=self.release,
             )
+            self.creator.add_redirect(
+                path=f'questions/{post["Id"]}',
+                target_path=path,
+            )
         del post_page
 
         for answer in post.get("answers", []):
             with self.lock:
                 self.creator.add_redirect(
                     path=f'a/{answer["Id"]}',
                     target_path=path,
```

### Comparing `sotoki-2.0.2/src/sotoki/renderer.py` & `sotoki-2.1.1/src/sotoki/renderer.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/scraper.py` & `sotoki-2.1.1/src/sotoki/scraper.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # vim: ai ts=4 sts=4 et sw=4 nu
 
 import shutil
 import pathlib
 import datetime
 
 from zimscraperlib.zim.items import URLItem
-from zimscraperlib.inputs import handle_user_provided_file
+from zimscraperlib.inputs import handle_user_provided_file, compute_descriptions
 from zimscraperlib.image.convertion import convert_image
 from zimscraperlib.image.transformation import resize_image
 
 from .constants import (
     Sotoconf,
     ROOT_DIR,
     NB_PAGINATED_QUESTIONS_PER_TAG,
@@ -73,48 +73,30 @@
         else:
             self.conf.fname = f"{self.conf.name}_{period}.zim"
 
         if not self.conf.title:
             self.conf.title = Global.site["LongName"]
         self.conf.title = self.conf.title.strip()
 
-        if not self.conf.description:
-            self.conf.description = Global.site["Tagline"]
-        self.conf.description = self.conf.description.strip()
+        default_description = Global.site["Tagline"].strip()
+        if self.conf.description:
+            user_description = self.conf.description.strip()
+        else:
+            user_description = None
+        self.conf.description, self.conf.long_description = compute_descriptions(default_description, user_description, self.conf.long_description)
 
         if not self.conf.author:
             self.conf.author = "Stack Exchange"
         self.conf.author = self.conf.author.strip()
 
         if not self.conf.publisher:
-            self.conf.publisher = "Openzim"
+            self.conf.publisher = "openZIM"
         self.conf.publisher = self.conf.publisher.strip()
 
-        self.conf.tags = list(
-            set(self.conf.tag + ["_category:stack_exchange", "stack_exchange"])
-        )
-
     def add_illustrations(self):
-        src_illus_fpath = self.build_dir / "illustration"
-
-        # if user provided a custom favicon, retrieve that
-        if not self.conf.favicon:
-            self.conf.favicon = Global.site["BadgeIconUrl"]
-        handle_user_provided_file(source=self.conf.favicon, dest=src_illus_fpath)
-
-        # convert to PNG (might already be PNG but it's OK)
-        illus_fpath = src_illus_fpath.with_suffix(".png")
-        convert_image(src_illus_fpath, illus_fpath)
-
-        # resize to appropriate size (ZIM uses 48x48 so we double for retina)
-        for size in (96, 48):
-            resize_image(illus_fpath, width=size, height=size, method="thumbnail")
-            with open(illus_fpath, "rb") as fh:
-                Global.creator.add_illustration(size, fh.read())
-
         # download and add actual favicon (ICO file)
         favicon_fpath = self.build_dir / "favicon.ico"
         handle_user_provided_file(source=Global.site["IconUrl"], dest=favicon_fpath)
         Global.creator.add_item_for("favicon.ico", fpath=favicon_fpath, is_front=False)
 
         # download apple-touch-icon
         Global.creator.add_item(
@@ -156,15 +138,15 @@
             f"with bucket: {s3_storage.bucket_name}"
             if s3_storage
             else ""
         )
         logger.info(
             f"Starting scraper with:\n"
             f"  domain: {self.domain}\n"
-            f"  lang: {self.conf.iso_lang_1} ({self.conf.iso_lang_3})\n"
+            f"  lang: {self.conf.iso_langs_1} ({self.conf.iso_langs_3})\n"
             f"  build_dir: {self.build_dir}\n"
             f"  output_dir: {self.conf.output_dir}\n"
             f"{s3_msg}"
         )
 
         logger.debug("Fetching site details…")
         Global.init(get_site(self.domain))
```

### Comparing `sotoki-2.0.2/src/sotoki/tags.py` & `sotoki-2.1.1/src/sotoki/tags.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/templates/about.html` & `sotoki-2.1.1/src/sotoki/templates/about.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/templates/base.html` & `sotoki-2.1.1/src/sotoki/templates/base.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/templates/pagination.html` & `sotoki-2.1.1/src/sotoki/templates/pagination.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/templates/post_layout.html` & `sotoki-2.1.1/src/sotoki/templates/post_layout.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/templates/question.html` & `sotoki-2.1.1/src/sotoki/templates/question.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/templates/question_list_item.html` & `sotoki-2.1.1/src/sotoki/templates/question_list_item.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/templates/questions.html` & `sotoki-2.1.1/src/sotoki/templates/questions.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/templates/single_comment.html` & `sotoki-2.1.1/src/sotoki/templates/single_comment.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/templates/tag.html` & `sotoki-2.1.1/src/sotoki/templates/tag.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/templates/tags.html` & `sotoki-2.1.1/src/sotoki/templates/tags.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/templates/user.html` & `sotoki-2.1.1/src/sotoki/templates/user.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/templates/user_card.html` & `sotoki-2.1.1/src/sotoki/templates/user_card.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/templates/users.html` & `sotoki-2.1.1/src/sotoki/templates/users.html`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/users.py` & `sotoki-2.1.1/src/sotoki/users.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/utils/database/common.py` & `sotoki-2.1.1/src/sotoki/utils/database/common.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/utils/database/posts.py` & `sotoki-2.1.1/src/sotoki/utils/database/posts.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/utils/database/redisdb.py` & `sotoki-2.1.1/src/sotoki/utils/database/redisdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # vim: ai ts=4 sts=4 et sw=4 nu
 
 import collections
 import threading
 import time
 from typing import Union
 
-import redis
 import bidict
+import redis
+from sotoki.constants import NB_PAGINATED_USERS, UTF8
 
+from ..misc import restart_redis_at
+from ..shared import Global, logger
 from .common import Database
 from .posts import PostsDatabaseMixin
 from .tags import TagsDatabaseMixin
 from .users import UsersDatabaseMixin
-from ..shared import Global, logger
-from ..misc import restart_redis_at
-from sotoki.constants import UTF8, NB_PAGINATED_USERS
 
 
 class TopDict(collections.UserDict):
     """A fixed-sized dict that keeps only the highest values"""
 
     def __init__(self, maxlen: int):
         super().__init__()
@@ -73,15 +73,15 @@
     @property
     def conn(self):
         """thread-specific Redis connection"""
         try:
             return self.connections[threading.get_ident()]
         except KeyError:
             self.connections[threading.get_ident()] = redis.StrictRedis.from_url(
-                Global.conf.redis_url.geturl(), charset=UTF8, decode_responses=False
+                Global.conf.redis_url, encoding=UTF8, decode_responses=False
             )
             return self.connections[threading.get_ident()]
 
     @property
     def pipe(self):
         """thread-specific Pipeline for this thread-specific connection"""
         try:
```

### Comparing `sotoki-2.0.2/src/sotoki/utils/database/tags.py` & `sotoki-2.1.1/src/sotoki/utils/database/tags.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/utils/database/users.py` & `sotoki-2.1.1/src/sotoki/utils/database/users.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/utils/executor.py` & `sotoki-2.1.1/src/sotoki/utils/executor.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/utils/generator.py` & `sotoki-2.1.1/src/sotoki/utils/generator.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/utils/html.py` & `sotoki-2.1.1/src/sotoki/utils/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import re
 import urllib.parse
 import warnings
 
 import bs4
 
-# import mistune
-# from mistune.plugins import plugin_strikethrough, plugin_table, plugin_footnotes
+import mistune
+from mistune.plugins import plugin_strikethrough, plugin_table, plugin_footnotes
 from tld import get_fld
 from slugify import slugify
 
 from .shared import logger, GlobalMixin
 from .misc import rebuild_uri
 
 
@@ -106,18 +106,18 @@
             re.compile(r"tags_page=[0-9]+$"),
             re.compile(r"api/tags.json$"),
             re.compile(r"about$"),
             re.compile(r"images/[0-9]+.webp$"),
         )
 
         self.redacted_string = bs4.NavigableString(self.redacted_text)
-        # self.markdown = mistune.create_markdown(
-        #     escape=False,
-        #     plugins=[plugin_strikethrough, plugin_table, plugin_footnotes],
-        # )
+        self.markdown = mistune.create_markdown(
+            escape=False,
+            plugins=[plugin_strikethrough, plugin_table, plugin_footnotes],
+        )
         if self.conf.censor_words_list:
             with open(self.conf.build_dir.joinpath("words.list"), "r") as fh:
                 # this will actually replace occurences of ~strings matching
                 # words in the list but those can be part of actual words or whole.
                 self.words_re = re.compile(
                     r"\b\b|\b\b".join(
                         map(re.escape, [line.strip() for line in fh.readlines()])
@@ -158,16 +158,16 @@
         """
         # Content might be empty
         content = content.strip()
         if not content:
             return ""
 
         try:
-            # soup = bs4.BeautifulSoup(self.markdown(content), "lxml")
-            soup = BeautifulSoup(content, "lxml")
+            soup = bs4.BeautifulSoup(self.markdown(content), "lxml")
+            # soup = BeautifulSoup(content, "lxml")
         except Exception as exc:
             logger.error(f"Unable to init soup or markdown for {content}: {exc}")
             return content
 
         if not soup:
             return ""
```

### Comparing `sotoki-2.0.2/src/sotoki/utils/imager.py` & `sotoki-2.1.1/src/sotoki/utils/imager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # vim: ai ts=4 sts=4 et sw=4 nu
 
 import io
 import re
-import zlib
+import hashlib
 import urllib.parse
 from typing import Optional
 
 import requests
 from PIL import Image
 from resizeimage.imageexceptions import ImageSizeError
 from zimscraperlib.download import stream_file
@@ -149,15 +149,16 @@
 
     def get_s3_key_for(self, url: str) -> str:
         """S3 key to use for that url"""
         return re.sub(r"^(https?)://", r"\1/", url)
 
     def get_digest_for(self, url: str) -> str:
         """Unique identifier of that url"""
-        return zlib.adler32(url.encode("UTF-8"))
+        return hashlib.md5(url.encode("UTF-8")).hexdigest()  # nosec
+
 
     def get_version_ident_for(self, url: str) -> str:
         """~version~ of the URL data to use for comparisons. Built from headers"""
         try:
             resp = requests.head(url, headers={"User-Agent": USER_AGENT})
             headers = resp.headers
         except Exception:
```

### Comparing `sotoki-2.0.2/src/sotoki/utils/misc.py` & `sotoki-2.1.1/src/sotoki/utils/misc.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/utils/paginator.py` & `sotoki-2.1.1/src/sotoki/utils/paginator.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/utils/preparation.py` & `sotoki-2.1.1/src/sotoki/utils/preparation.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,46 @@
 
     Main goal is to prepare combined XML dumps that gets all required data on a
     single node when traversing the document using SAX """
 
 import os
 import re
 import pathlib
-import xml.sax
+import xml.sax.saxutils
 import subprocess
 from typing import Union
 
 from .shared import logger
 from .misc import has_binary, get_available_memory
-from ..constants import UTF8
+from ..constants import UTF8, UTF16LE
 
 has_gnusort = has_binary("sort")
 
 
+def reencode_file(src: pathlib.Path):
+    """Reencode a file from dump format (UTF-16-LE as of March 2024) to expected format (UTF8)
+
+    This is based on a streaming on-the-fly reencoding of file chunks to limit memory pressure.
+
+    Content is read line-by-line to ensure it is not split in the middle of a grapheme cluster.
+
+    During reencoding, there will be two versions of the same content on the filesystem, one in
+    previous encoding and one in target encoding, filesystem needs enough space for that.
+    """
+    tmp = src.with_suffix(src.suffix + ".tmp")
+    with open(src, "r", encoding=UTF16LE) as sourceFile:
+        with open(tmp, "w", encoding=UTF8) as targetFile:
+            while True:
+                contents = sourceFile.readline()
+                if not contents:
+                    break
+                targetFile.write(contents)
+    src.unlink()
+    tmp.rename(src)
+
 def get_within_chars(nb_chars_glue: int, nb_ids: int) -> int:
     """nb of chars to combine `nb_ids`'s values with `nb_chars_glue`
 
     Used to compute `within` value for get_id_in()"""
     max_id_len = 8  # 8 chars can contain up to 99M ids
     return nb_chars_glue + (max_id_len * nb_ids)
 
@@ -208,31 +229,31 @@
         # read first badges line so we can compare it in loop
         current_sub = read_sub()
 
         # loop on main file as this is our base that we'll complete with sub rows
         for main_line in mainfh:
             main_id = get_id_in(main_line, field_index_in_main)
 
-            # write main line to dest; removing tag end (/> -> >) and CRLF
-            dsth.write(main_line[:-4])
+            # write main line to dest; removing tag end (/>) and LF
+            dsth.write(main_line[:-3])
             dsth.write(b">")
 
             # fetch subs matching this ID (IDs are sorted so it's continuous)
             has_subs = False
             while current_sub is not None and current_sub[0] < main_id:
                 current_sub = read_sub()
             while current_sub is not None and current_sub[0] == main_id:
                 if not has_subs:
                     dsth.write(nodes_start)
                     has_subs = True
 
                 dsth.write(node_start)
-                # write the sub line removing the 2 heading spaces, node name (<row)
-                # removing trailing CRLF as well. node already self closed in source
-                dsth.write(current_sub[1][6:-2])
+                # write the sub line removing node name (<row) and trailing LF as well. node already
+                # self closed in source
+                dsth.write(current_sub[1][4:-1])
                 current_sub = read_sub()
 
             if has_subs:
                 dsth.write(nodes_end)
             has_subs = False
             dsth.write(b"</row>\n")
 
@@ -309,17 +330,17 @@
     with open(src, "rb") as srch:
         for line in srch:
             try:
                 found_id = get_id_in(line, index, within=pattern_len)
             except IndexError:
                 break
             try:
-                # rewrite with new name replacing `  <row` and `row>`
+                # rewrite with new name replacing `<row` and `row>LF`
                 fhs[found_id].write(starts[found_id])
-                fhs[found_id].write(line[6:-5])
+                fhs[found_id].write(line[4:-5])
                 fhs[found_id].write(ends[found_id])
             except KeyError:
                 continue
 
     # close file descriptors
     _ = {fh.close() for fh in fhs.values()}
 
@@ -378,17 +399,17 @@
                 if current_csv is None:
                     break
 
             if current_csv is None:
                 break
 
             if current_csv[0] == post_id:
-                # write user line to dest; removing tag end and CRLF
+                # write user line to dest; removing tag open (<row), tag end (/>) and LF
                 dsth.write(b"<link")
-                dsth.write(line[6:-4])
+                dsth.write(line[4:-3])
                 # CSV title already includes appropriate quoting
                 dsth.write(b" PostName=")
                 dsth.write(current_csv[1])
                 dsth.write(b" />\n")
 
     if delete_src:
         links_src.unlink()
```

### Comparing `sotoki-2.0.2/src/sotoki/utils/progress.py` & `sotoki-2.1.1/src/sotoki/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/utils/s3.py` & `sotoki-2.1.1/src/sotoki/utils/s3.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/utils/sevenzip.py` & `sotoki-2.1.1/src/sotoki/utils/sevenzip.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki/utils/sites.py` & `sotoki-2.1.1/src/sotoki/utils/sites.py`

 * *Files identical despite different names*

### Comparing `sotoki-2.0.2/src/sotoki.egg-info/PKG-INFO` & `sotoki-2.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,105 @@
 Metadata-Version: 2.1
 Name: sotoki
-Version: 2.0.2
+Version: 2.1.1
 Summary: Turn StackExchange dumps into ZIM files for offline usage
 Home-page: https://github.com/openzim/sotoki
 Author: Kiwix
 Author-email: contact+dev@kiwix.org
 License: GPLv3+
-Description: Sotoki
-        ======
-        
-        `Sotoki` (*Stack Overflow to Kiwix*) is an
-        [openZIM](https://github.com/openzim) scraper to create offline
-        versions of [Stack Exchange](https://stackexchange.com) websites such
-        as [Stack Overflow](https://stackoverflow.com/).
-        
-        It is based on Stack Exchange's Data Dumps hosted by [The Internet
-        Archive](https://archive.org/download/stackexchange/).
-        
-        [![CodeFactor](https://www.codefactor.io/repository/github/openzim/sotoki/badge)](https://www.codefactor.io/repository/github/openzim/sotoki)
-        [![Docker](https://img.shields.io/docker/v/openzim/sotoki?label=docker&sort=semver)](https://hub.docker.com/r/openzim/sotoki)
-        [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-        [![PyPI version shields.io](https://img.shields.io/pypi/v/sotoki.svg)](https://pypi.org/project/sotoki/)
-        
-        ## Usage
-        
-        `Sotoki` works off a `domain` that you must provide. That is the
-        domain-name of the stackexchange website you want to scrape. Run
-        `sotoki --list-all` to get a list of those
-        
-        ### Docker
-        
-        ```bash
-        docker run -v my_dir:/output openzim/sotoki sotoki --help
-        ```
-        
-        ### Installation
-        
-        `sotoki` is a Python3 software. If you are not using the
-        [Docker](https://hub.docker.com/r/openzim/sotoki/) image, you are advised to use it in a
-        virtual environment to avoid installing software dependencies on your
-        system.
-        
-        ```sh
-        python3 -m venv ./env  # creates a virtual python environment in ./env folder
-        ./env/bin/pip install -U pip  # upgrade pip (package manager). recommended
-        ./env/bin/pip install -U sotoki  # install/upgrade sotoki inside virtualenv
-        
-        # direct access to in-virtualenv sotoki binary, without shell-attachment
-        ./env/bin/sotoki --help
-        # alias or link it for convenience
-        sudo ln -s $(pwd)/env/bin/sotoki /usr/local/bin/
-        
-        # alternatively, attach virtualenv to shell
-        source env/bin/activate
-        sotoki --help
-        deactivate  # unloads virtualenv from shell
-        ```
-        
-        ## Developers
-        
-        Anybody is welcome to improve the Sotoki.
-        
-        To run Sotoki off the git repository, you'll need to download a few
-        external dependencies that we pack in Python releases. Just run
-        `python src/sotoki/dependencies.py`.
-        
-        See `requirements.txt` for the list of python dependencies.
-        
-        ## Users
-        
-        You don't have to make your own ZIM files of Stack Exchange's Web 
-        sites. Updated ZIM files are built on a regular basis for all 
-        of them. Look at https://library.kiwix.org/?category=stack_exchange
-        to download them.
-        
 Keywords: kiwix zim offline stackechange stackoverflow
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: kiwixstorage<1.0,>=0.8.1
+Requires-Dist: pif<0.9,>=0.8.2
+Requires-Dist: zimscraperlib<4.0,>=3.3.0
+Requires-Dist: xml_to_dict<0.2,>=0.1.6
+Requires-Dist: cli-formatter<1.3,>=1.2.0
+Requires-Dist: py7zr<0.21,>=0.20.4
+Requires-Dist: python-slugify<9.0.0,>=8.0.1
+Requires-Dist: jinja2<3.2,>=3.1.0
+Requires-Dist: redis!=4.5.2,<5.0,>=4.5.1
+Requires-Dist: beautifulsoup4<5.0,>=4.9.3
+Requires-Dist: lxml<4.10,>=4.9.1
+Requires-Dist: jinja2-pluralize<0.4,>=0.3.0
+Requires-Dist: tld<0.14,>=0.13
+Requires-Dist: mistune<3.0.0,>=2.0.5
+Requires-Dist: python-dateutil<2.9,>=2.8.2
+Requires-Dist: psutil<6.0,>=5.9.4
+Requires-Dist: python-snappy<1.0,>=0.6.0
+Requires-Dist: bidict<0.23,>=0.22.1
+Requires-Dist: cchardet<2.2,>=2.1.7
+
+Sotoki
+======
+
+`Sotoki` (*Stack Overflow to Kiwix*) is an
+[openZIM](https://github.com/openzim) scraper to create offline
+versions of [Stack Exchange](https://stackexchange.com) websites such
+as [Stack Overflow](https://stackoverflow.com/).
+
+It is based on Stack Exchange's Data Dumps hosted by [The Internet
+Archive](https://archive.org/download/stackexchange/).
+
+[![CodeFactor](https://www.codefactor.io/repository/github/openzim/sotoki/badge)](https://www.codefactor.io/repository/github/openzim/sotoki)
+[![Docker](https://ghcr-badge.deta.dev/openzim/sotoki/latest_tag?label=docker)](https://ghcr.io/openzim/sotoki)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/sotoki.svg)](https://pypi.org/project/sotoki/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sotoki.svg)](https://pypi.org/project/sotoki)
+
+## Usage
+
+`Sotoki` works off a `domain` that you must provide. That is the
+domain-name of the stackexchange website you want to scrape. Run
+`sotoki --list-all` to get a list of those
+
+### Docker
+
+```bash
+docker run -v my_dir:/output ghcr.io/openzim/sotoki sotoki --help
+```
+
+### Installation
+
+`sotoki` is a Python3 software. If you are not using the
+[Docker](https://ghcr.io/openzim/sotoki/) image, you are advised to use it in a
+virtual environment to avoid installing software dependencies on your
+system.
+
+```sh
+python3 -m venv ./env  # creates a virtual python environment in ./env folder
+./env/bin/pip install -U pip  # upgrade pip (package manager). recommended
+./env/bin/pip install -U sotoki  # install/upgrade sotoki inside virtualenv
+
+# direct access to in-virtualenv sotoki binary, without shell-attachment
+./env/bin/sotoki --help
+# alias or link it for convenience
+sudo ln -s $(pwd)/env/bin/sotoki /usr/local/bin/
+
+# alternatively, attach virtualenv to shell
+source env/bin/activate
+sotoki --help
+deactivate  # unloads virtualenv from shell
+```
+
+## Developers
+
+Anybody is welcome to improve the Sotoki.
+
+To run Sotoki off the git repository, you'll need to download a few
+external dependencies that we pack in Python releases. Just run
+`python src/sotoki/dependencies.py`.
+
+See `requirements.txt` for the list of python dependencies.
+
+## Users
+
+You don't have to make your own ZIM files of Stack Exchange's Web 
+sites. Updated ZIM files are built on a regular basis for all 
+of them. Look at https://library.kiwix.org/?category=stack_exchange
+to download them.
```

