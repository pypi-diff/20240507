# Comparing `tmp/aanalyticsact_1-0.0.1.51.tar.gz` & `tmp/aanalyticsact_1-0.0.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aanalyticsact_1-0.0.1.51.tar", last modified: Thu May  2 08:43:33 2024, max compression
+gzip compressed data, was "aanalyticsact_1-0.0.1.52.tar", last modified: Tue May  7 05:33:25 2024, max compression
```

## Comparing `aanalyticsact_1-0.0.1.51.tar` & `aanalyticsact_1-0.0.1.52.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 08:43:33.956910 aanalyticsact_1-0.0.1.51/
--rw-rw-rw-   0        0        0      191 2024-05-02 08:43:33.955913 aanalyticsact_1-0.0.1.51/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 08:43:33.951026 aanalyticsact_1-0.0.1.51/aanalyticsact_1/
--rw-rw-rw-   0        0        0      151 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1/__init__.py
--rw-rw-rw-   0        0        0       24 2024-04-24 05:06:20.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1/__version__.py
--rw-rw-rw-   0        0        0     7109 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1/actExecute.py
--rw-rw-rw-   0        0        0    18036 2024-04-24 05:03:50.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1/actModuler.py
--rw-rw-rw-   0        0        0     9139 2024-04-18 06:51:22.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1/actRunner.py
-drwxrwxrwx   0        0        0        0 2024-05-02 08:43:33.954916 aanalyticsact_1-0.0.1.51/aanalyticsact_1.egg-info/
--rw-rw-rw-   0        0        0      191 2024-05-02 08:43:33.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-05-02 08:43:33.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 08:43:33.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-02 08:43:33.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 08:43:33.956910 aanalyticsact_1-0.0.1.51/setup.cfg
--rw-rw-rw-   0        0        0      732 2024-05-02 08:42:51.000000 aanalyticsact_1-0.0.1.51/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:33:25.120731 aanalyticsact_1-0.0.1.52/
+-rw-rw-rw-   0        0        0      191 2024-05-07 05:33:25.120731 aanalyticsact_1-0.0.1.52/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 05:33:25.115813 aanalyticsact_1-0.0.1.52/aanalyticsact_1/
+-rw-rw-rw-   0        0        0      151 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.52/aanalyticsact_1/__init__.py
+-rw-rw-rw-   0        0        0       24 2024-05-07 05:32:56.000000 aanalyticsact_1-0.0.1.52/aanalyticsact_1/__version__.py
+-rw-rw-rw-   0        0        0     7261 2024-05-07 04:48:27.000000 aanalyticsact_1-0.0.1.52/aanalyticsact_1/actExecute.py
+-rw-rw-rw-   0        0        0    20198 2024-05-07 04:55:56.000000 aanalyticsact_1-0.0.1.52/aanalyticsact_1/actModuler.py
+-rw-rw-rw-   0        0        0     9218 2024-05-07 04:14:10.000000 aanalyticsact_1-0.0.1.52/aanalyticsact_1/actRunner.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:33:25.119687 aanalyticsact_1-0.0.1.52/aanalyticsact_1.egg-info/
+-rw-rw-rw-   0        0        0      191 2024-05-07 05:33:24.000000 aanalyticsact_1-0.0.1.52/aanalyticsact_1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-05-07 05:33:25.000000 aanalyticsact_1-0.0.1.52/aanalyticsact_1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 05:33:24.000000 aanalyticsact_1-0.0.1.52/aanalyticsact_1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-07 05:33:24.000000 aanalyticsact_1-0.0.1.52/aanalyticsact_1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 05:33:25.121749 aanalyticsact_1-0.0.1.52/setup.cfg
+-rw-rw-rw-   0        0        0      732 2024-05-07 05:33:20.000000 aanalyticsact_1-0.0.1.52/setup.py
```

### Comparing `aanalyticsact_1-0.0.1.51/aanalyticsact_1/actExecute.py` & `aanalyticsact_1-0.0.1.52/aanalyticsact_1/actExecute.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # Created by Sunkyeong Lee
 # Inquiry : sunkyeong.lee@concentrix.com / sunkyong9768@gmail.com
+# Updated by Youngkwang Cho 
+# Inquiry : youngkwang.Cho@concentrix.com 
+# limit function and para order
 
 from copy import Error
 # from actModuler import *
 # from actRunner import *
 from .actModuler import *
 from .actRunner import *
 import time
 
 
