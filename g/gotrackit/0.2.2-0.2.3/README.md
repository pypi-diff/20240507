# Comparing `tmp/gotrackit-0.2.2.tar.gz` & `tmp/gotrackit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotrackit-0.2.2.tar", last modified: Sat Apr 27 14:32:17 2024, max compression
+gzip compressed data, was "gotrackit-0.2.3.tar", last modified: Tue May  7 06:29:21 2024, max compression
```

## Comparing `gotrackit-0.2.2.tar` & `gotrackit-0.2.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.790742 gotrackit-0.2.2/
--rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     7664 2024-04-27 14:32:17.789766 gotrackit-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     6918 2024-04-27 00:03:13.000000 gotrackit-0.2.2/README.md
--rw-rw-rw-   0        0        0      795 2024-04-27 14:31:39.000000 gotrackit-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-27 14:32:17.790742 gotrackit-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.697977 gotrackit-0.2.2/src/
--rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.702964 gotrackit-0.2.2/src/gotrackit/
--rw-rw-rw-   0        0        0    15805 2024-04-25 09:18:31.000000 gotrackit-0.2.2/src/gotrackit/GlobalVal.py
--rw-rw-rw-   0        0        0    15773 2024-04-27 14:03:24.000000 gotrackit-0.2.2/src/gotrackit/MapMatch.py
--rw-rw-rw-   0        0        0      624 2023-12-31 13:24:06.000000 gotrackit-0.2.2/src/gotrackit/WrapsFunc.py
--rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.2/src/gotrackit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.708948 gotrackit-0.2.2/src/gotrackit/generation/
--rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.2/src/gotrackit/generation/GpsGen.py
--rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.2/src/gotrackit/generation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.715937 gotrackit-0.2.2/src/gotrackit/gps/
--rw-rw-rw-   0        0        0     4259 2024-04-18 12:43:12.000000 gotrackit-0.2.2/src/gotrackit/gps/GpsArray.py
--rw-rw-rw-   0        0        0     8007 2024-04-14 02:50:11.000000 gotrackit-0.2.2/src/gotrackit/gps/GpsTrip.py
--rw-rw-rw-   0        0        0     3888 2024-04-16 14:22:42.000000 gotrackit-0.2.2/src/gotrackit/gps/GpsXfer.py
--rw-rw-rw-   0        0        0    22508 2024-04-22 09:39:54.000000 gotrackit-0.2.2/src/gotrackit/gps/LocGps.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.2/src/gotrackit/gps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.719926 gotrackit-0.2.2/src/gotrackit/map/
--rw-rw-rw-   0        0        0    18317 2024-04-25 15:48:16.000000 gotrackit-0.2.2/src/gotrackit/map/Link.py
--rw-rw-rw-   0        0        0    35933 2024-04-27 14:20:15.000000 gotrackit-0.2.2/src/gotrackit/map/Net.py
--rw-rw-rw-   0        0        0     4607 2024-04-09 00:43:47.000000 gotrackit-0.2.2/src/gotrackit/map/Node.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.2/src/gotrackit/map/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.720924 gotrackit-0.2.2/src/gotrackit/model/
--rw-rw-rw-   0        0        0    64510 2024-04-27 14:30:20.000000 gotrackit-0.2.2/src/gotrackit/model/Markov.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.2/src/gotrackit/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.727910 gotrackit-0.2.2/src/gotrackit/netreverse/
--rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.2/src/gotrackit/netreverse/GlobalVal.py
--rw-rw-rw-   0        0        0    26847 2024-04-20 03:45:37.000000 gotrackit-0.2.2/src/gotrackit/netreverse/NetGen.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.729905 gotrackit-0.2.2/src/gotrackit/netreverse/Parse/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Parse/__init__.py
--rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Parse/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.735889 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/
--rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/GeoProcess.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/GraphAna.py
--rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/IndexAna.py
--rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/MapProcess.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/__init__.py
--rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/od.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.737892 gotrackit-0.2.2/src/gotrackit/netreverse/Request/
--rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.739878 gotrackit-0.2.2/src/gotrackit/netreverse/Request/api/
--rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/api/WebApi.py
--rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/api/__init__.py
--rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/request_path.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.743867 gotrackit-0.2.2/src/gotrackit/netreverse/Request/usage/
--rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/usage/__init__.py
--rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/usage/bd_ts.py
--rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/usage/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.750848 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.752843 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/DupProcess/
--rw-rw-rw-   0        0        0    21741 2024-03-18 03:07:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.757830 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/
--rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
--rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.763814 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    12225 2024-03-06 12:24:39.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
--rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.765808 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
--rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.770795 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    21559 2024-04-12 02:47:41.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.774784 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/SaveStreets/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
--rw-rw-rw-   0        0        0    21115 2024-03-15 13:54:11.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.776799 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Split/
--rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Split/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.777777 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Tools/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
--rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Tools/process.py
--rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/__init__.py
--rw-rw-rw-   0        0        0     9629 2024-03-27 15:52:33.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/conn.py
--rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/increment.py
--rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/net_reverse.py
--rw-rw-rw-   0        0        0     5758 2024-04-20 03:45:37.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/optimize_net.py
--rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/save_file.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/__init__.py
--rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.2/src/gotrackit/netreverse/book_mark.py
--rw-rw-rw-   0        0        0     1868 2024-01-27 14:19:15.000000 gotrackit-0.2.2/src/gotrackit/netreverse/format_od.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.779771 gotrackit-0.2.2/src/gotrackit/netxfer/
--rw-rw-rw-   0        0        0    17197 2024-04-16 10:06:45.000000 gotrackit-0.2.2/src/gotrackit/netxfer/SumoConvert.py
--rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.2/src/gotrackit/netxfer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.781766 gotrackit-0.2.2/src/gotrackit/solver/
--rw-rw-rw-   0        0        0     9156 2024-04-21 05:56:15.000000 gotrackit-0.2.2/src/gotrackit/solver/Viterbi.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.2/src/gotrackit/solver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.786752 gotrackit-0.2.2/src/gotrackit/tools/
--rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.2/src/gotrackit/tools/__init__.py
--rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.2/src/gotrackit/tools/coord_trans.py
--rw-rw-rw-   0        0        0    12119 2024-04-08 08:18:36.000000 gotrackit-0.2.2/src/gotrackit/tools/geo_process.py
--rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.2/src/gotrackit/tools/group.py
--rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.2/src/gotrackit/tools/save_file.py
--rw-rw-rw-   0        0        0     9708 2024-04-27 06:20:00.000000 gotrackit-0.2.2/src/gotrackit/visualization.py
-drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.788747 gotrackit-0.2.2/src/gotrackit.egg-info/
--rw-rw-rw-   0        0        0     7664 2024-04-27 14:32:17.000000 gotrackit-0.2.2/src/gotrackit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3695 2024-04-27 14:32:17.000000 gotrackit-0.2.2/src/gotrackit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 14:32:17.000000 gotrackit-0.2.2/src/gotrackit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-27 14:32:17.000000 gotrackit-0.2.2/src/gotrackit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-27 14:32:17.000000 gotrackit-0.2.2/src/gotrackit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.036558 gotrackit-0.2.3/
+-rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     7782 2024-05-07 06:29:21.036558 gotrackit-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7036 2024-05-07 06:17:50.000000 gotrackit-0.2.3/README.md
+-rw-rw-rw-   0        0        0      795 2024-05-07 06:20:09.000000 gotrackit-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 06:29:21.036558 gotrackit-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.953780 gotrackit-0.2.3/src/
+-rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.958766 gotrackit-0.2.3/src/gotrackit/
+-rw-rw-rw-   0        0        0    15805 2024-04-29 14:02:05.000000 gotrackit-0.2.3/src/gotrackit/GlobalVal.py
+-rw-rw-rw-   0        0        0    17874 2024-05-07 03:22:33.000000 gotrackit-0.2.3/src/gotrackit/MapMatch.py
+-rw-rw-rw-   0        0        0      624 2023-12-31 13:24:06.000000 gotrackit-0.2.3/src/gotrackit/WrapsFunc.py
+-rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.3/src/gotrackit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.966745 gotrackit-0.2.3/src/gotrackit/generation/
+-rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.3/src/gotrackit/generation/GpsGen.py
+-rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.3/src/gotrackit/generation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.971732 gotrackit-0.2.3/src/gotrackit/gps/
+-rw-rw-rw-   0        0        0     4275 2024-04-30 05:17:12.000000 gotrackit-0.2.3/src/gotrackit/gps/GpsArray.py
+-rw-rw-rw-   0        0        0     8007 2024-04-14 02:50:11.000000 gotrackit-0.2.3/src/gotrackit/gps/GpsTrip.py
+-rw-rw-rw-   0        0        0     3896 2024-04-30 05:17:12.000000 gotrackit-0.2.3/src/gotrackit/gps/GpsXfer.py
+-rw-rw-rw-   0        0        0    22763 2024-05-07 03:27:27.000000 gotrackit-0.2.3/src/gotrackit/gps/LocGps.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.3/src/gotrackit/gps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.974724 gotrackit-0.2.3/src/gotrackit/map/
+-rw-rw-rw-   0        0        0    19143 2024-05-07 03:27:27.000000 gotrackit-0.2.3/src/gotrackit/map/Link.py
+-rw-rw-rw-   0        0        0    38187 2024-05-07 05:58:17.000000 gotrackit-0.2.3/src/gotrackit/map/Net.py
+-rw-rw-rw-   0        0        0     4848 2024-05-07 05:58:17.000000 gotrackit-0.2.3/src/gotrackit/map/Node.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.3/src/gotrackit/map/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.975721 gotrackit-0.2.3/src/gotrackit/model/
+-rw-rw-rw-   0        0        0    65946 2024-05-07 05:18:41.000000 gotrackit-0.2.3/src/gotrackit/model/Markov.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.3/src/gotrackit/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.981706 gotrackit-0.2.3/src/gotrackit/netreverse/
+-rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.3/src/gotrackit/netreverse/GlobalVal.py
+-rw-rw-rw-   0        0        0    27388 2024-05-07 03:33:38.000000 gotrackit-0.2.3/src/gotrackit/netreverse/NetGen.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.983700 gotrackit-0.2.3/src/gotrackit/netreverse/Parse/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Parse/__init__.py
+-rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Parse/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.988686 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/
+-rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/GeoProcess.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/GraphAna.py
+-rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/IndexAna.py
+-rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/MapProcess.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/__init__.py
+-rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/od.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.990681 gotrackit-0.2.3/src/gotrackit/netreverse/Request/
+-rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.992676 gotrackit-0.2.3/src/gotrackit/netreverse/Request/api/
+-rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/api/WebApi.py
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/api/__init__.py
+-rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/request_path.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:20.995668 gotrackit-0.2.3/src/gotrackit/netreverse/Request/usage/
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/usage/__init__.py
+-rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/usage/bd_ts.py
+-rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.3/src/gotrackit/netreverse/Request/usage/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.001652 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.003646 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/DupProcess/
+-rw-rw-rw-   0        0        0    21741 2024-03-18 03:07:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.007635 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/
+-rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
+-rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.012627 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    12225 2024-03-06 12:24:39.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
+-rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.014617 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
+-rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.019604 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    21559 2024-04-12 02:47:41.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.020601 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/SaveStreets/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
+-rw-rw-rw-   0        0        0    21421 2024-04-30 12:21:10.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.023593 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Split/
+-rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Split/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.024590 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Tools/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
+-rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Tools/process.py
+-rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/__init__.py
+-rw-rw-rw-   0        0        0     9629 2024-03-27 15:52:33.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/conn.py
+-rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/increment.py
+-rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/net_reverse.py
+-rw-rw-rw-   0        0        0     5758 2024-04-20 03:45:37.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/optimize_net.py
+-rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/save_file.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.3/src/gotrackit/netreverse/__init__.py
+-rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.3/src/gotrackit/netreverse/book_mark.py
+-rw-rw-rw-   0        0        0     1868 2024-01-27 14:19:15.000000 gotrackit-0.2.3/src/gotrackit/netreverse/format_od.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.028581 gotrackit-0.2.3/src/gotrackit/netxfer/
+-rw-rw-rw-   0        0        0    17197 2024-04-16 10:06:45.000000 gotrackit-0.2.3/src/gotrackit/netxfer/SumoConvert.py
+-rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.3/src/gotrackit/netxfer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.030575 gotrackit-0.2.3/src/gotrackit/solver/
+-rw-rw-rw-   0        0        0     9156 2024-04-21 05:56:15.000000 gotrackit-0.2.3/src/gotrackit/solver/Viterbi.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.3/src/gotrackit/solver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.034564 gotrackit-0.2.3/src/gotrackit/tools/
+-rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.3/src/gotrackit/tools/__init__.py
+-rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.3/src/gotrackit/tools/coord_trans.py
+-rw-rw-rw-   0        0        0    12123 2024-05-06 03:34:25.000000 gotrackit-0.2.3/src/gotrackit/tools/geo_process.py
+-rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.3/src/gotrackit/tools/group.py
+-rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.3/src/gotrackit/tools/save_file.py
+-rw-rw-rw-   0        0        0    10550 2024-05-07 01:39:06.000000 gotrackit-0.2.3/src/gotrackit/visualization.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:29:21.035561 gotrackit-0.2.3/src/gotrackit.egg-info/
+-rw-rw-rw-   0        0        0     7782 2024-05-07 06:29:20.000000 gotrackit-0.2.3/src/gotrackit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3695 2024-05-07 06:29:20.000000 gotrackit-0.2.3/src/gotrackit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 06:29:20.000000 gotrackit-0.2.3/src/gotrackit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-07 06:29:20.000000 gotrackit-0.2.3/src/gotrackit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 06:29:20.000000 gotrackit-0.2.3/src/gotrackit.egg-info/top_level.txt
```

### Comparing `gotrackit-0.2.2/LICENSE` & `gotrackit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/PKG-INFO` & `gotrackit-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,34 +34,42 @@
 ![PyPI - Version](https://img.shields.io/pypi/v/gotrackit)
 ![GitHub License](https://img.shields.io/github/license/zdsjjtTLG/Trackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gotrackit)
 
 ~ 一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位 ~
 
-唐铠, 794568794@qq.com, tangkai@zhechengdata.com
+Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com
 </div>
 <br>
 
 
 
-**版本状态：04.27即将更新更新: v0.2.2**
+**版本状态：05.07已经更新: v0.2.3**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
-- 向量化改造, 且引入FMM(Fast Map Matching)路径预存储机制, 大规模路网匹配效率大幅度提升
 
-- 完善报错机制, 遇到GPS脏数据不再报错停止, 而是跳过, 并且在所有的agents计算完毕后输出有问题的agent编号
+- 效率优化, 相较于v0.2.2小幅度提升
+
+- crs判断BUG修复、境外路网构建失败BUG修复
+
+- 报错机制优化
+
+- 输出文件目录指定参数html_fldr废除, 改为out_fldr
+
+- 增加环路处理功能
+    
+- 增加匹配结果即时输出参数, 每匹配完一条轨迹可马上进行结果存储
 
-- BUG修复
 
 <br>
 
 <div align=center>
-~ v0.2.2效率将大幅度提升 ~
+~ v0.2.2效率将大幅度提升, 最高可以提升10倍的性能 !~
 </div>
 
 <br>
 
 与上一版本对比:
 
 | 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.2版解算时间 |
@@ -151,15 +159,15 @@
 
 **文档齐全**
 
 - 中文文档，有详细的操作指引；
 - 算法原理讲解部分不涉及复杂的公式推导，使用动画形式剖析算法原理,简洁明了。
 
 **匹配结果自动优化**
-- 对基于HMM匹配的初步路径进行了优化，对于不连通的位置会自动补路，对于实际路网不连通的位置会输出警告，方便用户检查路网。
+- 对基于HMM匹配的初步路径进行了优化，对于不连通的位置会自动搜路补全，对于实际路网不连通的位置会输出警告信息，方便用户回溯问题。
 
 
 
 ### 1.1. 如何安装gotrackit
 
 #### __所需前置依赖__
```

### Comparing `gotrackit-0.2.2/README.md` & `gotrackit-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,34 +12,42 @@
 ![PyPI - Version](https://img.shields.io/pypi/v/gotrackit)
 ![GitHub License](https://img.shields.io/github/license/zdsjjtTLG/Trackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gotrackit)
 
 ~ 一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位 ~
 
-唐铠, 794568794@qq.com, tangkai@zhechengdata.com
+Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com
 </div>
 <br>
 
 
 
-**版本状态：04.27即将更新更新: v0.2.2**
+**版本状态：05.07已经更新: v0.2.3**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
-- 向量化改造, 且引入FMM(Fast Map Matching)路径预存储机制, 大规模路网匹配效率大幅度提升
 
-- 完善报错机制, 遇到GPS脏数据不再报错停止, 而是跳过, 并且在所有的agents计算完毕后输出有问题的agent编号
+- 效率优化, 相较于v0.2.2小幅度提升
+
+- crs判断BUG修复、境外路网构建失败BUG修复
+
+- 报错机制优化
+
+- 输出文件目录指定参数html_fldr废除, 改为out_fldr
+
+- 增加环路处理功能
+    
+- 增加匹配结果即时输出参数, 每匹配完一条轨迹可马上进行结果存储
 
-- BUG修复
 
 <br>
 
 <div align=center>
-~ v0.2.2效率将大幅度提升 ~
+~ v0.2.2效率将大幅度提升, 最高可以提升10倍的性能 !~
 </div>
 
 <br>
 
 与上一版本对比:
 
 | 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.2版解算时间 |
@@ -129,15 +137,15 @@
 
 **文档齐全**
 
 - 中文文档，有详细的操作指引；
 - 算法原理讲解部分不涉及复杂的公式推导，使用动画形式剖析算法原理,简洁明了。
 
 **匹配结果自动优化**
-- 对基于HMM匹配的初步路径进行了优化，对于不连通的位置会自动补路，对于实际路网不连通的位置会输出警告，方便用户检查路网。
+- 对基于HMM匹配的初步路径进行了优化，对于不连通的位置会自动搜路补全，对于实际路网不连通的位置会输出警告信息，方便用户回溯问题。
 
 
 
 ### 1.1. 如何安装gotrackit
 
 #### __所需前置依赖__
```

### Comparing `gotrackit-0.2.2/pyproject.toml` & `gotrackit-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gotrackit"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = ["geopandas>=0.14.1", "shapely", "networkx", "pandas", "numpy", "keplergl", "geopy"]
 requires-python = ">=3.8"
 authors = [
   { name="Kai Tang", email="794568794@qq.com" },
 ]
 description = "A Python Package for Map Matching Algorithm Based on Hidden Markov Model"
 readme = "README.md"
```

### Comparing `gotrackit-0.2.2/src/gotrackit/GlobalVal.py` & `gotrackit-0.2.3/src/gotrackit/GlobalVal.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/MapMatch.py` & `gotrackit-0.2.3/src/gotrackit/MapMatch.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 
 
 class MapMatch(object):
     def __init__(self, flag_name: str = 'test', net: Net = None, use_sub_net: bool = True, gps_df: pd.DataFrame = None,
                  time_format: str = "%Y-%m-%d %H:%M:%S", time_unit: str = 's',
                  gps_buffer: float = 200.0, gps_route_buffer_gap: float = 15.0,
                  max_increment_times: int = 2, increment_buffer: float = 15.0,
-                 beta: float = 20.0, gps_sigma: float = 20.0, dis_para: float = 0.1,
+                 beta: float = 6.0, gps_sigma: float = 30.0, dis_para: float = 0.1,
                  is_lower_f: bool = False, lower_n: int = 2,
                  use_heading_inf: bool = False, heading_para_array: np.ndarray = None,
                  dense_gps: bool = True, dense_interval: float = 80.0,
                  dwell_l_length: float = 10.0, dwell_n: int = 2, del_dwell: bool = True,
                  dup_threshold: float = 10.0,
                  is_rolling_average: bool = False, window: int = 2,
-                 export_html: bool = False, use_gps_source: bool = False, html_fldr: str = None,
+                 export_html: bool = False, use_gps_source: bool = False, out_fldr: str = None,
                  export_geo_res: bool = False,
                  node_num_threshold: int = 2000, top_k: int = 20, omitted_l: float = 6.0,
                  link_width: float = 1.5, node_radius: float = 1.5,
                  match_link_width: float = 5.0, gps_radius: float = 6.0, export_all_agents: bool = False,
-                 visualization_cache_times: int = 50, multi_core_save: bool = False):
+                 visualization_cache_times: int = 50, multi_core_save: bool = False, instant_output: bool = False):
         """
         :param flag_name: 标记字符名称, 会用于标记输出的可视化文件, 默认"test"
         :param net: gotrackit路网对象, 必须指定
         :param use_sub_net: 是否在子网络上进行计算, 默认True
         :param gps_df: GPS数据, 必须指定
         :param time_format: GPS数据中时间列的格式, 默认"%Y-%m-%d %H:%M:%S"
         :param time_unit: GPS数据中时间列的单位, 如果时间列是数值(秒或者毫秒), 默认's'
@@ -60,22 +60,23 @@
         :param dense_gps: 是否对GPS数据进行加密, 默认False
         :param dense_interval: 当前后GPS点的直线距离l超过dense_interval即进行加密, 进行 int(l / dense_interval) + 1 等分加密, 默认25.0
         :param dup_threshold: 利用GPS轨迹计算sub_net时, 先对GPS点原始轨迹做简化, 重复点检测阈值, 默认5m
         :param is_rolling_average: 是否启用滑动窗口平均对GPS数据进行降噪, 默认False
         :param window: 滑动窗口大小, 默认2
         :param export_html: 是否输出网页可视化结果html文件, 默认True
         :param use_gps_source: 是否在可视化结果中使用GPS源数据进行展示, 默认False
-        :param html_fldr: 保存网页可视化结果的文件目录, 默认当前目录
+        :param out_fldr: 保存匹配结果的文件目录, 默认当前目录
         :param export_geo_res: 是否输出匹配结果的几何可视化文件, 默认False
         :param node_num_threshold: 默认2000
         :param omitted_l: 当某GPS点与前后GPS点的平均距离小于该距离(m)时, 该GPS点的方向限制作用被取消
         :param gps_radius: HTML可视化中GPS点的半径大小，单位米，默认8米
         :param export_all_agents: 是否将所有agent的可视化存储于一个html文件中
-        :param visualization_cache_times: 每匹配完几辆车再进行结果的统一存储, 默认50
+        :param visualization_cache_times: 每匹配完几辆车再进行(html or geojson文件)结果的统一存储, 默认50
         :param multi_core_save: 是否启用多进程进行结果存储
+        :param instant_output: 是否每匹配完一条轨迹就存储csv匹配结果
         """
         # 坐标系投影
         self.plain_crs = net.planar_crs
         self.geo_crs = net.geo_crs
 
         # 用于自动确定是否使用全局路网的指标
         self.node_num_threshold = node_num_threshold
@@ -111,15 +112,15 @@
         self.beta = beta  # 状态转移概率参数, 概率与之成正比
         self.gps_sigma = gps_sigma  # 发射概率参数, 概率与之成正比
         self.flag_name = flag_name
         self.dis_para = dis_para
 
         self.export_html = export_html
         self.export_geo_res = export_geo_res
-        self.html_fldr = html_fldr
+        self.out_fldr = r'./' if out_fldr is None else out_fldr
 
         self.may_error_list = dict()
         self.error_list = list()
 
         self.my_net = net
         self.not_conn_cost = self.my_net.not_conn_cost
         self.use_gps_source = use_gps_source
@@ -130,14 +131,15 @@
         self.match_link_width = match_link_width
         self.gps_radius = gps_radius
 
         self.export_all_agents = export_all_agents
         self.visualization_cache_times = visualization_cache_times
         self.multi_core_save = multi_core_save
         self.sub_net_buffer = self.gps_buffer + self.gps_route_buffer_gap + max_increment_times * increment_buffer
+        self.instant_output = instant_output
 
     def execute(self) -> tuple[pd.DataFrame, dict, list]:
         match_res_df = pd.DataFrame()
         hmm_res_list = []  # save hmm_res
         if len(self.my_net.get_node_data()[node_id_field].unique()) <= self.node_num_threshold:
             self.use_sub_net = False
         self.gps_df.dropna(subset=[agent_id_field], inplace=True)
@@ -148,37 +150,57 @@
 
         # 对每辆车的轨迹进行匹配
         agent_count = 0
         add_single_ft = [True]
         for agent_id, _gps_df in self.gps_df.groupby(gps_field.AGENT_ID_FIELD):
             agent_count += 1
             print(rf'- gotrackit ------> No.{agent_count}: agent: {agent_id} ')
-            gps_obj = GpsPointsGdf(gps_points_df=_gps_df, time_format=self.time_format,
-                                   buffer=self.gps_buffer, time_unit=self.time_unit,
-                                   plane_crs=self.plain_crs,
-                                   max_increment_times=self.max_increment_times, increment_buffer=self.increment_buffer,
-                                   dense_gps=self.dense_gps, dense_interval=self.dense_interval,
-                                   dwell_l_length=self.dwell_l_length, dwell_n=self.dwell_n)
+            try:
+                gps_obj = GpsPointsGdf(gps_points_df=_gps_df, time_format=self.time_format,
+                                       buffer=self.gps_buffer, time_unit=self.time_unit,
+                                       plane_crs=self.plain_crs,
+                                       max_increment_times=self.max_increment_times,
+                                       increment_buffer=self.increment_buffer,
+                                       dense_gps=self.dense_gps, dense_interval=self.dense_interval,
+                                       dwell_l_length=self.dwell_l_length, dwell_n=self.dwell_n)
+            except Exception as e:
+                print('构建按GPS对象出错...')
+                print(repr(e))
+                self.error_list.append(agent_id)
+                continue
+
             del _gps_df
 
-            if self.del_dwell:
-                gps_obj.del_dwell_points()
+            # gps-process
+            try:
+                if self.del_dwell:
+                    print(rf'gps-preprocessing: del dwell')
+                    gps_obj.del_dwell_points()
+
+                # 降频处理
+                if self.is_lower_f:
+                    print(rf'gps-preprocessing: lower frequency, size: {self.lower_n}')
+                    gps_obj.lower_frequency(n=self.lower_n)
+
+                if self.is_rolling_average:
+                    print(rf'gps-preprocessing: rolling average, window size: {self.rolling_window}')
+                    gps_obj.rolling_average(window=self.rolling_window)
+
+                if self.dense_gps:
+                    print(rf'gps-preprocessing: dense gps by interval: {self.dense_interval}m')
+                    gps_obj.dense()
+            except Exception as e:
+                print(rf'gps数据预处理出错:{repr(e)}')
+                self.error_list.append(agent_id)
+                continue
 
-            # 降频处理
-            if self.is_lower_f:
-                print(rf'lower {self.lower_n} - frequency')
-                gps_obj.lower_frequency(n=self.lower_n)
-
-            if self.is_rolling_average:
-                print(rf'rolling average by window size - {self.rolling_window}')
-                gps_obj.rolling_average(window=self.rolling_window)
-
-            if self.dense_gps:
-                print(rf'dense gps by interval - {self.dense_interval}m')
-                gps_obj.dense()
+            if len(gps_obj.gps_gdf) <= 1:
+                print(r'经过数据预处理后GPS观测点数据不足2个')
+                self.error_list.append(agent_id)
+                continue
 
             # 依据当前的GPS数据(源数据)做一个子网络
             if self.use_sub_net:
                 print(rf'using sub net')
                 used_net = self.my_net.create_computational_net(
                     gps_array_buffer=gps_obj.get_gps_array_buffer(buffer=self.sub_net_buffer,
                                                                   dup_threshold=self.dup_threshold),
@@ -195,52 +217,77 @@
             # 初始化一个隐马尔可夫模型
             hmm_obj = HiddenMarkov(net=used_net, gps_points=gps_obj, beta=self.beta, gps_sigma=self.gps_sigma,
                                    not_conn_cost=self.not_conn_cost, use_heading_inf=self.use_heading_inf,
                                    heading_para_array=self.heading_para_array, dis_para=self.dis_para,
                                    top_k=self.top_k, omitted_l=self.omitted_l)
 
             # 求解参数
-            is_success = hmm_obj.generate_markov_para(add_single_ft)
+            try:
+                is_success = hmm_obj.generate_markov_para(add_single_ft)
+            except Exception as e:
+                print(rf'解算HMM参数出错:{repr(e)}')
+                is_success = False
             if not is_success:
+                self.error_list.append(agent_id)
+                continue
+
+            # 求解模型
+            try:
+                hmm_obj.solve()
+            except Exception as e:
+                print(rf'求解HMM模型出错:{repr(e)}')
+                self.error_list.append(agent_id)
+                continue
+
+            # 获取结果
+            try:
+                _match_res_df = hmm_obj.acquire_res()
+            except Exception as e:
+                print(rf'获取匹配结果出错:{repr(e)}')
+                self.error_list.append(agent_id)
                 continue
-            hmm_obj.solve()
-            _match_res_df = hmm_obj.acquire_res()
+            if self.instant_output:
+                _match_res_df.to_csv(os.path.join(self.out_fldr, rf'{agent_id}_match_res.csv'),
+                                     encoding='utf_8_sig', index=False)
+            else:
+                match_res_df = pd.concat([match_res_df, _match_res_df])
+
             hmm_obj.format_war_info()
             if hmm_obj.is_warn:
                 self.may_error_list[agent_id] = hmm_obj.format_warn_info
-            match_res_df = pd.concat([match_res_df, _match_res_df])
 
             # if export files
             if self.export_html or self.export_geo_res:
                 hmm_res_list.append(hmm_obj)
                 if len(hmm_res_list) >= self.visualization_cache_times or agent_count == agent_num:
                     export_visualization(hmm_obj_list=hmm_res_list, use_gps_source=self.use_gps_source,
                                          export_geo=self.export_geo_res, export_html=self.export_html,
                                          gps_radius=self.gps_radius, export_all_agents=self.export_all_agents,
-                                         out_fldr=self.html_fldr, flag_name=self.flag_name,
-                                         multi_core_save=self.multi_core_save)
+                                         out_fldr=self.out_fldr, flag_name=self.flag_name,
+                                         multi_core_save=self.multi_core_save, sub_net_buffer=self.sub_net_buffer,
+                                         dup_threshold=self.dup_threshold)
                     del hmm_res_list
                     hmm_res_list = []
 
         return match_res_df, self.may_error_list, self.error_list
 
     def multi_core_execute(self, core_num: int = 2) -> tuple[pd.DataFrame, dict, list]:
         agent_id_list = list(self.gps_df[gps_field.AGENT_ID_FIELD].unique())
         core_num = os.cpu_count() if core_num > os.cpu_count() else core_num
         agent_group = cut_group(agent_id_list, n=core_num)
         n = len(agent_group)
         print(f'using multiprocessing - {n} cores')
         pool = multiprocessing.Pool(processes=n)
         result_list = []
         for i in range(0, n):
-            core_html_fldr = os.path.join(self.html_fldr, rf'core{i}')
-            if os.path.exists(core_html_fldr):
+            core_out_fldr = os.path.join(self.out_fldr, rf'core{i}')
+            if os.path.exists(core_out_fldr):
                 pass
             else:
-                os.makedirs(core_html_fldr)
+                os.makedirs(core_out_fldr)
 
             agent_id_list = agent_group[i]
             gps_df = self.gps_df[self.gps_df[gps_field.AGENT_ID_FIELD].isin(agent_id_list)]
             mmp = MapMatch(gps_df=gps_df, net=self.my_net, use_sub_net=self.use_sub_net, time_format=self.time_format,
                            time_unit=self.time_unit, gps_buffer=self.gps_buffer,
                            gps_route_buffer_gap=self.gps_route_buffer_gap,
                            max_increment_times=self.max_increment_times, increment_buffer=self.increment_buffer,
@@ -250,23 +297,23 @@
                            use_heading_inf=self.use_heading_inf, heading_para_array=self.heading_para_array,
                            dense_gps=self.dense_gps,
                            dense_interval=self.dense_interval, dwell_l_length=self.dwell_l_length, dwell_n=self.dwell_n,
                            del_dwell=self.del_dwell,
                            dup_threshold=self.dup_threshold, is_rolling_average=self.is_rolling_average,
                            window=self.rolling_window,
                            export_html=self.export_html,
-                           use_gps_source=self.use_gps_source, html_fldr=core_html_fldr,
+                           use_gps_source=self.use_gps_source, out_fldr=core_out_fldr,
                            export_geo_res=self.export_geo_res,
                            node_num_threshold=self.node_num_threshold,
                            top_k=self.top_k, omitted_l=self.omitted_l, link_width=self.link_width,
                            node_radius=self.node_radius,
                            match_link_width=self.match_link_width, gps_radius=self.gps_radius,
                            export_all_agents=self.export_all_agents,
                            visualization_cache_times=self.visualization_cache_times,
-                           multi_core_save=False)
+                           multi_core_save=False, instant_output=self.instant_output)
             result = pool.apply_async(mmp.execute,
                                       args=())
             result_list.append(result)
         pool.close()
         pool.join()
 
         match_res, may_error, error = pd.DataFrame(), dict(), list()
```

### Comparing `gotrackit-0.2.2/src/gotrackit/WrapsFunc.py` & `gotrackit-0.2.3/src/gotrackit/WrapsFunc.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/generation/GpsGen.py` & `gotrackit-0.2.3/src/gotrackit/generation/GpsGen.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/gps/GpsArray.py` & `gotrackit-0.2.3/src/gotrackit/gps/GpsArray.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,23 +66,23 @@
         return self.gps_points_gdf.copy()
 
     @property
     def crs(self):
         return self.__crs
 
     def to_plane_prj(self) -> None:
-        if self.gps_points_gdf.crs.srs == self.plane_crs:
+        if self.gps_points_gdf.crs.srs.upper() == self.plane_crs:
             self.__crs = self.plane_crs
             pass
         else:
             self.gps_points_gdf = self.gps_points_gdf.to_crs(self.plane_crs)
             self.__crs = self.plane_crs
 
     def to_geo_prj(self) -> None:
-        if self.gps_points_gdf.crs.srs == self.geo_crs:
+        if self.gps_points_gdf.crs.srs.upper() == self.geo_crs:
             self.__crs = self.geo_crs
             pass
         else:
             self.gps_points_gdf = self.gps_points_gdf.to_crs(self.geo_crs)
             self.__crs = self.geo_crs
 
     @property
```

### Comparing `gotrackit-0.2.2/src/gotrackit/gps/GpsTrip.py` & `gotrackit-0.2.3/src/gotrackit/gps/GpsTrip.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/gps/GpsXfer.py` & `gotrackit-0.2.3/src/gotrackit/gps/GpsXfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         """
 
         :param path_gdf: path_id, seq, time_cost, geometry
         :param path_o_time_df: path_id, o_time(datetime format)
         :return:
         """
 
-        assert path_gdf.crs.srs == 'EPSG:4326'
+        assert path_gdf.crs.srs.upper() == 'EPSG:4326'
         assert len(path_o_time_df) >= 1
         assert {path_id_field, seq_field, time_cost_field, geometry_field}.issubset(set(path_gdf.columns))
         assert {path_id_field, o_time_field}.issubset(set(path_o_time_df.columns))
         self.path_gdf = path_gdf
         self.path_o_time_df = path_o_time_df
         self.path_gdf = self.path_gdf.to_crs(planar_crs)
         self.path_gdf[geometry_field] = self.path_gdf[geometry_field].remove_repeated_points(5.0)
```

### Comparing `gotrackit-0.2.2/src/gotrackit/gps/LocGps.py` & `gotrackit-0.2.3/src/gotrackit/gps/LocGps.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
                                                  crs=self.geo_crs)
         try:
             self.__gps_points_gdf[gps_field.TIME_FIELD] = \
                 pd.to_datetime(self.__gps_points_gdf[gps_field.TIME_FIELD], format=time_format)
         except ValueError:
             self.__gps_points_gdf[gps_field.TIME_FIELD] = \
                 pd.to_datetime(self.__gps_points_gdf[gps_field.TIME_FIELD], unit=time_unit)
+
         self.__gps_points_gdf.sort_values(by=[gps_field.TIME_FIELD], ascending=[True], inplace=True)
         self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD] = [i for i in range(len(self.__gps_points_gdf))]
         self.__gps_points_gdf[gps_field.ORIGIN_POINT_SEQ_FIELD] = self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD]
         self.__gps_points_gdf.reset_index(inplace=True, drop=True)
         self.to_plane_prj()
         # self.calc_gps_point_dis()
 
