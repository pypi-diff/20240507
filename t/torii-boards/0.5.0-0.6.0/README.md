# Comparing `tmp/torii-boards-0.5.0.tar.gz` & `tmp/torii_boards-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torii-boards-0.5.0.tar", last modified: Mon Oct 23 21:50:09 2023, max compression
+gzip compressed data, was "torii_boards-0.6.0.tar", last modified: Tue May  7 06:23:49 2024, max compression
```

## Comparing `torii-boards-0.5.0.tar` & `torii_boards-0.6.0.tar`

### file list

```diff
@@ -1,128 +1,139 @@
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.447409 torii-boards-0.5.0/
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.424076 torii-boards-0.5.0/.github/
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.427410 torii-boards-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1445 2022-12-18 05:55:54.000000 torii-boards-0.5.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      113 2022-12-18 05:55:31.000000 torii-boards-0.5.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      678 2022-12-18 05:55:23.000000 torii-boards-0.5.0/.github/ISSUE_TEMPLATE/feature_request.yml
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.427410 torii-boards-0.5.0/.github/workflows/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      845 2023-05-26 20:44:40.000000 torii-boards-0.5.0/.github/workflows/codeql.yml
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1053 2022-11-22 07:12:56.000000 torii-boards-0.5.0/.github/workflows/docs.yaml
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1291 2023-05-26 20:45:05.000000 torii-boards-0.5.0/.github/workflows/pr.yaml
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1096 2023-02-13 11:01:31.000000 torii-boards-0.5.0/.github/workflows/tests.yaml
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      195 2022-11-21 03:54:50.000000 torii-boards-0.5.0/.gitignore
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3131 2023-10-23 21:48:10.000000 torii-boards-0.5.0/CHANGELOG.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5222 2022-11-10 02:32:05.000000 torii-boards-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      922 2023-02-11 23:31:53.000000 torii-boards-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1366 2023-02-03 05:13:18.000000 torii-boards-0.5.0/LICENSE
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1896 2023-10-23 21:50:09.447409 torii-boards-0.5.0/PKG-INFO
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      353 2022-12-02 20:13:07.000000 torii-boards-0.5.0/README.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.430743 torii-boards-0.5.0/contrib/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      298 2022-11-21 03:55:08.000000 torii-boards-0.5.0/contrib/.flake8
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       30 2022-11-21 03:55:11.000000 torii-boards-0.5.0/contrib/.mypy.ini
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.430743 torii-boards-0.5.0/docs/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        8 2022-11-22 06:57:36.000000 torii-boards-0.5.0/docs/.gitignore
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.424076 torii-boards-0.5.0/docs/_static/
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.430743 torii-boards-0.5.0/docs/_static/css/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5062 2022-12-02 18:22:01.000000 torii-boards-0.5.0/docs/_static/css/styles.css
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       33 2022-12-02 18:33:02.000000 torii-boards-0.5.0/docs/changelog.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1938 2023-10-23 20:07:10.000000 torii-boards-0.5.0/docs/conf.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.430743 torii-boards-0.5.0/docs/gowin/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      360 2023-10-23 21:37:14.000000 torii-boards-0.5.0/docs/gowin/index.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      600 2023-10-23 21:37:25.000000 torii-boards-0.5.0/docs/index.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.430743 torii-boards-0.5.0/docs/intel/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1007 2022-12-02 19:10:53.000000 torii-boards-0.5.0/docs/intel/index.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.430743 torii-boards-0.5.0/docs/lattice/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2936 2023-10-23 20:06:47.000000 torii-boards-0.5.0/docs/lattice/index.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.430743 torii-boards-0.5.0/docs/quicklogic/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      342 2022-12-02 19:11:15.000000 torii-boards-0.5.0/docs/quicklogic/index.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       80 2022-12-02 18:22:37.000000 torii-boards-0.5.0/docs/requirements.txt
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.430743 torii-boards-0.5.0/docs/xilinx/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1844 2022-12-02 19:11:56.000000 torii-boards-0.5.0/docs/xilinx/index.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2522 2023-02-27 09:30:20.000000 torii-boards-0.5.0/noxfile.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       38 2023-10-23 21:50:09.447409 torii-boards-0.5.0/setup.cfg
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2444 2023-10-23 20:37:28.000000 torii-boards-0.5.0/setup.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.430743 torii-boards-0.5.0/torii_boards/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      465 2022-11-21 05:03:49.000000 torii-boards-0.5.0/torii_boards/__init__.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.434076 torii-boards-0.5.0/torii_boards/gowin/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-23 21:28:41.000000 torii-boards-0.5.0/torii_boards/gowin/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2366 2023-10-23 21:38:39.000000 torii-boards-0.5.0/torii_boards/gowin/tang_nano.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.434076 torii-boards-0.5.0/torii_boards/intel/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2022-11-21 04:03:29.000000 torii-boards-0.5.0/torii_boards/intel/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3413 2022-12-18 13:39:06.000000 torii-boards-0.5.0/torii_boards/intel/arrow_deca.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3862 2022-12-18 13:39:11.000000 torii-boards-0.5.0/torii_boards/intel/chameleon96.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4642 2022-12-18 13:39:17.000000 torii-boards-0.5.0/torii_boards/intel/de0.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4278 2022-12-18 13:39:14.000000 torii-boards-0.5.0/torii_boards/intel/de0_cv.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3807 2022-12-18 13:38:58.000000 torii-boards-0.5.0/torii_boards/intel/de10_lite.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3976 2023-10-23 20:42:48.000000 torii-boards-0.5.0/torii_boards/intel/de10_nano.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3611 2022-12-18 13:39:02.000000 torii-boards-0.5.0/torii_boards/intel/de1_soc.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5950 2023-10-23 20:43:05.000000 torii-boards-0.5.0/torii_boards/intel/mister.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4316 2022-12-18 13:38:45.000000 torii-boards-0.5.0/torii_boards/intel/rz_easyfpga_a2_2.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.440743 torii-boards-0.5.0/torii_boards/lattice/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2022-11-21 04:03:27.000000 torii-boards-0.5.0/torii_boards/lattice/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2638 2023-10-23 20:04:41.000000 torii-boards-0.5.0/torii_boards/lattice/blackice.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2681 2023-10-23 21:11:27.000000 torii-boards-0.5.0/torii_boards/lattice/blackice_ii.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4880 2023-10-23 20:03:30.000000 torii-boards-0.5.0/torii_boards/lattice/colorlight_5a75b_r7_0.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     6447 2023-10-23 20:03:31.000000 torii-boards-0.5.0/torii_boards/lattice/ecp5_5g_evn.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7923 2023-10-23 20:03:31.000000 torii-boards-0.5.0/torii_boards/lattice/ecpix5.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1678 2023-10-23 20:04:43.000000 torii-boards-0.5.0/torii_boards/lattice/fomu_hacker.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1688 2023-10-23 20:04:43.000000 torii-boards-0.5.0/torii_boards/lattice/fomu_pvt.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1883 2023-10-23 20:04:43.000000 torii-boards-0.5.0/torii_boards/lattice/ice40_hx1k_blink_evn.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2438 2023-10-23 20:04:43.000000 torii-boards-0.5.0/torii_boards/lattice/ice40_hx8k_b_evn.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2424 2023-10-23 20:04:43.000000 torii-boards-0.5.0/torii_boards/lattice/ice40_up5k_b_evn.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3021 2023-10-23 20:04:43.000000 torii-boards-0.5.0/torii_boards/lattice/icebreaker.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3081 2023-10-23 20:04:41.000000 torii-boards-0.5.0/torii_boards/lattice/icebreaker_bitsy.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1782 2023-10-23 20:04:43.000000 torii-boards-0.5.0/torii_boards/lattice/icestick.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2361 2023-10-23 20:04:41.000000 torii-boards-0.5.0/torii_boards/lattice/icesugar.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1616 2023-10-23 20:04:43.000000 torii-boards-0.5.0/torii_boards/lattice/icesugar_nano.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5127 2023-10-23 20:03:30.000000 torii-boards-0.5.0/torii_boards/lattice/logicbone.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2670 2023-10-23 20:05:45.000000 torii-boards-0.5.0/torii_boards/lattice/machxo3_sk.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1676 2023-10-23 21:38:48.000000 torii-boards-0.5.0/torii_boards/lattice/nandland_go.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4198 2023-10-23 20:03:30.000000 torii-boards-0.5.0/torii_boards/lattice/orangecrab_r0_1.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4932 2023-10-23 20:36:04.000000 torii-boards-0.5.0/torii_boards/lattice/orangecrab_r0_2.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     6831 2023-10-23 21:39:04.000000 torii-boards-0.5.0/torii_boards/lattice/supercon19badge.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      674 2023-10-23 20:05:05.000000 torii-boards-0.5.0/torii_boards/lattice/tinyfpga_ax1.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      675 2023-10-23 20:05:05.000000 torii-boards-0.5.0/torii_boards/lattice/tinyfpga_ax2.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1773 2023-10-23 20:04:41.000000 torii-boards-0.5.0/torii_boards/lattice/tinyfpga_bx.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7951 2023-10-23 20:03:32.000000 torii-boards-0.5.0/torii_boards/lattice/ulx3s.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1248 2023-10-23 20:04:43.000000 torii-boards-0.5.0/torii_boards/lattice/upduino_v1.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1021 2022-12-18 13:34:14.000000 torii-boards-0.5.0/torii_boards/lattice/upduino_v2.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1614 2023-10-23 21:39:40.000000 torii-boards-0.5.0/torii_boards/lattice/upduino_v3.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7244 2023-10-23 20:03:30.000000 torii-boards-0.5.0/torii_boards/lattice/versa_ecp5.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      384 2022-11-21 15:18:13.000000 torii-boards-0.5.0/torii_boards/lattice/versa_ecp5_5g.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        0 2022-12-02 19:39:42.000000 torii-boards-0.5.0/torii_boards/py.typed
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.440743 torii-boards-0.5.0/torii_boards/quicklogic/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2022-11-21 04:36:03.000000 torii-boards-0.5.0/torii_boards/quicklogic/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2436 2022-12-18 13:34:06.000000 torii-boards-0.5.0/torii_boards/quicklogic/quickfeather.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.444076 torii-boards-0.5.0/torii_boards/test/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2022-11-21 04:57:28.000000 torii-boards-0.5.0/torii_boards/test/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1418 2022-11-22 06:42:20.000000 torii-boards-0.5.0/torii_boards/test/blinky.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.447409 torii-boards-0.5.0/torii_boards/xilinx/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2022-12-02 18:47:30.000000 torii-boards-0.5.0/torii_boards/xilinx/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3060 2022-12-18 13:34:01.000000 torii-boards-0.5.0/torii_boards/xilinx/alchitry_au.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7705 2022-12-18 13:33:57.000000 torii-boards-0.5.0/torii_boards/xilinx/arty_a7.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8065 2023-02-27 09:18:16.000000 torii-boards-0.5.0/torii_boards/xilinx/arty_s7.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4653 2022-12-18 13:33:14.000000 torii-boards-0.5.0/torii_boards/xilinx/arty_z7.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    10970 2023-02-27 09:18:35.000000 torii-boards-0.5.0/torii_boards/xilinx/atlys.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2669 2023-10-23 21:38:53.000000 torii-boards-0.5.0/torii_boards/xilinx/cmod_a7.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2387 2023-10-23 21:38:59.000000 torii-boards-0.5.0/torii_boards/xilinx/cmod_s7.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1254 2022-12-18 13:33:01.000000 torii-boards-0.5.0/torii_boards/xilinx/ebaz4205.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    11854 2022-12-18 13:32:57.000000 torii-boards-0.5.0/torii_boards/xilinx/genesys2.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1302 2022-12-18 13:32:34.000000 torii-boards-0.5.0/torii_boards/xilinx/kc705.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1198 2022-12-18 13:32:31.000000 torii-boards-0.5.0/torii_boards/xilinx/kcu105.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8118 2022-11-27 12:27:00.000000 torii-boards-0.5.0/torii_boards/xilinx/mega65.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7757 2022-12-18 13:32:26.000000 torii-boards-0.5.0/torii_boards/xilinx/mercury.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1790 2022-11-26 12:46:27.000000 torii-boards-0.5.0/torii_boards/xilinx/microzed_z010.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1788 2022-12-02 18:52:46.000000 torii-boards-0.5.0/torii_boards/xilinx/microzed_z020.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7311 2022-12-18 13:32:15.000000 torii-boards-0.5.0/torii_boards/xilinx/nexys4ddr.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1599 2022-11-26 13:32:32.000000 torii-boards-0.5.0/torii_boards/xilinx/numato_mimas.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1735 2022-11-26 13:32:35.000000 torii-boards-0.5.0/torii_boards/xilinx/sk_xc6slx9.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2376 2022-11-26 13:32:37.000000 torii-boards-0.5.0/torii_boards/xilinx/te0714_03_50_2I.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1213 2022-11-26 12:47:57.000000 torii-boards-0.5.0/torii_boards/xilinx/zturn_lite_z007s.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      209 2022-11-26 13:32:43.000000 torii-boards-0.5.0/torii_boards/xilinx/zturn_lite_z010.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-23 21:50:09.434076 torii-boards-0.5.0/torii_boards.egg-info/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1896 2023-10-23 21:50:09.000000 torii-boards-0.5.0/torii_boards.egg-info/PKG-INFO
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3209 2023-10-23 21:50:09.000000 torii-boards-0.5.0/torii_boards.egg-info/SOURCES.txt
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        1 2023-10-23 21:50:09.000000 torii-boards-0.5.0/torii_boards.egg-info/dependency_links.txt
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       27 2023-10-23 21:50:09.000000 torii-boards-0.5.0/torii_boards.egg-info/requires.txt
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       13 2023-10-23 21:50:09.000000 torii-boards-0.5.0/torii_boards.egg-info/top_level.txt
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        1 2022-11-26 13:36:50.000000 torii-boards-0.5.0/torii_boards.egg-info/zip-safe
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.457485 torii_boards-0.6.0/
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.300819 torii_boards-0.6.0/.github/
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.344152 torii_boards-0.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1445 2022-12-18 05:55:54.000000 torii_boards-0.6.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      113 2022-12-18 05:55:31.000000 torii_boards-0.6.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      678 2022-12-18 05:55:23.000000 torii_boards-0.6.0/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.367485 torii_boards-0.6.0/.github/workflows/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      845 2024-03-14 08:08:26.000000 torii_boards-0.6.0/.github/workflows/codeql.yml
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1004 2024-03-14 08:08:59.000000 torii_boards-0.6.0/.github/workflows/docs.yaml
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1407 2024-03-14 08:09:14.000000 torii_boards-0.6.0/.github/workflows/pr.yaml
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1292 2024-03-14 08:09:44.000000 torii_boards-0.6.0/.github/workflows/tests.yaml
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      195 2022-11-21 03:54:50.000000 torii_boards-0.6.0/.gitignore
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3577 2024-05-07 06:20:15.000000 torii_boards-0.6.0/CHANGELOG.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5222 2022-11-10 02:32:05.000000 torii_boards-0.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      922 2023-02-11 23:31:53.000000 torii_boards-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1366 2023-02-03 05:13:18.000000 torii_boards-0.6.0/LICENSE
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1897 2024-05-07 06:23:49.454152 torii_boards-0.6.0/PKG-INFO
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      353 2022-12-02 20:13:07.000000 torii_boards-0.6.0/README.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.367485 torii_boards-0.6.0/contrib/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      298 2022-11-21 03:55:08.000000 torii_boards-0.6.0/contrib/.flake8
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       30 2022-11-21 03:55:11.000000 torii_boards-0.6.0/contrib/.mypy.ini
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.370818 torii_boards-0.6.0/docs/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        8 2022-11-22 06:57:36.000000 torii_boards-0.6.0/docs/.gitignore
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.304152 torii_boards-0.6.0/docs/_static/
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.370818 torii_boards-0.6.0/docs/_static/css/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5062 2022-12-02 18:22:01.000000 torii_boards-0.6.0/docs/_static/css/styles.css
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       33 2022-12-02 18:33:02.000000 torii_boards-0.6.0/docs/changelog.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1938 2023-10-23 20:07:10.000000 torii_boards-0.6.0/docs/conf.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.390819 torii_boards-0.6.0/docs/gowin/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      358 2023-10-23 22:48:34.000000 torii_boards-0.6.0/docs/gowin/index.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      600 2023-10-23 21:37:25.000000 torii_boards-0.6.0/docs/index.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.390819 torii_boards-0.6.0/docs/intel/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1007 2022-12-02 19:10:53.000000 torii_boards-0.6.0/docs/intel/index.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.400819 torii_boards-0.6.0/docs/lattice/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2936 2023-10-23 20:06:47.000000 torii_boards-0.6.0/docs/lattice/index.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.400819 torii_boards-0.6.0/docs/quicklogic/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      342 2022-12-02 19:11:15.000000 torii_boards-0.6.0/docs/quicklogic/index.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       80 2022-12-02 18:22:37.000000 torii_boards-0.6.0/docs/requirements.txt
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.407485 torii_boards-0.6.0/docs/xilinx/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1844 2022-12-02 19:11:56.000000 torii_boards-0.6.0/docs/xilinx/index.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2516 2023-10-23 21:54:25.000000 torii_boards-0.6.0/noxfile.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       38 2024-05-07 06:23:49.457485 torii_boards-0.6.0/setup.cfg
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2445 2024-05-07 05:59:28.000000 torii_boards-0.6.0/setup.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.420819 torii_boards-0.6.0/torii_boards/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      465 2022-11-21 05:03:49.000000 torii_boards-0.6.0/torii_boards/__init__.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.427485 torii_boards-0.6.0/torii_boards/altera/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2024-05-07 06:00:00.000000 torii_boards-0.6.0/torii_boards/altera/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3419 2024-05-07 06:14:04.000000 torii_boards-0.6.0/torii_boards/altera/arrow_deca.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3868 2024-05-07 06:14:08.000000 torii_boards-0.6.0/torii_boards/altera/chameleon96.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4648 2024-05-07 06:14:18.000000 torii_boards-0.6.0/torii_boards/altera/de0.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4284 2024-05-07 06:14:13.000000 torii_boards-0.6.0/torii_boards/altera/de0_cv.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3810 2024-05-07 06:13:48.000000 torii_boards-0.6.0/torii_boards/altera/de10_lite.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3982 2024-05-07 06:13:53.000000 torii_boards-0.6.0/torii_boards/altera/de10_nano.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3614 2024-05-07 06:13:48.000000 torii_boards-0.6.0/torii_boards/altera/de1_soc.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5956 2024-05-07 06:12:59.000000 torii_boards-0.6.0/torii_boards/altera/mister.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4323 2024-05-07 06:12:10.000000 torii_boards-0.6.0/torii_boards/altera/rz_easyfpga_a2_2.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.427485 torii_boards-0.6.0/torii_boards/gowin/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-23 21:28:41.000000 torii_boards-0.6.0/torii_boards/gowin/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2366 2023-10-23 21:38:39.000000 torii_boards-0.6.0/torii_boards/gowin/tang_nano.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.430819 torii_boards-0.6.0/torii_boards/intel/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2022-11-21 04:03:29.000000 torii_boards-0.6.0/torii_boards/intel/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      554 2024-05-07 06:09:45.000000 torii_boards-0.6.0/torii_boards/intel/arrow_deca.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      561 2024-05-07 06:10:09.000000 torii_boards-0.6.0/torii_boards/intel/chameleon96.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      529 2024-05-07 06:10:32.000000 torii_boards-0.6.0/torii_boards/intel/de0.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      538 2024-05-07 06:10:18.000000 torii_boards-0.6.0/torii_boards/intel/de0_cv.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      550 2024-05-07 06:11:04.000000 torii_boards-0.6.0/torii_boards/intel/de10_lite.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      550 2024-05-07 06:11:15.000000 torii_boards-0.6.0/torii_boards/intel/de10_nano.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      542 2024-05-07 06:10:54.000000 torii_boards-0.6.0/torii_boards/intel/de1_soc.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      541 2024-05-07 06:11:23.000000 torii_boards-0.6.0/torii_boards/intel/mister.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      575 2024-05-07 06:07:07.000000 torii_boards-0.6.0/torii_boards/intel/rz_easyfpga_a2_2.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.444152 torii_boards-0.6.0/torii_boards/lattice/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2022-11-21 04:03:27.000000 torii_boards-0.6.0/torii_boards/lattice/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2638 2023-10-23 20:04:41.000000 torii_boards-0.6.0/torii_boards/lattice/blackice.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2681 2023-10-23 21:11:27.000000 torii_boards-0.6.0/torii_boards/lattice/blackice_ii.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4880 2023-10-23 20:03:30.000000 torii_boards-0.6.0/torii_boards/lattice/colorlight_5a75b_r7_0.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     6447 2023-10-23 20:03:31.000000 torii_boards-0.6.0/torii_boards/lattice/ecp5_5g_evn.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7923 2023-10-23 20:03:31.000000 torii_boards-0.6.0/torii_boards/lattice/ecpix5.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1678 2023-10-23 20:04:43.000000 torii_boards-0.6.0/torii_boards/lattice/fomu_hacker.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1688 2023-10-23 20:04:43.000000 torii_boards-0.6.0/torii_boards/lattice/fomu_pvt.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1883 2023-10-23 20:04:43.000000 torii_boards-0.6.0/torii_boards/lattice/ice40_hx1k_blink_evn.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2438 2023-10-23 20:04:43.000000 torii_boards-0.6.0/torii_boards/lattice/ice40_hx8k_b_evn.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2424 2023-10-23 20:04:43.000000 torii_boards-0.6.0/torii_boards/lattice/ice40_up5k_b_evn.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3021 2023-10-23 20:04:43.000000 torii_boards-0.6.0/torii_boards/lattice/icebreaker.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3081 2023-10-23 20:04:41.000000 torii_boards-0.6.0/torii_boards/lattice/icebreaker_bitsy.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1782 2023-10-23 20:04:43.000000 torii_boards-0.6.0/torii_boards/lattice/icestick.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2361 2023-10-23 20:04:41.000000 torii_boards-0.6.0/torii_boards/lattice/icesugar.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1616 2023-10-23 20:04:43.000000 torii_boards-0.6.0/torii_boards/lattice/icesugar_nano.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5127 2023-10-23 20:03:30.000000 torii_boards-0.6.0/torii_boards/lattice/logicbone.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2670 2023-10-23 20:05:45.000000 torii_boards-0.6.0/torii_boards/lattice/machxo3_sk.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1676 2023-10-23 21:38:48.000000 torii_boards-0.6.0/torii_boards/lattice/nandland_go.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4198 2023-10-23 20:03:30.000000 torii_boards-0.6.0/torii_boards/lattice/orangecrab_r0_1.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4932 2023-10-23 20:36:04.000000 torii_boards-0.6.0/torii_boards/lattice/orangecrab_r0_2.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     6832 2024-03-14 07:39:28.000000 torii_boards-0.6.0/torii_boards/lattice/supercon19badge.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      674 2023-10-23 20:05:05.000000 torii_boards-0.6.0/torii_boards/lattice/tinyfpga_ax1.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      675 2023-10-23 20:05:05.000000 torii_boards-0.6.0/torii_boards/lattice/tinyfpga_ax2.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1773 2023-10-23 20:04:41.000000 torii_boards-0.6.0/torii_boards/lattice/tinyfpga_bx.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7951 2023-10-23 20:03:32.000000 torii_boards-0.6.0/torii_boards/lattice/ulx3s.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1248 2023-10-23 20:04:43.000000 torii_boards-0.6.0/torii_boards/lattice/upduino_v1.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1021 2022-12-18 13:34:14.000000 torii_boards-0.6.0/torii_boards/lattice/upduino_v2.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1614 2023-10-23 21:39:40.000000 torii_boards-0.6.0/torii_boards/lattice/upduino_v3.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7244 2023-10-23 20:03:30.000000 torii_boards-0.6.0/torii_boards/lattice/versa_ecp5.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      384 2022-11-21 15:18:13.000000 torii_boards-0.6.0/torii_boards/lattice/versa_ecp5_5g.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        0 2022-12-02 19:39:42.000000 torii_boards-0.6.0/torii_boards/py.typed
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.444152 torii_boards-0.6.0/torii_boards/quicklogic/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2022-11-21 04:36:03.000000 torii_boards-0.6.0/torii_boards/quicklogic/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2436 2022-12-18 13:34:06.000000 torii_boards-0.6.0/torii_boards/quicklogic/quickfeather.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.447485 torii_boards-0.6.0/torii_boards/test/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2022-11-21 04:57:28.000000 torii_boards-0.6.0/torii_boards/test/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1418 2022-11-22 06:42:20.000000 torii_boards-0.6.0/torii_boards/test/blinky.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.454152 torii_boards-0.6.0/torii_boards/xilinx/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2022-12-02 18:47:30.000000 torii_boards-0.6.0/torii_boards/xilinx/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3060 2022-12-18 13:34:01.000000 torii_boards-0.6.0/torii_boards/xilinx/alchitry_au.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7705 2022-12-18 13:33:57.000000 torii_boards-0.6.0/torii_boards/xilinx/arty_a7.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8065 2023-02-27 09:18:16.000000 torii_boards-0.6.0/torii_boards/xilinx/arty_s7.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4653 2022-12-18 13:33:14.000000 torii_boards-0.6.0/torii_boards/xilinx/arty_z7.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    10970 2023-02-27 09:18:35.000000 torii_boards-0.6.0/torii_boards/xilinx/atlys.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2669 2023-10-23 21:38:53.000000 torii_boards-0.6.0/torii_boards/xilinx/cmod_a7.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2387 2023-10-23 21:38:59.000000 torii_boards-0.6.0/torii_boards/xilinx/cmod_s7.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1254 2022-12-18 13:33:01.000000 torii_boards-0.6.0/torii_boards/xilinx/ebaz4205.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    11854 2022-12-18 13:32:57.000000 torii_boards-0.6.0/torii_boards/xilinx/genesys2.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1302 2022-12-18 13:32:34.000000 torii_boards-0.6.0/torii_boards/xilinx/kc705.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1198 2022-12-18 13:32:31.000000 torii_boards-0.6.0/torii_boards/xilinx/kcu105.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8118 2022-11-27 12:27:00.000000 torii_boards-0.6.0/torii_boards/xilinx/mega65.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7757 2022-12-18 13:32:26.000000 torii_boards-0.6.0/torii_boards/xilinx/mercury.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1790 2022-11-26 12:46:27.000000 torii_boards-0.6.0/torii_boards/xilinx/microzed_z010.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1788 2022-12-02 18:52:46.000000 torii_boards-0.6.0/torii_boards/xilinx/microzed_z020.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7311 2022-12-18 13:32:15.000000 torii_boards-0.6.0/torii_boards/xilinx/nexys4ddr.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1599 2022-11-26 13:32:32.000000 torii_boards-0.6.0/torii_boards/xilinx/numato_mimas.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1735 2022-11-26 13:32:35.000000 torii_boards-0.6.0/torii_boards/xilinx/sk_xc6slx9.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2376 2022-11-26 13:32:37.000000 torii_boards-0.6.0/torii_boards/xilinx/te0714_03_50_2I.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1213 2022-11-26 12:47:57.000000 torii_boards-0.6.0/torii_boards/xilinx/zturn_lite_z007s.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      209 2022-11-26 13:32:43.000000 torii_boards-0.6.0/torii_boards/xilinx/zturn_lite_z010.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 06:23:49.454152 torii_boards-0.6.0/torii_boards.egg-info/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1897 2024-05-07 06:23:47.000000 torii_boards-0.6.0/torii_boards.egg-info/PKG-INFO
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3534 2024-05-07 06:23:49.000000 torii_boards-0.6.0/torii_boards.egg-info/SOURCES.txt
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        1 2024-05-07 06:23:47.000000 torii_boards-0.6.0/torii_boards.egg-info/dependency_links.txt
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       27 2024-05-07 06:23:47.000000 torii_boards-0.6.0/torii_boards.egg-info/requires.txt
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       13 2024-05-07 06:23:47.000000 torii_boards-0.6.0/torii_boards.egg-info/top_level.txt
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        1 2022-11-26 13:36:50.000000 torii_boards-0.6.0/torii_boards.egg-info/zip-safe
```

### Comparing `torii-boards-0.5.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `torii_boards-0.6.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `torii_boards-0.6.0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/.github/workflows/codeql.yml` & `torii_boards-0.6.0/.github/workflows/codeql.yml`

 * *Files 26% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     strategy:
       fail-fast: false
       matrix:
         language: [ 'python' ]
 
     steps:
     - name: Setup Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: 3.11
 
     - name: Checkout repository
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     - name: Initialize CodeQL
-      uses: github/codeql-action/init@v2
+      uses: github/codeql-action/init@v3
       with:
         languages: ${{ matrix.language }}
 
     - name: Autobuild
-      uses: github/codeql-action/autobuild@v2
+      uses: github/codeql-action/autobuild@v3
 
     - name: Perform CodeQL Analysis
-      uses: github/codeql-action/analyze@v2
+      uses: github/codeql-action/analyze@v3
       with:
         category: "/language:${{matrix.language}}"
```