-def retrieve_FirstLevel(start_date, end_date, period, jsonLocation, tbColumn, dbTableName, epp, site_code_rs, limit, extra = "", start_hour="00:00", end_hour="00:00", site_code = ""):
-    if limit > 1000:
-        raise Error("limit은 0 ~ 1000 사이 값으로 넣어주세요")
+def retrieve_FirstLevel(start_date, end_date, period, jsonLocation, tbColumn, dbTableName, epp, site_code_rs, limit=0, extra = "", start_hour="00:00", end_hour="00:00", site_code = ""):
+    if limit > 10000:
+        raise Error("limit은 0 ~ 10000 사이 값으로 넣어주세요")
 
     dateCaller = dateGenerator(start_date, end_date, period)
     if_site_code = checkSiteCode(readJson(jsonLocation)["dimension"])
     
     tbColumn = tbColumnGenerator(tbColumn, if_site_code, False, False, site_code_rs)
     
     startDate = dateCaller[0]
@@ -47,15 +50,15 @@
 
             except ConnectionResetError:
                 print("Connection Error occurred, please wait for the next response")
                 continue 
             
             break
 
-def retrieve_SecondLevel(start_date, end_date, period, jsonLocation, jsonLocation_breakdown,tbColumn, dbTableName, epp, limit, extra = "", start_hour="00:00", end_hour="00:00", site_code=""):
+def retrieve_SecondLevel(start_date, end_date, period, jsonLocation, jsonLocation_breakdown,tbColumn, dbTableName, epp, limit=0, extra = "", start_hour="00:00", end_hour="00:00", site_code=""):
     dateCaller = dateGenerator(start_date, end_date, period)
     if_site_code = checkSiteCode(readJson(jsonLocation)["dimension"])
 
     if returnRsID(jsonLocation) == "sssamsungnewus":
         if_site_code = True
 
     site_code_rs = False
@@ -90,29 +93,29 @@
 
             except ConnectionResetError:
                 print("Connection Error occurred, please wait for the next response")
                 continue
 
             break
 
-def retrieve_by_RS(start_date, end_date, period, jsonLocation, rsInput, tbColumn, dbTableName, epp, extra = "", start_hour="00:00", end_hour="00:00"):
+def retrieve_by_RS(start_date, end_date, period, jsonLocation, rsInput, tbColumn, dbTableName, epp, limit=0, extra = "", start_hour="00:00", end_hour="00:00"):
     dateCaller = dateGenerator(start_date, end_date, period)
     site_code_rs = False
     tbColumn = tbColumnGenerator(tbColumn, False, False, True, site_code_rs)
     
     startDate = dateCaller[0]
     endDate = dateCaller[1]
 
     rsList = returnRsList(epp, rsInput)
 
     for i in range(len(startDate)):
         for j in range(len(rsList)):
             try:
                 start = time.time()
-                sample = refineRsIDChange(startDate[i], endDate[i], jsonLocation, rsList[j], period, tbColumn, epp, extra, start_hour, end_hour)
+                sample = refineRsIDChange(startDate[i], endDate[i], jsonLocation, rsList[j], period, tbColumn, epp, limit, extra, start_hour, end_hour)
 
             except KeyError:
                 print("Server Error occurred, please wait for the next response")
                 continue
 
             except IndexError:
                 print("Index Error occurred, please wait for the next response")
@@ -130,15 +133,15 @@
                 print("Connection Error occurred, please wait for the next response")
                 continue
 
             stackTodb(sample, dbTableName)
             timeSec = round(time.time() - start, 2)
             print("Time took: ", timeSec, "sec")
 
-def retrieve_by_RS_breakdown(startDate, endDate, period, jsonFile, jsonFilebreakdown, rsInput, tbColumn, dbTableName, limit, epp, extra = "", start_hour = "00:00", end_hour = "00:00"):
+def retrieve_by_RS_breakdown(startDate, endDate, period, jsonFile, jsonFilebreakdown, rsInput, tbColumn, dbTableName, epp, limit1=0, limit2=0, extra = "", start_hour = "00:00", end_hour = "00:00"):
     dateCaller = dateGenerator(startDate, endDate, period)
     defaultColumn = ["site_code", "dimension", "breakdown", "period", "start_date", "end_date", "is_epp"]
     
     if extra != "":
         defaultColumn.append("extra")
 
     newColumn = defaultColumn + tbColumn