@@ -148,23 +149,28 @@
         self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD] = [i for i in range(len(self.__gps_points_gdf))]
         self.__gps_points_gdf[gps_field.ORIGIN_POINT_SEQ_FIELD] = self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD]
 
     def calc_adj_dis_gap(self) -> None:
         # 距离差
         self.__gps_points_gdf[next_p_field] = self.__gps_points_gdf[geometry_field].shift(-1).fillna(
             self.__gps_points_gdf[geometry_field])
-        self.__gps_points_gdf[dis_gap_field] = self.__gps_points_gdf.apply(
-            lambda row: row[next_p_field].distance(row[geometry_field]), axis=1)
+        # self.__gps_points_gdf[dis_gap_field] = self.__gps_points_gdf.apply(
+        #     lambda row: row[next_p_field].distance(row[geometry_field]), axis=1)
+        self.__gps_points_gdf[dis_gap_field] = self.__gps_points_gdf[next_p_field].distance(
+            self.__gps_points_gdf[geometry_field])
 
     def calc_adj_time_gap(self) -> None:
         # 时间差
         self.__gps_points_gdf[next_time_field] = self.__gps_points_gdf[time_field].shift(-1).fillna(
             self.__gps_points_gdf[time_field])
-        self.__gps_points_gdf[time_gap_field] = self.__gps_points_gdf.apply(
-            lambda row: (row[next_time_field] - row[time_field]).seconds, axis=1)
+        # self.__gps_points_gdf[time_gap_field] = self.__gps_points_gdf.apply(
+        #     lambda row: (row[next_time_field] - row[time_field]).seconds, axis=1)
+        self.__gps_points_gdf[time_gap_field] = self.__gps_points_gdf[next_time_field] - self.__gps_points_gdf[
+            time_field]
+        self.__gps_points_gdf[time_gap_field] = self.__gps_points_gdf[time_gap_field].apply(lambda x: x.seconds)
 
     def calc_pre_next_dis(self) -> pd.DataFrame():
         self.calc_adj_dis_gap()
         # next_seq
         res = self.__gps_points_gdf.copy()
         res[next_seq_field] = res[gps_field.POINT_SEQ_FIELD].shift(-1)
         res.dropna(subset=[next_seq_field], inplace=True)
