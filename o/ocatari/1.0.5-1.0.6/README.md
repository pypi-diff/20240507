# Comparing `tmp/ocatari-1.0.5.tar.gz` & `tmp/ocatari-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocatari-1.0.5.tar", last modified: Tue Apr  9 09:14:58 2024, max compression
+gzip compressed data, was "ocatari-1.0.6.tar", last modified: Tue May  7 15:33:03 2024, max compression
```

## Comparing `ocatari-1.0.5.tar` & `ocatari-1.0.6.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-09 09:14:58.329941 ocatari-1.0.5/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1171 2023-06-14 17:01:45.000000 ocatari-1.0.5/LICENSE
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7744 2024-04-09 09:14:58.329941 ocatari-1.0.5/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6297 2024-03-13 13:04:01.000000 ocatari-1.0.5/README.md
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-09 09:14:58.317941 ocatari-1.0.5/ocatari/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       25 2024-02-13 13:58:13.000000 ocatari-1.0.5/ocatari/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    25223 2024-04-09 09:13:01.000000 ocatari-1.0.5/ocatari/core.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2891 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/environments.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-09 09:14:58.325941 ocatari-1.0.5/ocatari/ram/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:57:07.000000 ocatari-1.0.5/ocatari/ram/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3297 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/ram/_helper_methods.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14387 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/adventure.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7586 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/alien.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4015 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/amidar.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    15652 2024-03-19 14:28:41.000000 ocatari-1.0.5/ocatari/ram/assault.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5552 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/asterix.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     9111 2023-08-23 09:50:18.000000 ocatari-1.0.5/ocatari/ram/asterix_old.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14794 2024-02-12 14:35:56.000000 ocatari-1.0.5/ocatari/ram/asterix_old2.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    12738 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/asteroids.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14228 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/atlantis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4552 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/bankheist.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    19073 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/battlezone.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5410 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/beamrider.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10096 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/berzerk.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5888 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/bowling.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5593 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/boxing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7113 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/breakout.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11564 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/carnival.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11345 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/centipede.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    29613 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/choppercommand.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10183 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/crazyclimber.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6241 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/demonattack.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8247 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/donkeykong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2102 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/enduro.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    17884 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/extract_ram_info.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2068 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/extract_ram_info_short.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4745 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/fishingderby.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3136 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/freeway.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    12497 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/frostbite.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6054 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/ram/game_objects.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8640 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/gopher.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)   426388 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/hero.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4005 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/icehockey.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5966 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/jamesbond.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    13579 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/kangaroo.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14946 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/krull.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    38831 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/montezumarevenge.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6500 2024-03-20 15:36:32.000000 ocatari-1.0.5/ocatari/ram/mspacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4625 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/pacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    15746 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/pitfall.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5915 2024-04-09 09:11:16.000000 ocatari-1.0.5/ocatari/ram/pong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    16424 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/privateeye.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14403 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/qbert.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10776 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/riverraid.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    13893 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/roadrunner.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14619 2024-04-09 09:11:51.000000 ocatari-1.0.5/ocatari/ram/seaquest.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     9441 2024-03-18 13:29:46.000000 ocatari-1.0.5/ocatari/ram/skiing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    12471 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/spaceinvaders.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8869 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/tennis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    16258 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/timepilot.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7136 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/upndown.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3036 2023-07-31 09:59:59.000000 ocatari-1.0.5/ocatari/ram/utils.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     9308 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/venture.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5063 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/videopinball.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5946 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/yarsrevenge.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10737 2024-03-18 11:06:15.000000 ocatari-1.0.5/ocatari/utils.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-09 09:14:58.329941 ocatari-1.0.5/ocatari/vision/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:55:37.000000 ocatari-1.0.5/ocatari/vision/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5880 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/adventure.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2888 2023-09-07 09:07:40.000000 ocatari-1.0.5/ocatari/vision/alien.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2003 2023-11-15 16:35:48.000000 ocatari-1.0.5/ocatari/vision/amidar.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6175 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/assault.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8795 2023-03-14 16:04:08.000000 ocatari-1.0.5/ocatari/vision/asterix.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2588 2023-10-26 14:02:07.000000 ocatari-1.0.5/ocatari/vision/asteroids.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7361 2023-04-12 13:10:52.000000 ocatari-1.0.5/ocatari/vision/atlantis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2106 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/bankheist.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4570 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/battlezone.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6024 2023-04-12 13:10:52.000000 ocatari-1.0.5/ocatari/vision/beamrider.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2817 2023-05-29 14:25:14.000000 ocatari-1.0.5/ocatari/vision/berzerk.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2486 2023-03-14 16:04:08.000000 ocatari-1.0.5/ocatari/vision/bowling.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1812 2023-10-18 14:47:32.000000 ocatari-1.0.5/ocatari/vision/boxing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2992 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/breakout.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5182 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/carnival.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4292 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/centipede.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5801 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/choppercommand.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3765 2023-11-15 16:35:48.000000 ocatari-1.0.5/ocatari/vision/crazyclimber.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3168 2023-11-23 15:00:40.000000 ocatari-1.0.5/ocatari/vision/demonattack.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4350 2024-02-24 17:10:04.000000 ocatari-1.0.5/ocatari/vision/donkeykong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2418 2023-08-23 08:04:55.000000 ocatari-1.0.5/ocatari/vision/enduro.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7526 2024-02-13 14:20:55.000000 ocatari-1.0.5/ocatari/vision/extract_vision_info.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      597 2023-11-14 14:22:11.000000 ocatari-1.0.5/ocatari/vision/extract_vision_info_short.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5495 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/fishingderby.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1579 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/freeway.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5612 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/frostbite.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3683 2023-08-23 08:04:55.000000 ocatari-1.0.5/ocatari/vision/game_objects.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3016 2023-08-23 08:04:55.000000 ocatari-1.0.5/ocatari/vision/gopher.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11578 2023-10-10 09:58:35.000000 ocatari-1.0.5/ocatari/vision/hero.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2639 2023-07-19 13:40:30.000000 ocatari-1.0.5/ocatari/vision/icehockey.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4096 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/jamesbond.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5690 2023-08-23 08:04:55.000000 ocatari-1.0.5/ocatari/vision/kangaroo.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8432 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/krull.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6525 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/montezumarevenge.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2631 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/mspacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2334 2024-02-14 13:21:26.000000 ocatari-1.0.5/ocatari/vision/pacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7216 2023-11-12 17:10:19.000000 ocatari-1.0.5/ocatari/vision/pitfall.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2065 2023-06-16 08:15:13.000000 ocatari-1.0.5/ocatari/vision/pong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10116 2023-07-19 13:40:30.000000 ocatari-1.0.5/ocatari/vision/privateeye.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3978 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/qbert.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3867 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/riverraid.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8142 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/roadrunner.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4653 2023-08-23 08:04:55.000000 ocatari-1.0.5/ocatari/vision/seaquest.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2143 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/skiing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2909 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/spaceinvaders.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2499 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/tennis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6771 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/timepilot.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3629 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/upndown.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    21751 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/utils.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6659 2023-08-31 10:23:09.000000 ocatari-1.0.5/ocatari/vision/venture.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4132 2023-08-31 10:23:09.000000 ocatari-1.0.5/ocatari/vision/videopinball.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4128 2023-10-10 09:58:35.000000 ocatari-1.0.5/ocatari/vision/yarsrevenge.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-09 09:14:58.317941 ocatari-1.0.5/ocatari.egg-info/
--rw-r--r--   0 quentin   (1000) quentin   (1000)     7744 2024-04-09 09:14:58.000000 ocatari-1.0.5/ocatari.egg-info/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3413 2024-04-09 09:14:58.000000 ocatari-1.0.5/ocatari.egg-info/SOURCES.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2024-04-09 09:14:58.000000 ocatari-1.0.5/ocatari.egg-info/dependency_links.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      122 2024-04-09 09:14:58.000000 ocatari-1.0.5/ocatari.egg-info/requires.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       14 2024-04-09 09:14:58.000000 ocatari-1.0.5/ocatari.egg-info/top_level.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       38 2024-04-09 09:14:58.329941 ocatari-1.0.5/setup.cfg
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1025 2024-04-09 09:14:55.000000 ocatari-1.0.5/setup.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-09 09:14:58.329941 ocatari-1.0.5/tests/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-06-14 17:01:46.000000 ocatari-1.0.5/tests/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2509 2024-03-13 13:04:01.000000 ocatari-1.0.5/tests/display_game.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4339 2023-08-23 08:04:55.000000 ocatari-1.0.5/tests/display_game_both.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10431 2024-02-24 17:17:25.000000 ocatari-1.0.5/tests/get_metrics.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10493 2023-08-23 09:50:18.000000 ocatari-1.0.5/tests/metrics_utils.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1673 2023-06-14 17:01:46.000000 ocatari-1.0.5/tests/plot_speed_results.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1604 2024-03-13 13:04:01.000000 ocatari-1.0.5/tests/pong_test.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1851 2024-03-13 13:04:01.000000 ocatari-1.0.5/tests/test_explanation.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2921 2024-03-13 13:04:01.000000 ocatari-1.0.5/tests/test_game.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4637 2024-02-24 17:08:28.000000 ocatari-1.0.5/tests/test_game_both.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5963 2023-10-26 14:02:07.000000 ocatari-1.0.5/tests/test_game_both_interactive.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1281 2024-03-13 13:04:01.000000 ocatari-1.0.5/tests/test_speed.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-07 15:33:03.067300 ocatari-1.0.6/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1171 2023-06-14 17:01:45.000000 ocatari-1.0.6/LICENSE
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7744 2024-05-07 15:33:03.067300 ocatari-1.0.6/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6297 2024-03-13 13:04:01.000000 ocatari-1.0.6/README.md
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-07 15:33:02.967299 ocatari-1.0.6/ocatari/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       25 2024-02-13 13:58:13.000000 ocatari-1.0.6/ocatari/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    26172 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/core.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2891 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/environments.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-07 15:33:02.995299 ocatari-1.0.6/ocatari/ram/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:57:07.000000 ocatari-1.0.6/ocatari/ram/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3297 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/ram/_helper_methods.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14387 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/adventure.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7586 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/alien.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4015 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/amidar.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    15620 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/assault.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5552 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/asterix.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     9111 2023-08-23 09:50:18.000000 ocatari-1.0.6/ocatari/ram/asterix_old.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14794 2024-02-12 14:35:56.000000 ocatari-1.0.6/ocatari/ram/asterix_old2.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    12738 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/asteroids.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14088 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/atlantis.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4552 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/bankheist.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    19073 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/battlezone.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5410 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/beamrider.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10096 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/berzerk.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5888 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/bowling.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5534 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/boxing.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7113 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/breakout.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    11564 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/carnival.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    11345 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/centipede.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    29685 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/choppercommand.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10183 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/crazyclimber.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6241 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/demonattack.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8247 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/donkeykong.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2102 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/enduro.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    17884 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/extract_ram_info.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2068 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/extract_ram_info_short.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4743 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/fishingderby.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3136 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/freeway.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    12497 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/frostbite.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6054 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/ram/game_objects.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8640 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/gopher.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)   426388 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/hero.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4005 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/icehockey.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5966 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/jamesbond.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    13579 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/kangaroo.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14946 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/krull.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    38831 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/montezumarevenge.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6500 2024-03-20 15:36:32.000000 ocatari-1.0.6/ocatari/ram/mspacman.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4625 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/pacman.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    15588 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/pitfall.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5915 2024-04-09 09:11:16.000000 ocatari-1.0.6/ocatari/ram/pong.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    16424 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/privateeye.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14403 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/qbert.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10623 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/riverraid.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    13893 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/roadrunner.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14619 2024-04-09 09:11:51.000000 ocatari-1.0.6/ocatari/ram/seaquest.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8491 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/skiing.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    12411 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/ram/spaceinvaders.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8869 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/tennis.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    16258 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/timepilot.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7136 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/upndown.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3036 2023-07-31 09:59:59.000000 ocatari-1.0.6/ocatari/ram/utils.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     9308 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/venture.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5063 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/videopinball.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5946 2024-03-13 13:04:01.000000 ocatari-1.0.6/ocatari/ram/yarsrevenge.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10518 2024-05-07 15:31:43.000000 ocatari-1.0.6/ocatari/utils.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-07 15:33:03.055300 ocatari-1.0.6/ocatari/vision/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:55:37.000000 ocatari-1.0.6/ocatari/vision/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5880 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/adventure.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2888 2023-09-07 09:07:40.000000 ocatari-1.0.6/ocatari/vision/alien.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2003 2023-11-15 16:35:48.000000 ocatari-1.0.6/ocatari/vision/amidar.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6175 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/assault.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8795 2023-03-14 16:04:08.000000 ocatari-1.0.6/ocatari/vision/asterix.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2588 2023-10-26 14:02:07.000000 ocatari-1.0.6/ocatari/vision/asteroids.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7361 2023-04-12 13:10:52.000000 ocatari-1.0.6/ocatari/vision/atlantis.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2106 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/bankheist.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4570 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/battlezone.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6024 2023-04-12 13:10:52.000000 ocatari-1.0.6/ocatari/vision/beamrider.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2817 2023-05-29 14:25:14.000000 ocatari-1.0.6/ocatari/vision/berzerk.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2486 2023-03-14 16:04:08.000000 ocatari-1.0.6/ocatari/vision/bowling.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1812 2023-10-18 14:47:32.000000 ocatari-1.0.6/ocatari/vision/boxing.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2992 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/breakout.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5182 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/carnival.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4292 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/centipede.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5801 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/choppercommand.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3765 2023-11-15 16:35:48.000000 ocatari-1.0.6/ocatari/vision/crazyclimber.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3168 2023-11-23 15:00:40.000000 ocatari-1.0.6/ocatari/vision/demonattack.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4350 2024-02-24 17:10:04.000000 ocatari-1.0.6/ocatari/vision/donkeykong.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2418 2023-08-23 08:04:55.000000 ocatari-1.0.6/ocatari/vision/enduro.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7526 2024-02-13 14:20:55.000000 ocatari-1.0.6/ocatari/vision/extract_vision_info.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      597 2023-11-14 14:22:11.000000 ocatari-1.0.6/ocatari/vision/extract_vision_info_short.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5495 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/fishingderby.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1579 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/freeway.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5612 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/frostbite.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3683 2023-08-23 08:04:55.000000 ocatari-1.0.6/ocatari/vision/game_objects.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3016 2023-08-23 08:04:55.000000 ocatari-1.0.6/ocatari/vision/gopher.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    11578 2023-10-10 09:58:35.000000 ocatari-1.0.6/ocatari/vision/hero.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2639 2023-07-19 13:40:30.000000 ocatari-1.0.6/ocatari/vision/icehockey.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4096 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/jamesbond.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5690 2023-08-23 08:04:55.000000 ocatari-1.0.6/ocatari/vision/kangaroo.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8432 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/krull.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6525 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/montezumarevenge.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2631 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/mspacman.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2334 2024-02-14 13:21:26.000000 ocatari-1.0.6/ocatari/vision/pacman.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7216 2023-11-12 17:10:19.000000 ocatari-1.0.6/ocatari/vision/pitfall.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2065 2023-06-16 08:15:13.000000 ocatari-1.0.6/ocatari/vision/pong.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10116 2023-07-19 13:40:30.000000 ocatari-1.0.6/ocatari/vision/privateeye.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3978 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/qbert.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3867 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/riverraid.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8142 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/roadrunner.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4653 2023-08-23 08:04:55.000000 ocatari-1.0.6/ocatari/vision/seaquest.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2143 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/skiing.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2909 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/spaceinvaders.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2499 2023-06-14 17:01:46.000000 ocatari-1.0.6/ocatari/vision/tennis.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6771 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/timepilot.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3629 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/upndown.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    21751 2024-02-09 12:58:51.000000 ocatari-1.0.6/ocatari/vision/utils.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6659 2023-08-31 10:23:09.000000 ocatari-1.0.6/ocatari/vision/venture.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4132 2023-08-31 10:23:09.000000 ocatari-1.0.6/ocatari/vision/videopinball.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4128 2023-10-10 09:58:35.000000 ocatari-1.0.6/ocatari/vision/yarsrevenge.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-07 15:33:02.967299 ocatari-1.0.6/ocatari.egg-info/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     7744 2024-05-07 15:33:02.000000 ocatari-1.0.6/ocatari.egg-info/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3413 2024-05-07 15:33:02.000000 ocatari-1.0.6/ocatari.egg-info/SOURCES.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2024-05-07 15:33:02.000000 ocatari-1.0.6/ocatari.egg-info/dependency_links.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      122 2024-05-07 15:33:02.000000 ocatari-1.0.6/ocatari.egg-info/requires.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       14 2024-05-07 15:33:02.000000 ocatari-1.0.6/ocatari.egg-info/top_level.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       38 2024-05-07 15:33:03.067300 ocatari-1.0.6/setup.cfg
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1025 2024-05-07 15:32:52.000000 ocatari-1.0.6/setup.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-07 15:33:03.067300 ocatari-1.0.6/tests/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-06-14 17:01:46.000000 ocatari-1.0.6/tests/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2509 2024-03-13 13:04:01.000000 ocatari-1.0.6/tests/display_game.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4339 2023-08-23 08:04:55.000000 ocatari-1.0.6/tests/display_game_both.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10431 2024-02-24 17:17:25.000000 ocatari-1.0.6/tests/get_metrics.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10493 2023-08-23 09:50:18.000000 ocatari-1.0.6/tests/metrics_utils.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1673 2023-06-14 17:01:46.000000 ocatari-1.0.6/tests/plot_speed_results.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1604 2024-03-13 13:04:01.000000 ocatari-1.0.6/tests/pong_test.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1851 2024-03-13 13:04:01.000000 ocatari-1.0.6/tests/test_explanation.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2921 2024-03-13 13:04:01.000000 ocatari-1.0.6/tests/test_game.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4637 2024-02-24 17:08:28.000000 ocatari-1.0.6/tests/test_game_both.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5963 2023-10-26 14:02:07.000000 ocatari-1.0.6/tests/test_game_both_interactive.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1281 2024-03-13 13:04:01.000000 ocatari-1.0.6/tests/test_speed.py
```

### Comparing `ocatari-1.0.5/LICENSE` & `ocatari-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/PKG-INFO` & `ocatari-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 1.0.5
+Version: 1.0.6
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
 License: UNKNOWN
 Description: # Object-Centric Atari Environments
         Quentin Delfosse, Jannis Blüml, Bjarne Gregori, Sebastian Sztwiertnia, Anurag Maurya, Kévin-Lâm Quesnel and Simon Wulf