@@ -148,15 +151,15 @@
 
     rsList = returnRsList(epp, rsInput)
 
     for i in range(len(startDate)):
         for j in range(len(rsList)):
             try:
                 start = time.time()
-                secondCaller(startDate[i], endDate[i], jsonFile, jsonFilebreakdown, rsList[j], limit, period, newColumn, dbTableName, epp, extra, start_hour, end_hour)
+                secondCaller(startDate[i], endDate[i], jsonFile, jsonFilebreakdown, rsList[j],  period, newColumn, dbTableName, epp, limit1, limit2, extra, start_hour, end_hour)
                 timeSec = round(time.time() - start, 2)
                 print("Time took: ", timeSec, "sec")
                 
             except KeyError:
                 print("Server Error occurred, please wait for the next response")
                 continue
```

### Comparing `aanalyticsact_1-0.0.1.51/aanalyticsact_1/actModuler.py` & `aanalyticsact_1-0.0.1.52/aanalyticsact_1/actModuler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Created by Sunkyeong Lee
 # Inquiry : sunkyeong.lee@concentrix.com / sunkyong9768@gmail.com
 # Updated by Youngkwang Cho 
 # Inquiry : youngkwang.Cho@concentrix.com 
-# encoding, create_engine()
+# encoding, create_engine(),apply & map, limit function 
 
 
 import aanalytics2 as api2
 import aanalyticsactauth as auth
 import json
 from datetime import datetime, timedelta
 from copy import deepcopy
@@ -197,22 +197,23 @@
  
     stackTodb(df, dbTableName)
 
 def create_connection_pool():   ###YK
     db_connection_str = 'mysql+pymysql://root:12345@127.0.0.1:3307/act?charset=utf8mb4'
     pool_size = 20  
     max_overflow = 10  
-    return create_engine(db_connection_str, poolclass=pool.QueuePool, pool_size=pool_size, max_overflow=max_overflow)
+    return create_engine(db_connection_str, encoding='utf-8', poolclass=pool.QueuePool, pool_size=pool_size, max_overflow=max_overflow)
 
 def stackTodb(dataFrame, dbTableName):  ###YK
     print(dataFrame)
+    # UNICODE 전처리
+    dataFrame = unicodeCompile_df(dataFrame)
     db_connection = create_connection_pool()
     with db_connection.connect() as conn:
-    	dataFrame = unicodeCompile_df(dataFrame)
-    	dataFrame.to_sql(name=dbTableName, con=conn, if_exists='append', index=False)
+        dataFrame.to_sql(name=dbTableName, con=conn, if_exists='append', index=False)
     db_connection.dispose()
     print("finished")
    
 """ MST breakdown """
 
 # breakdown itemID
 def ChangeItemID(itemID, breakdownJson):
@@ -286,15 +287,15 @@
 
     def remove_non_bmp(text):
         if isinstance(text, str):
             return only_BMP_pattern.sub(r'', text) # only BMP characters
         else:
             return text  # 문자열이 아닌 경우 그대로 반환
 
-    return df.apply(remove_non_bmp)
+    return df.apply(lambda col: col.map(remove_non_bmp))#df.apply(remove_non_bmp)
 
 # Save as dictionary format return in tuple
 def ReturnJsonchanged(startDate, endDate, jsonFile, jsonFilebreakdown, start_hour, end_hour, site_code):
     itemIDList = returnItemID(startDate, endDate, jsonFile, start_hour, end_hour, site_code)
 
     itemIDdict = {}
     for i in range(len(itemIDList)):
@@ -378,20 +379,24 @@
 
 def rsIDchange(jsonFile, rsID):
     temp_simple = deepcopy(jsonFile)
     temp_simple['rsid'] = rsID
 
     return temp_simple
 
-def refineRsIDChange(startDate, endDate, jsonFile, rsList, period, tbColumn, epp, extra, start_hour, end_hour):
+def refineRsIDChange(startDate, endDate, jsonFile, rsList, period, tbColumn, epp, limit, extra, start_hour, end_hour):
     datechanged = jsonDateChange(startDate, endDate, jsonFile, start_hour, end_hour)
     rschanged = rsIDchange(datechanged, rsList[1])
 
     dataInitiator()
-    dataFrame = dataretriever_data(rschanged)
+    dataFrame1 = dataretriever_data(rschanged)
+    if limit == 0 :
+        dataFrame=dataFrame1
+    else :
+        dataFrame=dataFrame1.head(limit)
 
     columnList = []
     for i in range(dataFrame.shape[1]):
         columnList.append(i)
 
     dataFrame.columns = columnList
 