@@ -285,31 +291,27 @@
 
     @property
     def crs(self):
         return self.__crs
 
     def get_gps_array_buffer(self, buffer: float = 200.0, dup_threshold: float = 10.0) -> Polygon or None:
         """输出gps路径的buffer范围面域"""
-        if len(self.__gps_points_gdf) <= 1:
-            print(r'经过数据预处理后GPS观测点数据不足2个')
-            return None
-        else:
-            gps_route_l = gpd.GeoSeries(LineString(self.__gps_points_gdf[gps_field.GEOMETRY_FIELD].to_list()))
-            simplify_gps_route_l = gps_route_l.remove_repeated_points(dup_threshold)
-            gps_array_buffer = simplify_gps_route_l[0].buffer(buffer)
-            return gps_array_buffer
+        gps_route_l = gpd.GeoSeries(LineString(self.__gps_points_gdf[gps_field.GEOMETRY_FIELD].to_list()))
+        simplify_gps_route_l = gps_route_l.remove_repeated_points(dup_threshold)
+        gps_array_buffer = simplify_gps_route_l[0].buffer(buffer)
+        return gps_array_buffer
 
     def generate_candidate_link(self, net: Net = None) -> tuple[pd.DataFrame, list[int]]:
         """
         计算GPS观测点的候选路段
         :param net:
         :return: GPS候选路段信息, 未匹配到候选路段的gps点id
         """
         gps_buffer_gdf = self.__gps_points_gdf[[gps_field.POINT_SEQ_FIELD, gps_field.GEOMETRY_FIELD]].copy()
