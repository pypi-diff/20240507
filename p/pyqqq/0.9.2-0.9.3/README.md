# Comparing `tmp/pyqqq-0.9.2.tar.gz` & `tmp/pyqqq-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.9.2.tar", max compression
+gzip compressed data, was "pyqqq-0.9.3.tar", max compression
```

## Comparing `pyqqq-0.9.2.tar` & `pyqqq-0.9.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.9.2/README.md
--rw-r--r--   0        0        0      791 2024-05-03 09:30:39.993641 pyqqq-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     1606 2024-04-30 07:51:35.706752 pyqqq-0.9.2/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.9.2/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.9.2/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    41866 2024-04-26 06:58:08.897413 pyqqq-0.9.2/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.9.2/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24448 2024-04-25 01:42:27.858549 pyqqq-0.9.2/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.9.2/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.9.2/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.9.2/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5356 2024-04-23 09:05:13.260008 pyqqq-0.9.2/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.9.2/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24390 2024-04-22 04:52:35.372119 pyqqq-0.9.2/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.9.2/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.9.2/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.9.2/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     9684 2024-05-03 09:30:10.903300 pyqqq-0.9.2/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     9628 2024-05-03 08:51:32.698077 pyqqq-0.9.2/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1521 2024-05-03 08:51:15.982807 pyqqq-0.9.2/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4136 2024-05-03 08:53:53.080239 pyqqq-0.9.2/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.9.2/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.9.2/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.9.2/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.9.2/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      519 2024-05-03 08:48:33.699191 pyqqq-0.9.2/pyqqq/utils/api_client.py
--rw-r--r--   0        0        0      941 2024-04-30 08:35:54.600146 pyqqq-0.9.2/pyqqq/utils/array.py
--rw-r--r--   0        0        0     3229 2024-04-30 08:36:37.055899 pyqqq-0.9.2/pyqqq/utils/compute.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.9.2/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3962 2024-04-23 09:09:34.322415 pyqqq-0.9.2/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     2641 2024-04-30 08:36:57.232261 pyqqq-0.9.2/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     2233 2024-04-30 07:41:29.806969 pyqqq-0.9.2/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.9.2/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.9.2/pyqqq/utils/mock_api.py
--rw-r--r--   0        0        0     2065 2024-04-30 07:36:13.157361 pyqqq-0.9.2/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 pyqqq-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.9.3/README.md
+-rw-r--r--   0        0        0      791 2024-05-07 09:20:54.015932 pyqqq-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1606 2024-04-30 07:51:35.706752 pyqqq-0.9.3/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.9.3/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.9.3/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    43409 2024-05-07 06:54:47.220204 pyqqq-0.9.3/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.9.3/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24448 2024-04-25 01:42:27.858549 pyqqq-0.9.3/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.9.3/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.9.3/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187522 2024-05-07 09:02:33.261786 pyqqq-0.9.3/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5356 2024-04-23 09:05:13.260008 pyqqq-0.9.3/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.9.3/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24390 2024-04-22 04:52:35.372119 pyqqq-0.9.3/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.9.3/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.9.3/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.9.3/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     9684 2024-05-03 09:30:10.903300 pyqqq-0.9.3/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     9628 2024-05-03 08:51:32.698077 pyqqq-0.9.3/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1521 2024-05-03 08:51:15.982807 pyqqq-0.9.3/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4136 2024-05-03 08:53:53.080239 pyqqq-0.9.3/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.9.3/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.9.3/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.9.3/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.9.3/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      519 2024-05-03 08:48:33.699191 pyqqq-0.9.3/pyqqq/utils/api_client.py
+-rw-r--r--   0        0        0      941 2024-04-30 08:35:54.600146 pyqqq-0.9.3/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3229 2024-04-30 08:36:37.055899 pyqqq-0.9.3/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.9.3/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3962 2024-04-23 09:09:34.322415 pyqqq-0.9.3/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     2641 2024-04-30 08:36:57.232261 pyqqq-0.9.3/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     2233 2024-04-30 07:41:29.806969 pyqqq-0.9.3/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.9.3/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.9.3/pyqqq/utils/mock_api.py
+-rw-r--r--   0        0        0     2065 2024-04-30 07:36:13.157361 pyqqq-0.9.3/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 pyqqq-0.9.3/PKG-INFO
```

### Comparing `pyqqq-0.9.2/README.md` & `pyqqq-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyproject.toml` & `pyqqq-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.9.2"
+version = "0.9.3"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.9.2/pyqqq/__init__.py` & `pyqqq-0.9.3/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.9.3/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,31 +315,62 @@
     ):
         """
         ([주식]차트) API전용주식챠트(일주월년) (t8410)
 
         Args:
             shcode (str): 종목 코드
             gubun (str): 주기구분 (d:일 w:주 m:월 y:년)
-            qrycnt (int): 요청건수 (최대-압축:2000비압축:500)
             edate (dtm.date): 종료일자 - 처음조회기준일(LE) 처음 조회일 경우 이 값 기준으로 조회
             sdate (dtm.date): 시작일자 - 기본값(None)인 경우 edate 기준으로  qrycnt 만큼 조회. 조회구간을 설정하여 필터링하고 싶은 경우 입력.
+            qrycnt (int): 요청건수 (최대-압축:2000비압축:500)
             cts_date (str): 연속일자 - 연속조회시 OutBlock의 동일필드 입력
             comp_yn (bool): 압축여부 (True:압축 False:비압축)
             sujung_yn (bool): 수정주가적용여부 (True:수정주가적용 False:비적용)
             tr_cont_key (str): 연속조회키 - 연속조회시 이전 응답 헤더의 동일필드 입력
 
         Returns:
             dict: 주식 차트 정보
 
             - rsp_cd (str): 응답코드
             - rsp_msg (str): 응답메시지
             - tr_cont (str): 연속조회여부
             - tr_cont_key (str): 연속조회키
             - output1 (dict): 전일/당일 시세 정보
+                - shcode (str): 단축코드
+                - jisiga (int): 전일시가
+                - jihigh (int): 전일고가
+                - jilow (int): 전일저가
+                - jiclose (int): 전일종가
+                - jivolume (int): 전일거래량
+                - disiga (int): 당일시가
+                - dihigh (int): 당일고가
+                - dilow (int): 당일저가
+                - diclose (int): 당일종가
+                - highend (int): 상한가
+                - lowend (int): 하한가
+                - cts_date (str): 연속일자
+                - s_time (str): 장시작시간 (HHMMSS)
+                - e_time (str): 장종료시간 (HHMMSS)
+                - dshmin (int): 동시호가처리시간 (MM:분)
+                - rec_count (int): 레코드카운트
+                - svi_uplmtprice (float): 정적VI상한가
+                - svi_dnlmtprice (float): 정적VI하한가
             - output2 (list): 주기별 시세 정보
+                - date (str): 날짜
+                - open (int): 시가
+                - high (int): 고가
+                - low (int): 저가
+                - close (int): 종가
+                - jdiff_vol (int): 거래량
+                - value (int): 거래대금
+                - jongchk (str): 수정구분
+                - rate (float): 수정비율
+                - pricechk (int): 수정가반영항목
+                - ratevalue (int): 수정비율반영거래대금
+                - sign (str): 종가등락구분 (1:상한 2:상승 3:보합 4:하한 5:하락 주식일만사용)
         """
 
         CallLimiter().wait_limit_rate(1, scope="ebest/t8410")
 
         assert len(shcode) == 6, "Invalid asset code"
         assert gubun.lower() in ["d", "w", "m", "y"], "Invalid gubun"
