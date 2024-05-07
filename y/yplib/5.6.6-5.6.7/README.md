# Comparing `tmp/yplib-5.6.6.tar.gz` & `tmp/yplib-5.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yplib-5.6.6.tar", last modified: Tue May  7 03:27:19 2024, max compression
+gzip compressed data, was "yplib-5.6.7.tar", last modified: Tue May  7 06:50:15 2024, max compression
```

## Comparing `yplib-5.6.6.tar` & `yplib-5.6.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 03:27:19.051218 yplib-5.6.6/
--rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.6.6/LICENSE
--rw-rw-rw-   0        0        0      355 2024-05-07 03:27:19.051218 yplib-5.6.6/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.6.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-07 03:27:19.051218 yplib-5.6.6/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-05-07 03:26:54.000000 yplib-5.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:27:19.036223 yplib-5.6.6/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 02:25:38.000000 yplib-5.6.6/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.6.6/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.6.6/yplib/chart_html.py
--rw-rw-rw-   0        0        0    11786 2024-04-29 03:59:19.000000 yplib-5.6.6/yplib/db.py
--rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.6.6/yplib/file.py
--rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.6.6/yplib/http_util.py
--rw-rw-rw-   0        0        0    41364 2024-05-07 03:26:32.000000 yplib-5.6.6/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.6.6/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.6.6/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.6.6/yplib/markdown.py
--rw-rw-rw-   0        0        0     1683 2024-05-07 03:26:17.000000 yplib-5.6.6/yplib/multi_thread.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.6.6/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:27:19.051218 yplib-5.6.6/yplib.egg-info/
--rw-rw-rw-   0        0        0      355 2024-05-07 03:27:18.000000 yplib-5.6.6/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-07 03:27:18.000000 yplib-5.6.6/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 03:27:18.000000 yplib-5.6.6/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-07 03:27:18.000000 yplib-5.6.6/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 06:50:15.210533 yplib-5.6.7/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.6.7/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-05-07 06:50:15.210533 yplib-5.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.6.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 06:50:15.210533 yplib-5.6.7/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-05-07 06:49:53.000000 yplib-5.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:50:15.195536 yplib-5.6.7/yplib/
+-rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.6.7/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.6.7/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.6.7/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    11732 2024-05-07 06:49:39.000000 yplib-5.6.7/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.6.7/yplib/file.py
+-rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.6.7/yplib/http_util.py
+-rw-rw-rw-   0        0        0    41364 2024-05-07 03:26:32.000000 yplib-5.6.7/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.6.7/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.6.7/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.6.7/yplib/markdown.py
+-rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.6.7/yplib/multi_thread.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.6.7/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:50:15.210533 yplib-5.6.7/yplib.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-05-07 06:50:14.000000 yplib-5.6.7/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-07 06:50:14.000000 yplib-5.6.7/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 06:50:14.000000 yplib-5.6.7/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-07 06:50:14.000000 yplib-5.6.7/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.6.6/LICENSE` & `yplib-5.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-5.6.6/setup.py` & `yplib-5.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.6.6",
+    version="5.6.7",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.6.6/yplib/__init__.py` & `yplib-5.6.7/yplib/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,7 +21,9 @@
 from yplib.mail import *
 from yplib.mail_html import *
 # 生成 markdown 的文本
 from yplib.markdown import *
 
 # 临时添加的工具类
 from yplib.temp import *
+# 多线程处理类的数据
+from yplib.multi_thread import *
```

### Comparing `yplib-5.6.6/yplib/chart.py` & `yplib-5.6.7/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.6/yplib/chart_html.py` & `yplib-5.6.7/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.6/yplib/db.py` & `yplib-5.6.7/yplib/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,40 +38,44 @@
         if is_log:
             to_log_file(sql)
         db_cursor.execute(str(sql))
     if commit:
         db_conn.commit()
 
 
-# 执行 sql 语句, 并且提交, 默认值提交的了
-def exec_doris_sql(sql='', db_config='doris'):
+def get_doris_conn(db_config='doris'):
     config_db = get_config_data(db_config)
     my_uri = config_db['uri']
     my_db_kwargs = {
         adbc_driver_manager.DatabaseOptions.USERNAME.value: config_db['username'],
         adbc_driver_manager.DatabaseOptions.PASSWORD.value: config_db['password'],
     }
     conn = flight_sql.connect(uri=my_uri, db_kwargs=my_db_kwargs)
+    return conn
+
+
+# 执行 sql 语句, 并且提交, 默认值提交的了
+def exec_doris_sql(sql='', db_config='doris'):
+    conn = get_doris_conn(db_config)
     cursor = conn.cursor()
     cursor.execute(sql)
     cursor.close()
+    conn.close()
 
 
 def get_data_from_doris(sql='', db_config='doris'):