-        if gps_buffer_gdf.crs.srs != self.plane_crs:
+        if gps_buffer_gdf.crs.srs.upper() != self.plane_crs:
             gps_buffer_gdf = gps_buffer_gdf.to_crs(self.plane_crs)
 
         single_link_gdf = net.get_link_data()[[net_field.SINGLE_LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
                                                net_field.TO_NODE_FIELD, net_field.DIRECTION_FIELD,
                                                net_field.LENGTH_FIELD, net_field.GEOMETRY_FIELD]]
         single_link_gdf.reset_index(inplace=True, drop=True)
         candidate_link = pd.DataFrame()
@@ -340,23 +342,23 @@
             candidate_link = pd.merge(candidate_link,
                                       single_link_gdf[[net_field.SINGLE_LINK_ID_FIELD, 'single_link_geo']],
                                       on=net_field.SINGLE_LINK_ID_FIELD, how='left')
             candidate_link.reset_index(inplace=True, drop=True)
         return candidate_link, remain_gps_list
 
     def to_plane_prj(self) -> None:
-        if self.__gps_points_gdf.crs.srs == self.plane_crs:
+        if self.__gps_points_gdf.crs.srs.upper() == self.plane_crs:
             self.__crs = self.plane_crs
             pass
         else:
             self.__gps_points_gdf = self.__gps_points_gdf.to_crs(self.plane_crs)
             self.__crs = self.plane_crs
 
     def to_geo_prj(self) -> None:
-        if self.__gps_points_gdf.crs.srs == self.geo_crs:
+        if self.__gps_points_gdf.crs.srs.upper() == self.geo_crs:
             self.__crs = self.geo_crs
             pass
         else:
             self.__gps_points_gdf = self.__gps_points_gdf.to_crs(self.geo_crs)
             self.__crs = self.geo_crs
 
     def get_point(self, seq: int = 0):
```

### Comparing `gotrackit-0.2.2/src/gotrackit/map/Link.py` & `gotrackit-0.2.3/src/gotrackit/map/Link.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,50 +3,49 @@
 # @Author  : TangKai
 # @Team    : ZheChengData
 
 """
 路网线层存储与相关方法
 """
 
-import warnings
 import numpy as np
 import pandas as pd
 import networkx as nx
 import geopandas as gpd
 from shapely.geometry import LineString
 from ..GlobalVal import NetField, PrjConst
 from ..WrapsFunc import function_time_cost
 from ..netreverse.RoadNet.Tools.process import merge_double_link
 
 net_field = NetField()
 prj_const = PrjConst()
 
-
 geo_crs = prj_const.PRJ_CRS
 link_id_field = net_field.LINK_ID_FIELD
 dir_field = net_field.DIRECTION_FIELD
 from_node_field = net_field.FROM_NODE_FIELD
 to_node_field = net_field.TO_NODE_FIELD
 length_field = net_field.LENGTH_FIELD
 geometry_field = net_field.GEOMETRY_FIELD
 link_vec_field = net_field.LINK_VEC_FIELD
 
 
 class Link(object):
     def __init__(self, link_gdf: gpd.GeoDataFrame = None, planar_crs: str = None,
                  weight_field: str = None, is_check: bool = True, not_conn_cost: float = 999.0,
-                 init_available_link: bool = True):
+                 init_available_link: bool = True, delete_circle: bool = True):
 
         self.not_conn_cost = not_conn_cost
         self.geo_crs = geo_crs
         self.planar_crs = planar_crs
         self.link_gdf = link_gdf.copy()
         self.link_gdf.index = self.link_gdf[link_id_field]
         self.weight_field = weight_field
         self.__available_link_id = []
+        self.delete_circle = delete_circle
         if is_check:
             self.check()
         self.max_link_id = 999
         if init_available_link:
             self.init_available_link_id()
         self.__single_link_gdf = gpd.GeoDataFrame()
         self.__double_single_mapping: dict[int, tuple[int, int, int, int]] = dict()
@@ -55,28 +54,36 @@
         self.__graph = nx.DiGraph()
         self.__ud_graph = nx.Graph()
         self.__one_out_degree_nodes = None
         self.__link_ft_mapping: dict[int, tuple[int, int]] = dict()
         self.done_link_vec = False
 
     def check(self):
-        assert self.link_gdf.crs.srs == self.geo_crs, rf'Link层数据必须为WGS84 - EPSG:4326, 实际输入: {self.link_gdf.crs.srs}'
+        assert self.link_gdf.crs.srs.upper() == self.geo_crs, \
+            rf'Link层数据必须为WGS84 - EPSG:4326, 实际输入: {self.link_gdf.crs.srs}'
         gap_set = {net_field.LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
                    net_field.TO_NODE_FIELD, net_field.DIRECTION_FIELD, self.weight_field,
                    net_field.GEOMETRY_FIELD} - set(self.link_gdf.columns)
         assert len(gap_set) == 0, rf'线层Link缺少以下字段:{gap_set}'
         assert len(self.link_gdf[net_field.LINK_ID_FIELD]) == len(self.link_gdf[net_field.LINK_ID_FIELD].unique()), \
             rf'字段{net_field.LINK_ID_FIELD}不唯一...'
         assert set(self.link_gdf[net_field.DIRECTION_FIELD]).issubset({0, 1}), \
             rf'{net_field.DIRECTION_FIELD}字段值只能为0或者1'
         for col in [net_field.LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
                     net_field.TO_NODE_FIELD, net_field.DIRECTION_FIELD]:
             assert len(self.link_gdf[self.link_gdf[col].isna()]) == 0, rf'线层Link字段{col}有空值...'
             self.link_gdf[col] = self.link_gdf[col].astype(int)
 