```

### Comparing `pyqqq-0.9.2/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.9.3/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.9.3/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.9.3/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.9.3/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files 1% similar despite different names*

```diff
@@ -607,23 +607,28 @@
         output1 = res_body['output1']
 
         int_keys = [
             'prdy_vrss', 'prdy_vrss_sign', 'stck_prdy_clpr', 'acml_vol',
             'acml_tr_pbmn', 'stck_prpr', 'prdy_vol', 'stck_mxpr',
             'stck_llam', 'stck_oprc', 'stck_hgpr', 'stck_lwpr',
             'stck_prdy_oprc', 'stck_prdy_hgpr', 'stck_prdy_lwpr',
-            'askp', 'bidp', 'prdy_vrss_vol', 'stck_fcam',
+            'askp', 'bidp', 'prdy_vrss_vol',
             'lstn_stcn', 'cpfn', 'hts_avls']
         for k in int_keys:
             if k in output1 and len(output1[k]) > 0:
                 output1[k] = int(output1[k])
 
         decimal_keys = [
-            'prdy_ctrt', 'vol_tnrt', 'per', 'eps', 'pbr',
-            'itewhol_loan_rmnd_ratem name'
+            "prdy_ctrt",
+            "vol_tnrt",
+            "per",
+            "eps",
+            "pbr",
+            "itewhol_loan_rmnd_ratem name",
+            "stck_fcam",
         ]
         for k in decimal_keys:
             if k in output1 and len(output1[k]) > 0:
                 output1[k] = Decimal(output1[k])
 
         output2 = []
         for el in res_body['output2']:
```

### Comparing `pyqqq-0.9.2/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.9.3/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.9.3/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.9.3/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.9.3/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/data/domestic.py` & `pyqqq-0.9.3/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/data/minutes.py` & `pyqqq-0.9.3/pyqqq/data/minutes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/data/realtime.py` & `pyqqq-0.9.3/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/data/ticks.py` & `pyqqq-0.9.3/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/datatypes.py` & `pyqqq-0.9.3/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/executors/hook.py` & `pyqqq-0.9.3/pyqqq/executors/hook.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/utils/api_client.py` & `pyqqq-0.9.3/pyqqq/utils/api_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/utils/array.py` & `pyqqq-0.9.3/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/utils/compute.py` & `pyqqq-0.9.3/pyqqq/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/utils/display.py` & `pyqqq-0.9.3/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/utils/kvstore.py` & `pyqqq-0.9.3/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/utils/limiter.py` & `pyqqq-0.9.3/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/utils/logger.py` & `pyqqq-0.9.3/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/utils/market_schedule.py` & `pyqqq-0.9.3/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/utils/mock_api.py` & `pyqqq-0.9.3/pyqqq/utils/mock_api.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/pyqqq/utils/retry.py` & `pyqqq-0.9.3/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.2/PKG-INFO` & `pyqqq-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.9.2
+Version: 0.9.3
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