### Comparing `torii-boards-0.5.0/.github/workflows/docs.yaml` & `torii_boards-0.6.0/.github/workflows/docs.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
       - 'main'
 
 jobs:
   build-docs:
     runs-on: ubuntu-latest
     steps:
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
-          python-version: 3.9
+          python-version: "3.10"
 
       - name: Initialize Env
         shell: bash
         env:
           WORKSPACE: ${{ github.workspace }}
         run: |
           echo "$HOME/.local/bin:$PATH" >> $GITHUB_PATH
           echo "GITHUB_WORKSPACE=\"`pwd`\"" >> $GITHUB_ENV
 
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Setup
         shell: bash
         run: |
           sudo apt-get update
@@ -36,11 +36,10 @@
         shell: bash
         run: |
           nox -s docs
 
       - name: Deploy
         uses: JamesIves/github-pages-deploy-action@v4
         with:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-          BRANCH: gh-pages
-          FOLDER: build/docs/
-          CLEAN: true
+          branch: gh-pages
+          folder: build/docs/
+          clean: true
```

### Comparing `torii-boards-0.5.0/.github/workflows/pr.yaml` & `torii_boards-0.6.0/.github/workflows/pr.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -3,36 +3,36 @@
   pull_request: {}
 
 jobs:
   test-torii:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ '3.9', '3.10', '3.11', '3.12-dev', 'pypy-3.9-v7.3.11']