```

### Comparing `ocatari-1.0.5/README.md` & `ocatari-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/core.py` & `ocatari-1.0.6/ocatari/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,19 @@
     import pygame
 except ModuleNotFoundError:
     print(
         "\npygame is required for human rendering. ",
         "Try `pip install pygame`.\n",
     )
 
-DEVICE = "cpu" if torch.cuda.is_available() else "cpu"
-
+if torch_imported:
+    DEVICE = "gpu" if torch.cuda.is_available() else "cpu"
+else:
+    DEVICE = "cpu" 
+    
 AVAILABLE_GAMES = ["Adventure", "Alien", "Amidar", "Assault", "Asterix", "Asteroids", "Atlantis", "Bankheist", "BattleZone","BeamRider", "Berzerk", "Bowling", "Boxing",
                    "Breakout", "Carnival", "Centipede", "ChoppperCommand", "CrazyClimber", "DemonAttack", "DonkeyKong", "Enduro", "FishingDerby", "Freeway",                   
                    "Frostbite", "Gopher", "Hero", "IceHockey", "Jamesbond", "Kangaroo", "Krull", "MontezumaRevenge", "MsPacman", "Pacman", "Pitfall", "Pong", "PrivateEye",
                    "Qbert", "Riverraid", "RoadRunner", "Seaquest", "Skiing", "SpaceInvaders", "Tennis", "TimePilot", "UpNDown", "Videocube", "VideoPinball", "Venture",
                    "Yarsrevenge", "Zaxxon"]
 
 