-    config_db = get_config_data(db_config)
-    my_uri = config_db['uri']
-    my_db_kwargs = {
-        adbc_driver_manager.DatabaseOptions.USERNAME.value: config_db['username'],
-        adbc_driver_manager.DatabaseOptions.PASSWORD.value: config_db['password'],
-    }
-    conn = flight_sql.connect(uri=my_uri, db_kwargs=my_db_kwargs)
+    conn = get_doris_conn(db_config)
     cursor = conn.cursor()
     cursor.execute(sql)
     arrow_data = cursor.fetchallarrow()
-    return arrow_data
+    dataframe = arrow_data.to_pandas()
+    json_data = dataframe.to_json(orient='records')
+    cursor.close()
+    conn.close()
+    return json_data
 
 
 # 执行 sql 语句, 不提交
 def exec_sql_un_commit(sql='', db_conn=None, database=None):
     exec_sql(sql=sql, db_conn=db_conn, commit=False, database=database)
```

### Comparing `yplib-5.6.6/yplib/file.py` & `yplib-5.6.7/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.6/yplib/http_util.py` & `yplib-5.6.7/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.6/yplib/index.py` & `yplib-5.6.7/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.6/yplib/mail.py` & `yplib-5.6.7/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.6/yplib/mail_html.py` & `yplib-5.6.7/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.6/yplib/markdown.py` & `yplib-5.6.7/yplib/markdown.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.6/yplib/multi_thread.py` & `yplib-5.6.7/yplib/multi_thread.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,62 @@
-# from yplib.index import *
-# import threading
-#
-#
-# # all_list   : 所有的线程,需要处理的数据总数
-# # thread_num : 线程数量
-# # thread_fun : 每个线程需要执行的函数
-# def do_thread(all_list=[], thread_num=100, thread_fun=None):
-#     # 线程数量
-#     t_num = int(thread_num) if thread_num is not None else 10
-#     # 所有的线程,需要做的任务总数
-#     one_thread_do_num = int(len(all_list) / thread_count) + 1 if int(len(all_list) % thread_count) > 0 else 0
-#     for t_i in range(t_num):
-#         temp_list = all_list[t_i * one_thread_do_num:(t_i + 1) * one_thread_do_num]
-#         ta = threading.Thread(target=do_thread, args=(temp_list, index))
-#         ta.start()
-#     print('do_thread done')
-#
-#
-# ##############################################################################################################
+from yplib.index import *
+import threading
+
+
+# all_list   : 所有的线程,需要处理的数据总数
+# thread_num : 线程数量
+# thread_fun : 每个线程需要执行的函数
+def do_multi_thread(all_list=None, thread_num=100, thread_fun=None):
+    # 线程数量
+    if all_list is None:
+        all_list = []
+    t_num = int(thread_num) if thread_num is not None else 100
+    need_param_list = len(all_list)
+    # 所有的线程,需要做的任务总数
+    one_thread_do_num = int(len(all_list) / t_num)
+    one_thread_do_num = one_thread_do_num + 1 if int(len(all_list) % t_num) > 0 else one_thread_do_num
+    for t_i in range(t_num):
+        temp_list = all_list[t_i * one_thread_do_num:(t_i + 1) * one_thread_do_num]
+        # 当数据量过多的时候,就不用开那么多的线程了
+        if not len(temp_list) and need_param_list:
+            continue
+        # print('list_sub_index', t_i * one_thread_do_num, (t_i + 1) * one_thread_do_num)
+        ta = threading.Thread(target=thread_fun, args=(t_i + 1, temp_list))
+        ta.start()
+
+##############################################################################################################
 # from yplib import *
-#
-#
-# # 50 个线程
-# def do_thread_fun(do_list=[], index=1):
-#     print('do_thread done')
-#
+
+
+# def do_thread_fun(index=1, do_list=[]):
+#     # print(index, 'do_thread done', len(do_list), do_list[0])
+#     print(index, 'do_thread done')
+
+
 #
 # sql = "SELECT data FROM tb_data WHERE JSON_EXTRACT(data, '$.type') = 'oss_data_ng' order by id desc limit 1;"
 # id_list = json.loads(get_data_from_sql(sql=sql, db_config='dev_db')[0][0])['data']
 #
+# id_list = id_list[0:31]
+# id_list = id_list[0:310]
+#
 # print('start')
 # print(len(id_list))
+#
+# do_multi_thread(id_list, thread_fun=do_thread_fun, thread_num=5)
+
+
+# do_multi_thread(thread_fun=do_thread_fun, thread_num=100)
+
 # # 线程数量
 # thread_count = 100
 # # 所有的线程,需要做的任务总数
 #
 # one_thread_do_num = int(len(id_list) / thread_count) + 1 if int(len(id_list) % thread_count) > 0 else 0
 #
 # print(one_thread_do_num)
 # for i in range(one_thread_do_num):
 #     temp_list = id_list[use_length: use_length + 100]
 #     ta = threading.Thread(target=do_thread, args=(temp_list, index))
 #     ta.start()
-#
+
 # print('end')
```