+        # 环路检测
+        if self.delete_circle:
+            circle_idx = self.link_gdf[from_node_field] == self.link_gdf[to_node_field]
+            if not self.link_gdf[circle_idx].empty:
+                print(rf'检测到线层数据有环路, 自动删除...')
+                self.link_gdf.drop(index=self.link_gdf[circle_idx].index, inplace=True, axis=0)
+
     def init_link(self):
         """
         初始化Link, 这里会创建一个single层的link, 并将single_link设置为索引
         :return:
         """
         self.create_single_link(link_gdf=self.link_gdf)
         self.__single_link_gdf.set_index(net_field.SINGLE_LINK_ID_FIELD, inplace=True)
@@ -107,15 +114,17 @@
             self.__single_link_gdf = link_gdf.copy()
         else:
             neg_link[[net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD]] = neg_link[
                 [net_field.TO_NODE_FIELD, net_field.FROM_NODE_FIELD]]
             neg_link[net_field.GEOMETRY_FIELD] = neg_link[net_field.GEOMETRY_FIELD].apply(
                 lambda line_geo: LineString(list(line_geo.coords)[::-1]))
             self.__single_link_gdf = pd.concat([link_gdf, neg_link])
-            self.__single_link_gdf.reset_index(inplace=True, drop=True)
+            # self.__single_link_gdf.reset_index(inplace=True, drop=True)
+        self.__single_link_gdf.drop_duplicates(subset=[from_node_field, to_node_field], keep='first', inplace=True)
+        self.__single_link_gdf.reset_index(inplace=True, drop=True)
         self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD] = [i for i in range(1, len(self.__single_link_gdf) + 1)]
         self.__single_link_gdf['path'] = self.__single_link_gdf.apply(
             lambda row: [row[net_field.FROM_NODE_FIELD], row[net_field.TO_NODE_FIELD]], axis=1)
         self.__double_single_mapping = {single_link_id: (link_id, int(direction), f, t) for
                                         single_link_id, link_id, direction, f, t in
                                         zip(self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD],
                                             self.__single_link_gdf[net_field.LINK_ID_FIELD],
@@ -195,15 +204,15 @@
                      dir_field: dir_val, geometry_field: geo}
         attr_dict.update(kwargs)
         self.link_gdf = pd.concat(
             [self.link_gdf, gpd.GeoDataFrame(attr_dict, geometry=geometry_field, crs=self.link_gdf.crs.srs)])
         self.link_gdf.index = self.link_gdf[link_id_field]
 
     def append_link_gdf(self, link_gdf: gpd.GeoDataFrame = None) -> None:
-        assert link_gdf.crs.srs == self.crs
+        assert link_gdf.crs.srs.upper() == self.crs
         assert set(link_gdf[link_id_field]) & set(self.link_gdf[link_id_field]) == set()
         self.link_gdf = pd.concat(
             [self.link_gdf, link_gdf])
         self.link_gdf.index = self.link_gdf[link_id_field]
 
     def renew_single_link(self):
         pass
@@ -309,33 +318,37 @@
     def get_geo_by_ft(self, from_node: int = None, to_node: int = None) -> LineString:
         return self.__single_link_gdf.at[self.__ft_link_mapping[(from_node, to_node)], net_field.GEOMETRY_FIELD]
 
     def get_ft_link_mapping(self) -> dict[tuple[int, int], int]:
         return self.__ft_link_mapping
 
     def to_plane_prj(self) -> None:
-        if self.link_gdf.crs.srs == self.planar_crs:
+        if self.check_same_crs(self.link_gdf,  self.planar_crs):
             pass
         else:
             if self.__single_link_gdf is None or self.__single_link_gdf.empty:
                 pass
             else:
                 self.__single_link_gdf = self.__single_link_gdf.to_crs(self.planar_crs)
             self.link_gdf = self.link_gdf.to_crs(self.planar_crs)
 
     def to_geo_prj(self) -> None:
-        if self.link_gdf.crs.srs == self.geo_crs:
+        if self.check_same_crs(self.link_gdf, self.geo_crs):
             pass
         else:
             if self.__single_link_gdf is None or self.__single_link_gdf.empty:
                 pass
             else:
                 self.__single_link_gdf = self.__single_link_gdf.to_crs(self.geo_crs)
             self.link_gdf = self.link_gdf.to_crs(self.geo_crs)
 
+    @staticmethod
+    def check_same_crs(gdf: gpd.GeoDataFrame = None, format_crs: str = None) -> bool:
+        return gdf.crs.srs.upper() == format_crs
+
     @property
     def crs(self):
         return self.link_gdf.crs.srs
 
     @property
     def bilateral_unidirectional_mapping(self) -> dict[int, tuple[int, int, int, int]]:
         return self.__double_single_mapping.copy()
```

### Comparing `gotrackit-0.2.2/src/gotrackit/map/Net.py` & `gotrackit-0.2.3/src/gotrackit/map/Net.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                  node_gdf: gpd.GeoDataFrame = None, weight_field: str = 'length', init_from_existing: bool = False,
                  is_check: bool = True, create_single: bool = True, search_method: str = 'dijkstra',
                  ft_link_mapping: dict = None, double_single_mapping: dict = None, link_ft_mapping: dict = None,
                  not_conn_cost: float = 999.0, cache_path: bool = True, cache_id: bool = True,
                  is_sub_net: bool = False, fmm_cache: bool = False, cache_cn: int = 2, cache_slice: int = None,
                  fmm_cache_fldr: str = None,
                  cache_name: str = 'cache', recalc_cache: bool = True,
-                 cut_off: float = 1200.0, max_cut_off: float = 5000.0):
+                 cut_off: float = 1200.0, max_cut_off: float = 5000.0, delete_circle: bool = True):
         """
         创建Net类
         :param link_path: link层的路网文件路径, 若指定了该参数, 则直接从磁盘IO创建Net线层
         :param node_path: node层的路网文件路径, 若指定了该参数, 则直接从磁盘IO创建Net点层
         :param link_gdf: 若指定了该参数, 则直接从内存中的gdf创建Net线层
         :param node_gdf: 若指定了该参数, 则直接从内存中的gdf创建Net点层
         :param weight_field: 搜路权重字段
@@ -95,48 +95,51 @@
         if cache_cn > os.cpu_count():
             cache_cn = os.cpu_count()
         self.cache_cn = cache_cn
         self.cache_name = cache_name
         self.fmm_cache_fldr = fmm_cache_fldr
         self.recalc_cache = recalc_cache
         self.cache_slice = cache_slice
+        self.delete_circle = delete_circle
         if self.cache_slice is None:
             self.cache_slice = 2 * self.cache_cn
 
         if node_gdf is None:
             self.__node = Node(node_gdf=gpd.read_file(node_path), is_check=is_check, init_available_node=self.cache_id)
         else:
             self.__node = Node(node_gdf=node_gdf, is_check=is_check, init_available_node=self.cache_id)
 
+        if not init_from_existing:
+            self.__node.init_node()
+        else:
+            pass
+
         if link_gdf is None:
             self.__link = Link(link_gdf=gpd.read_file(link_path), weight_field=self.weight_field, is_check=is_check,
                                planar_crs=self.__node.planar_crs, init_available_link=self.cache_id,
-                               not_conn_cost=self.not_conn_cost)
+                               not_conn_cost=self.not_conn_cost, delete_circle=self.delete_circle)
         else:
             self.__link = Link(link_gdf=link_gdf, weight_field=self.weight_field, is_check=is_check,
                                planar_crs=self.__node.planar_crs, init_available_link=self.cache_id,
-                               not_conn_cost=self.not_conn_cost)
+                               not_conn_cost=self.not_conn_cost, delete_circle=self.delete_circle)
         self.__planar_crs = self.__node.planar_crs
         self.to_plane_prj()
         if not self.is_sub_net:
+            self.del_zero_degree_nodes()
             self.__link.renew_length()
         if not init_from_existing:
             if create_single:
                 self.__link.init_link()
         else:
             if create_single:
                 # for sub net
                 self.__link.init_link_from_existing_single_link(single_link_gdf=link_gdf,
                                                                 double_single_mapping=double_single_mapping,
                                                                 ft_link_mapping=ft_link_mapping,
                                                                 link_ft_mapping=link_ft_mapping)
-        if not init_from_existing:
-            self.__node.init_node()
-        else:
-            pass
         if is_check:
             self.check()
 
     @property
     def planar_crs(self):
         return self.__planar_crs
 
@@ -335,28 +338,30 @@
         """
         if gps_array_buffer is None:
             return None
         gps_array_buffer_gdf = gpd.GeoDataFrame({'geometry': [gps_array_buffer]}, geometry='geometry',
                                                 crs=self.planar_crs)
         sub_single_link_gdf = gpd.sjoin(self.get_link_data(), gps_array_buffer_gdf)
         if sub_single_link_gdf.empty:
-            raise ValueError(rf'GPS数据在指定的buffer范围内关联不到任何路网数据...')
+            print(rf'GPS数据在指定的buffer范围内关联不到任何路网数据...')
+            return None
         sub_single_link_gdf.drop(columns=['index_right'], axis=1, inplace=True)
         sub_single_link_gdf.drop_duplicates(subset=[net_field.SINGLE_LINK_ID_FIELD], inplace=True)
         sub_node_list = list(set(sub_single_link_gdf[net_field.FROM_NODE_FIELD]) | \
                              set(sub_single_link_gdf[net_field.TO_NODE_FIELD]))
         sub_node_gdf = self.__node.get_node_data().loc[sub_node_list, :].copy()
         sub_net = Net(link_gdf=sub_single_link_gdf,
                       node_gdf=sub_node_gdf,
                       weight_field=weight_field,
                       init_from_existing=True, is_check=False, cache_path=cache_path, cache_id=cache_id,
                       not_conn_cost=not_conn_cost, is_sub_net=True, fmm_cache=fmm_cache,
                       ft_link_mapping=self.get_ft_node_link_mapping(),
                       link_ft_mapping=self.link_ft_map,
-                      double_single_mapping=self.bilateral_unidirectional_mapping, cut_off=self.cut_off)
+                      double_single_mapping=self.bilateral_unidirectional_mapping, cut_off=self.cut_off,
+                      delete_circle=False)
         sub_net.init_net(stp_cost_cache_df=self.get_path_cache(), cache_prj_inf=self.get_prj_cache())
         return sub_net
 
     @property
     def graph(self) -> nx.DiGraph:
         return self.__link.get_graph()
 
@@ -525,14 +530,53 @@
             self.__link.init_available_link_id()
             self.__node.init_available_node_id()
             if is_init_link:
                 self.check()
                 self.__link.init_link()
                 self.__node.init_node()
 