@@ -115,22 +118,24 @@
         self._objects : list[GameObject] = init_objects(self.game_name, self.hud)
         self._fill_buffer = lambda *args, **kwargs: None
         self._reset_buffer = lambda *args, **kwargs: None
         if obs_mode == "dqn":
             if torch_imported:
                 self._fill_buffer = self._fill_buffer_dqn
                 self._reset_buffer = self._reset_buffer_dqn
+                self._env.observation_space = gym.spaces.Box(0,255.0,(4,84,84))
             else:
                 print("To use the buffer of OCAtari, you need to install torch.")
         elif obs_mode == "ori":
             self._fill_buffer = self._fill_buffer_ori
             self._reset_buffer = self._reset_buffer_ori
         elif obs_mode == "obj":
             print("Using OBJ State Representation")
             if mode == "ram":
+                self._env.observation_space = gym.spaces.Box(0,255.0,(4,3,4))
                 self._fill_buffer = self._fill_buffer_obj
                 self._reset_buffer = self._reset_buffer_obj
             else:
                 print(colored("This obs mode is only available in ram mode", "red"))
                 exit(1)
         elif obs_mode is not None:
             print(colored("Undefined mode for observation (obs_mode), has to be one of ['dqn', 'ori', None]", "red"))
@@ -167,14 +172,22 @@
     def _step_ram(self, *args, **kwargs):
         obs, reward, terminated, truncated, info = self._env.step(*args, **kwargs)
         if self.mode == "ram" or self.mode == "revised":
             self.detect_objects(self._objects, self._env.env.unwrapped.ale.getRAM(), self.game_name, self.hud)
         else:  # mode == "raw" because in raw mode we augment the info dictionary
             self.detect_objects(info, self._env.env.unwrapped.ale.getRAM(), self.game_name, self.hud)
         self._fill_buffer()