+        python-version: ['3.10', '3.11', '3.12', 'pypy3.10-v7.3.15']
       fail-fast: true
 
     steps:
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Initialize Env
         shell: bash
         env:
           WORKSPACE: ${{ github.workspace }}
         run: |
           echo "$HOME/.local/bin:$PATH" >> $GITHUB_PATH
           echo "GITHUB_WORKSPACE=\"`pwd`\"" >> $GITHUB_ENV
 
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Setup OSS CAD Suite
-        uses: YosysHQ/setup-oss-cad-suite@v2
+        uses: YosysHQ/setup-oss-cad-suite@v3
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Setup
         shell: bash
         run: |
           python -m pip install --user --upgrade pip setuptools wheel setuptools_scm nox
@@ -46,8 +46,12 @@
       - name: Run Tests
         shell: bash
         run: |
           nox -s test
 
       - name: Codecov
         if: success() && github.repository == 'shrine-maiden-heavy-industries/torii-boards'
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
+        with:
+          verbose: true
+          files: ./build/tests/coverage.xml
+          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `torii-boards-0.5.0/.github/workflows/tests.yaml` & `torii_boards-0.6.0/.github/workflows/tests.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -6,44 +6,51 @@
   pull_request: {}
 
 jobs:
   test-torii:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ '3.9', '3.10', '3.11', ]
+        python-version: ['3.10', '3.11', '3.12']
       fail-fast: false
 
     steps:
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Initialize Env
         shell: bash
         env:
           WORKSPACE: ${{ github.workspace }}
         run: |
           echo "$HOME/.local/bin:$PATH" >> $GITHUB_PATH
           echo "GITHUB_WORKSPACE=\"`pwd`\"" >> $GITHUB_ENV
 
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Setup OSS CAD Suite
-        uses: YosysHQ/setup-oss-cad-suite@v2
+        uses: YosysHQ/setup-oss-cad-suite@v3
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Setup
         shell: bash
         run: |
           python -m pip install --user --upgrade pip setuptools wheel setuptools_scm nox
 
 
       - name: Run Tests
         shell: bash
         run: |
           nox -s test
+
+      - name: Codecov Upload
+        uses: codecov/codecov-action@v4
+        with:
+          verbose: true
+          files: ./build/tests/coverage.xml
+          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `torii-boards-0.5.0/CHANGELOG.md` & `torii_boards-0.6.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,29 @@
 ## [Unreleased]
 ### Added
 ### Changed
 ### Deprecated
 ### Removed
 ### Fixed
 