+    def get_circle_link(self) -> set[int]:
+        link_gdf = self.__link.link_gdf
+        return set(link_gdf[link_gdf[from_node_field] == link_gdf[to_node_field]][link_id_field])
+
+    def get_same_ft_link(self) -> set[int]:
+        link_gdf = self.__link.link_gdf
+        link_gdf['__temp__'] = link_gdf.apply(
+            lambda row: tuple(sorted((row[net_field.FROM_NODE_FIELD], row[net_field.TO_NODE_FIELD]))), axis=1)
+        dup_ft = set(link_gdf[link_gdf.duplicated(subset=['__temp__'])][
+                         net_field.LINK_ID_FIELD])
+        del link_gdf['__temp__']
+        return dup_ft
+
+    def process_circle(self):
+        """处理环路和相同f-t node的路"""
+        candidate_link_set = self.get_circle_link()
+        self.process_target(target_link_list=candidate_link_set)
+
+        candidate_link_set = self.get_same_ft_link()
+        self.process_target(target_link_list=candidate_link_set)
+
+        self.check()
+
+    def process_target(self, target_link_list: list[int] or set[int] = None):
+        for target_link in target_link_list:
+            target_geo = self.__link.get_link_geo(target_link, _type='bilateral')
+            split_ok, prj_p, modified_link, res_type = \
+                self.split_link(target_geo.interpolate(target_geo.length / 2),
+                                target_link, omitted_length_threshold=0.01)
+            if split_ok:
+                new_node_id = self.__node.available_node_id
+                self.__node.append_nodes(node_id=[new_node_id], geo=[prj_p])
+                self.modify_link_gdf(link_id_list=[modified_link[0]], attr_field_list=[to_node_field],
+                                     val_list=[[new_node_id]])
+                self.modify_link_gdf(link_id_list=[modified_link[1]], attr_field_list=[from_node_field],
+                                     val_list=[[new_node_id]])
+                self.renew_link_tail_geo(link_list=[modified_link[0]])
+                self.renew_link_head_geo(link_list=[modified_link[1]])
+
     @staticmethod
     def generate_new_ft(origin_f: int = None, origin_t: int = None,
                         divide_num: int = 2, start_node: int = None) -> tuple[list, list]:
         _ = [origin_f] + [start_node + i for i in range(divide_num)] + [origin_t]
         return [[_[i], _[i + 1]] for i in range(len(_) - 1)], _[1:-1]
 
     def divide_links_beta(self, divide_l: float = 70.0, min_l: float = 1.0, is_init_link: bool = True):
@@ -645,16 +689,16 @@
     def single_source_cache(self, node_list: list = None, g: nx.DiGraph = None,
                             cut_off: float = 500.0, weight_field: str = 'length', n: int = 2) -> pd.DataFrame:
         done_cost_cache, done_stp_cache = {}, {}
         for node in node_list:
             try:
                 done_cost_cache[node], done_stp_cache[node] = nx.single_source_dijkstra(g, node, weight=weight_field,
                                                                                         cutoff=cut_off)
-            except nx.exception.NodeNotFound as e:
-                print(repr(e))
+            except Exception as e:
+                pass
 
         done_stp_cost_df = self.slice_save(done_stp_cache=done_stp_cache,
                                            done_cost_cache=done_cost_cache,
                                            n=n)
         return done_stp_cost_df
 
     def single_link_ft_cost(self) -> pd.DataFrame:
```

### Comparing `gotrackit-0.2.2/src/gotrackit/map/Node.py` & `gotrackit-0.2.3/src/gotrackit/map/Node.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         if is_check:
             self.planar_crs = judge_plain_crs_based_on_node(node_gdf=self.__node_gdf)
             self.check()
         if init_available_node:
             self.init_available_node_id()
 
     def check(self):
-        assert self.__node_gdf.crs.srs == self.geo_crs, rf'Node层数据必须为WGS84 - EPSG:4326, 实际输入: {self.__node_gdf.crs.srs}'
+        assert self.__node_gdf.crs.srs.upper() == self.geo_crs, \
+            rf'Node层数据必须为WGS84 - EPSG:4326, 实际输入: {self.__node_gdf.crs.srs}'
         gap_set = {node_id_field, geometry_field} - set(self.__node_gdf.columns)
         assert len(gap_set) == 0, rf'线层Link缺少以下字段:{gap_set}'
         assert len(self.__node_gdf[node_id_field]) == len(self.__node_gdf[node_id_field].unique()), \
             rf'字段{node_id_field}不唯一...'
         for col in [node_id_field]:
             assert len(self.__node_gdf[self.__node_gdf[col].isna()]) == 0, rf'点层Node字段{col}有空值...'
             self.__node_gdf[col] = self.__node_gdf[col].astype(int)
@@ -64,21 +65,21 @@
         self.__node_gdf.loc[node_id_list, attr_field_list] = val_list
 
     @property
     def crs(self):
         return self.__node_gdf.crs.srs
 
     def to_plane_prj(self) -> None:
-        if self.__node_gdf.crs.srs == self.planar_crs:
+        if self.check_same_crs(self.__node_gdf, self.planar_crs):
             pass
         else:
             self.__node_gdf = self.__node_gdf.to_crs(self.planar_crs)
 
     def to_geo_prj(self) -> None:
-        if self.__node_gdf.crs.srs == self.geo_crs:
+        if self.check_same_crs(self.__node_gdf, self.geo_crs):
             pass
         else:
             self.__node_gdf = self.__node_gdf.to_crs(self.geo_crs)
 
     def init_available_node_id(self) -> None:
         max_node = self.__node_gdf[node_id_field].max()
         self.max_node_id = max_node
@@ -109,12 +110,17 @@
         assert set(node_gdf[node_id_field]) & set(self.__node_gdf[node_id_field]) == set()
         node_gdf.index = node_gdf[node_id_field]
         self.__node_gdf = pd.concat(
             [self.__node_gdf, node_gdf])
 
     def delete_nodes(self, node_list: list[int]) -> gpd.GeoDataFrame:
         del_node_gdf = self.__node_gdf.loc[node_list, :].copy()
-        self.__node_gdf.drop(index=node_list, inplace=True, axis=0)
+        if node_list:
+            self.__node_gdf.drop(index=node_list, inplace=True, axis=0)
         return del_node_gdf
 
     def node_id_set(self) -> set[int]:
-        return set(self.__node_gdf.index)
+        return set(self.__node_gdf[node_id_field])
+
+    @staticmethod
+    def check_same_crs(gdf: gpd.GeoDataFrame = None, format_crs: str = None) -> bool:
+        return gdf.crs.srs.upper() == format_crs
```

### Comparing `gotrackit-0.2.2/src/gotrackit/model/Markov.py` & `gotrackit-0.2.3/src/gotrackit/model/Markov.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # @Time    : 2023/12/9 8:29
 # @Author  : TangKai
 # @Team    : ZheChengData
 
 """Markov Model Class"""
 
 import os.path
+import time
 import warnings
 import numpy as np
 import pandas as pd
 import networkx as nx
 import geopandas as gpd
 from ..map.Net import Net
 from datetime import timedelta
@@ -289,15 +290,14 @@
         self.__s2s_route_l = s2s_route_l
         self.__done_prj_df = prj_done_df
 
         if not is_sub_net and not fmm_cache:
             self.net.set_path_cache(stp_cost_df=done_stp_cost_df)
         return True
 
-    # @function_time_cost
     def generate_transition_mat_beta(self, single_link_ft_df: pd.DataFrame = None,
                                      pre_seq_candidate: pd.DataFrame = None,
                                      gps_pre_next_dis_df: pd.DataFrame = None,
                                      g: nx.DiGraph = None,
                                      method: str = None, weight_field: str = 'length',
                                      cache_path: bool = True, not_conn_cost: float = 999.0,
                                      done_stp_cost_df: pd.DataFrame = None,
@@ -306,25 +306,30 @@
                                      add_single_ft: list[bool] = None) -> \
             tuple[dict, dict, pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
         # K候选
         seq_k_candidate_info = \
             self.filter_k_candidates(preliminary_candidate_link=pre_seq_candidate, using_cache=fmm_cache,
                                      top_k=self.top_k, cache_prj_inf=cache_prj_inf)
         # print(rf'{len(seq_k_candidate_info)}个候选路段...')
+        seq_k_candidate_info.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD], inplace=True)
+
         seq_k_candidate_info['idx'] = seq_k_candidate_info.groupby(gps_field.POINT_SEQ_FIELD)[
                                           net_field.SINGLE_LINK_ID_FIELD].rank(method='min').astype(int) - 1
 
         ft_idx_map = seq_k_candidate_info[[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD, 'idx']].copy()
-        ft_idx_map.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD], inplace=True)
+
+        # ft_idx_map.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD], inplace=True)
         del seq_k_candidate_info['idx']
         del pre_seq_candidate
-        seq_k_candidate = seq_k_candidate_info.groupby(gps_field.POINT_SEQ_FIELD).agg(
-            {net_field.SINGLE_LINK_ID_FIELD: list, gps_field.POINT_SEQ_FIELD: list}).rename(
-            columns={gps_field.POINT_SEQ_FIELD: 'g_s'})
 
+        seq_k_candidate = seq_k_candidate_info.groupby(gps_field.POINT_SEQ_FIELD).agg(
+            {net_field.SINGLE_LINK_ID_FIELD: list, gps_field.POINT_SEQ_FIELD: list,
+             net_field.FROM_NODE_FIELD: 'count'}).rename(
+            columns={gps_field.POINT_SEQ_FIELD: 'g_s', net_field.FROM_NODE_FIELD: 'count'})
+        seq_len_dict = {s: l for s, l in zip(seq_k_candidate.index, seq_k_candidate['count'])}
         gps_match_link_route_dis = seq_k_candidate_info[
             [gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD, 'route_dis']].copy()
         seq_k_candidate.rename(columns={net_field.SINGLE_LINK_ID_FIELD: markov_field.FROM_STATE,
                                         'g_s': gps_field.FROM_GPS_SEQ}, inplace=True)
 
         seq_k_candidate[markov_field.TO_STATE] = seq_k_candidate[markov_field.FROM_STATE].shift(-1)
         seq_k_candidate[gps_field.TO_GPS_SEQ] = seq_k_candidate[gps_field.FROM_GPS_SEQ].shift(-1)
@@ -394,27 +399,28 @@
             del done_stp_cost_df
             done_stp_cost_df = pd.DataFrame()
 
         transition_df[cost_field] = transition_df[cost_field].fillna(0)
         transition_df.reset_index(inplace=True, drop=True)
         transition_df[markov_field.ROUTE_LENGTH] = not_conn_cost * 1.0
 
-        _ = transition_df[transition_df[cost_field] > 0]
+        normal_path_idx_a = transition_df[cost_field] > 0
+        _ = transition_df[normal_path_idx_a]
         adj_seq_path_dict = {(int(f_state), int(t_state)): node_path for f_state, t_state, node_path, c in
                              zip(_[markov_field.FROM_STATE],
                                  _[markov_field.TO_STATE],
                                  _[path_field],
                                  _[cost_field]) if c > 0}
         same_link_idx = transition_df[markov_field.FROM_STATE] == transition_df[markov_field.TO_STATE]
         transition_df.loc[same_link_idx, markov_field.ROUTE_LENGTH] = \
             np.abs(transition_df.loc[same_link_idx, :]['from_route_dis'] -
                    transition_df.loc[same_link_idx, :]['to_route_dis'])
         transition_df['2nd_node'] = -1
         transition_df['-2nd_node'] = -1