+        if self.obs_mode == "dqn":
+            obs = self.dqn_obs[0]
+        if self.obs_mode == "obj":
+            tensor = []
+            for obj in self._objects:
+                tensor.append(np.asarray(obj.xywh))
+            obs = np.asarray(tensor)
+            #obs = self.dqn_obs[0]
         return obs, reward, truncated, terminated, info
 
     def _step_vision(self, *args, **kwargs):
         obs, reward, terminated, truncated, info = self._env.step(*args, **kwargs)
         self.detect_objects(self._objects, obs, self.game_name, self.hud)
         self._fill_buffer()
         return obs, reward, truncated, terminated, info
@@ -215,14 +228,24 @@
         self._objects = init_objects(self.game_name, self.hud)
         return self._env.reset(*args, **kwargs)
 
     def _fill_buffer_dqn(self):
         state = cv2.resize(
             self._ale.getScreenGrayscale(), (84, 84), interpolation=cv2.INTER_AREA,
         )
+        if self.game_name == "Skiing":
+            #import ipdb;ipdb.set_trace()
+            tmp = self._state_buffer[1]
+            tmp[tmp >= 0] = self.objects[0].orientation
+            self._state_buffer[1] = tmp
+        elif self.game_name == "Seaquest":
+            #import ipdb;ipdb.set_trace()
+            tmp = self._state_buffer[1]
+            tmp[tmp >= 0] = self.objects[0].orientation.value
+            self._state_buffer[1] = tmp
         self._state_buffer.append(torch.tensor(state, dtype=torch.uint8,
                                                device=DEVICE))
 
     def _fill_buffer_ori(self):
         state = self._ale.getScreenRGB()
         self._state_buffer.append(torch.tensor(state, dtype=torch.uint8,
                                                device=DEVICE))
@@ -376,15 +399,15 @@
     def dqn_obs(self):
         """
         The 4 (grey+down)scaled last frames (84x84) of the environment, used notably by dqn agents as states.
 
         :type: torch.tensor
         """
         return self._get_buffer_as_stack()
