# Comparing `tmp/sumo-rl-1.4.4.tar.gz` & `tmp/sumo_rl-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumo-rl-1.4.4.tar", last modified: Mon Mar 25 15:53:59 2024, max compression
+gzip compressed data, was "sumo_rl-1.4.5.tar", last modified: Tue May  7 14:50:56 2024, max compression
```

## Comparing `sumo-rl-1.4.4.tar` & `sumo_rl-1.4.5.tar`

### file list

```diff
@@ -1,31 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:59.827316 sumo-rl-1.4.4/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-03-25 15:53:59.827316 sumo-rl-1.4.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    11539 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 15:53:59.827316 sumo-rl-1.4.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      842 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:59.823316 sumo-rl-1.4.4/sumo_rl/
--rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/sumo_rl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:59.827316 sumo-rl-1.4.4/sumo_rl/agents/
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/sumo_rl/agents/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1351 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/sumo_rl/agents/ql_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:59.827316 sumo-rl-1.4.4/sumo_rl/environment/
--rwxr-xr-x   0 runner    (1001) docker     (127)      230 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/sumo_rl/environment/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24404 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/sumo_rl/environment/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/sumo_rl/environment/observations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/sumo_rl/environment/resco_envs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13778 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/sumo_rl/environment/traffic_signal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:59.827316 sumo-rl-1.4.4/sumo_rl/exploration/
--rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/sumo_rl/exploration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      926 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/sumo_rl/exploration/epsilon_greedy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      530 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/sumo_rl/exploration/plot_epsilon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:59.827316 sumo-rl-1.4.4/sumo_rl/util/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/sumo_rl/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9411 2024-03-25 15:53:55.000000 sumo-rl-1.4.4/sumo_rl/util/gen_route.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:53:59.827316 sumo-rl-1.4.4/sumo_rl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-03-25 15:53:59.000000 sumo-rl-1.4.4/sumo_rl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-25 15:53:59.000000 sumo-rl-1.4.4/sumo_rl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 15:53:59.000000 sumo-rl-1.4.4/sumo_rl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-25 15:53:59.000000 sumo-rl-1.4.4/sumo_rl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 15:53:59.000000 sumo-rl-1.4.4/sumo_rl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.409410 sumo_rl-1.4.5/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-05-07 14:50:56.409410 sumo_rl-1.4.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11636 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:50:56.409410 sumo_rl-1.4.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      842 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.373409 sumo_rl-1.4.5/sumo_rl/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.377410 sumo_rl-1.4.5/sumo_rl/agents/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/agents/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1351 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/agents/ql_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.377410 sumo_rl-1.4.5/sumo_rl/environment/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      230 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/environment/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24853 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/environment/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/environment/observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/environment/resco_envs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13778 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/environment/traffic_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.377410 sumo_rl-1.4.5/sumo_rl/exploration/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/exploration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      926 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/exploration/epsilon_greedy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      530 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/exploration/plot_epsilon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.377410 sumo_rl-1.4.5/sumo_rl/nets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.377410 sumo_rl-1.4.5/sumo_rl/nets/2way-single-intersection/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7658 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/2way-single-intersection/single-intersection-gen.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2171 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/2way-single-intersection/single-intersection-horizontal.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2170 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/2way-single-intersection/single-intersection-vertical.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7211 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/2way-single-intersection/single-intersection-vhvh.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      396 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/2way-single-intersection/single-intersection.edg.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12028 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/2way-single-intersection/single-intersection.net.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      279 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/2way-single-intersection/single-intersection.nod.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/2way-single-intersection/single-intersection.sumocfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.377410 sumo_rl-1.4.5/sumo_rl/nets/2x2grid/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34345 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/2x2grid/2x2.net.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      579 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/2x2grid/2x2.rou.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.381410 sumo_rl-1.4.5/sumo_rl/nets/3x3grid/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   106271 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/3x3grid/3x3Grid2lanes.net.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      390 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/3x3grid/3x3grid.sumocfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)   697063 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/3x3grid/routes14000.rou.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.381410 sumo_rl-1.4.5/sumo_rl/nets/4x4-Lucas/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2025 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4-Lucas/4x4.edg.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    63950 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4-Lucas/4x4.net.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1627 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4-Lucas/4x4.nod.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4-Lucas/4x4.sumocfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4-Lucas/4x4c1.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4-Lucas/4x4c1c2.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4302 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4-Lucas/4x4c1c2c1c2.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1061 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4-Lucas/4x4c2.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4-Lucas/4x4c2c1.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      552 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4-Lucas/4x4teste.rou.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.381410 sumo_rl-1.4.5/sumo_rl/nets/4x4-Lucas/metrics/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1549 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4-Lucas/metrics/result_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.385409 sumo_rl-1.4.5/sumo_rl/nets/4x4loop/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2498 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4loop/4x4loop.edg.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    80847 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4loop/4x4loop.net.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1627 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4loop/4x4loop.nod.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4loop/4x4loop.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      346 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4loop/4x4loop.sumocfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1856 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4loop/circle.add.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1193282 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/4x4loop/output_sumo.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.389410 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.393410 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/flows/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   451007 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/flows/nguyen2lanes.rou.alt.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   233007 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/flows/nguyen2lanes.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/flows/nguyen500.flows.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/flows/nguyen700.flows.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      309 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/flows/nguyenTeste.flows.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   445637 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/flows/nguyenTeste.rou.alt.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   227637 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/flows/nguyenTeste.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1198 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyen.edg.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      688 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyen.flows.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyen.nod.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      235 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyen.sumocfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyen.taz.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   298843 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyen.trips.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   431546 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyenBlog.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38041 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyenNoTL.net.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1032373 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyencontext.rou.alt.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   530973 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyencontext.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyencontextroutes.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   704046 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyentesteod.rou.alt.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   431546 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyentesteod.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38735 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/Nguyen/nguyentl.net.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.393410 sumo_rl-1.4.5/sumo_rl/nets/OW/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      343 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/OW/OW-nowait-single.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      710 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/OW/OW-nowait-small.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   172641 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/OW/OW-nowait.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      296 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/OW/OW-traci.sumocfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    98611 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/OW/OW.net.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.373409 sumo_rl-1.4.5/sumo_rl/nets/RESCO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.397410 sumo_rl-1.4.5/sumo_rl/nets/RESCO/arterial4x4/
+-rw-r--r--   0 runner    (1001) docker     (127)   157653 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/arterial4x4/arterial4x4.net.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/arterial4x4/arterial4x4.sumocfg
+-rw-r--r--   0 runner    (1001) docker     (127)   459999 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/arterial4x4/arterial4x4_1.rou.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.397410 sumo_rl-1.4.5/sumo_rl/nets/RESCO/cologne1/
+-rw-r--r--   0 runner    (1001) docker     (127)    38633 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/cologne1/cologne1.net.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   182234 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/cologne1/cologne1.rou.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/cologne1/cologne1.sumocfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.397410 sumo_rl-1.4.5/sumo_rl/nets/RESCO/cologne3/
+-rw-r--r--   0 runner    (1001) docker     (127)   149615 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/cologne3/cologne3.net.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   763448 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/cologne3/cologne3.rou.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/cologne3/cologne3.sumocfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.401410 sumo_rl-1.4.5/sumo_rl/nets/RESCO/cologne8/
+-rw-r--r--   0 runner    (1001) docker     (127)   354765 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/cologne8/cologne8.net.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   188137 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/cologne8/cologne8.rou.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/cologne8/cologne8.sumocfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.401410 sumo_rl-1.4.5/sumo_rl/nets/RESCO/grid4x4/
+-rw-r--r--   0 runner    (1001) docker     (127)   462097 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/grid4x4/grid4x4.net.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/grid4x4/grid4x4.sumocfg
+-rw-r--r--   0 runner    (1001) docker     (127)   171190 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/grid4x4/grid4x4_1.rou.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.401410 sumo_rl-1.4.5/sumo_rl/nets/RESCO/ingolstadt1/
+-rw-r--r--   0 runner    (1001) docker     (127)    33252 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/ingolstadt1/ingolstadt1.net.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   172052 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/ingolstadt1/ingolstadt1.rou.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/ingolstadt1/ingolstadt1.sumocfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.405410 sumo_rl-1.4.5/sumo_rl/nets/RESCO/ingolstadt21/
+-rw-r--r--   0 runner    (1001) docker     (127)  1860885 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/ingolstadt21/ingolstadt21.net.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   425201 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/ingolstadt21/ingolstadt21.rou.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/ingolstadt21/ingolstadt21.sumocfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.405410 sumo_rl-1.4.5/sumo_rl/nets/RESCO/ingolstadt7/
+-rw-r--r--   0 runner    (1001) docker     (127)   273925 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/ingolstadt7/ingolstadt7.net.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   302634 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/ingolstadt7/ingolstadt7.rou.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/RESCO/ingolstadt7/ingolstadt7.sumocfg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.405410 sumo_rl-1.4.5/sumo_rl/nets/double/
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/double/flow.rou.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    50571 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/double/network.net.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.409410 sumo_rl-1.4.5/sumo_rl/nets/simple/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/simple/simple-empty.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      468 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/simple/simple-traci.sumocfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      647 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/simple/simple.edg.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10178 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/simple/simple.net.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      329 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/simple/simple.nod.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/simple/simple.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/simple/simple.sumocfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      117 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/simple/simple.typ.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.409410 sumo_rl-1.4.5/sumo_rl/nets/single-intersection/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      205 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/single-intersection/single-intersection.edg.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4817 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/single-intersection/single-intersection.net.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      279 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/single-intersection/single-intersection.nod.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/single-intersection/single-intersection.rou.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/nets/single-intersection/single-intersection.sumocfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.409410 sumo_rl-1.4.5/sumo_rl/util/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9411 2024-05-07 14:50:51.000000 sumo_rl-1.4.5/sumo_rl/util/gen_route.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:50:56.409410 sumo_rl-1.4.5/sumo_rl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-05-07 14:50:56.000000 sumo_rl-1.4.5/sumo_rl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-07 14:50:56.000000 sumo_rl-1.4.5/sumo_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:50:56.000000 sumo_rl-1.4.5/sumo_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-07 14:50:56.000000 sumo_rl-1.4.5/sumo_rl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 14:50:56.000000 sumo_rl-1.4.5/sumo_rl.egg-info/top_level.txt
```

### Comparing `sumo-rl-1.4.4/LICENSE` & `sumo_rl-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.4/PKG-INFO` & `sumo_rl-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumo-rl
-Version: 1.4.4
+Version: 1.4.5
 Summary: RL environments and learning code for traffic signal control in SUMO.
 Author-email: Lucas Alegre <lucasnale@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://lucasalegre.github.io/sumo-rl
 Project-URL: Repository, https://github.com/LucasAlegre/sumo-rl
 Project-URL: Documentation, https://lucasalegre.github.io/sumo-rl
 Project-URL: Bug Report, https://github.com/LucasAlegre/sumo-rl/issues