-        normal_path_idx_a = transition_df[cost_field] > 0
+        # normal_path_idx_a = transition_df[cost_field] > 0
         # normal_path_idx_a可能全是False
         try:
             transition_df.loc[normal_path_idx_a, '2nd_node'] = transition_df.loc[normal_path_idx_a, :][
                 path_field].apply(
                 lambda x: x[1])
             transition_df.loc[normal_path_idx_a, '-2nd_node'] = transition_df.loc[normal_path_idx_a, :][
                 path_field].apply(
@@ -437,18 +443,25 @@
         transition_df[markov_field.DIS_GAP] = np.abs(
             -transition_df[markov_field.ROUTE_LENGTH] + transition_df[gps_field.ADJ_DIS])
 
         s2s_route_l = transition_df[[gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ, markov_field.ROUTE_LENGTH,
                                      markov_field.FROM_STATE, markov_field.TO_STATE]].copy()
         transition_df['trans_values'] = \
             self.transition_probability(self.beta, transition_df[markov_field.DIS_GAP].values, self.dis_para)
-        ft_transition_dict = {f_gps_seq: df[
-            [markov_field.FROM_STATE, markov_field.TO_STATE, 'trans_values']].set_index(
-            [markov_field.FROM_STATE, markov_field.TO_STATE]).unstack().values for (f_gps_seq, t_gps_seq), df in
+
+        # ft_transition_dict = {f_gps_seq: df[
+        #     [markov_field.FROM_STATE, markov_field.TO_STATE, 'trans_values']].set_index(
+        #     [markov_field.FROM_STATE, markov_field.TO_STATE]).unstack().values for (f_gps_seq, t_gps_seq), df in
+        #                       transition_df.groupby([gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ])}
+
+        ft_transition_dict = {f_gps_seq: df['trans_values'].values.reshape(seq_len_dict[f_gps_seq],
+                                                                           int(len(df) / seq_len_dict[f_gps_seq])) for
+                              (f_gps_seq, t_gps_seq), df in
                               transition_df.groupby([gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ])}
+
         return adj_seq_path_dict, ft_transition_dict, ft_idx_map, s2s_route_l, seq_k_candidate_info, done_stp_cost_df
 
     def add_path_cache(self, done_stp_cost_df: pd.DataFrame = None, source_node_list: list[int] or set[int] = None,
                        g: nx.DiGraph = None, method: str = 'dijkstra', single_link_ft_path_df: pd.DataFrame = None,
                        weight_field: str = None, cut_off: float = 600.0, add_single_ft: list[bool] = True) \
             -> pd.DataFrame:
         _done_stp_cost_df = self.single_source_path_cache(node_list=source_node_list, method=method, cut_off=cut_off,
@@ -475,16 +488,16 @@
         for n in node_list:
             try:
                 cost[n], stp[n] = \
                     self._single_source_path_alpha(g, source=n,
                                                    method=method,
                                                    weight_field=weight_field,
                                                    cut_off=cut_off)
-            except nx.NetworkXNoPath:
-                pass
+            except Exception as e:
+                print(repr(e))
         if stp:
             stp_df = pd.DataFrame(stp).stack().reset_index(drop=False).rename(
                 columns={'level_0': d_node_field, 'level_1': o_node_field, 0: path_field})
             cost_df = pd.DataFrame(cost).stack().reset_index(drop=False).rename(
                 columns={'level_0': d_node_field, 'level_1': o_node_field, 0: cost_field})
             cost_df[cost_field] = np.around(cost_df[cost_field], decimals=1)
             stp_cost_df = pd.merge(stp_df, cost_df, on=[o_node_field, d_node_field])
@@ -504,15 +517,14 @@
 
             df.drop(columns=[right_key], axis=1, inplace=True)
         else:
             df.rename(columns={'route_dis': label + '_route_dis'}, inplace=True)
             df.drop(columns=right_key, axis=1, inplace=True)
         return df
 
-
     @staticmethod
     def _single_source_path_alpha(g: nx.DiGraph = None, source: int = None, method: str = 'dijkstra',
                                   weight_field: str = None, cut_off: float = 600.0) -> \
             tuple[dict[int, int], dict[int, list]]:
         if method == 'dijkstra':
             return nx.single_source_dijkstra(g, source, weight=weight_field, cutoff=cut_off)
         else:
@@ -567,18 +579,17 @@
 
         self.__s2s_route_l.rename(columns={gps_field.FROM_GPS_SEQ: gps_field.POINT_SEQ_FIELD,
                                            gps_field.TO_GPS_SEQ: 'next_seq',
                                            markov_field.FROM_STATE: net_field.SINGLE_LINK_ID_FIELD,
                                            markov_field.TO_STATE: 'next_single',
                                            markov_field.ROUTE_LENGTH: markov_field.DIS_TO_NEXT}, inplace=True)
 
-        gps_link_state_df = pd.merge(gps_link_state_df, self.__s2s_route_l, how='left', on=[gps_field.POINT_SEQ_FIELD,
-                                                                                            'next_seq',
-                                                                                            net_field.SINGLE_LINK_ID_FIELD,
-                                                                                            'next_single'])
+        gps_link_state_df = pd.merge(gps_link_state_df, self.__s2s_route_l, how='left',
+                                     on=[gps_field.POINT_SEQ_FIELD, 'next_seq',
+                                         net_field.SINGLE_LINK_ID_FIELD, 'next_single'])
         # agent_id, seq
         gps_match_res_gdf = self.gps_points.gps_gdf
 
         # 获取补全的路径
         # gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD, gps_field.SUB_SEQ_FIELD
         # net_field.LINK_ID_FIELD, net_field.DIRECTION_FIELD, net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD
         # gps_field.TIME_FIELD, net_field.GEOMETRY_FIELD
@@ -719,22 +730,34 @@
         omitted_gps_state_df[gps_field.TIME_FIELD] = omitted_gps_points_time
         omitted_gps_state_df[net_field.GEOMETRY_FIELD] = [Point(loc) for loc in omitted_gps_points]
 
         return omitted_gps_state_df
 
     def acquire_visualization_res(self, use_gps_source: bool = False,
                                   link_width: float = 1.5, node_radius: float = 1.5,
-                                  match_link_width: float = 5.0, gps_radius: float = 3.0) -> tuple[gpd.GeoDataFrame,
-                                  gpd.GeoDataFrame, gpd.GeoDataFrame, gpd.GeoDataFrame]:
+                                  match_link_width: float = 5.0, gps_radius: float = 3.0,
+                                  sub_net_buffer: float = 200.0, dup_threshold: float = 10.0) -> \
+            tuple[gpd.GeoDataFrame, gpd.GeoDataFrame, gpd.GeoDataFrame, gpd.GeoDataFrame]:
         """获取可视化结果"""
         if self.__plot_mix_gdf is None:
             # print('初次计算')
             single_link_gdf = self.net.get_link_data()
             single_link_gdf.reset_index(inplace=True, drop=True)
             node_gdf = self.net.get_node_data()
+
+            # 如果不是子网络则要计算buffer范围内的路网
+            if not self.net.is_sub_net:
+                gps_array_buffer = self.gps_points.get_gps_array_buffer(buffer=sub_net_buffer,
+                                                                        dup_threshold=dup_threshold)
+                gps_array_buffer_gdf = gpd.GeoDataFrame({'geometry': [gps_array_buffer]}, geometry='geometry',
+                                                        crs=self.net.planar_crs)
+                single_link_gdf = gpd.sjoin(single_link_gdf, gps_array_buffer_gdf)
+                used_node = set(single_link_gdf[net_field.FROM_NODE_FIELD]) | set(single_link_gdf[net_field.TO_NODE_FIELD])
+                node_gdf = node_gdf[node_gdf[net_field.NODE_ID_FIELD].isin(used_node)].copy()
+
             net_crs = self.net.crs
             plain_crs = self.net.planar_crs
             is_geo_crs = self.net.is_geo_crs()
 
             if self.gps_match_res_gdf is None:
                 self.acquire_res()
```

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/GlobalVal.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/GlobalVal.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/NetGen.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/NetGen.py`

 * *Files 2% similar despite different names*

```diff
@@ -432,14 +432,27 @@
         # divide_l: 所有长度大于divide_l的路段都将按照divide_l进行划分
         # min_l: 划分后如果剩下的路段长度小于min_l, 那么此次划分将不被允许
         # is_init_link: 划分后是否重新初始化路网对象
         # method: alpha 或者 beta, 前一种方法可保留与划分前的link的映射关系(_parent_link字段)
         my_net.divide_links(divide_l=divide_l, min_l=min_l, is_init_link=False, method='alpha')
         return my_net.get_bilateral_link_data().reset_index(drop=True), my_net.get_node_data().reset_index(drop=True)
 
+    @staticmethod
+    def circle_process(link_gdf: gpd.GeoDataFrame, node_gdf: gpd.GeoDataFrame = None) -> \
+            tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]:
+        """
+        :param link_gdf:
+        :param node_gdf:
+        :return:
+        """
+        my_net = Net(link_gdf=link_gdf,
+                     node_gdf=node_gdf, create_single=False, delete_circle=False)
+        my_net.process_circle()
+        return my_net.get_bilateral_link_data().reset_index(drop=True), my_net.get_node_data().reset_index(drop=True)
+
     def redivide_link_node(self, link_gdf: gpd.GeoDataFrame = None):
         """
         对link进行线层和点层的重新划分
         :param link_gdf: gpd.GeoDataFrame, 要求至少有geometry字段
         """
         link_gdf = link_gdf.to_crs('EPSG:4326')
```

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/Parse/gd_car_path.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/Parse/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/GeoProcess.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/GeoProcess.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/GraphAna.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/GraphAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/IndexAna.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/IndexAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/od.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/PublicTools/od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/Request/api/WebApi.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/Request/api/WebApi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/Request/request_path.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/Request/request_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/Request/usage/bd_ts.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/Request/usage/bd_ts.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/Request/usage/gd_car_path.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/Request/usage/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,19 @@
         if net_field.TO_NODE_FIELD in update_link_field_list:
             update_link_field_list.remove(net_field.TO_NODE_FIELD)
 
     # 3.更新线层数据
     link_gdf = update_link(link_gdf=link_gdf, node_gdf=node_gdf, update_link_field_list=update_link_field_list,
                            origin_crs=origin_crs, plain_prj=plain_prj, fill_dir=fill_dir)
 
+    # 去除没有link连接的节点
+    used_node = set(link_gdf[net_field.FROM_NODE_FIELD]) | set(link_gdf[net_field.TO_NODE_FIELD])
+    node_gdf.drop(index=node_gdf[~node_gdf[net_field.NODE_ID_FIELD].isin(used_node)].index, inplace=True, axis=1)
+    node_gdf.reset_index(inplace=True, drop=True)
+
     if save_streets_before_modify_minimum:
         save_file(data_item=link_gdf, file_type=net_file_type, out_fldr=out_fldr, file_name='LinkBeforeModify')
         save_file(data_item=node_gdf, file_type=net_file_type, out_fldr=out_fldr, file_name='NodeBeforeModify')
 
     # 极小间隔点优化
     node_group_status_gdf = gpd.GeoDataFrame()
     if execute_modify:
```

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Tools/process.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/Tools/process.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/conn.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/conn.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/increment.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/increment.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/net_reverse.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/net_reverse.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/optimize_net.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/optimize_net.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/save_file.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/RoadNet/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/book_mark.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/book_mark.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netreverse/format_od.py` & `gotrackit-0.2.3/src/gotrackit/netreverse/format_od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/netxfer/SumoConvert.py` & `gotrackit-0.2.3/src/gotrackit/netxfer/SumoConvert.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/solver/Viterbi.py` & `gotrackit-0.2.3/src/gotrackit/solver/Viterbi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/tools/coord_trans.py` & `gotrackit-0.2.3/src/gotrackit/tools/coord_trans.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/tools/geo_process.py` & `gotrackit-0.2.3/src/gotrackit/tools/geo_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,16 +305,17 @@
 def angle_base_north(v: np.ndarray = None):
     angle = vector_angle(v, np.array([0, 1]))
     if v[0] <= 0:
         return angle
     else:
         return 360 - angle
 
+
 def judge_plain_crs(lng: float = None) -> str:
-    six_df = pd.DataFrame([(i * 6, 32631 + i) for i in range(0, 60)],
+    six_df = pd.DataFrame([(i * 6, 32631 + i) for i in range(-30, 30)],
                           columns=['start_lng', 'plain_crs'])
     res = six_df[lng - six_df['start_lng'] >= 0]['plain_crs'].max()
     return rf'EPSG:{res}'
 
 def judge_plain_crs_based_on_node(node_gdf: gpd.GeoDataFrame = None) -> str:
     mean_x = np.array([geo.x for geo in node_gdf['geometry']]).mean()
     return judge_plain_crs(lng=mean_x)
```

### Comparing `gotrackit-0.2.2/src/gotrackit/tools/group.py` & `gotrackit-0.2.3/src/gotrackit/tools/group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/tools/save_file.py` & `gotrackit-0.2.3/src/gotrackit/tools/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.2/src/gotrackit/visualization.py` & `gotrackit-0.2.3/src/gotrackit/visualization.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,46 +23,49 @@
 kepler_config = KeplerConfig()
 
 
 @function_time_cost
 def export_visualization(hmm_obj_list: list[HiddenMarkov], export_all_agents: bool = False, use_gps_source: bool = True,
                          out_fldr: str = None, gps_radius: float = 6.0,
                          export_geo: bool = True, export_html: bool = True, flag_name: str = 'test',
-                         multi_core_save: bool = False):
+                         multi_core_save: bool = False, sub_net_buffer: float = 200.0, dup_threshold: float = 10.0):
     """
 
     :param hmm_obj_list:
     :param export_all_agents:
     :param use_gps_source:
     :param out_fldr:
     :param gps_radius:
     :param export_geo:
     :param export_html:
     :param flag_name
     :param multi_core_save
+    :param sub_net_buffer:
+    :param dup_threshold
     :return:
     """
     out_fldr = './' if out_fldr is None else out_fldr
 
     if not multi_core_save or len(hmm_obj_list) <= 10 or os.cpu_count() <= 1:
         # print('single export')
         export_vs(hmm_obj_list=hmm_obj_list, use_gps_source=use_gps_source, gps_radius=gps_radius,
-                  out_fldr=out_fldr, export_geo=export_geo, export_html=export_html, flag_name=flag_name)
+                  out_fldr=out_fldr, export_geo=export_geo, export_html=export_html, flag_name=flag_name,
+                  sub_net_buffer=sub_net_buffer, dup_threshold=dup_threshold)
     else:
         # print('multi export')
         core_num = 3 if os.cpu_count() >= 3 else os.cpu_count()
         hmm_group = cut_group(obj_list=hmm_obj_list, n=core_num)
         del hmm_obj_list
         hmm_obj_list = []
         pool = multiprocessing.Pool(processes=len(hmm_group))
         res_list = []
         for i in range(0, len(hmm_group)):
             res = pool.apply_async(export_vs,
                                    args=(hmm_group[i], use_gps_source, gps_radius, out_fldr, export_geo, export_html,
-                                         flag_name))
+                                         flag_name, sub_net_buffer, dup_threshold))
             res_list.append(res)
         pool.close()
         pool.join()
         del hmm_group
         for res in res_list:
             hmm_obj_list.extend(res.get())
 