@@ -416,15 +421,15 @@
             
     dataFrame.columns = tbColumn
     if extra != "":
         dataFrame.insert(7, "extra", extra, True)
 
     return dataFrame
 
-def secondCaller(startDate, endDate, jsonFile, jsonFilebreakdown, rsList, limit, period, tbColumn, dbTableName, epp, extra="", start_hour="00:00", end_hour="00:00"):
+def secondCaller1(startDate, endDate, jsonFile, jsonFilebreakdown, rsList, limit, period, tbColumn, dbTableName, epp, extra="", start_hour="00:00", end_hour="00:00"):
     dateChanged_json = jsonDateChange(startDate, endDate, jsonFile, start_hour, end_hour)
     dateChanged_bd_json = jsonDateChange(startDate, endDate, jsonFilebreakdown, start_hour, end_hour)
     
     rsChanged_json = rsIDchange(dateChanged_json, rsList[1])
     rsChanged_json_bd = rsIDchange(dateChanged_bd_json, rsList[1])
 
     itemIDList = returnItemID_rs(rsChanged_json)
@@ -453,8 +458,51 @@
             dataFrame2.insert(4, "start_date", "{0} {1}".format(startDate, start_hour), True)
             dataFrame2.insert(5, "end_date", "{0} {1}".format(EndDateCalculation("0", endDate)[1], end_hour), True)
         dataFrame2.insert(6, "epp", epp, True)
         
         if extra != "":
             dataFrame2.insert(7, "extra", extra, True)
         dataFrame2.columns = tbColumn
-        stackTodb(dataFrame2, dbTableName)
+        stackTodb(dataFrame2, dbTableName)
+
+def secondCaller(startDate, endDate, jsonFile, jsonFilebreakdown, rsList, period, tbColumn, dbTableName, epp, limit1, limit2, extra="", start_hour="00:00", end_hour="00:00"):
+    dateChanged_json = jsonDateChange(startDate, endDate, jsonFile, start_hour, end_hour)
+    dateChanged_bd_json = jsonDateChange(startDate, endDate, jsonFilebreakdown, start_hour, end_hour)
+    
+    rsChanged_json = rsIDchange(dateChanged_json, rsList[1])
+    rsChanged_json_bd = rsIDchange(dateChanged_bd_json, rsList[1])
+
+    itemIDList = returnItemID_rs(rsChanged_json)
+    itemIDdict = {}
+    for i in range(len(itemIDList)):
+        itemIDdict[itemIDList[i][0]] = ChangeItemID(itemIDList[i][1], rsChanged_json_bd)
+    
+    itemIDdict = list(zip(itemIDdict.keys(), itemIDdict.values()))
+
+    if limit1==0:
+        lenItemID = len(itemIDdict)
+    else :
+        lenItemID = limit1
+
+    for i in range(lenItemID):
+        dataFrame = dataretriever_data(itemIDdict[i][1])
+        
+        if limit2 == 0:
+            dataFrame2 = dataFrame
+        else:
+            dataFrame2 = dataFrame.head(limit2)
+
+        dataFrame2.insert(0, "site_code", rsList[0], True)
+        dataFrame2.insert(1, "dimension", itemIDdict[i][0], True)
+        dataFrame2.insert(3, "period", period, True)
+        if start_hour == "00:00" and end_hour == "00:00":
+            dataFrame2.insert(4, "start_date", startDate, True)
+            dataFrame2.insert(5, "end_date", endDate, True)
+        else :
+            dataFrame2.insert(4, "start_date", "{0} {1}".format(startDate, start_hour), True)
+            dataFrame2.insert(5, "end_date", "{0} {1}".format(EndDateCalculation("0", endDate)[1], end_hour), True)
+        dataFrame2.insert(6, "epp", epp, True)
+        
+        if extra != "":
+            dataFrame2.insert(7, "extra", extra, True)
+        dataFrame2.columns = tbColumn
+        stackTodb(dataFrame2, dbTableName)
```

### Comparing `aanalyticsact_1-0.0.1.51/aanalyticsact_1/actRunner.py` & `aanalyticsact_1-0.0.1.52/aanalyticsact_1/actRunner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Created by Sunkyeong Lee
 # Inquiry : sunkyeong.lee@concentrix.com / sunkyong9768@gmail.com