+## [0.6.0]
+
+### Changed
+
+ - Bumped the minium version of Python to match with Torii 0.6.0
+ - Bumped the minimum version of Torii to be 0.6.0
+
+### Deprecated
+
+ - Deprecated the `torii_boards.intel` boards in favor of `torii_boards.altera`, following the `IntelPlatform` deprecation in Torii 0.6.0
+
+### Fixed
+
+ - Fixed the Gowin boards title in the docs
+
 ## [0.5.0]
 
 ### Added
 
  - Added the `cmod_a7` and `cmod_s7` Xilinx FPGA boards from digilent.
  - Added the `Upduino v3` Lattice FPGA board from TinyVision.
  - Added the `Tang Nano` Gowin FPGA board from sipeed.
@@ -77,13 +92,14 @@
 - Fixed indentation.
 
 ## [0.1.0] - [0.3.0]
 
 No changelog is provided for these versions as they are all older untagged releases of [Amaranth Boards](https://github.com/amaranth-lang/amaranth-boards) from before the fork.
 
 
-[unreleased]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.5.0...main
+[unreleased]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.6.0...main
+[0.5.0]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.5.0...v0.6.0
 [0.4.1]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.4.1...v0.5.0
 [0.4.1]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.4.0...v0.4.1
 [0.4.0]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/amaranth-fork...v0.4.0
 [0.3.0]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/amaranth-fork...main
 [0.1.0]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/amaranth-fork...main
```

### Comparing `torii-boards-0.5.0/CODE_OF_CONDUCT.md` & `torii_boards-0.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/CONTRIBUTING.md` & `torii_boards-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/LICENSE` & `torii_boards-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/PKG-INFO` & `torii_boards-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torii-boards
-Version: 0.5.0
+Version: 0.6.0
 Summary: Board and connector definitions for Torii-HDL
 Home-page: https://torii-boards.shmdn.link/
 Author: Aki Van Ness, Rachel Mant
 Author-email: aki@lethalbit.net, git@dragonmux.network
 License:  BSD-2-Clause
 Project-URL: Documentation, https://torii-boards.shmdn.link/
 Project-URL: Source Code, https://github.com/shrine-maiden-heavy-industries/torii-boards
@@ -22,18 +22,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Python: ~=3.9
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torii<1.0,>=0.5
+Requires-Dist: torii<1.0,>=0.6
 Provides-Extra: dev
 Requires-Dist: nox; extra == "dev"
 
 # Torii-HDL Board Definitions
 
 This package contains evaluation board definitions for [Torii](https://github.com/shrine-maiden-heavy-industries/torii-hdl)
```

### Comparing `torii-boards-0.5.0/docs/_static/css/styles.css` & `torii_boards-0.6.0/docs/_static/css/styles.css`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/docs/conf.py` & `torii_boards-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/docs/index.md` & `torii_boards-0.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/docs/intel/index.md` & `torii_boards-0.6.0/docs/intel/index.md`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/docs/lattice/index.md` & `torii_boards-0.6.0/docs/lattice/index.md`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/docs/xilinx/index.md` & `torii_boards-0.6.0/docs/xilinx/index.md`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/noxfile.py` & `torii_boards-0.6.0/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,9 +92,9 @@
 @nox.session
 def upload(session: nox.Session) -> None:
 	session.install('twine')
 	dist(session)
 	session.log(f'Uploading torii-boards-{torii_boards_version()} to PyPi')
 	session.run(
 		'python', '-m', 'twine',
-		'upload', f'{DIST_DIR}/torii-boards-{torii_boards_version()}*'
+		'upload', f'{DIST_DIR}/torii*-{torii_boards_version()}*'
 	)
```

### Comparing `torii-boards-0.5.0/setup.py` & `torii_boards-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,29 +28,29 @@
 	]),
 	author_email     = ', '.join([
 		'aki@lethalbit.net',
 		'git@dragonmux.network',
 	]),
 	description      = 'Board and connector definitions for Torii-HDL',
 	license          = ' BSD-2-Clause',
