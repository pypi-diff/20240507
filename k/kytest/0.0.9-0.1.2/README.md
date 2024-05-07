# Comparing `tmp/kytest-0.0.9.tar.gz` & `tmp/kytest-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kytest-0.0.9.tar", last modified: Mon Dec 11 12:26:11 2023, max compression
+gzip compressed data, was "kytest-0.1.2.tar", last modified: Tue May  7 09:13:38 2024, max compression
```

## Comparing `kytest-0.0.9.tar` & `kytest-0.1.2.tar`

### file list

```diff
@@ -1,80 +1,83 @@
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.312135 kytest-0.0.9/
--rw-r--r--   0 UI         (502) staff       (20)      310 2023-12-11 12:26:11.311479 kytest-0.0.9/PKG-INFO
--rw-r--r--   0 UI         (502) staff       (20)     5022 2023-12-06 06:47:55.000000 kytest-0.0.9/README.md
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.265505 kytest-0.0.9/demo/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-11-17 09:46:58.000000 kytest-0.0.9/demo/__init__.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.269543 kytest-0.0.9/demo/pages/
--rw-r--r--   0 UI         (502) staff       (20)       49 2023-11-17 09:46:58.000000 kytest-0.0.9/demo/pages/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      376 2023-11-22 00:59:13.000000 kytest-0.0.9/demo/pages/adr_page.py
--rw-r--r--   0 UI         (502) staff       (20)      383 2023-11-22 09:34:21.000000 kytest-0.0.9/demo/pages/image_page.py
--rw-r--r--   0 UI         (502) staff       (20)      273 2023-11-22 00:56:24.000000 kytest-0.0.9/demo/pages/ios_page.py
--rw-r--r--   0 UI         (502) staff       (20)      619 2023-11-22 09:40:23.000000 kytest-0.0.9/demo/pages/web_page.py
--rw-r--r--   0 UI         (502) staff       (20)      222 2023-12-04 13:15:52.000000 kytest-0.0.9/demo/run.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.274508 kytest-0.0.9/demo/tests/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-11-17 09:46:58.000000 kytest-0.0.9/demo/tests/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      634 2023-12-04 13:14:35.000000 kytest-0.0.9/demo/tests/test_adr.py
--rw-r--r--   0 UI         (502) staff       (20)      544 2023-11-22 01:02:26.000000 kytest-0.0.9/demo/tests/test_api.py
--rw-r--r--   0 UI         (502) staff       (20)      664 2023-12-04 13:15:18.000000 kytest-0.0.9/demo/tests/test_image.py
--rw-r--r--   0 UI         (502) staff       (20)      620 2023-12-04 13:14:52.000000 kytest-0.0.9/demo/tests/test_ios.py
--rw-r--r--   0 UI         (502) staff       (20)     1033 2023-12-04 13:15:18.000000 kytest-0.0.9/demo/tests/test_web.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.277772 kytest-0.0.9/kytest/
--rw-r--r--   0 UI         (502) staff       (20)      521 2023-12-11 12:26:00.000000 kytest-0.0.9/kytest/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     3700 2023-11-22 09:29:35.000000 kytest-0.0.9/kytest/case.py
--rw-r--r--   0 UI         (502) staff       (20)      491 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/cli.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.281278 kytest-0.0.9/kytest/core/
--rw-r--r--   0 UI         (502) staff       (20)       51 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/core/__init__.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.283654 kytest-0.0.9/kytest/core/android/
--rw-r--r--   0 UI         (502) staff       (20)      134 2023-11-22 01:37:15.000000 kytest-0.0.9/kytest/core/android/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     7149 2023-12-06 05:50:28.000000 kytest-0.0.9/kytest/core/android/driver.py
--rw-r--r--   0 UI         (502) staff       (20)     9044 2023-12-07 09:29:06.000000 kytest-0.0.9/kytest/core/android/element.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.285122 kytest-0.0.9/kytest/core/api/
--rw-r--r--   0 UI         (502) staff       (20)        1 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/core/api/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)    12317 2023-12-11 12:25:33.000000 kytest-0.0.9/kytest/core/api/request.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.287518 kytest-0.0.9/kytest/core/image/
--rw-r--r--   0 UI         (502) staff       (20)       53 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/core/image/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     1692 2023-11-22 02:05:24.000000 kytest-0.0.9/kytest/core/image/driver.py
--rw-r--r--   0 UI         (502) staff       (20)     3100 2023-11-22 02:08:29.000000 kytest-0.0.9/kytest/core/image/element.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.290499 kytest-0.0.9/kytest/core/ios/
--rw-r--r--   0 UI         (502) staff       (20)      134 2023-11-22 01:37:52.000000 kytest-0.0.9/kytest/core/ios/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     6582 2023-12-06 05:52:08.000000 kytest-0.0.9/kytest/core/ios/driver.py
--rw-r--r--   0 UI         (502) staff       (20)    11574 2023-12-05 07:23:56.000000 kytest-0.0.9/kytest/core/ios/element.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.293326 kytest-0.0.9/kytest/core/ocr/
--rw-r--r--   0 UI         (502) staff       (20)       85 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/core/ocr/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      746 2023-11-22 02:07:34.000000 kytest-0.0.9/kytest/core/ocr/driver.py
--rw-r--r--   0 UI         (502) staff       (20)     4222 2023-11-22 02:09:35.000000 kytest-0.0.9/kytest/core/ocr/element.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.295760 kytest-0.0.9/kytest/core/web/
--rw-r--r--   0 UI         (502) staff       (20)       95 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/core/web/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     2745 2023-11-22 01:58:00.000000 kytest-0.0.9/kytest/core/web/driver.py
--rw-r--r--   0 UI         (502) staff       (20)    10636 2023-11-22 02:04:39.000000 kytest-0.0.9/kytest/core/web/element.py
--rw-r--r--   0 UI         (502) staff       (20)      772 2023-12-11 06:53:03.000000 kytest-0.0.9/kytest/page.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.297815 kytest-0.0.9/kytest/running/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/running/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      182 2023-12-05 07:51:08.000000 kytest-0.0.9/kytest/running/conf.yml
--rw-r--r--   0 UI         (502) staff       (20)     3809 2023-12-04 13:14:48.000000 kytest-0.0.9/kytest/running/runner.py
--rw-r--r--   0 UI         (502) staff       (20)     2667 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/scaffold.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.299279 kytest-0.0.9/kytest/testdata/
--rw-r--r--   0 UI         (502) staff       (20)    10650 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/testdata/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)    18623 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/testdata/data.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.310844 kytest-0.0.9/kytest/utils/
--rw-r--r--   0 UI         (502) staff       (20)        1 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/utils/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     6789 2023-11-22 02:40:54.000000 kytest-0.0.9/kytest/utils/allure_util.py
--rw-r--r--   0 UI         (502) staff       (20)     8036 2023-11-22 02:43:09.000000 kytest-0.0.9/kytest/utils/common.py
--rw-r--r--   0 UI         (502) staff       (20)     3445 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/utils/config.py
--rw-r--r--   0 UI         (502) staff       (20)     1396 2023-11-22 02:43:46.000000 kytest-0.0.9/kytest/utils/des_util.py
--rw-r--r--   0 UI         (502) staff       (20)     3277 2023-11-22 02:43:56.000000 kytest-0.0.9/kytest/utils/dingtalk.py
--rw-r--r--   0 UI         (502) staff       (20)     3787 2023-11-22 02:44:11.000000 kytest-0.0.9/kytest/utils/excel.py
--rw-r--r--   0 UI         (502) staff       (20)      159 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/utils/exceptions.py
--rw-r--r--   0 UI         (502) staff       (20)      710 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/utils/log.py
--rw-r--r--   0 UI         (502) staff       (20)     3930 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/utils/mail.py
--rw-r--r--   0 UI         (502) staff       (20)     2179 2023-11-17 09:46:58.000000 kytest-0.0.9/kytest/utils/mysql_util.py
--rw-r--r--   0 UI         (502) staff       (20)     2402 2023-11-22 02:45:31.000000 kytest-0.0.9/kytest/utils/pytest_util.py
--rw-r--r--   0 UI         (502) staff       (20)     4022 2023-11-22 02:45:53.000000 kytest-0.0.9/kytest/utils/swagger_util.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-12-11 12:26:11.280804 kytest-0.0.9/kytest.egg-info/
--rw-r--r--   0 UI         (502) staff       (20)      310 2023-12-11 12:26:11.000000 kytest-0.0.9/kytest.egg-info/PKG-INFO
--rw-r--r--   0 UI         (502) staff       (20)     1521 2023-12-11 12:26:11.000000 kytest-0.0.9/kytest.egg-info/SOURCES.txt
--rw-r--r--   0 UI         (502) staff       (20)        1 2023-12-11 12:26:11.000000 kytest-0.0.9/kytest.egg-info/dependency_links.txt
--rw-r--r--   0 UI         (502) staff       (20)       43 2023-12-11 12:26:11.000000 kytest-0.0.9/kytest.egg-info/entry_points.txt
--rw-r--r--   0 UI         (502) staff       (20)      301 2023-12-11 12:26:11.000000 kytest-0.0.9/kytest.egg-info/requires.txt
--rw-r--r--   0 UI         (502) staff       (20)       12 2023-12-11 12:26:11.000000 kytest-0.0.9/kytest.egg-info/top_level.txt
--rw-r--r--   0 UI         (502) staff       (20)       38 2023-12-11 12:26:11.312297 kytest-0.0.9/setup.cfg
--rw-r--r--   0 UI         (502) staff       (20)     1363 2023-11-17 09:53:12.000000 kytest-0.0.9/setup.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.118482 kytest-0.1.2/
+-rw-r--r--   0 UI         (502) staff       (20)      370 2024-05-07 09:13:38.118019 kytest-0.1.2/PKG-INFO
+-rw-r--r--   0 UI         (502) staff       (20)     5180 2024-04-30 01:38:53.000000 kytest-0.1.2/README.md
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.084011 kytest-0.1.2/demo/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-11-17 09:46:58.000000 kytest-0.1.2/demo/__init__.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.085602 kytest-0.1.2/demo/pages/
+-rw-r--r--   0 UI         (502) staff       (20)       49 2023-11-17 09:46:58.000000 kytest-0.1.2/demo/pages/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      681 2024-05-07 08:48:29.000000 kytest-0.1.2/demo/pages/adr_page.py
+-rw-r--r--   0 UI         (502) staff       (20)     1301 2024-05-07 08:47:31.000000 kytest-0.1.2/demo/pages/web_page.py
+-rw-r--r--   0 UI         (502) staff       (20)      138 2024-05-06 07:11:47.000000 kytest-0.1.2/demo/run_adr.py
+-rw-r--r--   0 UI         (502) staff       (20)      170 2024-04-30 09:32:08.000000 kytest-0.1.2/demo/run_api.py
+-rw-r--r--   0 UI         (502) staff       (20)      210 2024-05-06 07:11:56.000000 kytest-0.1.2/demo/run_web.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.087277 kytest-0.1.2/demo/tests/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-11-17 09:46:58.000000 kytest-0.1.2/demo/tests/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      503 2024-05-07 08:48:41.000000 kytest-0.1.2/demo/tests/test_adr.py
+-rw-r--r--   0 UI         (502) staff       (20)      487 2024-04-23 03:27:33.000000 kytest-0.1.2/demo/tests/test_api.py
+-rw-r--r--   0 UI         (502) staff       (20)      452 2024-05-07 08:47:31.000000 kytest-0.1.2/demo/tests/test_web.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.088012 kytest-0.1.2/kytest/
+-rw-r--r--   0 UI         (502) staff       (20)      318 2024-05-07 09:05:34.000000 kytest-0.1.2/kytest/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      190 2024-05-07 08:29:01.000000 kytest-0.1.2/kytest/cli.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.091763 kytest-0.1.2/kytest/core/
+-rw-r--r--   0 UI         (502) staff       (20)       49 2024-05-07 08:25:11.000000 kytest-0.1.2/kytest/core/__init__.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.094680 kytest-0.1.2/kytest/core/adr/
+-rw-r--r--   0 UI         (502) staff       (20)      171 2024-05-06 03:40:30.000000 kytest-0.1.2/kytest/core/adr/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     3615 2024-05-07 08:40:46.000000 kytest-0.1.2/kytest/core/adr/case.py
+-rw-r--r--   0 UI         (502) staff       (20)     5209 2024-05-07 08:49:14.000000 kytest-0.1.2/kytest/core/adr/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     6058 2024-05-07 08:42:04.000000 kytest-0.1.2/kytest/core/adr/element.py
+-rw-r--r--   0 UI         (502) staff       (20)      187 2024-04-23 03:21:17.000000 kytest-0.1.2/kytest/core/adr/page.py
+-rw-r--r--   0 UI         (502) staff       (20)     2365 2024-05-07 08:42:04.000000 kytest-0.1.2/kytest/core/adr/utils.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.096069 kytest-0.1.2/kytest/core/api/
+-rw-r--r--   0 UI         (502) staff       (20)        1 2023-11-17 09:46:58.000000 kytest-0.1.2/kytest/core/api/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     1358 2024-05-07 08:36:23.000000 kytest-0.1.2/kytest/core/api/case.py
+-rw-r--r--   0 UI         (502) staff       (20)    18767 2024-05-06 07:27:04.000000 kytest-0.1.2/kytest/core/api/request.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.097642 kytest-0.1.2/kytest/core/img/
+-rw-r--r--   0 UI         (502) staff       (20)       53 2023-11-17 09:46:58.000000 kytest-0.1.2/kytest/core/img/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     1732 2024-03-15 01:59:59.000000 kytest-0.1.2/kytest/core/img/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     3125 2024-05-07 08:42:59.000000 kytest-0.1.2/kytest/core/img/element.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.100602 kytest-0.1.2/kytest/core/ios/
+-rw-r--r--   0 UI         (502) staff       (20)      169 2024-04-30 07:58:33.000000 kytest-0.1.2/kytest/core/ios/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     3629 2024-05-07 08:43:21.000000 kytest-0.1.2/kytest/core/ios/case.py
+-rw-r--r--   0 UI         (502) staff       (20)     2000 2024-05-07 08:43:39.000000 kytest-0.1.2/kytest/core/ios/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     7739 2024-05-07 08:44:58.000000 kytest-0.1.2/kytest/core/ios/elem.py
+-rw-r--r--   0 UI         (502) staff       (20)      186 2024-04-23 03:22:35.000000 kytest-0.1.2/kytest/core/ios/page.py
+-rw-r--r--   0 UI         (502) staff       (20)     3401 2024-05-07 08:44:58.000000 kytest-0.1.2/kytest/core/ios/utils.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.101785 kytest-0.1.2/kytest/core/ocr/
+-rw-r--r--   0 UI         (502) staff       (20)       85 2023-11-17 09:46:58.000000 kytest-0.1.2/kytest/core/ocr/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      852 2024-05-07 08:44:58.000000 kytest-0.1.2/kytest/core/ocr/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     3505 2024-05-07 08:45:19.000000 kytest-0.1.2/kytest/core/ocr/element.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.104418 kytest-0.1.2/kytest/core/web/
+-rw-r--r--   0 UI         (502) staff       (20)      171 2024-05-06 07:15:50.000000 kytest-0.1.2/kytest/core/web/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     3728 2024-05-07 08:45:38.000000 kytest-0.1.2/kytest/core/web/case.py
+-rw-r--r--   0 UI         (502) staff       (20)     3937 2024-05-06 07:30:07.000000 kytest-0.1.2/kytest/core/web/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     5078 2024-05-07 08:46:12.000000 kytest-0.1.2/kytest/core/web/element.py
+-rw-r--r--   0 UI         (502) staff       (20)      874 2024-05-07 08:46:25.000000 kytest-0.1.2/kytest/core/web/page.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.107734 kytest-0.1.2/kytest/running/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-11-17 09:46:58.000000 kytest-0.1.2/kytest/running/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)       96 2024-04-29 07:45:44.000000 kytest-0.1.2/kytest/running/conf.py
+-rw-r--r--   0 UI         (502) staff       (20)      168 2024-05-07 08:49:37.000000 kytest-0.1.2/kytest/running/conf.yml
+-rw-r--r--   0 UI         (502) staff       (20)     5229 2024-04-29 07:41:25.000000 kytest-0.1.2/kytest/running/execution_scheduler.py
+-rw-r--r--   0 UI         (502) staff       (20)     5713 2024-04-29 07:41:25.000000 kytest-0.1.2/kytest/running/runner.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.117068 kytest-0.1.2/kytest/utils/
+-rw-r--r--   0 UI         (502) staff       (20)        1 2023-11-17 09:46:58.000000 kytest-0.1.2/kytest/utils/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      909 2024-03-18 06:55:00.000000 kytest-0.1.2/kytest/utils/aes_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     7369 2024-02-27 08:34:38.000000 kytest-0.1.2/kytest/utils/allure_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     1508 2024-05-07 08:32:46.000000 kytest-0.1.2/kytest/utils/common.py
+-rw-r--r--   0 UI         (502) staff       (20)     1973 2024-05-07 08:34:09.000000 kytest-0.1.2/kytest/utils/config.py
+-rw-r--r--   0 UI         (502) staff       (20)     3196 2024-05-07 08:33:46.000000 kytest-0.1.2/kytest/utils/cv_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     3266 2024-01-12 13:06:16.000000 kytest-0.1.2/kytest/utils/dingtalk.py
+-rw-r--r--   0 UI         (502) staff       (20)     3908 2024-04-12 06:14:54.000000 kytest-0.1.2/kytest/utils/excel_util.py
+-rw-r--r--   0 UI         (502) staff       (20)      261 2024-05-07 08:31:34.000000 kytest-0.1.2/kytest/utils/log.py
+-rw-r--r--   0 UI         (502) staff       (20)     2269 2024-01-12 13:06:37.000000 kytest-0.1.2/kytest/utils/mail.py
+-rw-r--r--   0 UI         (502) staff       (20)     2126 2024-03-18 06:45:28.000000 kytest-0.1.2/kytest/utils/mysql_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     1536 2024-05-07 09:04:22.000000 kytest-0.1.2/kytest/utils/nacos_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     2524 2024-01-18 02:04:34.000000 kytest-0.1.2/kytest/utils/pytest_util.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2024-05-07 09:13:38.091215 kytest-0.1.2/kytest.egg-info/
+-rw-r--r--   0 UI         (502) staff       (20)      370 2024-05-07 09:13:38.000000 kytest-0.1.2/kytest.egg-info/PKG-INFO
+-rw-r--r--   0 UI         (502) staff       (20)     1618 2024-05-07 09:13:38.000000 kytest-0.1.2/kytest.egg-info/SOURCES.txt
+-rw-r--r--   0 UI         (502) staff       (20)        1 2024-05-07 09:13:38.000000 kytest-0.1.2/kytest.egg-info/dependency_links.txt
+-rw-r--r--   0 UI         (502) staff       (20)       43 2024-05-07 09:13:38.000000 kytest-0.1.2/kytest.egg-info/entry_points.txt
+-rw-r--r--   0 UI         (502) staff       (20)      316 2024-05-07 09:13:38.000000 kytest-0.1.2/kytest.egg-info/requires.txt
+-rw-r--r--   0 UI         (502) staff       (20)       12 2024-05-07 09:13:38.000000 kytest-0.1.2/kytest.egg-info/top_level.txt
+-rw-r--r--   0 UI         (502) staff       (20)       38 2024-05-07 09:13:38.118649 kytest-0.1.2/setup.cfg
+-rw-r--r--   0 UI         (502) staff       (20)     1403 2024-05-07 08:29:17.000000 kytest-0.1.2/setup.py
```

### Comparing `kytest-0.0.9/README.md` & `kytest-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,21 @@
 
 [demo](/demo) 提供了丰富实例，帮你快速了解ktest的用法。
 
 ## 使用方式
 
 ### 安卓
 