@@ -73,36 +76,44 @@
         try:
             all_vc.visualization(zoom=15, out_fldr=out_fldr, file_name=rf'{flag_name}-all_agents',
                                  gps_radius=gps_radius)
         except Exception as e:
             print(repr(e))
             print(rf'输出HTML可视化文件, 出现某些错误, 输出失败...')
 
+
 def export_vs(hmm_obj_list: list[HiddenMarkov], use_gps_source: bool = True,
               gps_radius: float = 8.0, out_fldr: str = None, export_geo: bool = True, export_html: bool = True,
-              flag_name: str = 'test') -> list[HiddenMarkov]:
+              flag_name: str = 'test', sub_net_buffer: float = 200.0, dup_threshold: float = 10.0) -> \
+        list[HiddenMarkov]:
     _ = [export_v(hmm_obj=hmm_obj, use_gps_source=use_gps_source, gps_radius=gps_radius,
-                  out_fldr=out_fldr, export_geo=export_geo, export_html=export_html, flag_name=flag_name) for hmm_obj in hmm_obj_list]
+                  out_fldr=out_fldr, export_geo=export_geo, export_html=export_html, flag_name=flag_name,
+                  sub_net_buffer=sub_net_buffer, dup_threshold=dup_threshold) for hmm_obj in hmm_obj_list]
     return _
 
 def export_v(hmm_obj: HiddenMarkov, use_gps_source: bool = True, gps_radius: float = 8.0, out_fldr: str = None,
-             export_geo: bool = True, export_html: bool = True, flag_name: str = 'test') -> HiddenMarkov:
+             export_geo: bool = True, export_html: bool = True, flag_name: str = 'test',
+             sub_net_buffer: float = 200.0, dup_threshold: float = 10.0) -> HiddenMarkov:
     vc = VisualizationCombination(use_gps_source=use_gps_source, hmm_obj=hmm_obj)
     file_name = flag_name + '-' + str(hmm_obj.gps_points.agent_id)
     if export_html:
         try:
             vc.visualization(file_name=file_name, out_fldr=out_fldr, zoom=15,
-                             gps_radius=gps_radius)
+                             gps_radius=gps_radius, sub_net_buffer=sub_net_buffer, dup_threshold=dup_threshold)
         except Exception as e:
             print(repr(e))
             print(rf'输出HTML可视化文件, 出现某些错误, 输出失败...')
 
     if export_geo:
-        hmm_obj.acquire_geo_res(out_fldr=out_fldr,
-                                flag_name=file_name)
+        try:
+            hmm_obj.acquire_geo_res(out_fldr=out_fldr,
+                                    flag_name=file_name)
+        except Exception as e:
+            print(repr(e))
+            print(rf'输出geojson可视化文件, 出现某些错误, 输出失败...')
     return hmm_obj
 
 
 class VisualizationCombination(object):
     def __init__(self, hmm_obj: HiddenMarkov = None, use_gps_source: bool = False):
         if hmm_obj is None:
             self.__hmm_obj_list = []
@@ -121,24 +132,26 @@
 
     @hmm_obj_list.setter
     def hmm_obj_list(self, hmm_obj_list: list[HiddenMarkov]):
         self.__hmm_obj_list = hmm_obj_list
 
     def visualization(self, zoom: int = 15, out_fldr: str = None, file_name: str = None,
                       link_width: float = 1.5, node_radius: float = 1.5,
-                      match_link_width: float = 5.0, gps_radius: float = 3.0) -> None:
+                      match_link_width: float = 5.0, gps_radius: float = 3.0, sub_net_buffer: float = 200.0,
+                      dup_threshold: float = 10.0) -> None:
         out_fldr = r'./' if out_fldr is None else out_fldr
         base_link_gdf = gpd.GeoDataFrame()
         base_node_gdf = gpd.GeoDataFrame()
         gps_link_gdf = gpd.GeoDataFrame()
         may_error_gdf = gpd.GeoDataFrame()
         for hmm in self.__hmm_obj_list:
             _gps_link_gdf, _base_link_gdf, _base_node_gdf, _error_gdf = hmm.acquire_visualization_res(
                 use_gps_source=self.use_gps_source, link_width=link_width, gps_radius=gps_radius,
-                match_link_width=match_link_width, node_radius=node_radius)
+                match_link_width=match_link_width, node_radius=node_radius, sub_net_buffer=sub_net_buffer,
+                dup_threshold=dup_threshold)
             base_link_gdf = pd.concat([base_link_gdf, _base_link_gdf])
             base_node_gdf = pd.concat([base_node_gdf, _base_node_gdf])
             gps_link_gdf = pd.concat([gps_link_gdf, _gps_link_gdf])
             may_error_gdf = pd.concat([may_error_gdf, _error_gdf])
 
         gps_link_gdf.reset_index(inplace=True, drop=True)
         base_link_gdf.drop_duplicates(subset=[net_field.LINK_ID_FIELD], keep='first', inplace=True)
```

### Comparing `gotrackit-0.2.2/src/gotrackit.egg-info/PKG-INFO` & `gotrackit-0.2.3/src/gotrackit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,34 +34,42 @@
 ![PyPI - Version](https://img.shields.io/pypi/v/gotrackit)
 ![GitHub License](https://img.shields.io/github/license/zdsjjtTLG/Trackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gotrackit)
 
 ~ 一个包搞定：路网获取、路网优化、宏微观地图匹配、匹配可视化、问题路段快速定位 ~
 
-唐铠, 794568794@qq.com, tangkai@zhechengdata.com
+Developed by Tang Kai, Email: 794568794@qq.com & tangkai@zhechengdata.com
 </div>
 <br>
 
 
 
-**版本状态：04.27即将更新更新: v0.2.2**
+**版本状态：05.07已经更新: v0.2.3**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
-- 向量化改造, 且引入FMM(Fast Map Matching)路径预存储机制, 大规模路网匹配效率大幅度提升
 
-- 完善报错机制, 遇到GPS脏数据不再报错停止, 而是跳过, 并且在所有的agents计算完毕后输出有问题的agent编号
+- 效率优化, 相较于v0.2.2小幅度提升
+
+- crs判断BUG修复、境外路网构建失败BUG修复
+
+- 报错机制优化
+
+- 输出文件目录指定参数html_fldr废除, 改为out_fldr
+
+- 增加环路处理功能
+    
+- 增加匹配结果即时输出参数, 每匹配完一条轨迹可马上进行结果存储
 
-- BUG修复
 
 <br>
 
 <div align=center>
-~ v0.2.2效率将大幅度提升 ~
+~ v0.2.2效率将大幅度提升, 最高可以提升10倍的性能 !~
 </div>
 
 <br>
 
 与上一版本对比:
 
 | 样例数据           | 有效的GPS点数 | top_k(k邻近候选参数) | gps_buffer(临域半径) | 候选路段条数 | 状态转移次数  | v0.2.1版解算时间 | v0.2.2版解算时间 |
@@ -151,15 +159,15 @@
 
 **文档齐全**
 
 - 中文文档，有详细的操作指引；
 - 算法原理讲解部分不涉及复杂的公式推导，使用动画形式剖析算法原理,简洁明了。
 
 **匹配结果自动优化**
-- 对基于HMM匹配的初步路径进行了优化，对于不连通的位置会自动补路，对于实际路网不连通的位置会输出警告，方便用户检查路网。
+- 对基于HMM匹配的初步路径进行了优化，对于不连通的位置会自动搜路补全，对于实际路网不连通的位置会输出警告信息，方便用户回溯问题。
 
 
 
 ### 1.1. 如何安装gotrackit
 
 #### __所需前置依赖__
```

### Comparing `gotrackit-0.2.2/src/gotrackit.egg-info/SOURCES.txt` & `gotrackit-0.2.3/src/gotrackit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