-	python_requires  = '~=3.9',
+	python_requires  = '~=3.10',
 	zip_safe         = True,
 	url              = 'https://torii-boards.shmdn.link/',
 
 	long_description = README_FILE.read_text(),
 	long_description_content_type = 'text/markdown',
 
 	setup_requires   = [
 		'wheel',
 		'setuptools',
 		'setuptools_scm'
 	],
 
 	install_requires = [
-		'torii>=0.5,<1.0',
+		'torii>=0.6,<1.0',
 	],
 
 	extras_require   = {
 		'dev': [
 			'nox'
 		],
 	},
```

### Comparing `torii-boards-0.5.0/torii_boards/gowin/tang_nano.py` & `torii_boards-0.6.0/torii_boards/gowin/tang_nano.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/intel/arrow_deca.py` & `torii_boards-0.6.0/torii_boards/altera/arrow_deca.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
-from torii.build                 import Connector, Resource, Pins, Clock, Attrs
-from torii.build.run             import BuildProducts
-from torii.platform.vendor.intel import IntelPlatform
-from torii.platform.resources    import LEDResources, ButtonResources, SwitchResources
+from torii.build                  import Connector, Resource, Pins, Clock, Attrs
+from torii.build.run              import BuildProducts
+from torii.platform.vendor.altera import AlteraPlatform
+from torii.platform.resources     import LEDResources, ButtonResources, SwitchResources
 
 __all__ = (
 	'ArrowDECAPlatform',
 )
 
 