-
+    
     def set_ram(self, target_ram_position, new_value):
         """
         Directly set a given value at a targeted RAM position.
 
         :param target_ram_position: The ram position to be altered
         :type target_ram_position: int
         :param new_value: The value to put at this RAM position
```

### Comparing `ocatari-1.0.5/ocatari/environments.py` & `ocatari-1.0.6/ocatari/environments.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/_helper_methods.py` & `ocatari-1.0.6/ocatari/ram/_helper_methods.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/adventure.py` & `ocatari-1.0.6/ocatari/ram/adventure.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/alien.py` & `ocatari-1.0.6/ocatari/ram/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/amidar.py` & `ocatari-1.0.6/ocatari/ram/amidar.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/assault.py` & `ocatari-1.0.6/ocatari/ram/assault.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,14 @@
     global horizontal_pos_right
     global horizontal_pos_left
 
     # player missile horizontal
     if ram_state[24] == 88:
         mis = PlayerMissileHorizontal()
         mis_offset = 2
-        # print(horizontal_pos)
         #if horizontal_pos == 0 or horizontal_pos > 130 or horizontal_pos < 20:
         #    horizontal_pos = player.x
         if horizontal_pos == 0:
             horizontal_pos_right = player.x + player.w + mis_offset
             horizontal_pos_left = player.x
 
         if ram_state[26] == 128:    # shot to the right
```

### Comparing `ocatari-1.0.5/ocatari/ram/asterix.py` & `ocatari-1.0.6/ocatari/ram/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/asterix_old.py` & `ocatari-1.0.6/ocatari/ram/asterix_old.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/asterix_old2.py` & `ocatari-1.0.6/ocatari/ram/asterix_old2.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/asteroids.py` & `ocatari-1.0.6/ocatari/ram/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/atlantis.py` & `ocatari-1.0.6/ocatari/ram/atlantis.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,14 @@
 
     prev_x_p1 = ram_state[60]
 
     if ram_state[59] != 0 and ram_state[61] != 0:
         proj = Projectile()
         if prev_x_p2 < ram_state[61]:
             proj.xy = ram_state[61]-3, missile_pos(ram_state[59])-1
-            # print("LEFT 2")
         elif prev_x_p2 == ram_state[61]:
             # proj.xy = ram_state[61], int(214 - 1.0775 * ram_state[59])
             proj.xy = ram_state[61], missile_pos(ram_state[59])
             # if 204 - ram_state[59] <= 22:
             #     proj.xy = ram_state[61], 210 - ram_state[59] - 9
             # elif 204 - ram_state[59] <= 32:
             #     proj.xy = ram_state[61], 210 - ram_state[59] - 8
@@ -274,23 +273,20 @@
             #     proj.xy = ram_state[61], 210 - ram_state[59] - 7
             # elif 204 - ram_state[59] <= 78:
             #     proj.xy = ram_state[61], 204 - ram_state[59]
             # elif 204 - ram_state[59] < 90:
             #     proj.xy = ram_state[61], 210 - ram_state[59] - 5
             # else:
             #     proj.xy = ram_state[61], 210 - ram_state[59] - 4
-            # print("CENTER 2")
         else:
             proj.xy = ram_state[61]+3, missile_pos(ram_state[59])-1
-            # print("RIGHT 2")
         objects.append(proj)
 
     prev_x_p2 = ram_state[61]
 
-    # print('-'*20)
     # The visual representation of the Sprite relative to the ram_state
     # seems to differ depending on the ship entering on the left/right.
     # These variables help to determine where the ship entered
     global prev_x1
     global prev_x2
     global prev_x3
     global prev_x4
@@ -457,15 +453,14 @@
         ray_available = False
 
     # Deathray can only be shot by ships on lane 4
     if ram_state[30] < 152 and ray_available:
         ray = Deathray()
         if prev_x4 < ram_state[36]:
             ray.xy = ram_state[36] - 1, 92
-            #print(ray.xy)
         else:
             ray.xy = ram_state[36] + 1, 92
         objects.append(ray)
 
     prev_x4 = ram_state[36]
     buildings_amount = buildings_count
```

### Comparing `ocatari-1.0.5/ocatari/ram/bankheist.py` & `ocatari-1.0.6/ocatari/ram/bankheist.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/battlezone.py` & `ocatari-1.0.6/ocatari/ram/battlezone.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/beamrider.py` & `ocatari-1.0.6/ocatari/ram/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/berzerk.py` & `ocatari-1.0.6/ocatari/ram/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/bowling.py` & `ocatari-1.0.6/ocatari/ram/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/boxing.py` & `ocatari-1.0.6/ocatari/ram/boxing.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,15 +153,14 @@
     player, enemy = objects[:2]
     player.xy = ram_state[32]+5, ram_state[34]+38
     player.right_arm_length = ram_state[57] # from 0 to 72
     player.left_arm_length = ram_state[55] # from 0 to 72
     enemy.xy = ram_state[33]+4, ram_state[35]+38
     enemy.left_arm_length = ram_state[61] # from 0 to 72
     enemy.right_arm_length = ram_state[59]
-    print(player.left_arm_length, player.right_arm_length)
     if hud:
         # scores
         global plscore
         global enscore
         plscore.value = ram_state[18]
         enscore.value = ram_state[19]
         if ram_state[19] > 10:  # enemy score
```

### Comparing `ocatari-1.0.5/ocatari/ram/breakout.py` & `ocatari-1.0.6/ocatari/ram/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/carnival.py` & `ocatari-1.0.6/ocatari/ram/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/centipede.py` & `ocatari-1.0.6/ocatari/ram/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/choppercommand.py` & `ocatari-1.0.6/ocatari/ram/choppercommand.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 MAX_NB_OBJECTS =  {'Player': 1, 'MiniPlayer': 1, 'Truck': 3, 'MiniTruck': 9, 'MiniEnemy': 12, 'Shot': 1, 'EnemyPlane': 3, 'EnemyHelicopter': 3, 'Bomb': 3}
 MAX_NB_OBJECTS_HUD =  {'Player': 1, 'Truck': 3, 'MiniPlayer': 1, 'MiniEnemy': 12, 'MiniTruck': 9, 'Shot': 1, 'EnemyPlane': 3, 'EnemyHelicopter': 3, 'Bomb': 3, 'Score': 4, 'Life': 2 }
 
 
 # parses MAX_NB* dicts, returns default init list of objects
 def _get_max_objects(hud=False):
-
     def fromdict(max_obj_dict):
         objects = []
         mod = sys.modules[__name__]
         for k, v in max_obj_dict.items():
             for _ in range(0, v):
                 objects.append(getattr(mod, k)())    
         return objects
@@ -518,15 +517,15 @@
     objects[3] = None
 
     for s in b_shot_line:
         if s:
             w = w + 4
         elif w > 0:
             shot = Shot()
-            shot.xy = x-w, player.y + 5 # last_y
+            shot.xy = x-w, 210-ram_state[65]-43 # player.y + 5 # last_y
             shot.wh = w, 1
             objects[3] = shot
             w = 0
         x = x + 4
 
     if ram_state[97] <= 100 and ram_state[97] >= 95:
         truck_x = 10
@@ -960,15 +959,18 @@
             for i in range(2):
                 score = Score()
                 score.xy = 75 - (i * 8), 16
                 objects[42+i] = score
         else:
             score = Score()
             objects[42] = score
-        score.value = _convert_number(ram_state[108]) * 10000 + _convert_number(ram_state[110]) * 100 + _convert_number(ram_state[112])
+        try:
+            score.value = _convert_number(ram_state[108]) * 10000 + _convert_number(ram_state[110]) * 100 + _convert_number(ram_state[112])
+        except:
+            pass
 
     # score
     # x: value 35+i*8
     # y: value 16
     # value: computable by 33,108,110,112
     # 33: score update
     # 108: hundred- and ten-thousands
```

### Comparing `ocatari-1.0.5/ocatari/ram/crazyclimber.py` & `ocatari-1.0.6/ocatari/ram/crazyclimber.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/demonattack.py` & `ocatari-1.0.6/ocatari/ram/demonattack.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/donkeykong.py` & `ocatari-1.0.6/ocatari/ram/donkeykong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/enduro.py` & `ocatari-1.0.6/ocatari/ram/enduro.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/extract_ram_info.py` & `ocatari-1.0.6/ocatari/ram/extract_ram_info.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/extract_ram_info_short.py` & `ocatari-1.0.6/ocatari/ram/extract_ram_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/fishingderby.py` & `ocatari-1.0.6/ocatari/ram/fishingderby.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
     p1s.wh = 3, 3
     p2s.wh = 3, 3
 
     # Considering that the first fish is the one at the top layer and
     fishes_hooked = []
     if ram_state[112] != 0:
-        fishes_hooked.append([6 - ram_state[112]])
+        fishes_hooked.append(6 - ram_state[112])
     if ram_state[113] != 0:
         fishes_hooked.append(6 - ram_state[113])
 
     for i in range(6):
         if i in fishes_hooked:
             objects[2 + i].hooked = True
         else:
```

### Comparing `ocatari-1.0.5/ocatari/ram/freeway.py` & `ocatari-1.0.6/ocatari/ram/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/frostbite.py` & `ocatari-1.0.6/ocatari/ram/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/game_objects.py` & `ocatari-1.0.6/ocatari/ram/game_objects.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/gopher.py` & `ocatari-1.0.6/ocatari/ram/gopher.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/hero.py` & `ocatari-1.0.6/ocatari/ram/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/icehockey.py` & `ocatari-1.0.6/ocatari/ram/icehockey.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/jamesbond.py` & `ocatari-1.0.6/ocatari/ram/jamesbond.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/kangaroo.py` & `ocatari-1.0.6/ocatari/ram/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/krull.py` & `ocatari-1.0.6/ocatari/ram/krull.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/montezumarevenge.py` & `ocatari-1.0.6/ocatari/ram/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/mspacman.py` & `ocatari-1.0.6/ocatari/ram/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/pacman.py` & `ocatari-1.0.6/ocatari/ram/pacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/pitfall.py` & `ocatari-1.0.6/ocatari/ram/pitfall.py`

 * *Files 2% similar despite different names*

```diff
@@ -537,18 +537,15 @@
     # import ipdb; ipdb.set_trace()
     if rope_visible:
         r = Rope()
         r.xy = get_pos_rope(ram_state)
         # r.xy = 78,106
         # if r.xy == (109,96):
         #     get_pos_rope(25, 67, 4)
-        #     print(ram_state[88],ram_state[89],ram_state[90])
         objects[10] = r
-        # print(r.xy)
-        # print(get_pos_rope(ram_state[88],ram_state[89],ram_state[90]))
 
     if hud:
         objects.extend([None] * 10)
         # PlayerScores related to ram_state 86 and 87
         p1 = PlayerScore()
         p1.value = _convert_number(ram_state[85])*1000 + _convert_number(ram_state[86]) * 100 + _convert_number(ram_state[87])
         size = 0
```

### Comparing `ocatari-1.0.5/ocatari/ram/pong.py` & `ocatari-1.0.6/ocatari/ram/pong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/privateeye.py` & `ocatari-1.0.6/ocatari/ram/privateeye.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/qbert.py` & `ocatari-1.0.6/ocatari/ram/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/riverraid.py` & `ocatari-1.0.6/ocatari/ram/riverraid.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,19 +227,14 @@
         objects[1] = None
     
     global cntr, prev11, prev70, enemies
     if ram_state[70] == 0 or ram_state[70] != prev70:
         speed = 1
     else: # hasn't fired yet
         speed = 0
-    # print(framskips)
-    # print(ram_state[70])
-    # if prev70 == 0 and ram_state[70]:
-    #     objects[2:8] = [None] * 6
-    # print(ram_state[11])
     if ram_state[11] < prev11: # every object drop
         enemies = enemies[1:] + [None]
         
     for i in range(6):
         en = enemies[i]
         obj_type = ram_state[32 + i]
         obj_class = _ram_to_class[obj_type]
```

### Comparing `ocatari-1.0.5/ocatari/ram/roadrunner.py` & `ocatari-1.0.6/ocatari/ram/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/seaquest.py` & `ocatari-1.0.6/ocatari/ram/seaquest.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/skiing.py` & `ocatari-1.0.6/ocatari/ram/skiing.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,34 +5,14 @@
 """
 RAM extraction for the game Skiing.
 """
 
 MAX_NB_OBJECTS =  {'Player': 1, 'Tree': 4, 'Mogul': 3, 'Flag': 4}
 MAX_NB_OBJECTS_HUD =  {'Player': 1, 'Tree': 4, 'Mogul': 3, 'Flag': 4, 'Score': 2, 'Clock': 7}
 
-# from termcolor import colored
-# def print_state(state):
-#     print("-"*10)
-#     for el in state:
-#         x, y, type = el
-#         coord = el[0:2]
-#         attr = []
-#         if y > 177 or y < 25 or x == 155:
-#             attr.append("dark")
-#         if type == 2:
-#             print(colored(coord, "blue", attrs=attr))
-#         elif type == 5:
-#             print(colored(coord, "grey", attrs=attr))
-#         elif type == 85:
-#             print(colored(coord, "green", attrs=attr))
-#         else:
-#             print(colored("Error in print_state", "red"))
-#             exit(1)
-#     print("-"*10)
-
 
 TREE_COLOR = {
     2: (110, 156, 66),
     3: (82, 126, 45),
     6: (158, 208, 101),
     7: (72, 160, 72),
 }
@@ -238,22 +218,15 @@
 
 
 # import numpy as np
 def _detect_objects_skiing_ram(objects, ram_state, hud=False):
     player = objects[0]
     player.xy = (ram_state[25], ram_state[26]-80)
     player.orientation = ram_state[15]
-    # info["speed"] = ram_state[14] or ram[20] both seem to have very similar behavior
-    # info["time"] = _time_skiing(ram_state)
     offset = 1 if not hud else 11
-    # xs = ram_state[62:70]
-    # ys = 178-ram_state[86:94]
-    # types = ram_state[70:78]
-    # state = np.array([xs, ys, types]).T
-    # print_state(state)
     for i in range(8):
         height = 75 - ram_state[90+i]
         type = ram_state[70+i]
         subtype = ram_state[78+i]
         x, y = ram_state[62+i], 178-ram_state[86+i]
         if offset < len(objects):
             currobj = objects[offset]
@@ -296,31 +269,29 @@
                 if not y == 28 or y == 27:
                     objects.append(Tree(x, y, subtype))
             else:
                 currobj.xy = x, y
                 if y <= 28:
                     currobj.wh = currobj.wh[0], height+2
         offset += 1
-    # print(objects)
 
 
 def _detect_objects_skiing_raw(info, ram_state):
     # player starts at x = 76
     relevant_info = ram_state[25:27] + ram_state[62:94]
     # info["player_x"] = ram_state[25]  # can go up to 150 (170 and you are back to the left side)
     # info["player_y"] = ram_state[26]  # constant 120
     info["score"] = _convert_number(ram_state[107])
     # info["speed"] = ram_state[14] or ram[20] both seem to have very similar behavior
     info["time"] = _time_skiing(ram_state)
     info["relavant_ram_info"] = relevant_info
     # info["object_x"] = ram_state[62:69]  # 69 is the newest object, 62 is the oldest
     # info["object_y"] = ram_state[86:94]  # 93 is the newest object, 86 is the oldest
     # info["object_type"] = ram_state[70:78]  # 77 is the newest object, 70 is the oldest | 85 tree | 2 flag | 5 mogul
-    # info["object_colour"] = ram_state[79:86]  # 85 is the newest object, 78 is the oldest  |probably not important
-    # print(ram_state)
+    # info["object_colour"] = ram_state[78:86]  # 85 is the newest object, 78 is the oldest  |probably not important
 
 
 def _time_skiing(ram_state):
     time = {}
     # minutes
     time["minutes"] = _convert_number(ram_state[104])
     # seconds
```

### Comparing `ocatari-1.0.5/ocatari/ram/spaceinvaders.py` & `ocatari-1.0.6/ocatari/ram/spaceinvaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 MAX_NB_OBJECTS_HUD = {'Player': 1, 'Shield': 3, 'Alien': 36, 'Bullet': 3, 'Satellite': 1, 'Score': 4, 'Lives': 2}
 
 
 def make_bitmap(alien_states):
     emptc = 6 - int(max(alien_states)).bit_length()  # nb empty columns
     return [(format(el, '06b')[emptc:] + "0" * emptc) for el in alien_states], emptc
 
-def print_bmp(bmp):
-    print(colored("\n".join(bmp)[::-1], "green"))
+# def print_bmp(bmp):
+#     print(colored("\n".join(bmp)[::-1], "green"))
 
 
 class Player(GameObject):
     """
     The player figure i.e., the laser cannon.
     """
     
@@ -191,15 +191,14 @@
     #
     # # for an array-value for score there is two digits and arithmetic transfer(like from ram_state[104]) gets added
     # # to most significant digits (ram_state[102])
     # info["score_player_green"] = {ram_state[102], ram_state[104]}  # score is saved in hexadecimal in this order
     # info["score_player_yellow"] = {ram_state[103], ram_state[105]}  # score is saved in hexadecimal
     # # 200 points for destroying satellite dish
     # # x*5 points for destroying an alien from row_x
-    # print(ram_state)
 
 
 def _init_objects_spaceinvaders_ram(hud=False):
     """
     (Re)Initialize the objects
     """
     objects = [Player(1)]
@@ -277,16 +276,14 @@
 
     # updating positions of aliens
     x, y = ram_state[26], ram_state[16]
 
     bitmap, emptc = make_bitmap(ram_state[18:24])
 
     # aliens (permanent) deletion from array aliens:
-    #print("-"*6)
-    #print_bmp(bitmap)
     for i in range(6):
         for j in range(6):
             if aliens[35 - (i * 6 + j)] and not int(bitmap[i][j]):  # enemies alive are saved in ram_state[18:24]
                 aliens[35 - (i * 6 + j)] = None  # 5 = max(range(6)) so we are counting lines in the other way around
             elif not aliens[35 - (i * 6 + j)] and int(bitmap[i][j]):
                 aliens[35 - (i * 6 + j)] = Alien() # 5 = max(range(6)) so we are counting lines in the other way around
```

### Comparing `ocatari-1.0.5/ocatari/ram/tennis.py` & `ocatari-1.0.6/ocatari/ram/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/timepilot.py` & `ocatari-1.0.6/ocatari/ram/timepilot.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/upndown.py` & `ocatari-1.0.6/ocatari/ram/upndown.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/utils.py` & `ocatari-1.0.6/ocatari/ram/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/venture.py` & `ocatari-1.0.6/ocatari/ram/venture.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/videopinball.py` & `ocatari-1.0.6/ocatari/ram/videopinball.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/ram/yarsrevenge.py` & `ocatari-1.0.6/ocatari/ram/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/utils.py` & `ocatari-1.0.6/ocatari/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -217,35 +217,27 @@
 #     if opt.path == "h":
 #         return HumanAgent()
 #     ckpt_path = Path(opt.path)
 
 
 def load_agent(opt, nb_actions=None):
     pth = opt if isinstance(opt, str) else opt.path
-    game = opt.game.replace("ALE/", "")
-    if "ALE/" in opt.game:
-        pth = pth.replace("ALE/", "").replace(".gz", f"_{game.lower()}.cleanrl")
-        ckpt = torch.load(pth, map_location=torch.device('cpu'))
-    
-    if "dqn" in pth:
+    if pth.endswith("dqn") or pth.endswith("c51"):
+        pth = pth.replace("ALE/", "")
         agent = AtariNet(nb_actions, distributional="c51" in pth)
-        ckpt2 = ckpt.copy()
-        ckpt2.clear()
-        for el in ckpt:
-            el2 = el.replace("_QNetwork__", "_AtariNet__")
-            ckpt2[el2] = ckpt[el]
-        agent.load_state_dict(ckpt2)
-    elif "c51" in pth:
-        agent = QNetwork(nb_actions)
-        agent.load_state_dict(ckpt["model_weights"])   
-    elif "ppo" in pth:
-        agent = PPOAgent(nb_actions)
-        agent.load_state_dict(ckpt["model_weights"]) 
-    else:
-        return None
+    elif pth.endswith("cleanrl_model"):
+        ckpt = torch.load(pth, map_location=torch.device('cpu'))
+        if "c51" in pth:
+            agent = QNetwork(nb_actions)
+            agent.load_state_dict(ckpt["model_weights"])   
+        elif "ppo" in pth:
+            agent = PPOAgent(nb_actions)
+            agent.load_state_dict(ckpt["model_weights"]) 
+        else:
+            return None
     
     return agent
 
 
 class RandomAgent():
     """
     A agent acting randomly (following a uniform distribution).