@@ -24,14 +24,15 @@
 Provides-Extra: all
 Requires-Dist: pyvirtualdisplay; extra == "all"
 Provides-Extra: testing
 Requires-Dist: pytest==7.1.3; extra == "testing"
 
 <img src="docs/_static/logo.png" align="right" width="30%"/>
 
+[![DOI](https://zenodo.org/badge/161216111.svg)](https://zenodo.org/doi/10.5281/zenodo.10869789)
 [![tests](https://github.com/LucasAlegre/sumo-rl/actions/workflows/linux-test.yml/badge.svg)](https://github.com/LucasAlegre/sumo-rl/actions/workflows/linux-test.yml)
 [![PyPI version](https://badge.fury.io/py/sumo-rl.svg)](https://badge.fury.io/py/sumo-rl)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/LucasAlegre/sumo-rl/blob/main/LICENSE)
 
 # SUMO-RL
```

### Comparing `sumo-rl-1.4.4/README.md` & `sumo_rl-1.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 <img src="docs/_static/logo.png" align="right" width="30%"/>
 
+[![DOI](https://zenodo.org/badge/161216111.svg)](https://zenodo.org/doi/10.5281/zenodo.10869789)
 [![tests](https://github.com/LucasAlegre/sumo-rl/actions/workflows/linux-test.yml/badge.svg)](https://github.com/LucasAlegre/sumo-rl/actions/workflows/linux-test.yml)
 [![PyPI version](https://badge.fury.io/py/sumo-rl.svg)](https://badge.fury.io/py/sumo-rl)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/LucasAlegre/sumo-rl/blob/main/LICENSE)
 
 # SUMO-RL
```

### Comparing `sumo-rl-1.4.4/pyproject.toml` & `sumo_rl-1.4.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,17 @@
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["sumo_rl", "sumo_rl.*"]
 
 [tool.setuptools.package-data]
-sumo_rl = [
-    "nets/*",
+"*" = ["*.xml", "*.sumocfg"]
+nets = [
+    "*.xml", "*.sumocfg",
 ]
 
 # Linters and Test tools #######################################################
 
 [tool.black]
 safe = true
 line-length = 127
```

### Comparing `sumo-rl-1.4.4/setup.py` & `sumo_rl-1.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.4/sumo_rl/agents/ql_agent.py` & `sumo_rl-1.4.5/sumo_rl/agents/ql_agent.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.4/sumo_rl/environment/env.py` & `sumo_rl-1.4.5/sumo_rl/environment/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,15 +301,15 @@
         """Apply the action(s) and then step the simulation for delta_time seconds.
 
         Args:
             action (Union[dict, int]): action(s) to be applied to the environment.
             If single_agent is True, action is an int, otherwise it expects a dict with keys corresponding to traffic signal ids.
         """
         # No action, follow fixed TL defined in self.phases
-        if action is None or action == {}:
+        if self.fixed_ts or action is None or action == {}:
             for _ in range(self.delta_time):
                 self._sumo_step()
         else:
             self._apply_actions(action)
             self._run_steps()
 
         observations = self._compute_observations()
@@ -360,23 +360,35 @@
         if self.add_per_agent_info:
             info.update(self._get_per_agent_info())
         self.metrics.append(info.copy())
         return info
 
     def _compute_observations(self):
         self.observations.update(
-            {ts: self.traffic_signals[ts].compute_observation() for ts in self.ts_ids if self.traffic_signals[ts].time_to_act}
+            {
+                ts: self.traffic_signals[ts].compute_observation()
+                for ts in self.ts_ids
+                if self.traffic_signals[ts].time_to_act or self.fixed_ts
+            }
         )
-        return {ts: self.observations[ts].copy() for ts in self.observations.keys() if self.traffic_signals[ts].time_to_act}
+        return {
+            ts: self.observations[ts].copy()
+            for ts in self.observations.keys()
+            if self.traffic_signals[ts].time_to_act or self.fixed_ts
+        }
 
     def _compute_rewards(self):
         self.rewards.update(
-            {ts: self.traffic_signals[ts].compute_reward() for ts in self.ts_ids if self.traffic_signals[ts].time_to_act}
+            {
+                ts: self.traffic_signals[ts].compute_reward()
+                for ts in self.ts_ids
+                if self.traffic_signals[ts].time_to_act or self.fixed_ts
+            }
         )
-        return {ts: self.rewards[ts] for ts in self.rewards.keys() if self.traffic_signals[ts].time_to_act}
+        return {ts: self.rewards[ts] for ts in self.rewards.keys() if self.traffic_signals[ts].time_to_act or self.fixed_ts}
 
     @property
     def observation_space(self):
         """Return the observation space of a traffic signal.
 
         Only used in case of single-agent environment.
         """
@@ -576,18 +588,24 @@
         agent = self.agent_selection
         if not self.action_spaces[agent].contains(action):
             raise Exception(
                 "Action for agent {} must be in Discrete({})."
                 "It is currently {}".format(agent, self.action_spaces[agent].n, action)
             )
 
-        self.env._apply_actions({agent: action})
+        if not self.env.fixed_ts:
+            self.env._apply_actions({agent: action})
 
         if self._agent_selector.is_last():
-            self.env._run_steps()
+            if not self.env.fixed_ts:
+                self.env._run_steps()
+            else:
+                for _ in range(self.env.delta_time):
+                    self.env._sumo_step()
+
             self.env._compute_observations()
             self.rewards = self.env._compute_rewards()
             self.compute_info()
         else:
             self._clear_rewards()
 
         done = self.env._compute_dones()["__all__"]
```

### Comparing `sumo-rl-1.4.4/sumo_rl/environment/observations.py` & `sumo_rl-1.4.5/sumo_rl/environment/observations.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.4/sumo_rl/environment/resco_envs.py` & `sumo_rl-1.4.5/sumo_rl/environment/resco_envs.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
     Number of agents = 16
     Number of actions = 4
     Agents have the same observation and action space
     """
     kwargs.update(
         {
-            "net_file": PATH + "/../nets/RESCO/grid4x4/grid4x4.net.xml",
-            "route_file": PATH + "/../nets/RESCO/grid4x4/grid4x4_1.rou.xml",
+            "net_file": PATH + "/nets/RESCO/grid4x4/grid4x4.net.xml",
+            "route_file": PATH + "/nets/RESCO/grid4x4/grid4x4_1.rou.xml",
             "num_seconds": 3600,
         }
     )
     if parallel:
         return parallel_env(**kwargs)
     else:
         return env(**kwargs)
@@ -33,16 +33,16 @@
 
     Number of agents = 16
     Number of actions = 5
     Agents have the same observation and action space
     """
     kwargs.update(
         {
-            "net_file": PATH + "/../nets/RESCO/arterial4x4/arterial4x4.net.xml",
-            "route_file": PATH + "/../nets/RESCO/arterial4x4/arterial4x4_1.rou.xml",
+            "net_file": PATH + "/nets/RESCO/arterial4x4/arterial4x4.net.xml",
+            "route_file": PATH + "/nets/RESCO/arterial4x4/arterial4x4_1.rou.xml",
             "num_seconds": 3600,
         }
     )
     if parallel:
         return parallel_env(**kwargs)
     else:
         return env(**kwargs)
@@ -52,16 +52,16 @@
     """Cologne 1 network.
 
     Number of agents: 1
     Number of actions: 4
     """
     kwargs.update(
         {
-            "net_file": PATH + "/../nets/RESCO/cologne1/cologne1.net.xml",
-            "route_file": PATH + "/../nets/RESCO/cologne1/cologne1.rou.xml",
+            "net_file": PATH + "/nets/RESCO/cologne1/cologne1.net.xml",
+            "route_file": PATH + "/nets/RESCO/cologne1/cologne1.rou.xml",
             "begin_time": 25200,
             "num_seconds": 28800 - 25200,
         }
     )
     if parallel:
         return parallel_env(**kwargs)
     else:
@@ -73,16 +73,16 @@
 
     Number of agents: 3
     Number of actions: 2 agents with 4 actions and 1 agent with 3 actions
     2 agents have the same observation and action space and 1 has different spaces
     """
     kwargs.update(
         {
-            "net_file": PATH + "/../nets/RESCO/cologne3/cologne3.net.xml",
-            "route_file": PATH + "/../nets/RESCO/cologne3/cologne3.rou.xml",
+            "net_file": PATH + "/nets/RESCO/cologne3/cologne3.net.xml",
+            "route_file": PATH + "/nets/RESCO/cologne3/cologne3.rou.xml",
             "begin_time": 25200,
             "num_seconds": 28800 - 25200,
         }
     )
     if parallel:
         return parallel_env(**kwargs)
     else:
@@ -93,16 +93,16 @@
     """Cologne 8 network.
 
     Number of agents: 8
     Number of actions: variable
     """
     kwargs.update(
         {
-            "net_file": PATH + "/../nets/RESCO/cologne8/cologne8.net.xml",
-            "route_file": PATH + "/../nets/RESCO/cologne8/cologne8.rou.xml",
+            "net_file": PATH + "/nets/RESCO/cologne8/cologne8.net.xml",
+            "route_file": PATH + "/nets/RESCO/cologne8/cologne8.rou.xml",
             "begin_time": 25200,
             "num_seconds": 28800 - 25200,
         }
     )
     if parallel:
         return parallel_env(**kwargs)
     else:
@@ -113,16 +113,16 @@
     """Ingolstadt 1 network.
 
     Number of agents: 1
     Number of actions: 3
     """
     kwargs.update(
         {
-            "net_file": PATH + "/../nets/RESCO/ingolstadt1/ingolstadt1.net.xml",
-            "route_file": PATH + "/../nets/RESCO/ingolstadt1/ingolstadt1.rou.xml",
+            "net_file": PATH + "/nets/RESCO/ingolstadt1/ingolstadt1.net.xml",
+            "route_file": PATH + "/nets/RESCO/ingolstadt1/ingolstadt1.rou.xml",
             "begin_time": 57600,
             "num_seconds": 61200 - 57600,
         }
     )
     if parallel:
         return parallel_env(**kwargs)
     else:
@@ -133,16 +133,16 @@
     """Ingolstadt 7 network.
 
     Number of agents: 7
     Number of actions: variable
     """
     kwargs.update(
         {
-            "net_file": PATH + "/../nets/RESCO/ingolstadt7/ingolstadt7.net.xml",
-            "route_file": PATH + "/../nets/RESCO/ingolstadt7/ingolstadt7.rou.xml",
+            "net_file": PATH + "/nets/RESCO/ingolstadt7/ingolstadt7.net.xml",
+            "route_file": PATH + "/nets/RESCO/ingolstadt7/ingolstadt7.rou.xml",
             "begin_time": 57600,
             "num_seconds": 61200 - 57600,
         }
     )
     if parallel:
         return parallel_env(**kwargs)
     else:
@@ -153,16 +153,16 @@
     """Ingolstadt 21 network.
 
     Number of agents: 21
     Number of actions: variable
     """
     kwargs.update(
         {
-            "net_file": PATH + "/../nets/RESCO/ingolstadt21/ingolstadt21.net.xml",
-            "route_file": PATH + "/../nets/RESCO/ingolstadt21/ingolstadt21.rou.xml",
+            "net_file": PATH + "/nets/RESCO/ingolstadt21/ingolstadt21.net.xml",
+            "route_file": PATH + "/nets/RESCO/ingolstadt21/ingolstadt21.rou.xml",
             "begin_time": 57600,
             "num_seconds": 61200 - 57600,
         }
     )
     if parallel:
         return parallel_env(**kwargs)
     else:
```

### Comparing `sumo-rl-1.4.4/sumo_rl/environment/traffic_signal.py` & `sumo_rl-1.4.5/sumo_rl/environment/traffic_signal.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.4/sumo_rl/exploration/epsilon_greedy.py` & `sumo_rl-1.4.5/sumo_rl/exploration/epsilon_greedy.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.4/sumo_rl/exploration/plot_epsilon.py` & `sumo_rl-1.4.5/sumo_rl/exploration/plot_epsilon.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.4/sumo_rl/util/gen_route.py` & `sumo_rl-1.4.5/sumo_rl/util/gen_route.py`

 * *Files identical despite different names*

### Comparing `sumo-rl-1.4.4/sumo_rl.egg-info/PKG-INFO` & `sumo_rl-1.4.5/sumo_rl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumo-rl
-Version: 1.4.4
+Version: 1.4.5
 Summary: RL environments and learning code for traffic signal control in SUMO.
 Author-email: Lucas Alegre <lucasnale@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://lucasalegre.github.io/sumo-rl
 Project-URL: Repository, https://github.com/LucasAlegre/sumo-rl
 Project-URL: Documentation, https://lucasalegre.github.io/sumo-rl
 Project-URL: Bug Report, https://github.com/LucasAlegre/sumo-rl/issues
@@ -24,14 +24,15 @@
 Provides-Extra: all
 Requires-Dist: pyvirtualdisplay; extra == "all"
 Provides-Extra: testing
 Requires-Dist: pytest==7.1.3; extra == "testing"
 
 <img src="docs/_static/logo.png" align="right" width="30%"/>
 
+[![DOI](https://zenodo.org/badge/161216111.svg)](https://zenodo.org/doi/10.5281/zenodo.10869789)
 [![tests](https://github.com/LucasAlegre/sumo-rl/actions/workflows/linux-test.yml/badge.svg)](https://github.com/LucasAlegre/sumo-rl/actions/workflows/linux-test.yml)
 [![PyPI version](https://badge.fury.io/py/sumo-rl.svg)](https://badge.fury.io/py/sumo-rl)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/LucasAlegre/sumo-rl/blob/main/LICENSE)
 
 # SUMO-RL
```