-class ArrowDECAPlatform(IntelPlatform):
+class ArrowDECAPlatform(AlteraPlatform):
 	device      = '10M50DA' # MAX 10
 	package     = 'F484'
 	speed       = 'C6'
 	suffix      = 'GES'
 	default_clk = 'clk50'
 
 	resources   = [
```

### Comparing `torii-boards-0.5.0/torii_boards/intel/chameleon96.py` & `torii_boards-0.6.0/torii_boards/altera/chameleon96.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
-from torii.build                 import Connector, Resource, Pins, Subsignal, Attrs
-from torii.build.run             import BuildProducts
-from torii.platform.vendor.intel import IntelPlatform
-from torii.platform.resources    import (
+from torii.build                  import Connector, Resource, Pins, Subsignal, Attrs
+from torii.build.run              import BuildProducts
+from torii.platform.vendor.altera import AlteraPlatform
+from torii.platform.resources     import (
 	LEDResources, I2CResource, SDCardResources, UARTResource
 )
 
 __all__ = (
 	'Chameleon96Platform',
 )
 
-class Chameleon96Platform(IntelPlatform):
+class Chameleon96Platform(AlteraPlatform):
 	device      = '5CSEBA6' # Cyclone V SE 110K LEs
 	package     = 'U19'     # UBGA-484
 	speed       = 'I7'
 	default_clk = 'cyclonev_oscillator'
 
 	resources   = [
 		# WIFI and BT LEDs
```

### Comparing `torii-boards-0.5.0/torii_boards/intel/de0.py` & `torii_boards-0.6.0/torii_boards/altera/de0.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
-from torii.build                 import Connector, Resource, Pins, Clock, Attrs, Subsignal
-from torii.build.run             import BuildProducts
-from torii.platform.vendor.intel import IntelPlatform
-from torii.platform.resources    import (
+from torii.build                  import Connector, Resource, Pins, Clock, Attrs, Subsignal
+from torii.build.run              import BuildProducts
+from torii.platform.vendor.altera import AlteraPlatform
+from torii.platform.resources     import (
 	LEDResources, ButtonResources, SwitchResources, Display7SegResource,
 	UARTResource, VGAResource, PS2Resource, SDCardResources, SDRAMResource,
 	NORFlashResources
 )
 
 __all__ = (
 	'DE0Platform',
 )
 
-class DE0Platform(IntelPlatform):
+class DE0Platform(AlteraPlatform):
 	device      = 'EP3C16' # Cyclone III 15K LEs
 	package     = 'F484'   # FBGA-484
 	speed       = 'C6'
 	default_clk = 'clk50'
 
 	resources   = [
 		Resource(
```

### Comparing `torii-boards-0.5.0/torii_boards/intel/de0_cv.py` & `torii_boards-0.6.0/torii_boards/altera/de0_cv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
-from torii.build                 import Connector, Resource, Pins, Clock, Attrs
-from torii.build.run             import BuildProducts
-from torii.platform.vendor.intel import IntelPlatform
-from torii.platform.resources    import (
+from torii.build                  import Connector, Resource, Pins, Clock, Attrs
+from torii.build.run              import BuildProducts
+from torii.platform.vendor.altera import AlteraPlatform
+from torii.platform.resources     import (
 	LEDResources, ButtonResources, SwitchResources, Display7SegResource,
 	VGAResource, PS2Resource, SDCardResources, SDRAMResource
 )
 
 __all__ = (
 	'DE0CVPlatform',
 )
 
 
-class DE0CVPlatform(IntelPlatform):
+class DE0CVPlatform(AlteraPlatform):
 	device      = '5CEBA4' # Cyclone V 49K LEs
 	package     = 'F23'    # FBGA-484
 	speed       = 'C7'
 	default_clk = 'clk50'
 	resources   = [
 		Resource(
 			'clk50', 0, Pins('M9', dir = 'i'),  Clock(50e6), Attrs(io_standard = '3.3-V LVTTL')
```

### Comparing `torii-boards-0.5.0/torii_boards/intel/de10_lite.py` & `torii_boards-0.6.0/torii_boards/altera/de10_lite.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
 from torii.build                 import Connector, Resource, Pins, Clock, Attrs
 from torii.build.run             import BuildProducts
-from torii.platform.vendor.intel import IntelPlatform
+from torii.platform.vendor.altera import AlteraPlatform
 from torii.platform.resources    import (
 	LEDResources, ButtonResources, SwitchResources, Display7SegResource,
 	UARTResource, SDRAMResource, VGAResource
 )
 
 __all__ = (
 	'DE10LitePlatform',
 )
 
 
-class DE10LitePlatform(IntelPlatform):
+class DE10LitePlatform(AlteraPlatform):
 	device      = '10M50DA' # MAX10
 	package     = 'F484'    # FBGA-484
 	speed       = 'C7'
 	suffix      = 'G'
 	default_clk = 'clk50'
 
 	resources   = [
```

### Comparing `torii-boards-0.5.0/torii_boards/intel/de10_nano.py` & `torii_boards-0.6.0/torii_boards/altera/de10_nano.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
-from torii.build                 import (
+from torii.build                  import (
 	Connector, Resource, Pins, Clock, Attrs, Subsignal
 )
-from torii.build.run             import BuildProducts
-from torii.platform.vendor.intel import IntelPlatform
-from torii.platform.resources    import (
+from torii.build.run              import BuildProducts
+from torii.platform.vendor.altera import AlteraPlatform
+from torii.platform.resources     import (
 	LEDResources, ButtonResources, SwitchResources, UARTResource,
 	SPIResource
 )
 
 __all__ = (
 	'DE10NanoPlatform',
 )
 
 
 # The MiSTer platform is built around the DE10-Nano; if you update one you should update the other.
-class DE10NanoPlatform(IntelPlatform):
+class DE10NanoPlatform(AlteraPlatform):
 	device      = '5CSEBA6' # Cyclone V 110K LEs
 	package     = 'U23'     # UBGA-484
 	speed       = 'I7'
 	default_clk = 'clk50'
 
 	resources   = [
 		Resource(
```

### Comparing `torii-boards-0.5.0/torii_boards/intel/de1_soc.py` & `torii_boards-0.6.0/torii_boards/altera/de1_soc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
 from torii.build                 import Connector, Resource, Pins, Clock, Attrs
 from torii.build.run             import BuildProducts
-from torii.platform.vendor.intel import IntelPlatform
+from torii.platform.vendor.altera import AlteraPlatform
 from torii.platform.resources    import (
 	LEDResources, ButtonResources, SwitchResources, Display7SegResource
 )
 
 __all__ = (
 	'DE1SoCPlatform',
 )
 
 
-class DE1SoCPlatform(IntelPlatform):
+class DE1SoCPlatform(AlteraPlatform):
 	device      = '5CSEMA5' # Cyclone V 85K LEs
 	package     = 'F31'     # FBGA-896
 	speed       = 'C6'
 	default_clk = 'clk50'
 
 	resources   = [
 		Resource(
```

### Comparing `torii-boards-0.5.0/torii_boards/intel/mister.py` & `torii_boards-0.6.0/torii_boards/altera/mister.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
-from torii.build                 import (
+from torii.build                  import (
 	Connector, Resource, Pins, Clock, Attrs, Subsignal, PinsN
 )
-from torii.build.run             import BuildProducts
-from torii.platform.vendor.intel import IntelPlatform
-from torii.platform.resources    import (
+from torii.build.run              import BuildProducts
+from torii.platform.vendor.altera import AlteraPlatform
+from torii.platform.resources     import (
 	LEDResources, ButtonResources, SwitchResources, UARTResource, SPIResource,
 	SDRAMResource, SDCardResources, VGAResource
 )
 
 __all__ = (
 	'MisterPlatform',
 )
 
 
 # The MiSTer platform is built around the DE10-Nano; if you update one you should update the other.
-class MisterPlatform(IntelPlatform):
+class MisterPlatform(AlteraPlatform):
 	device      = '5CSEBA6' # Cyclone V 110K LEs
 	package     = 'U23'     # UBGA-484
 	speed       = 'I7'
 	default_clk = 'clk50'
 
 	resources   = [
 		Resource(
```

### Comparing `torii-boards-0.5.0/torii_boards/intel/rz_easyfpga_a2_2.py` & `torii_boards-0.6.0/torii_boards/altera/rz_easyfpga_a2_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
-from torii.build                 import (
+from torii.build                  import (
 	Connector, Resource, Pins, Clock, Attrs, Subsignal, PinsN
 )
-from torii.hdl.ir                import Fragment
-from torii.build.run             import BuildProducts
-from torii.platform.vendor.intel import IntelPlatform
-from torii.platform.resources    import (
+from torii.hdl.ir                 import Fragment
+from torii.build.run              import BuildProducts
+from torii.platform.vendor.altera import AlteraPlatform
+from torii.platform.resources     import (
 	LEDResources, ButtonResources, SDRAMResource, VGAResource, Display7SegResource,
 	PS2Resource, I2CResource, UARTResource
 )
 
 __all__ = (
 	'RZEasyFPGAA2_2Platform',
 )
 
 
-class RZEasyFPGAA2_2Platform(IntelPlatform):
+class RZEasyFPGAA2_2Platform(AlteraPlatform):
 	device      = 'EP4CE6' # Cyclone IV 6K LEs
 	package     = 'E22'    # EQFP 144 pins
 	speed       = 'C8'
 	default_clk = 'clk50'  # 50MHz builtin clock
 	default_rst = 'rst'
 
 	resources   = [
```

### Comparing `torii-boards-0.5.0/torii_boards/lattice/blackice.py` & `torii_boards-0.6.0/torii_boards/lattice/blackice.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/blackice_ii.py` & `torii_boards-0.6.0/torii_boards/lattice/blackice_ii.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/colorlight_5a75b_r7_0.py` & `torii_boards-0.6.0/torii_boards/lattice/colorlight_5a75b_r7_0.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/ecp5_5g_evn.py` & `torii_boards-0.6.0/torii_boards/lattice/ecp5_5g_evn.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/ecpix5.py` & `torii_boards-0.6.0/torii_boards/lattice/ecpix5.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/fomu_hacker.py` & `torii_boards-0.6.0/torii_boards/lattice/fomu_hacker.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/fomu_pvt.py` & `torii_boards-0.6.0/torii_boards/lattice/fomu_pvt.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/ice40_hx1k_blink_evn.py` & `torii_boards-0.6.0/torii_boards/lattice/ice40_hx1k_blink_evn.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/ice40_hx8k_b_evn.py` & `torii_boards-0.6.0/torii_boards/lattice/ice40_hx8k_b_evn.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/ice40_up5k_b_evn.py` & `torii_boards-0.6.0/torii_boards/lattice/ice40_up5k_b_evn.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/icebreaker.py` & `torii_boards-0.6.0/torii_boards/lattice/icebreaker.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/icebreaker_bitsy.py` & `torii_boards-0.6.0/torii_boards/lattice/icebreaker_bitsy.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/icestick.py` & `torii_boards-0.6.0/torii_boards/lattice/icestick.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/icesugar.py` & `torii_boards-0.6.0/torii_boards/lattice/icesugar.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/icesugar_nano.py` & `torii_boards-0.6.0/torii_boards/lattice/icesugar_nano.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/logicbone.py` & `torii_boards-0.6.0/torii_boards/lattice/logicbone.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/machxo3_sk.py` & `torii_boards-0.6.0/torii_boards/lattice/machxo3_sk.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/nandland_go.py` & `torii_boards-0.6.0/torii_boards/lattice/nandland_go.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/orangecrab_r0_1.py` & `torii_boards-0.6.0/torii_boards/lattice/orangecrab_r0_1.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/orangecrab_r0_2.py` & `torii_boards-0.6.0/torii_boards/lattice/orangecrab_r0_2.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/supercon19badge.py` & `torii_boards-0.6.0/torii_boards/lattice/supercon19badge.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 			Attrs(IO_TYPE = 'LVCMOS33', PULLMODE = 'UP')
 		),
 
 		# Direct HDMI on the bottom of the board.
 		Resource('hdmi', 0,
 			Subsignal('clk', DiffPairsN('P20', 'R20'), Attrs(IO_TYPE = 'TMDS_33')),
 			Subsignal('d', DiffPairs('N19 L20 L16', 'N20 M20 L17'), Attrs(IO_TYPE = 'TMDS_33')),
-			Subsignal('hpd', PinsN('R18'), Attrs(IO_TYPE = 'LVCMOS33')),# Also called HDMI_HEAC_n
+			Subsignal('hpd', PinsN('R18'), Attrs(IO_TYPE = 'LVCMOS33')), # Also called HDMI_HEAC_n
 			Subsignal('hdmi_heac_p', PinsN('T19'), Attrs(IO_TYPE = 'LVCMOS33')),
 			Attrs(DRIVE = '4'),
 		),
 
 		Resource('lcd', 0,
 			Subsignal('db',
 				Pins('J3 H1 K4 J1 K3 K2 L4 K1 L3 L2 M4 L1 M3 M1 N4 N2 N3 N1'),
```

### Comparing `torii-boards-0.5.0/torii_boards/lattice/tinyfpga_ax1.py` & `torii_boards-0.6.0/torii_boards/lattice/tinyfpga_ax1.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/tinyfpga_ax2.py` & `torii_boards-0.6.0/torii_boards/lattice/tinyfpga_ax2.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/tinyfpga_bx.py` & `torii_boards-0.6.0/torii_boards/lattice/tinyfpga_bx.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/ulx3s.py` & `torii_boards-0.6.0/torii_boards/lattice/ulx3s.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/upduino_v1.py` & `torii_boards-0.6.0/torii_boards/lattice/upduino_v1.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/upduino_v2.py` & `torii_boards-0.6.0/torii_boards/lattice/upduino_v2.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/upduino_v3.py` & `torii_boards-0.6.0/torii_boards/lattice/upduino_v3.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/lattice/versa_ecp5.py` & `torii_boards-0.6.0/torii_boards/lattice/versa_ecp5.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/quicklogic/quickfeather.py` & `torii_boards-0.6.0/torii_boards/quicklogic/quickfeather.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/test/blinky.py` & `torii_boards-0.6.0/torii_boards/test/blinky.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/alchitry_au.py` & `torii_boards-0.6.0/torii_boards/xilinx/alchitry_au.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/arty_a7.py` & `torii_boards-0.6.0/torii_boards/xilinx/arty_a7.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/arty_s7.py` & `torii_boards-0.6.0/torii_boards/xilinx/arty_s7.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/arty_z7.py` & `torii_boards-0.6.0/torii_boards/xilinx/arty_z7.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/atlys.py` & `torii_boards-0.6.0/torii_boards/xilinx/atlys.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/cmod_a7.py` & `torii_boards-0.6.0/torii_boards/xilinx/cmod_a7.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/cmod_s7.py` & `torii_boards-0.6.0/torii_boards/xilinx/cmod_s7.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/ebaz4205.py` & `torii_boards-0.6.0/torii_boards/xilinx/ebaz4205.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/genesys2.py` & `torii_boards-0.6.0/torii_boards/xilinx/genesys2.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/kc705.py` & `torii_boards-0.6.0/torii_boards/xilinx/kc705.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/kcu105.py` & `torii_boards-0.6.0/torii_boards/xilinx/kcu105.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/mega65.py` & `torii_boards-0.6.0/torii_boards/xilinx/mega65.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/mercury.py` & `torii_boards-0.6.0/torii_boards/xilinx/mercury.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/microzed_z010.py` & `torii_boards-0.6.0/torii_boards/xilinx/microzed_z010.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/microzed_z020.py` & `torii_boards-0.6.0/torii_boards/xilinx/microzed_z020.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/nexys4ddr.py` & `torii_boards-0.6.0/torii_boards/xilinx/nexys4ddr.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/numato_mimas.py` & `torii_boards-0.6.0/torii_boards/xilinx/numato_mimas.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/sk_xc6slx9.py` & `torii_boards-0.6.0/torii_boards/xilinx/sk_xc6slx9.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/te0714_03_50_2I.py` & `torii_boards-0.6.0/torii_boards/xilinx/te0714_03_50_2I.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards/xilinx/zturn_lite_z007s.py` & `torii_boards-0.6.0/torii_boards/xilinx/zturn_lite_z007s.py`

 * *Files identical despite different names*

### Comparing `torii-boards-0.5.0/torii_boards.egg-info/PKG-INFO` & `torii_boards-0.6.0/torii_boards.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torii-boards
-Version: 0.5.0
+Version: 0.6.0
 Summary: Board and connector definitions for Torii-HDL
 Home-page: https://torii-boards.shmdn.link/
 Author: Aki Van Ness, Rachel Mant
 Author-email: aki@lethalbit.net, git@dragonmux.network
 License:  BSD-2-Clause
 Project-URL: Documentation, https://torii-boards.shmdn.link/
 Project-URL: Source Code, https://github.com/shrine-maiden-heavy-industries/torii-boards
@@ -22,18 +22,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Python: ~=3.9
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torii<1.0,>=0.5
+Requires-Dist: torii<1.0,>=0.6
 Provides-Extra: dev
 Requires-Dist: nox; extra == "dev"
 
 # Torii-HDL Board Definitions
 
 This package contains evaluation board definitions for [Torii](https://github.com/shrine-maiden-heavy-industries/torii-hdl)
```

### Comparing `torii-boards-0.5.0/torii_boards.egg-info/SOURCES.txt` & `torii_boards-0.6.0/torii_boards.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -30,14 +30,24 @@
 torii_boards/py.typed
 torii_boards.egg-info/PKG-INFO
 torii_boards.egg-info/SOURCES.txt
 torii_boards.egg-info/dependency_links.txt
 torii_boards.egg-info/requires.txt
 torii_boards.egg-info/top_level.txt
 torii_boards.egg-info/zip-safe
+torii_boards/altera/__init__.py
+torii_boards/altera/arrow_deca.py
+torii_boards/altera/chameleon96.py
+torii_boards/altera/de0.py
+torii_boards/altera/de0_cv.py
+torii_boards/altera/de10_lite.py
+torii_boards/altera/de10_nano.py
+torii_boards/altera/de1_soc.py
+torii_boards/altera/mister.py
+torii_boards/altera/rz_easyfpga_a2_2.py
 torii_boards/gowin/__init__.py
 torii_boards/gowin/tang_nano.py
 torii_boards/intel/__init__.py
 torii_boards/intel/arrow_deca.py
 torii_boards/intel/chameleon96.py
 torii_boards/intel/de0.py
 torii_boards/intel/de0_cv.py
```