```

### Comparing `ocatari-1.0.5/ocatari/vision/adventure.py` & `ocatari-1.0.6/ocatari/vision/adventure.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/alien.py` & `ocatari-1.0.6/ocatari/vision/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/amidar.py` & `ocatari-1.0.6/ocatari/vision/amidar.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/assault.py` & `ocatari-1.0.6/ocatari/vision/assault.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/asterix.py` & `ocatari-1.0.6/ocatari/vision/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/asteroids.py` & `ocatari-1.0.6/ocatari/vision/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/atlantis.py` & `ocatari-1.0.6/ocatari/vision/atlantis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/bankheist.py` & `ocatari-1.0.6/ocatari/vision/bankheist.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/battlezone.py` & `ocatari-1.0.6/ocatari/vision/battlezone.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/beamrider.py` & `ocatari-1.0.6/ocatari/vision/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/berzerk.py` & `ocatari-1.0.6/ocatari/vision/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/bowling.py` & `ocatari-1.0.6/ocatari/vision/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/boxing.py` & `ocatari-1.0.6/ocatari/vision/boxing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/breakout.py` & `ocatari-1.0.6/ocatari/vision/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/carnival.py` & `ocatari-1.0.6/ocatari/vision/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/centipede.py` & `ocatari-1.0.6/ocatari/vision/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/choppercommand.py` & `ocatari-1.0.6/ocatari/vision/choppercommand.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/crazyclimber.py` & `ocatari-1.0.6/ocatari/vision/crazyclimber.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/demonattack.py` & `ocatari-1.0.6/ocatari/vision/demonattack.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/donkeykong.py` & `ocatari-1.0.6/ocatari/vision/donkeykong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/enduro.py` & `ocatari-1.0.6/ocatari/vision/enduro.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/extract_vision_info.py` & `ocatari-1.0.6/ocatari/vision/extract_vision_info.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/extract_vision_info_short.py` & `ocatari-1.0.6/ocatari/vision/extract_vision_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/fishingderby.py` & `ocatari-1.0.6/ocatari/vision/fishingderby.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/freeway.py` & `ocatari-1.0.6/ocatari/vision/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/frostbite.py` & `ocatari-1.0.6/ocatari/vision/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/game_objects.py` & `ocatari-1.0.6/ocatari/vision/game_objects.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/gopher.py` & `ocatari-1.0.6/ocatari/vision/gopher.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/hero.py` & `ocatari-1.0.6/ocatari/vision/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/icehockey.py` & `ocatari-1.0.6/ocatari/vision/icehockey.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/jamesbond.py` & `ocatari-1.0.6/ocatari/vision/jamesbond.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/kangaroo.py` & `ocatari-1.0.6/ocatari/vision/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/krull.py` & `ocatari-1.0.6/ocatari/vision/krull.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/montezumarevenge.py` & `ocatari-1.0.6/ocatari/vision/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/mspacman.py` & `ocatari-1.0.6/ocatari/vision/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/pacman.py` & `ocatari-1.0.6/ocatari/vision/pacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/pitfall.py` & `ocatari-1.0.6/ocatari/vision/pitfall.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/pong.py` & `ocatari-1.0.6/ocatari/vision/pong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/privateeye.py` & `ocatari-1.0.6/ocatari/vision/privateeye.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/qbert.py` & `ocatari-1.0.6/ocatari/vision/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/riverraid.py` & `ocatari-1.0.6/ocatari/vision/riverraid.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/roadrunner.py` & `ocatari-1.0.6/ocatari/vision/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/seaquest.py` & `ocatari-1.0.6/ocatari/vision/seaquest.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/skiing.py` & `ocatari-1.0.6/ocatari/vision/skiing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/spaceinvaders.py` & `ocatari-1.0.6/ocatari/vision/spaceinvaders.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/tennis.py` & `ocatari-1.0.6/ocatari/vision/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/timepilot.py` & `ocatari-1.0.6/ocatari/vision/timepilot.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/upndown.py` & `ocatari-1.0.6/ocatari/vision/upndown.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/utils.py` & `ocatari-1.0.6/ocatari/vision/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/venture.py` & `ocatari-1.0.6/ocatari/vision/venture.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/videopinball.py` & `ocatari-1.0.6/ocatari/vision/videopinball.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari/vision/yarsrevenge.py` & `ocatari-1.0.6/ocatari/vision/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/ocatari.egg-info/PKG-INFO` & `ocatari-1.0.6/ocatari.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 1.0.5
+Version: 1.0.6
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
 License: UNKNOWN
 Description: # Object-Centric Atari Environments
         Quentin Delfosse, Jannis Blüml, Bjarne Gregori, Sebastian Sztwiertnia, Anurag Maurya, Kévin-Lâm Quesnel and Simon Wulf
```

### Comparing `ocatari-1.0.5/ocatari.egg-info/SOURCES.txt` & `ocatari-1.0.6/ocatari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/setup.py` & `ocatari-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-__version__ = '1.0.5'
+__version__ = '1.0.6'
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
```

### Comparing `ocatari-1.0.5/tests/display_game.py` & `ocatari-1.0.6/tests/display_game.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/tests/display_game_both.py` & `ocatari-1.0.6/tests/display_game_both.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/tests/get_metrics.py` & `ocatari-1.0.6/tests/get_metrics.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/tests/metrics_utils.py` & `ocatari-1.0.6/tests/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/tests/plot_speed_results.py` & `ocatari-1.0.6/tests/plot_speed_results.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/tests/pong_test.py` & `ocatari-1.0.6/tests/pong_test.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/tests/test_explanation.py` & `ocatari-1.0.6/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/tests/test_game.py` & `ocatari-1.0.6/tests/test_game.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/tests/test_game_both.py` & `ocatari-1.0.6/tests/test_game_both.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/tests/test_game_both_interactive.py` & `ocatari-1.0.6/tests/test_game_both_interactive.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.5/tests/test_speed.py` & `ocatari-1.0.6/tests/test_speed.py`

 * *Files identical despite different names*