+# Updated by Youngkwang Cho
+# Inquiry : youngkwang.cho@concentrix.com 
 
 from datetime import datetime, timedelta
 from calendar import monthrange
 
 
 def dateConverter(date):
     return datetime.strptime(str(date), '%Y-%m-%d').date()
@@ -106,15 +108,15 @@
     #22.04.01 si, hr epp 추가
     #22.07.26 iq_ar, lb 추가
     #22.09.01 cl epp 추가
     #22.10.24 ph epp 추가
     #23.02.02 iq_ar epp 추가
     #23.03.03 jp epp 추가
     #23.04.24 mn, ge 추가
-    #24.04.16 semicon 추가
+    #24.04.16 semiconductor 추가
     defaultEpp = [["us", "sssamsungnewus"], ["ae", "sssamsung4aeepp"], ["at", "sssamsung4atepp"], ["au", "sssamsung4auepp"], ["be", "sssamsung4beepp"], ["ca", "sssamsung4caepp"], ["ch", "sssamsung4chepp"], ["cn", "sssamsung4cnepp"], ["cz", "sssamsung4czepp"], ["de", "sssamsung4deepp"], ["dk", "sssamsung4dkepp"], ["ee", "sssamsung4eeepp"], ["eg", "sssamsung4egepp"], ["es", "sssamsung4esepp"], ["fi", "sssamsung4fiepp"], ["fr", "sssamsung4frepp"], ["hk", "sssamsung4hkepp"], ["hu", "sssamsung4huepp"], ["id", "sssamsung4idepp"], ["il", "sssamsung4ilepp"], ["in", "sssamsung4inepp"], ["it", "sssamsung4itepp"], ["levant", "sssamsung4levantepp"], ["lt", "sssamsung4ltepp"], ["lv", "sssamsung4lvepp"], ["my", "sssamsung4myepp"], ["n_africa", "sssamsung4nafricaepp"], ["nl", "sssamsung4nlepp"], ["no", "sssamsung4noepp"], ["nz", "sssamsung4nzepp"], ["pk", "sssamsung4pkepp"], ["pt", "sssamsung4ptepp"], ["ru", "sssamsung4ruepp"], ["sa", "sssamsung4saepp"], ["se", "sssamsung4seepp"], ["sec", "sssamsung4secepp"], ["sg", "sssamsung4sgepp"], ["sk", "sssamsung4skepp"], ["th", "sssamsung4thepp"], ["tw", "sssamsung4twepp"], ["uk", "sssamsung4ukepp"], ["vn", "sssamsung4vnepp"], ["za", "sssamsung4zaepp"], ["kz_kz", "sssamsung4kzkzepp"], ["ua", "sssamsung4uaepp"], ["si", "sssssamsung4siepp"], ["hr", "sssamsung4hrepp"], ["cl", "sssamsung4clepp"], ["ph", "sssamsung4phepp"], ["africa_en", "sssamsung4africaenepp"], ["co", "sssamsung4coepp"], ["gr", "sssamsung4grepp"], ["ie", "sssamsung4ieepp"], ["mx", "sssamsung4mxepp"], ["pe", "sssamsung4peepp"], ["pl", "sssamsung4plepp"], ["ro", "sssamsung4roepp"], ["iq_ar", "sssamsung4iqarepp"], ["jp", "sssamsung4jpepp"]]
     defaultNone = [["us", "sssamsungnewus"], ["sec", "sssamsung4sec"], ["ae", "sssamsung4ae"], ["ae_ar", "sssamsung4aear"], ["africa_en", "sssamsung4africaen"], ["africa_fr", "sssamsung4africafr"], ["africa_pt", "sssamsung4africapt"], ["al", "sssamsung4al"], ["ar", "sssamsung4ar"], ["at", "sssamsung4at"], ["au", "sssamsung4au"], ["ba", "sssamsung4ba"], ["be", "sssamsung4be"], ["be_fr", "sssamsung4befr"], ["bg", "sssamsung4bg"], ["br", "sssamsung4br"], ["ca", "sssamsung4ca"], ["ca_fr", "sssamsung4cafr"], ["ch", "sssamsung4ch"], ["ch_fr", "sssamsung4chfr"], ["cl", "sssamsung4cl"], ["cn", "sssamsung4cn"], ["co", "sssamsung4co"], ["cz", "sssamsung4cz"], ["de", "sssamsung4de"], ["dk", "sssamsung4dk"], ["ee", "sssamsung4ee"], ["eg", "sssamsung4eg"], ["es", "sssamsung4es"], ["fi", "sssamsung4fi"], ["fr", "sssamsung4fr"], ["gr", "sssamsung4gr"], ["hk", "sssamsung4hk"], ["hk_en", "sssamsung4hken"], ["hr", "sssamsung4hr"], ["hu", "sssamsung4hu"], ["id", "sssamsung4id"], ["ie", "sssamsung4ie"], ["il", "sssamsung4il"], ["in", "sssamsung4in"], ["iran", "sssamsung4iran"], ["it", "sssamsung4it"], ["jp", "sssamsung4jp"], ["kz_kz", "sssamsung4kzkz"], ["kz_ru", "sssamsung4kzru"], ["latin", "sssamsung4latin"], ["latin_en", "sssamsung4latinen"], ["levant", "sssamsung4levant"], ["levant_ar", "sssamsung4levantar"], ["lt", "sssamsung4lt"], ["lv", "sssamsung4lv"], ["mk", "sssamsung4mk"], ["mm", "sssamsung4mm"], ["mx", "sssamsung4mx"], ["my", "sssamsung4my"], ["n_africa", "sssamsung4nafrica"], ["nl", "sssamsung4nl"], ["no", "sssamsung4no"], ["nz", "sssamsung4nz"], ["pe", "sssamsung4pe"], ["ph", "sssamsung4ph"], ["pk", "sssamsung4pk"], ["pl", "sssamsung4pl"], ["ps", "sssamsung4ps"], ["pt", "sssamsung4pt"], ["py", "sssamsung4py"], ["ro", "sssamsung4ro"], ["rs", "sssamsung4rs"], ["ru", "sssamsung4ru"], ["sa", "sssamsung4sa"], ["sa_en", "sssamsung4saen"], ["se", "sssamsung4se"], ["sg", "sssamsung4sg"], ["si", "sssamsung4si"], ["sk", "sssamsung4sk"], ["th", "sssamsung4th"], ["tr", "sssamsung4tr"], ["tw", "sssamsung4tw"], ["ua", "sssamsung4ua"], ["uk", "sssamsung4uk"], ["uy", "sssamsung4uy"], ["uz_ru", "sssamsung4uzru"], ["uz_uz", "sssamsung4uzuz"], ["vn", "sssamsung4vn"], ["za", "sssamsung4za"], ["az", "sssamsung4az"], ["bd", "sssamsung4bd"], ["mst_sena", "vrs_samsun0_p4webmstsena_0"], ["mst_sehk", "vrs_samsun0_p6webmstsehk"], ["mst_sebn", "vrs_samsun0_p4websebn"], ["mst_mena", "vrs_samsun0_p4webmstmena"], ["mst_seca", "vrs_samsun0_p4webmstseca"], ["mst_eu", "vrs_samsun0_p4webmsteu_0"], ["mst_seao", "vrs_samsun0_p4webmstseao"], ["iq_ar", "sssamsung4iqar"], ["lb", "sssamsung4lb"], ["mn", "sssamsung4mn"], ["ge", "sssamsung4ge"],["ds-global","sssamsung4b2bsemi"], ["ds-cn","sssamsung4b2bsemicn"],["ds-us","sssamsung4b2bsemius"],["ds-kr","sssamsung4b2bsemikr"],["ds-emea","sssamsung4b2bsemiemea"],["ds-jp","sssamsung4b2csemi"],["ds-total","sssamsung4b2bsemiconductor"]]
 
     if epp == True:
         return rsListGenerator(inputSiteCode, defaultEpp)
     else:
         return rsListGenerator(inputSiteCode, defaultNone)
```

### Comparing `aanalyticsact_1-0.0.1.51/setup.py` & `aanalyticsact_1-0.0.1.52/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import sys
 
 from setuptools import find_packages, setup
 
 # Package meta-data.
 NAME = 'aanalyticsact_1'
-Version= '0.0.1.51'
+Version= '0.0.1.52'
 URL = 'https://github.com/Glory-Cho/aanalyticsact)1'
 Summary= 'adobe analytics library for Team ACT'
 EMAIL = 'youngkwang.cho@concentrix.com'
 AUTHOR = 'Youngkwang Cho'
 
 here = os.path.abspath(os.path.dirname(__file__))
```