+* UI Inspector
+```shell script
+pip install uiauto-dev
+# 启动
+uiauto.dev
+```
+
 * 不同机型设置
     - 小米：开启 “开发者选项” -> "USB调试（安全设置）允许通过usb调试修改权限或模拟点击"
     - OPPO：oppo存在权限监控，需要在开发者-> 开启 禁止权限监控 即可
 
 * 定位方式
     - rid：根据resourceId属性定位
     - className：根据className属性定位
@@ -64,14 +71,21 @@
     - assert_text：断言元素文本属性包含文本关键字
 
 
 ### IOS
 
 * [安装WebDriverAgent](https://testerhome.com/topics/7220)
 
+* UI Inspector
+```shell script
+pip install uiauto-dev
+# 启动
+uiauto.dev
+```
+
 * 定位方式
     - name：根据name属性定位
     - label：根据label属性定位
     - labelCont：模糊匹配label属性
     - value：根据value属性定位
     - valueCont：模糊匹配value属性
     - text：根据text属性定位
```

### Comparing `kytest-0.0.9/kytest/case.py` & `kytest-0.1.2/kytest/core/adr/case.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """
 @Author: kang.yang
 @Date: 2023/10/26 09:48
 """
 import time
+import allure
+
+from .driver import Driver
+from .element import Elem
 
-from urllib import parse
-from typing import Union
 from kytest.utils.log import logger
-from kytest.utils.config import config
+from kytest.utils.config import kconfig
 from kytest.core.api.request import HttpReq
-from kytest.core.ios.driver import IosDriver
-from kytest.core.web.driver import WebDriver
-from kytest.core.android.driver import AdrDriver
+from kytest.running.conf import App
 
 
 class TestCase(HttpReq):
     """
     测试用例基类，所有测试用例需要继承该类
     """
 
-    driver: Union[AdrDriver, IosDriver, WebDriver] = None
+    driver: Driver = None
+    start_auto: bool = True
 
     # ---------------------初始化-------------------------------
     def start_class(self):
         """
         Hook method for setup_class fixture
         :return:
         """
@@ -34,19 +35,25 @@
         Hook method for teardown_class fixture
         :return:
         """
         pass
 
     @classmethod
     def setup_class(cls):
-        cls().start_class()
+        try:
+            cls().start_class()
+        except BaseException as e:
+            logger.error(f"start_class Exception: {e}")
 
     @classmethod
     def teardown_class(cls):
-        cls().end_class()
+        try:
+            cls().end_class()
+        except BaseException as e:
+            logger.error(f"end_class Exception: {e}")
 
     def start(self):
         """
         Hook method for setup_method fixture
         :return:
         """
         pass
@@ -54,84 +61,107 @@
     def end(self):
         """
         Hook method for teardown_method fixture
         :return:
         """
         pass
 
+    def config(self):
+        """
+        目前就是用来设置是否自动启动应用
+        @return:
+        """
+        pass
+
     def setup_method(self):
-        self.start_time = time.time()
+        # 设置调整
+        self.config()
 
-        platform = config.get_common("platform")
-        if platform == "android":
-            device_id = config.get_app("device_id")
-            pkg_name = config.get_app("pkg_name")
-            self.driver = AdrDriver(device_id, pkg_name)
-        elif platform == "ios":
-            device_id = config.get_app("device_id")
-            pkg_name = config.get_app("pkg_name")
-            self.driver = IosDriver(device_id, pkg_name)
-        elif platform == "web":
-            browserName = config.get_web("browser_name")
-            headless = config.get_web("headless")
-            self.driver = WebDriver(browserName=browserName,
-                                    headless=headless)
-
-        if platform in ["android", "ios"]:
-            if config.get_app("auto_start") is True:
-                self.driver.start_app()
+        # 设置默认feature
+        project_name = kconfig['project']
+        if project_name:
+            allure.dynamic.feature(project_name)
+
+        # 驱动初始化
+        self.driver = Driver(App.did)
+
+        # 启动应用
+        if self.start_auto is True:
+            self.driver.util.start_app(App.pkg)
 
         self.start()
 
     def teardown_method(self):
         self.end()
 
-        platform = config.get_common("platform")
-        if platform in ["android", "ios"]:
-            if config.get_app("auto_start") is True:
-                self.driver.stop_app()
-
-        take_time = time.time() - self.start_time
-        logger.info("用例耗时: {:.2f} s".format(take_time))
+        # 停止应用
+        if self.start_auto is True:
+            self.driver.util.stop_app(App.pkg)
 
     # 公共方法
     @staticmethod
     def sleep(n: float):
         """休眠"""
         logger.info(f"暂停: {n}s")
         time.sleep(n)
 
     def screenshot(self, name: str):
         """截图"""
         self.driver.screenshot(name)
 
-    # 安卓方法
-    def assert_act(self, activity_name: str, timeout=5):
-        """断言当前页面的activity"""
-        self.driver.assert_act(activity_name, timeout)
-
-    # web方法
-    def assert_title(self, title: str, timeout: int = 5):
-        """断言页面标题"""
-        self.driver.assert_title(title, timeout)
+    # UI方法
+    def elem(self,
+             rid=None,
+             className=None,
+             text=None,
+             xpath=None,
+             index=None):
+        """
+        元素定位方法
+        @param rid:
+        @param className:
+        @param text:
+        @param xpath:
+        @param index:
+        @return:
+        """
+        _kwargs = {}
+        if rid is not None:
+            _kwargs["resourceId"] = rid
+        if className is not None:
+            _kwargs["className"] = className
+        if text is not None:
+            _kwargs["text"] = text
+        if xpath:
+            _kwargs["xpath"] = xpath
+        if index is not None:
+            _kwargs["instance"] = index
 
-    @staticmethod
-    def is_url_has_http(url):
-        """针对为空和只有路径的情况，使用默认host进行补全"""
-        host = config.get_common("base_url")
-        if url is None:
-            url = host
-        if 'http' not in url:
-            url = parse.urljoin(host, url)
-        return url
-
-    def assert_url(self, url: str = None, timeout: int = 5):
-        """断言页面url"""
-        url = self.is_url_has_http(url)
-        self.driver.assert_url(url, timeout)
-
-    def open(self, url):
-        """打开页面"""
-        url = self.is_url_has_http(url)
-        self.driver.open(url)
+        return Elem(driver=self.driver, **_kwargs)
 
+    def uninstall_app(self):
+        """
+        卸载应用
+        @return:
+        """
+        self.driver.util.uninstall_app(App.pkg)
 
+    def install_app(self, apk_url):
+        """
+        安装应用
+        @return:
+        """
+        self.driver.util.install_app(apk_url)
+
+    def start_app(self):
+        """
+        启动应用
+        @return:
+        """
+        self.driver.util.start_app(App.pkg)
+
+    def stop_app(self):
+        """
+        停止应用
+        @return:
+        """
+        self.driver.util.stop_app(App.pkg)
```

### Comparing `kytest-0.0.9/kytest/core/android/element.py` & `kytest-0.1.2/kytest/core/ios/elem.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,260 +1,256 @@
-import typing
+import time
+import threading
 
-from uiautomator2 import UiObject
-from uiautomator2.xpath import XPathSelector
+from .driver import Driver
 
-from kytest.core.android.driver import AdrDriver
-from kytest.utils.exceptions import KError
 from kytest.utils.log import logger
-from kytest.utils.common import calculate_time, \
-    draw_red_by_coordinate
-from kytest.core.image.element import ImgElem
-from kytest.core.ocr.element import OcrElem
 
 
-class AdrElem(object):
+lock = threading.Lock()
+
+
+class Elem(object):
     """
-    安卓元素定义
+    IOS原生元素定义
     """
 
     def __init__(self,
-                 driver: AdrDriver = None,
-                 rid: str = None,
-                 className: str = None,
+                 driver: Driver = None,
+                 name: str = None,
+                 label: str = None,
+                 value: str = None,
                  text: str = None,
-                 textCont: str = None,
+                 className: str = None,
                  xpath: str = None,
-                 image: str = None,
-                 ocr: str = None,
-                 region: int = None,
-                 grade: float = 0.8,
-                 index: int = None,
-                 _debug: bool = False):
+                 index: int = None):
         """
 
-        @param driver: 安卓驱动
-        @param rid: resourceId定位
+        @param driver: IOS驱动
+        @param name: name定位
+        @param label: label定位
+        @param value: value定位
+        @param text: text定位，应该是包含了label、value
         @param className: className定位
-        @param text: 文本定位
-        @param textCont: 文本模糊匹配
         @param xpath: xpath定位
-        @param image: 图像识别
-        @param ocr: ocr识别
-        @param region: ocr识别区域设置，支持1、2、3、4
-        @param grade: 识别下限得分设置，针对图像识别和ocr识别
-        @param index: 识别到多个元素时，根据index获取其中一个
-        @param _debug: 对定位到的元素进行截图并圈选位置，用于调试
+        @param index: 识别到多个控件时，根据index获取其中一个
         """
         self._kwargs = {}
-        if rid is not None:
-            self._kwargs["resourceId"] = rid
-        if className is not None:
-            self._kwargs["className"] = className
+        if name is not None:
+            self._kwargs["name"] = name
+        if label is not None:
+            self._kwargs["label"] = label
+        if value is not None:
+            self._kwargs["value"] = value
         if text is not None:
             self._kwargs["text"] = text
-        if textCont is not None:
-            self._kwargs["textContains"] = textCont
-        if xpath:
-            self._kwargs["xpath"] = xpath
+        if className is not None:
+            self._kwargs["className"] = className
         if index is not None:
-            self._kwargs["instance"] = index
+            self._kwargs["index"] = index
 
         self._driver = driver
         self._xpath = xpath
-        self._debug = _debug
-        self._image = image
-        self._ocr = ocr
-        self._pos = region
-        self._grade = grade
 
     def __get__(self, instance, owner):
         """po模式中element初始化不需要带driver的关键"""
         if instance is None:
             return None
 
         self._driver = instance.driver
         return self
 
-    @calculate_time
-    def find(self, timeout=10, watch=None):
+    def _match(self, text):
         """
-        增加截图的方法
-        @param timeout: 每次查找时间
-        @param watch: 增加弹窗检测，定位方式列表，用text定位
-        watch为True时，使用内置库
-            when("继续使用")
-            when("移入管控").when("取消")
-            when("^立即(下载|更新)").when("取消")
-            when("同意")
-            when("^(好的|确定)")
-            when("继续安装")
-            when("安装")
-            when("Agree")
-            when("ALLOW")
-        watch为list时，使用内置库+watch
+        判断元素是否存在当前页面
         @return:
         """
-        rid = self._kwargs.get("resourceId", None)
-        if rid is not None:
-            pkg_name = self._driver.pkg_name
-            if pkg_name not in rid:
-                if "id/" not in rid:
-                    self._kwargs["resourceId"] = pkg_name + ":id/" + rid
-                else:
-                    self._kwargs["resourceId"] = pkg_name + ":" + rid
-
-        def _find():
-            if self._xpath is not None:
-                logger.info(f'查找控件: xpath={self._xpath}')
+        _element = self._driver.d(text=text)
+        result = text if _element.wait(timeout=0.1,
+                                       raise_error=False) else None
+        return result
+
+    def watch(self, loc_list, timeout=3):
+        logger.info("开始弹窗检测")
+        # 多线程match，如果match到，获取第一个非None内容，进行点击
+        # match完休息1s，如果休息3s也没有match到，就停止（定义一个flag，match到就清零）
+        # 如果3s内仍然能match到就继续（如果flag大于3就停止）
+        _build_info = ["允许", "使用App时允许", "始终允许", "同意"]
+        if loc_list is True:
+            loc_list = _build_info
+        else:
+            loc_list = list(set(_build_info + loc_list))
+        flag = timeout
+        while flag > 0:
+            import concurrent.futures
+
+            logger.info(f"匹配: {loc_list}")
+            with concurrent.futures.ThreadPoolExecutor() as executor:
+                results = executor.map(self._match, loc_list)
+                results = [item for item in results if item is not None]
+
+            if results:
+                logger.info(f"匹配到: {results}")
+                self._driver.d(text=results[0]).click()
+                logger.info("点击成功")
+                flag = timeout
             else:
-                logger.info(f'查找控件: {self._kwargs}')
-            _element = self._driver.d.xpath(self._xpath) if \
-                self._xpath is not None else self._driver.d(**self._kwargs)
+                logger.info("匹配失败")
+
+            flag -= 1
+            time.sleep(1)
+        logger.info("结束检测")
+
+    def find(self, timeout=5, capture=True):
+        """
+        针对元素定位失败的情况，抛出KError异常
+        @param capture: 查找失败是否截图
+        @param timeout:
+        ["允许", "同意"]
+        @return:
+        """
+        # 元素定义
+        _element = self._driver.d.xpath(self._xpath) if \
+            self._xpath else self._driver.d(**self._kwargs)
 
+        # 定位过程
+        try:
             if _element.wait(timeout=timeout):
                 logger.info(f"查找成功")
-                if self._debug is True:
-                    file_path = self._driver.screenshot("查找成功")
-                    logger.debug(file_path)
-                    draw_red_by_coordinate(file_path, _element.bounds())
                 return _element
             else:
                 logger.info(f"查找失败")
-                self._driver.screenshot("查找失败")
-                raise KError(f"控件: {self._kwargs}, 查找失败")
+                if capture is True:
+                    self._driver.util.screenshot("查找失败")
+                raise Exception(f"控件 {self._kwargs} 查找失败")
+        except ConnectionError:
+            logger.info('wda连接失败, 进行重连!!!')
+            self._driver.util.start_wda()
 
-        if watch:
-            logger.info("开启弹窗检测")
-            if isinstance(watch, list):
-                with self._driver.d.watch_context(builtin=True) as ctx:
-                    for text in watch:
-                        ctx.when(text).click()
-                    ctx.wait_stable()
-                    logger.info("结束检测")
-                    return _find()
+            logger.info('重连成功, 重新开始查找控件')
+            if _element.wait(timeout=timeout):
+                logger.info(f"查找成功")
+                return _element
             else:
-                with self._driver.d.watch_context(builtin=True) as ctx:
-                    ctx.wait_stable()
-                    logger.info("结束检测")
-                    return _find()
-        else:
-            return _find()
+                logger.info(f"查找失败")
+                if capture is True:
+                    self._driver.util.screenshot("查找失败")
+                raise Exception(f"控件 {self._kwargs} 查找失败")
 
     def text(self):
-        logger.info(f"获取文本属性")
-        _elem = self.find(timeout=3)
-        if isinstance(_elem, XPathSelector):
-            elems = _elem.all()
-        else:
-            elems = list(_elem)
-        text = []
-        for elem in elems:
-            text.append(elem.get_text())
-        logger.info(text)
-        return text
+        """获取元素文本"""
+        logger.info(f"获取 {self._kwargs} 文本属性")
+        return self.find().text
 
     def exists(self, timeout=5):
-        logger.info(f"检查控件是否存在")
-        if self._image is not None:
-            return ImgElem(self._driver,
-                           file=self._image,
-                           grade=self._grade,
-                           _debug=self._debug).exists(timeout=timeout)
-        elif self._ocr is not None:
-            return OcrElem(self._driver,
-                           text=self._ocr,
-                           pos=self._pos,
-                           grade=self._grade,
-                           _debug=self._debug).exists(timeout=timeout)
-        else:
+        """
+        判断元素是否存在当前页面
+        @param timeout:
+        @return:
+        """
+        logger.info(f"检查 {self._kwargs} 是否存在")
+        result = False
+        try:
+            _element = self.find(timeout=timeout, capture=False)
+            result = True
+        except:
             result = False
-            try:
-                _element = self.find(timeout=timeout)
-                result = True
-            except Exception as e:
-                logger.debug(str(e))
-                result = False
-            finally:
-                logger.info(result)
-                return result
-
-    @staticmethod
-    def _adapt_center(e: typing.Union[UiObject, XPathSelector],
-                      offset=(0.5, 0.5)):
+        finally:
+            logger.info(result)
+            return result
+
+    def _adapt_center(self, timeout=5):
         """
         修正控件中心坐标
         """
-        if isinstance(e, UiObject):
-            return e.center(offset=offset)
-        else:
-            return e.offset(offset[0], offset[1])
+        bounds = self.find(timeout=timeout).bounds
+        left_top_x, left_top_y, width, height = \
+            bounds.x, bounds.y, bounds.width, bounds.height
+        center_x = int(left_top_x + width/2)
+        center_y = int(left_top_y + height/2)
+        logger.info(f'{center_x}, {center_y}')
+        return center_x, center_y
+
+    def click(self, timeout=5):
+        """
+        单击
+        @param: retry，重试次数
+        @param: timeout，每次重试超时时间
+        """
+        logger.info(f'点击 {self._kwargs}')
 
-    def click(self, timeout=5, watch=None):
-        logger.info(f"点击 {self._kwargs}")
-        if self._image is not None:
-            return ImgElem(self._driver,
-                           file=self._image,
-                           grade=self._grade,
-                           _debug=self._debug).click(timeout=timeout)
-        elif self._ocr is not None:
-            return OcrElem(self._driver,
-                           text=self._ocr,
-                           pos=self._pos,
-                           grade=self._grade,
-                           _debug=self._debug).click(timeout=timeout)
+        def _click():
+            x, y = self._adapt_center(timeout=timeout)
+            self._driver.d.appium_settings({"snapshotMaxDepth": 0})
+            self._driver.d.tap(x, y)
+            self._driver.d.appium_settings({"snapshotMaxDepth": 50})
+
+        count = 0
+        while count < 5:
+            if count > 1:
+                logger.info(f"操作失败，第{count}次重试.")
+            try:
+                _click()
+            except Exception as e:
+                logger.debug(str(e))
+                time.sleep(3)
+                count += 1
+                continue
+            else:
+                break
         else:
-            element = self.find(timeout=timeout, watch=watch)
-            # 这种方式经常点击不成功，感觉是页面刷新有影响
-            # element.click()
-            x, y = self._adapt_center(element)
-            self._driver.d.click(x, y)
+            logger.info("重试5次仍然失败.")
 
-    def click_exists(self, timeout=5, watch=None):
+    def click_exists(self, timeout=5):
         logger.info(f"{self._kwargs} 存在才点击")
         if self.exists(timeout=timeout):
-            self.click(watch=watch)
+            self.click()
 
-    def input(self, text, watch=None, enter=False):
-        logger.info(f"输入文本: {text}")
-        self.find(watch=watch).set_text(text)
-        if enter is True:
-            self._driver.enter()
+    def clear(self, timeout=5):
+        """清除文本"""
+        logger.info("清除输入框文本")
+        self.find(timeout=timeout).clear_text()
+
+    def input(self, text, timeout=5):
+        """输入内容"""
+        logger.info(f"输入文本：{text}")
+        self.find(timeout=timeout).set_text(text)
 
-    def input_exists(self, text: str, timeout=5, watch=None, enter=False):
+    def input_exists(self, text: str, timeout=5):
         logger.info(f"{self._kwargs} 存在才输入: {text}")
         if self.exists(timeout=timeout):
-            self.input(text, watch=watch, enter=enter)
-
-    def input_pwd(self, text, watch=None, enter=False):
-        """密码输入框输入有时候用input输入不了"""
-        logger.info(f"输入密码: {text}")
-        self.find(watch=watch).click()
-        self._driver.d(focused=True).set_text(text)
-        if enter is True:
-            self._driver.enter()
-
-    def clear(self, watch=None):
-        logger.info("清空输入框")
-        self.find(watch=watch).clear_text()
+            self.input(text, timeout=timeout)
+            logger.info("输入成功")
+        else:
+            logger.info("控件不存在")
 
     def assert_exists(self, timeout=3):
         logger.info(f"断言 {self._kwargs} 存在")
         status = self.exists(timeout=timeout)
-        assert status, "控件不存在"
+        assert status, f"控件不存在"
 
-    def assert_text(self, text, timeout=3, watch=None):
+    def assert_text(self, text, timeout=3):
         logger.info(f"断言 {self._kwargs} 文本属性包括: {text}")
-        self.find(timeout=timeout, watch=watch)
+        self.find(timeout=timeout)
         _text = self.text
         assert text in _text, f"文本属性 {_text} 不包含 {text}"
 
 
 if __name__ == '__main__':
     pass
 
 
 
 
 
 
 
+
+
+
+
+
+
+
+
+
+
```

### Comparing `kytest-0.0.9/kytest/core/image/driver.py` & `kytest-0.1.2/kytest/core/img/driver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# 'pip install opencv-python==4.6.0.66'
 import os
 import cv2
 import numpy as np
 
 
 class ImageDiscern:
     def __init__(self, target_image, source_image, grade=0.8, gauss_num=111) -> None:
```

### Comparing `kytest-0.0.9/kytest/core/image/element.py` & `kytest-0.1.2/kytest/core/img/element.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+# 'pip install opencv-python==4.6.0.66'
 import time
 
+from .driver import ImageDiscern
+
 from kytest.utils.log import logger
-from kytest.core.image.driver import ImageDiscern
-from kytest.utils.common import draw_red_by_rect
+from kytest.utils.cv_util import draw_red_by_rect
 
 
 class ImgElem(object):
     """图像识别定位"""
 
     def __init__(self,
                  driver=None,
```

### Comparing `kytest-0.0.9/kytest/core/ocr/element.py` & `kytest-0.1.2/kytest/core/ocr/element.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,37 @@
+# 依赖通过easyocr起一个识别服务
 import time
 
+from typing import Optional, Literal
+
+from .driver import ocr_discern
+
 from kytest.utils.log import logger
-from kytest.utils.exceptions import KError
-from kytest.core.ocr.driver import ocr_discern
-from kytest.utils.common import draw_red_by_rect
-
-# 先上下左右分成四块，然后再上下对半分
-POSITION = {
-    1: "top_left",
-    11: "top_left_1",
-    12: "top_left_2",
-    2: "top_right",
-    21: "top_right_1",
-    22: "top_right_2",
-    3: "bottom_left",
-    31: "bottom_left_1",
-    32: "bottom_left_2",
-    4: "bottom_right",
-    41: "bottom_right_1",
-    42: "bottom_right_2"
-}
+from kytest.utils.cv_util import draw_red_by_rect
 
 
 class OcrElem(object):
     """ocr识别定位"""
 
     def __init__(self,
                  driver=None,
                  text: str = None,
-                 pos: int = None,
+                 pos: Optional[Literal["TOP_LEFT", "TOP_RIGHT", "BOTTOM_LEFT", "BOTTOM_RIGHT"]] = None,
                  grade=0.8,
                  _debug: bool = False):
         """
         @param driver: 设备驱动
         @param text: 需要识别的文本
-        @param pos: 把图片分成八块，具体定义见上POSITION
+        @param pos: 把图片分成四块，TOP_LEFT、TOP_RIGHT、BOTTOM_LEFT、BOTTOM_RIGHT（左上、右上、左下、右下）
         @param grade: 置信度，最大1，越高代表准确率越高
         @param _debug: 截图并圈选位置，用于调试
         """
         self.driver = driver
         self.text = text
         self._position = pos
-        if pos is not None:
-            self._position = POSITION[pos]
         self._grade = grade
         self._debug = _debug
 
     def __get__(self, instance, owner):
         if instance is None:
             return None
 
@@ -68,43 +53,35 @@
             res = ocr_discern(image_path, self.text)
             if res:
                 x, y = res
                 if self._position is not None:
                     logger.debug(self._position)
                     width = info.get("width")
                     height = info.get("height")
-                    cut_height = info.get("cut_height")
 
-                    if 'top_right' in self._position:
+                    if self._position == 'TOP_RIGHT':
                         x = width / 2 + x
-                        if self._position == "top_right_2":
-                            y = y + cut_height
-                    elif 'top_left' in self._position:
-                        if self._position == 'top_left_2':
-                            y = y + cut_height
-                    elif 'bottom_left' in self._position:
+                    elif self._position == 'TOP_LEFT':
+                        pass
+                    elif self._position == 'BOTTOM_LEFT':
                         y = height / 2 + y
-                        if self._position == "bottom_left_2":
-                            y = y + cut_height
-                    elif 'bottom_right' in self._position:
+                    elif self._position == 'BOTTOM_RIGHT':
                         x = width / 2 + x
                         y = height / 2 + y
-                        if self._position == "bottom_right_2":
-                            y = y + cut_height
 
                 x, y = int(x), int(y)
                 logger.info(f'识别坐标为: ({x}, {y})')
                 if self._debug is True:
                     file_path = self.driver.screenshot(f'ocr识别定位成功')
                     draw_red_by_rect(file_path,
                                      (x - 100, y - 100, 200, 200))
                 return x, y
         else:
             self.driver.screenshot(f'ocr识别定位失败')
-            raise KError('通过OCR未识别指定文字或置信度过低，无法进行点击操作！')
+            raise Exception('通过OCR未识别指定文字或置信度过低，无法进行点击操作！')
 
     def exists(self, timeout=1):
         logger.info(f'ocr识别文本: {self.text} 是否存在')
         try:
             self.find_element(timeout=timeout)
         except Exception as e:
             logger.debug(str(e))
@@ -120,7 +97,8 @@
 
 
 if __name__ == '__main__':
     pass
 
 
 
+
```

### Comparing `kytest-0.0.9/kytest/core/web/driver.py` & `kytest-0.1.2/kytest/core/ios/driver.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,92 @@
-"""
-@Author: kang.yang
-@Date: 2023/5/12 20:49
-"""
-from kytest.utils.log import logger
-from kytest.utils.common import screenshot_util
-from playwright.sync_api import sync_playwright, expect
+import time
+
+import allure
+import wda
 
+from .utils import Utils
+
+from kytest.utils.log import logger
+from kytest.utils.common import general_file_path
 
-class WebDriver:
 
-    def __init__(self, browserName: str, headless: bool = False, state: dict = None):
-        logger.info("初始化playwright驱动")
+class Driver(object):
 
-        self.browserName = browserName
-        self.headless = headless
-        self.playwright = sync_playwright().start()
-        if browserName == 'firefox':
-            self.browser = self.playwright.firefox.launch(headless=headless)
-        elif browserName == 'webkit':
-            self.browser = self.playwright.webkit.launch(headless=headless)
+    def __init__(self, udid: str = None):
+        if udid is None:
+            self.device_id = Utils.get_first_device()
         else:
-            self.browser = self.playwright.chromium.launch(headless=headless)
-        if state:
-            self.context = self.browser.new_context(storage_state=state,
-                                                    no_viewport=True)
+            self.device_id = udid
+        logger.info(f"初始化ios驱动: {self.device_id}")
+
+        self.port = int(self.device_id.split("-")[0][-4:])
+        self.d = wda.USBClient(self.device_id,
+                               port=self.port)
+        self.util = Utils(self.device_id)
+
+        if self.d.is_ready():
+            logger.info('wda已就绪')
         else:
-            self.context = self.browser.new_context(no_viewport=True)
-        self.page = self.context.new_page()
+            logger.info('wda未就绪, 现在启动')
+            self.util.start_wda()
 
-    def switch_tab(self, locator):
-        logger.info("开始切换tab")
-        with self.page.expect_popup() as popup_info:
-            locator.click()
-        self.page = popup_info.value
-
-    def open(self, url):
-        logger.info(f"访问页面: {url}")
-        self.page.goto(url)
-
-    def storage_state(self, path=None):
-        logger.info("保存浏览器状态信息")
-        if not path:
-            raise ValueError("路径不能为空")
-        self.context.storage_state(path=path)
-
-    @property
-    def page_content(self):
-        """获取页面内容"""
-        logger.info("获取页面内容")
-        content = self.page.content()
-        logger.info(content)
-        return content
-
-    def set_cookies(self, cookies: list):
-        logger.info("添加cookie并刷新页面")
-        self.context.add_cookies(cookies)
-        self.page.reload()
+    def back(self):
+        logger.info("返回上一页")
+        time.sleep(1)
+        self.d.swipe(0, 100, 100, 100)
+
+    def enter(self):
+        logger.info("点击回车")
+        self.d.send_keys("\n")
+
+    def clear(self):
+        logger.info("清空输入框")
+        self.d.send_keys("")
+
+    def input(self, text: str):
+        logger.info(f"输入文本: {text}")
+        self.d.send_keys(text)
+
+    def click(self, x, y):
+        logger.info(f"点击坐标: {x}, {y}")
+        self.d.click(x, y)
+
+    def swipe(self, x1, y1, x2, y2):
+        """
+        从x1，y1滑动到x2，y2
+
+        @param x1:
+        @param y1:
+        @param x2:
+        @param y2:
+        @return:
+        """
+        logger.info(f"滑动")
+        self.d.swipe(x1, y1, x2, y2)
 
     def screenshot(self, file_name=None):
-        return screenshot_util(self.page,
-                               file_name=file_name)
-
-    def close(self):
-        logger.info("关闭浏览器")
-        self.page.close()
-        self.context.close()
-        self.browser.close()
-        self.playwright.stop()
-
-    def assert_title(self, title: str, timeout: int = 5):
-        logger.info(f"断言页面标题等于: {title}")
-        expect(self.page).to_have_title(title,
-                                        timeout=timeout * 1000)
-
-    def assert_url(self, url: str, timeout: int = 5):
-        logger.info(f"断言页面url等于: {url}")
-        expect(self.page).to_have_url(url,
-                                      timeout=timeout * 1000)
+        file_path = general_file_path(file_name)
+        logger.info(f"截图保存至: {file_path}")
+        self.d.screenshot(file_path)
+
+        logger.info("截图上传allure报告")
+        allure.attach.file(
+            file_path,
+            attachment_type=allure.attachment_type.PNG,
+            name=f"{file_path}",
+        )
+        return file_path
 
 
 if __name__ == '__main__':
     pass
 
 
+
+
+
+
+
+
+
+
+
```

### Comparing `kytest-0.0.9/kytest/page.py` & `kytest-0.1.2/kytest/core/web/page.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 """
 @Author: kang.yang
 @Date: 2023/9/20 11:21
 """
+import time
+
 from urllib import parse
-from kytest.utils.config import config
-from kytest.utils.exceptions import KError
+
+from kytest.utils.config import kconfig
+from kytest.utils.log import logger
 
 
 class Page(object):
     """页面基类，用于pom模式封装"""
 
     def __init__(self, driver):
         self.driver = driver
 
     def open(self, url: str = None):
         if getattr(self, 'url', None) is None:
             if url is None:
-                raise KError('url不能为空')
+                raise Exception('url不能为空')
         else:
             url = getattr(self, 'url')
 
         if not url.startswith('http'):
-            host = config.get_common('base_url')
+            host = kconfig['base_url']
             if host is not None:
                 url = parse.urljoin(host, url)
             else:
-                raise KError('host不能为空')
+                raise Exception('host不能为空')
 
         self.driver.open(url)
 
+    @staticmethod
+    def sleep(n):
+        logger.info(f"等待: {n}s")
+        time.sleep(n)
+
+
+
```

### Comparing `kytest-0.0.9/kytest/utils/allure_util.py` & `kytest-0.1.2/kytest/utils/allure_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os.path
 import time
 
 from urllib.parse import urlparse
-from allure import feature, story, \
-    title, step
+from allure import feature as project, story as module, title, step
+# 这里的project和runner中的project不能同时使用，不然报告中会出现重复用例
 
 
 class AllureData:
     """解析allure_results的数据"""
 
     def __init__(self, result_path='report'):
         self.result_path = result_path
@@ -32,123 +32,142 @@
         """获取文件内容并转成json"""
         with open(file_path, 'r', encoding='UTF-8') as f:
             content = json.load(f)
         return content
 
     def parser_content(self, content):
         """解析执行结果"""
-        name = content.get('name')
-        status = content.get('status')
-        full_name = content.get('fullName')
-        description = content.get('description')
-        parameters = content.get('parameters', None)
-        try:
-            log_name_list = [os.path.join(self.result_path, item.get('source'))
-                             for item in content.get('attachments')
-                             if item.get('name') == 'log']
-        except Exception as e:
-            print(e)
-            log_name_list = []
-        if log_name_list:
-            log_name = log_name_list[0]
-            log_data = open(log_name, 'r', encoding='utf8').read()
-        else:
-            log_data = None
+        project = '未知项目'
+        module = '未知模块'
+        labels = content["labels"]
+        for label in labels:
+            if label['name'] == 'feature':
+                project = label['value']
+            if label['name'] == 'story':
+                module = label['value']
+
+        name = content['name']
+        full_name = content['fullName']
+        parameters = content.get('parameters', [])
+
+        status = content['status']
+        log_path = ''
+        screen_path = []
+        attachments = content['attachments']
+        for attach in attachments:
+            if attach['type'] == 'text/plain' and attach['name'] == 'log':
+                log_path = os.path.join(self.result_path, attach['source'])
+            if attach['type'] == 'image/png':
+                screen_path.append(os.path.join(self.result_path, attach['source']))
+
+        interfaces = []
+        if log_path:
+            log_content = open(log_path, 'r', encoding='utf8').read()
+            for line in log_content.split("\n"):
+                if 'url]: ' in line:
+                    interface = line.strip().split('url]: ')[1]
+                    parsed_url = urlparse(interface)
+                    path = parsed_url.path
+                    method = line.strip().split('[method]: ')[1].split()[0].lower()
+                    interfaces.append((method, path))
+
         start = content.get('start')
         end = content.get('stop')
+        start_time, end_time = time.strftime("%Y-%m-%d %H:%M:%S",
+                                             time.localtime(start / 1000)), \
+                               time.strftime("%Y-%m-%d %H:%M:%S",
+                                             time.localtime(end / 1000))
         cost = (end - start) / 1000
         if cost > 60:
             cost = '{}min'.format(round(cost / 60, 1))
         else:
             cost = '{}s'.format(round((end - start) / 1000, 1))
+
         case_data = {
-            "title": name,
-            "name": full_name,
-            "description": description,
-            "log": log_data,
+            "project": project,
+            "module": module,
+            "name": name,
+            "full_name": full_name,
+            "parameters": parameters,
             "status": status,
-            "start_time": start,
-            "end_time": end,
-            "cost": cost,
-            "parameters": parameters
+            "log": log_path,
+            "interfaces": interfaces,
+            "screenshots": screen_path,
+            'start_stamp': start,
+            'start_time': start_time,
+            'end_time': end_time,
+            'end_stamp': end,
+            'cost': cost
         }
         return case_data
 
     @staticmethod
     def remove_duplicate(json_contents):
         """去除失败重试的重复结果"""
         case_list = []
         no_repeat_tags = []
         for item in json_contents:
-            full_name = item["name"]
+            full_name = item["full_name"]
             parameters = item["parameters"]
             if (full_name, parameters) not in no_repeat_tags:
                 no_repeat_tags.append((full_name, parameters))
                 case_list.append(item)
             else:
                 for case in case_list:
-                    if case.get('name') == full_name and \
-                            case.get('parameters') == parameters:
-                        if case.get('status') != 'passed':
+                    if case['full_name'] == full_name and case['parameters'] == parameters:
+                        if case['status'] != 'passed':
                             case_list.remove(case)
                             case_list.append(item)
         return case_list
 
-    def get_results(self):
+    def get_result_list(self):
         """获取对外的测试结果列表"""
         file_list = self.get_files()
         result_list = []
         for file in file_list:
             content = self.get_file_content(file)
             parser_content = self.parser_content(content)
             result_list.append(parser_content)
         return self.remove_duplicate(result_list)
 
-    def get_interfaces(self):
-        interface_list = []
-        try:
-            case_list = self.get_results()
-            for case in case_list:
-                log = case.get('log')
-                for line in log.split("\n"):
-                    if 'url]: ' in line:
-                        interface = line.strip().split('url]: ')[1]
-                        parsed_url = urlparse(interface)
-                        path = parsed_url.path
-                        method = line.strip().split('[method]: ')[1].split()[0].lower()
-                        interface_list.append((method, path))
-
-            interface_list = list(set(interface_list))
-        except Exception as e:
-            print(e)
-        return interface_list
-
     def get_statistical_data(self):
-        case_list = self.get_results()
+        case_list = self.get_result_list()
 
         # 获取用例统计数据
         passed_list = []
         fail_list = []
+        broken_list = []
+        skipped_list = []
+        unknown_list = []
         for case in case_list:
             status = case.get('status')
             if status == 'passed':
                 passed_list.append(case)
-            else:
+            elif status == 'failed':
                 fail_list.append(case)
+            elif status == 'broken':
+                broken_list.append(case)
+            elif status == 'skipped':
+                skipped_list.append(case)
+            else:
+                unknown_list.append(case)
         total = len(case_list)
         passed = len(passed_list)
         failed = len(fail_list)
+        broken = len(broken_list)
+        skipped = len(skipped_list)
+        unknown = len(unknown_list)
         rate = round((passed / total) * 100, 2)
 
         # 获取整个任务的开始和结束时间
         start_time_timestamp, end_time_timestamp = \
-            case_list[0].get('start_time'), case_list[0].get('end_time')
+            case_list[0].get('start_stamp'), case_list[0].get('end_stamp')
         for case in case_list:
-            inner_start = case.get('start_time')
-            inner_end = case.get('end_time')
+            inner_start = case.get('start_stamp')
+            inner_end = case.get('end_stamp')
             if inner_start < start_time_timestamp:
                 start_time_timestamp = inner_start
             if inner_end > end_time_timestamp:
                 end_time_timestamp = inner_end
 
         # 时间戳转成日期
         start_time, end_time = time.strftime("%Y-%m-%d %H:%M:%S",
@@ -161,35 +180,25 @@
         else:
             cost = '{}s'.format(round((end_time_timestamp - start_time_timestamp) / 1000, 1))
 
         return {
             'total': total,
             'passed': passed,
             'failed': failed,
+            'broken': broken,
+            'skipped': skipped,
+            'unknown': unknown,
             'rate': rate,
             'start': start_time,
             'end': end_time,
-            'cost': cost
-        }
-
-    @property
-    def report_data(self):
-        return {
-            "summary": self.get_statistical_data(),
-            "interfaces": self.get_interfaces(),
-            "tests": [
-                {
-                    "id": i+1,
-                    "title": case.get("title"),
-                    "name": case.get("name"),
-                    "status": case.get("status"),
-                    "cost": case.get("cost"),
-                    "log": case.get("log")
-                } for i, case in enumerate(self.get_results())
-            ]
+            'cost': cost,
+            'tests': case_list
         }
 
 
 def get_allure_data(result_path):
     """兼容邮件和钉钉的调用"""
     return AllureData(result_path).get_statistical_data()
 
+
+if __name__ == '__main__':
+    print(AllureData('../../demo/tests/report').get_statistical_data())
```

### Comparing `kytest-0.0.9/kytest/utils/dingtalk.py` & `kytest-0.1.2/kytest/utils/dingtalk.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             print('消息发送失败: {}'.format(ret_dict.get('errmsg')))
 
     # 从allure报告中获取数据并发送消息
     def send_report(self, msg_title, report_url):
         allure_data = get_allure_data('report')
         total = allure_data.get('total')
         passed = allure_data.get('passed')
-        fail = allure_data.get('failed')
+        fail = total - passed
         rate = allure_data.get('rate')
 
         color_red = 'FF0000'
         color_green = '00FF00'
         if rate < 100:
             color_str = color_red
         else:
```

### Comparing `kytest-0.0.9/kytest/utils/mysql_util.py` & `kytest-0.1.2/kytest/utils/mysql_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# @Time    : 2022/2/11 16:52
-# @Author  : kang.yang@qizhidao.com
-# @File    : mysql_util.py
-# pip install PyMySQL==0.10.1
+"""
+pip install pymysql==1.1.0
+@Author: kang.yang
+@Date: 2024/3/18 14:43
+"""
 import pymysql
 
 
 class MysqlDB(object):
     def __init__(self, host, username, password, database):
         self.host = host
         self.username = username
@@ -69,15 +70,7 @@
             return items
         finally:
             self.close()
 
     def close(self):
         self.cursor.close()
         self.con.close()
-
-
-
-
-
-
-
-
```

### Comparing `kytest-0.0.9/kytest/utils/pytest_util.py` & `kytest-0.1.2/kytest/utils/pytest_util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
-import json
-import yaml
+# import json
+# import yaml
 
 
 def order(index):
     """
     指定用例执行顺序, pip install pytest-ordering==0.6
     doc: https://blog.csdn.net/weixin_43880991/article/details/116221362
     """
@@ -18,72 +18,72 @@
     """
     if isinstance(depends, str):
         depends = [depends]
     return pytest.mark.dependency(name=name, depends=depends)
 
 
 # 参数化数据
-def data(list_data: list):
+def data(out_name, list_data: list):
     """
     必须传入一个list，使用时通过在参数列表传入parma进行调用
     """
-    return pytest.mark.parametrize('param', list_data)
+    return pytest.mark.parametrize(out_name, list_data)
 
 
-# 从json文件获取数据进行参数化
-def file_data(file=None, key=None):
-    # logger.debug(config.get_env())
-
-    """
-    感觉excel和csv不常用，去掉
-    @param file: 文件名
-    @param key: 针对json和yaml文件
-    """
-    file_path = file  # 去掉文件查找机制，不好理解，用处也不大
-
-    # logger.debug(file_path)
-    if file_path.endswith(".json"):
-        content = read_json(file_path, key)
-    elif file_path.endswith(".yml"):
-        content = read_yaml(file_path, key)
-    # elif file_path.endswith(".csv"):
-    #     content = read_csv(file_path, row)
-    # elif file_path.endswith(".xlsx"):
-    #     content = read_excel(file_path, row)
-    else:
-        raise TypeError("不支持的文件类型，仅支持json、yml")
-
-    if content:
-        return data(content)
-    else:
-        raise ValueError('数据不能为空')
-
-
-def read_json(file_path, key=None):
-    """
-    读取json文件中的指定key
-    @return
-    """
-    with open(file_path, 'r', encoding='utf-8') as f:
-        json_data = json.load(f)
-    if isinstance(json_data, list):
-        return json_data
-    else:
-        if key:
-            return json_data[key]
-        raise ValueError('key不能为空')
-
-
-def read_yaml(file_path, key=None):
-    """
-    读取yaml文件中的指定key
-    @param file_path:
-    @param key:
-    """
-    with open(file_path, 'r', encoding='utf-8') as f:
-        yaml_data = yaml.load(f, Loader=yaml.FullLoader)
-    if isinstance(yaml_data, list):
-        return yaml_data
-    else:
-        if key:
-            return yaml_data[key]
-        raise ValueError('key不能为空')
+# # 从json文件获取数据进行参数化
+# def file_data(file=None, key=None):
+#     # logger.debug(config.get_env())
+#
+#     """
+#     感觉excel和csv不常用，去掉
+#     @param file: 文件名
+#     @param key: 针对json和yaml文件
+#     """
+#     file_path = file  # 去掉文件查找机制，不好理解，用处也不大
+#
+#     # logger.debug(file_path)
+#     if file_path.endswith(".json"):
+#         content = read_json(file_path, key)
+#     elif file_path.endswith(".yml"):
+#         content = read_yaml(file_path, key)
+#     # elif file_path.endswith(".csv"):
+#     #     content = read_csv(file_path, row)
+#     # elif file_path.endswith(".xlsx"):
+#     #     content = read_excel(file_path, row)
+#     else:
+#         raise TypeError("不支持的文件类型，仅支持json、yml")
+#
+#     if content:
+#         return data(content)
+#     else:
+#         raise ValueError('数据不能为空')
+
+
+# def read_json(file_path, key=None):
+#     """
+#     读取json文件中的指定key
+#     @return
+#     """
+#     with open(file_path, 'r', encoding='utf-8') as f:
+#         json_data = json.load(f)
+#     if isinstance(json_data, list):
+#         return json_data
+#     else:
+#         if key:
+#             return json_data[key]
+#         raise ValueError('key不能为空')
+#
+#
+# def read_yaml(file_path, key=None):
+#     """
+#     读取yaml文件中的指定key
+#     @param file_path:
+#     @param key:
+#     """
+#     with open(file_path, 'r', encoding='utf-8') as f:
+#         yaml_data = yaml.load(f, Loader=yaml.FullLoader)
+#     if isinstance(yaml_data, list):
+#         return yaml_data
+#     else:
+#         if key:
+#             return yaml_data[key]
+#         raise ValueError('key不能为空')
```

### Comparing `kytest-0.0.9/kytest.egg-info/SOURCES.txt` & `kytest-0.1.2/kytest.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 README.md
 setup.py
 demo/__init__.py
-demo/run.py
+demo/run_adr.py
+demo/run_api.py
+demo/run_web.py
 demo/pages/__init__.py
 demo/pages/adr_page.py
-demo/pages/image_page.py
-demo/pages/ios_page.py
 demo/pages/web_page.py
 demo/tests/__init__.py
 demo/tests/test_adr.py
 demo/tests/test_api.py
-demo/tests/test_image.py
-demo/tests/test_ios.py
 demo/tests/test_web.py
 kytest/__init__.py
-kytest/case.py
 kytest/cli.py
-kytest/page.py
-kytest/scaffold.py
 kytest.egg-info/PKG-INFO
 kytest.egg-info/SOURCES.txt
 kytest.egg-info/dependency_links.txt
 kytest.egg-info/entry_points.txt
 kytest.egg-info/requires.txt
 kytest.egg-info/top_level.txt
 kytest/core/__init__.py
-kytest/core/android/__init__.py
-kytest/core/android/driver.py
-kytest/core/android/element.py
+kytest/core/adr/__init__.py
+kytest/core/adr/case.py
+kytest/core/adr/driver.py
+kytest/core/adr/element.py
+kytest/core/adr/page.py
+kytest/core/adr/utils.py
 kytest/core/api/__init__.py
+kytest/core/api/case.py
 kytest/core/api/request.py
-kytest/core/image/__init__.py
-kytest/core/image/driver.py
-kytest/core/image/element.py
+kytest/core/img/__init__.py
+kytest/core/img/driver.py
+kytest/core/img/element.py
 kytest/core/ios/__init__.py
+kytest/core/ios/case.py
 kytest/core/ios/driver.py
-kytest/core/ios/element.py
+kytest/core/ios/elem.py
+kytest/core/ios/page.py
+kytest/core/ios/utils.py
 kytest/core/ocr/__init__.py
 kytest/core/ocr/driver.py
 kytest/core/ocr/element.py
 kytest/core/web/__init__.py
+kytest/core/web/case.py
 kytest/core/web/driver.py
 kytest/core/web/element.py
+kytest/core/web/page.py
 kytest/running/__init__.py
+kytest/running/conf.py
 kytest/running/conf.yml
+kytest/running/execution_scheduler.py
 kytest/running/runner.py
-kytest/testdata/__init__.py
-kytest/testdata/data.py
 kytest/utils/__init__.py
+kytest/utils/aes_util.py
 kytest/utils/allure_util.py
 kytest/utils/common.py
 kytest/utils/config.py
-kytest/utils/des_util.py
+kytest/utils/cv_util.py
 kytest/utils/dingtalk.py
-kytest/utils/excel.py
-kytest/utils/exceptions.py
+kytest/utils/excel_util.py
 kytest/utils/log.py
 kytest/utils/mail.py
 kytest/utils/mysql_util.py
-kytest/utils/pytest_util.py
-kytest/utils/swagger_util.py
+kytest/utils/nacos_util.py
+kytest/utils/pytest_util.py
```

### Comparing `kytest-0.0.9/setup.py` & `kytest-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,30 +23,31 @@
         "Programming Language :: Python :: 3.9"
     ],
     include_package_data=True,
     package_data={
         r'': ['*.yml'],
     },
     install_requires=[
-        'requests-toolbelt==0.10.1',
-        'jmespath==0.9.5',
-        'jsonschema==4.17.0',
         'pytest==6.2.5',
         'pytest-rerunfailures==10.2',
         'pytest-xdist==2.5.0',
         'allure-pytest==2.9.45',
+        'requests==2.31.0',
+        'urllib3==1.26.15',
+        'requests-toolbelt==0.10.1',
+        'jmespath==0.9.5',
+        'jsonschema==4.17.0',
         'click~=8.1.3',
         'loguru==0.7.0',
-        'urllib3==1.26.15',
-        'PyYAML~=6.0',
-        'uiautomator2==2.16.23',
-        'opencv-python==4.6.0.66',
-        'tidevice==0.6.1',
-        'facebook-wda==1.4.6',
-        'playwright==1.33.0'
+        'PyYAML~=6.0'
     ],
+    extras_require={
+        "web": ['playwright==1.33.0'],
+        "adr": ['uiautomator2==2.16.23'],
+        "ios": ['tidevice==0.12.9', 'facebook-wda==1.4.6']
+    },
     entry_points={
         'console_scripts': [
             'kytest = kytest.cli:main'
         ]
     }
 )
```

