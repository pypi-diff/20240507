# Comparing `tmp/coll-filter-1.2.5.tar.gz` & `tmp/coll-filter-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coll-filter-1.2.5.tar", last modified: Mon Apr 29 02:27:39 2024, max compression
+gzip compressed data, was "coll-filter-1.2.6.tar", last modified: Tue May  7 01:36:07 2024, max compression
```

## Comparing `coll-filter-1.2.5.tar` & `coll-filter-1.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-29 02:27:39.294486 coll-filter-1.2.5/
--rw-r--r--   0 summy      (501) staff       (20)      960 2024-04-29 02:27:39.293685 coll-filter-1.2.5/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      605 2024-04-29 01:47:24.000000 coll-filter-1.2.5/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-29 02:27:39.286876 coll-filter-1.2.5/cf/
--rw-r--r--   0 summy      (501) staff       (20)     7683 2024-04-29 02:25:10.000000 coll-filter-1.2.5/cf/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    10125 2024-04-29 01:13:18.000000 coll-filter-1.2.5/cf/base.py
--rw-r--r--   0 summy      (501) staff       (20)     5350 2024-04-29 01:13:18.000000 coll-filter-1.2.5/cf/pooling.py
--rw-r--r--   0 summy      (501) staff       (20)      867 2023-11-27 02:09:24.000000 coll-filter-1.2.5/cf/utils.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-29 02:27:39.291206 coll-filter-1.2.5/coll_filter.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      960 2024-04-29 02:27:39.000000 coll-filter-1.2.5/coll_filter.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      258 2024-04-29 02:27:39.000000 coll-filter-1.2.5/coll_filter.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-29 02:27:39.000000 coll-filter-1.2.5/coll_filter.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-28 11:32:15.000000 coll-filter-1.2.5/coll_filter.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        3 2024-04-29 02:27:39.000000 coll-filter-1.2.5/coll_filter.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-29 02:27:39.294833 coll-filter-1.2.5/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      846 2024-04-29 02:27:29.000000 coll-filter-1.2.5/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-29 02:27:39.292119 coll-filter-1.2.5/test/
--rw-r--r--   0 summy      (501) staff       (20)      277 2024-01-05 03:59:08.000000 coll-filter-1.2.5/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-07 01:36:07.145910 coll-filter-1.2.6/
+-rw-r--r--   0 summy      (501) staff       (20)      960 2024-05-07 01:36:07.144832 coll-filter-1.2.6/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      605 2024-04-29 01:47:24.000000 coll-filter-1.2.6/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-07 01:36:07.137034 coll-filter-1.2.6/cf/
+-rw-r--r--   0 summy      (501) staff       (20)     6531 2024-05-07 01:16:48.000000 coll-filter-1.2.6/cf/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    10144 2024-05-07 01:30:25.000000 coll-filter-1.2.6/cf/base.py
+-rw-r--r--   0 summy      (501) staff       (20)     4532 2024-05-07 01:32:27.000000 coll-filter-1.2.6/cf/pooling.py
+-rw-r--r--   0 summy      (501) staff       (20)     2840 2024-05-07 01:21:41.000000 coll-filter-1.2.6/cf/utils.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-07 01:36:07.141626 coll-filter-1.2.6/coll_filter.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      960 2024-05-07 01:36:07.000000 coll-filter-1.2.6/coll_filter.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-07 01:36:07.000000 coll-filter-1.2.6/coll_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-07 01:36:07.000000 coll-filter-1.2.6/coll_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-07 01:36:07.000000 coll-filter-1.2.6/coll_filter.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        3 2024-05-07 01:36:07.000000 coll-filter-1.2.6/coll_filter.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-07 01:36:07.146180 coll-filter-1.2.6/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      846 2024-05-07 01:35:45.000000 coll-filter-1.2.6/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-07 01:36:07.142693 coll-filter-1.2.6/test/
+-rw-r--r--   0 summy      (501) staff       (20)      277 2024-01-05 03:59:08.000000 coll-filter-1.2.6/test/test.py
```

### Comparing `coll-filter-1.2.5/PKG-INFO` & `coll-filter-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: coll-filter
-Version: 1.2.5
+Version: 1.2.6
 Summary: Collaborative Filtering with multi-process parallelism.
 Home-page: https://gitee.com/summry/myai
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: Collaborative Filtering,recommend
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
```

### Comparing `coll-filter-1.2.5/README.rst` & `coll-filter-1.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `coll-filter-1.2.5/cf/__init__.py` & `coll-filter-1.2.6/cf/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,34 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
-"""coll filter"""
+"""
+Collaborative filter
+
+Examples
+--------
+>>> from cf import CollFilter
+>>> data = read_data('file_path')
+>>> data = pre_process(data)  # return List(user_id: Any, item_id: Any, rating: float)]
+>>> cf = CollFilter(data)
+>>> ucf = cf.user_cf()  # return {user_id: [(item_id, score),],}
+>>> icf = cf.item_cf()  # return {user_id: [(item_id, score),],}
+>>> recommend = cf.recommend(user_id, recall_num=5) # return [(item_id, score),]
+>>> recommends = cf.recommends(user_ids, recall_num=5) # return {user_id: [(item_id, score),],}
+>>> cf.release()
+"""
 
 import os
 import math
 from enum import Enum
 from typing import Iterable, Tuple, List, Mapping, Collection, Generic, TypeVar
 
+from .utils import fusion
+
+
 U = TypeVar('U')
 T = TypeVar('T')
 
 
 class CFType(Enum):
     UCF = 'ucf'
     ICF = 'icf'
@@ -103,15 +120,15 @@
         if recall_num == 1:
             if icf_items:
                 return icf_items
             else:
                 return self.user_cf(recall_num, similar_num, [user_id], None, similar_fn)[user_id]
         else:
             ucf_items = self.user_cf(recall_num, similar_num, [user_id], None, similar_fn)[user_id]
-            return self._fusion(icf_items, ucf_items, recall_num, ratio)
+            return fusion(icf_items, ucf_items, recall_num, ratio)
 
     def recommends(self,
                    user_ids: Collection[U],
                    recall_num=64,
                    similar_num=8,
                    similar_fn=None,
                    ratio=0.5
@@ -131,15 +148,15 @@
             for user_id, items in icf.items():
                 if not items:
                     icf[user_id] = self.user_cf(recall_num, similar_num, [user_id], user_similar, similar_fn)[user_id]
         else:
             ucf = self.user_cf(recall_num, similar_num, user_ids, None, similar_fn)
             for user_id, icf_items in icf.items():
                 ucf_items = ucf[user_id]
-                icf[user_id] = self._fusion(icf_items, ucf_items, recall_num, ratio)
+                icf[user_id] = fusion(icf_items, ucf_items, recall_num, ratio)
 
         return icf
 
     def get_user_similar(self, similar_num=256, similar_fn=None) -> Mapping[U, Mapping[U, float]]:
         """
         用户相似矩阵
         """
@@ -150,39 +167,7 @@
         物品相似矩阵
         """
         return self._coll_filter.cal_similar(CFType.ICF, similar_num, similar_fn)
 
     def release(self):
         self._coll_filter.release()
 
-    @staticmethod
-    def _fusion(icf_items, ucf_items, recall_num, ratio):
-        ucf_items_dict = dict(ucf_items)
-        # item_cf和user_cf共同出现的先放进result_items里
-        result_items = [(item[0], item[1] + ucf_items_dict[item[0]]) for item in icf_items if item[0] in ucf_items_dict]
-        result_items_len = len(result_items)
-        if result_items_len >= recall_num:
-            return result_items[:recall_num]
-
-        leave_num = recall_num - result_items_len
-        half = round(leave_num * ratio + 0.01)  # 加0.01避免*.5是四舍五入向下取整
-        result_item_ids = [item[0] for item in result_items]
-        leave_icf_items = [item for item in icf_items if item[0] not in result_item_ids]
-        leave_ucf_items = [item for item in ucf_items if item[0] not in result_item_ids]
-        if len(leave_icf_items) > half and len(leave_ucf_items) > (leave_num - half):
-            result_items.extend(icf_items[:half])
-            result_items.extend(leave_ucf_items[:(leave_num - half)])
-            return result_items
-        elif len(leave_icf_items) < half:
-            result_items.extend(leave_icf_items)
-            result_items.extend(leave_ucf_items[:(leave_num - half)])
-            return result_items
-        elif len(leave_ucf_items) < (leave_num - half):
-            result_items.extend(leave_icf_items[:(leave_num - len(leave_ucf_items))])
-            result_items.extend(leave_ucf_items)
-            return result_items
-
-        result_items.extend(leave_icf_items[:leave_num])
-        leave_num = recall_num - len(result_items)
-        if leave_num > 0:
-            result_items.extend(leave_ucf_items[:leave_num])
-        return result_items
```

### Comparing `coll-filter-1.2.5/cf/base.py` & `coll-filter-1.2.6/cf/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 # -*- coding:utf-8 -*-
 
 """base_coll_filter, one process"""
 
 import os
 import time
 import math
-from cf import default_similar_func, CFType, U, T
-from cf.utils import print_cost_time, sort_similar
 from typing import Iterable, Mapping, Tuple, Generic
 
+from . import default_similar_func, CFType, U, T
+from .utils import print_cost_time, sort_similar, logger
+
 
 class CollFilterHelper:
     @staticmethod
     def _rating_user_cf(user_item_ratings, similar_dict, user_items_list, recall_num):
         start_time = time.perf_counter()
         result = {}
         for user_id, items in user_items_list:
@@ -27,15 +28,15 @@
                         continue
                     item_score[item] = item_score.get(item, 0.0) + math.sqrt(similar * rating)
             if len(item_score) > 0:
                 result[user_id] = sorted(item_score.items(), key=lambda x: x[1], reverse=True)[:recall_num]
             else:
                 result[user_id] = []
 
-        print_cost_time(f"\t进程: {os.getpid()}, 处理 {len(user_items_list)} 条记录, 生成 {len(result)} 条记录, 耗时", start_time)
+        print_cost_time(f"\t\t进程<{os.getpid()}> 处理 {len(user_items_list)} 条记录, 生成 {len(result)} 条记录, 耗时", start_time)
         return result
 
     @staticmethod
     def _rating_item_cf(_user_item_ratings, similar_dict, user_items_list, recall_num):
         start_time = time.perf_counter()
         result = {}
         for user_id, item_ratings in user_items_list:
@@ -48,15 +49,15 @@
                         continue
                     item_score[item2] = item_score.get(item2, 0.0) + math.sqrt(similar * rating)
             if len(item_score) > 0:
                 result[user_id] = sorted(item_score.items(), key=lambda x: x[1], reverse=True)[:recall_num]
             else:
                 result[user_id] = []
 
-        print_cost_time(f"\t进程: {os.getpid()}, 处理 {len(user_items_list)} 条记录, 生成 {len(result)} 条记录, 耗时", start_time)
+        print_cost_time(f"\t\t进程<{os.getpid()}> 处理 {len(user_items_list)} 条记录, 生成 {len(result)} 条记录, 耗时", start_time)
         return result
 
 
 class BaseCollFilter(CollFilterHelper, Generic[U, T]):
 
     def __init__(self, data: Iterable[Tuple[U, T, float]], similar_fn=default_similar_func, cache_similar=False):
         self.similar_fn = similar_fn
@@ -69,15 +70,15 @@
             self._data_process(user_id, item_id, rating)
 
         self.item_users = {item_id: list(set(users)) for item_id, users in self.item_users.items()}
         self._cache_similar = cache_similar
         if cache_similar:
             self._user_similar_cache, self._item_similar_cache = None, None
 
-        print_cost_time(f"数据处理, 当前进程: {os.getpid()}, 处理 {cnt} 条记录, "
+        print_cost_time(f"数据处理, 当前进程<{os.getpid()}> 处理 {cnt} 条记录, "
                         f"user数: {len(self.user_item_ratings)}, item数: {len(self.item_users)}, 耗时", start_time)
 
     def user_cf(self, recall_num=10, similar_num=256, user_ids=None, user_similar=None, similar_fn=None):
         """
         用户协同过滤
 
         @param recall_num  每个用户推荐结果数目
@@ -133,21 +134,21 @@
 
     def _cal_similar(self, cf_type: CFType, similar_num, similar_fn):
         """
         计算相似度
 
         @return dict{:List()}    {user1: {user2: similar}}
         """
-        print(f'开始{cf_type.value}相似度计算, similar_num = {similar_num}')
+        logger.info(f'开始{cf_type.value}相似度计算, similar_num = {similar_num}')
         func_start_time = time.perf_counter()
         dict1, items_list, cal_similar_func = self._get_cal_similar_inputs(cf_type)
         similar_fn = similar_fn if similar_fn else self.similar_fn
         similar = cal_similar_func(dict1, items_list, similar_fn)
         similar = sort_similar(similar, similar_num)
-        print_cost_time(f"完成{cf_type.value}相似度计算, 当前进程: {os.getpid()}, 总生成 {len(similar)} 条记录, 总耗时", func_start_time)
+        print_cost_time(f"完成{cf_type.value}相似度计算, 当前进程<{os.getpid()}> 总生成 {len(similar)} 条记录, 总耗时", func_start_time)
         return similar
 
     def _data_process(self, user_id: U, item_id: T, rating: float):
         user_item_rating = self.user_item_ratings.get(user_id)
         if user_item_rating:
             user_item_rating[item_id] = user_item_rating.get(item_id, 0) + rating
         else:
@@ -178,15 +179,15 @@
                 if item1 not in similar:
                     similar[item1] = {}
                 for item2 in items:
                     if item1 == item2:
                         continue
                     # 计算两个item间的相似性
                     similar[item1][item2] = similar[item1].get(item2, 0.0) + similar_func(list(dict1.get(item1, {}).keys()), list(dict1.get(item2, {}).keys()))
-        print_cost_time(f"\t进程: {os.getpid()}, 生成 {len(similar)} 条记录, 耗时", start_time)
+        print_cost_time(f"\t\t进程<{os.getpid()}> 生成 {len(similar)} 条记录, 耗时", start_time)
         return similar
 
     @staticmethod
     def _cal_icf_similar(dict1: Mapping, items_list: Iterable[Iterable], similar_func):
         start_time = time.perf_counter()
         similar = {}
 
@@ -199,28 +200,28 @@
                     similar[item1] = {}
                 for item2 in items:
                     if item1 == item2:
                         continue
                     # 计算两个item间的相似性
                     similar[item1][item2] = similar[item1].get(item2, 0.0) + similar_func(dict1.get(item1, []),
                                                                                           dict1.get(item2, []))
-        print_cost_time(f"\t进程: {os.getpid()}, 生成 {len(similar)} 条记录, 耗时", start_time)
+        print_cost_time(f"\t\t进程<{os.getpid()}> 生成 {len(similar)} 条记录, 耗时", start_time)
         return similar
 
     def _cf(self, user_ids, similar_dict, recall_num, cf_type: CFType):
-        print(f'开始{cf_type.value}推理, recall_num = {recall_num}')
+        logger.info(f'开始{cf_type.value}推理, recall_num = {recall_num}')
         func_start_time = time.perf_counter()
         if user_ids:
             if not set(user_ids).intersection(self.user_item_ratings.keys()):
                 return {user_id: [] for user_id in user_ids}
 
             user_items_list = [(user_id, self.user_item_ratings.get(user_id, {})) for user_id in user_ids]
         else:
             user_items_list = self.user_item_ratings.items()
 
         if cf_type == CFType.UCF:
             cf_result = self._rating_user_cf(self.user_item_ratings, similar_dict, user_items_list, recall_num)
         else:
             cf_result = self._rating_item_cf(self.user_item_ratings, similar_dict, user_items_list, recall_num)
-        print_cost_time(f"完成{cf_type.value}推理, 当前进程: {os.getpid()}, 生成{len(cf_result)}条记录, 总耗时", func_start_time)
+        print_cost_time(f"完成{cf_type.value}推理, 当前进程<{os.getpid()}> 生成{len(cf_result)}条记录, 总耗时", func_start_time)
         return cf_result
```

### Comparing `coll-filter-1.2.5/cf/pooling.py` & `coll-filter-1.2.6/cf/pooling.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 """pool_coll_filter"""
 
 import os
 import time
 import math
 from multiprocessing import Pool
 from typing import Iterable, Tuple
-from cf.base import BaseCollFilter
-from cf import default_similar_func, CFType, U, T
-from cf.utils import print_cost_time, sort_similar
+from .base import BaseCollFilter
+from . import default_similar_func, CFType, U, T
+from .utils import print_cost_time, sort_similar, logger
 
 
 class PoolMultiProcessor:
 
     def __init__(self, parallel_num):
         cpu_count = os.cpu_count()
         self.parallel_num = cpu_count if parallel_num <= 1 else parallel_num
@@ -73,64 +73,37 @@
 
     def _cal_similar(self, cf_type: CFType, similar_num, similar_fn):
         """
         计算相似度
 
         @return dict{:dict}    {user1: {user2: similar}}
         """
-        print(f'开始{cf_type.value}相似度计算, similar_num: {similar_num}')
+        logger.info(f'开始{cf_type.value}相似度计算, similar_num: {similar_num}')
         func_start_time = time.perf_counter()
         dict1, items_list, cal_similar_func = self._get_cal_similar_inputs(cf_type)
         items_list = list(items_list)
         similar_fn = similar_fn if similar_fn else self.similar_fn
         similar = self.processor.cal_similar(dict1, items_list, cal_similar_func, similar_fn)
         similar = sort_similar(similar, similar_num)
-        print_cost_time(f"完成{cf_type.value}相似度计算, 当前进程: {os.getpid()}, 总生成 {len(similar)} 条记录, 总耗时", func_start_time)
+        print_cost_time(f"完成{cf_type.value}相似度计算, 当前进程<{os.getpid()}>, 总生成 {len(similar)} 条记录, 总耗时", func_start_time)
         return similar
         self.processor.release()
 
     def _cf(self, user_ids, similar_dict, recall_num, cf_type: CFType):
-        print(f'开始{cf_type.value}推理, recall_num: {recall_num}')
+        logger.info(f'开始{cf_type.value}推理, recall_num: {recall_num}')
         func_start_time = time.perf_counter()
         if user_ids:
             if not set(user_ids).intersection(self.user_item_ratings.keys()):
                 return {user_id: [] for user_id in user_ids}
 
             user_items_list = list(map(lambda x: (x, self.user_item_ratings.get(x, [])), user_ids))
         else:
             user_items_list = self.user_item_ratings.items()
 
         cf_func = self._rating_user_cf if cf_type == CFType.UCF else self._rating_item_cf
         if len(user_items_list) > 4096:
             cf_result = self.processor.cf(self.user_item_ratings, user_items_list, similar_dict, recall_num, cf_func)
         else:
             cf_result = cf_func(self.user_item_ratings, similar_dict, user_items_list, recall_num)
-        print_cost_time(f"完成{cf_type.value}推理, 当前进程: {os.getpid()}, 生成{len(cf_result)}条记录, 总耗时", func_start_time)
+        print_cost_time(f"完成{cf_type.value}推理, 当前进程<{os.getpid()}>, 生成{len(cf_result)}条记录, 总耗时", func_start_time)
         return cf_result
 
-
-if __name__ == '__main__':
-    import json
-    from cf.utils import read_data, pre_process
-    # train_path = '/Users/summy/project/rust/ai/train.csv'
-    # data = read_data(train_path)
-    # data = pre_process(data)
-    # cf = PoolCollFilter(data, 4)
-    # ucf = cf.user_cf()
-    # with open('../ucf_op', 'w') as f:
-    #     json.dump(ucf, f)
-    # icf = cf.item_cf()
-    # with open('../icf_op', 'w') as f:
-    #     json.dump(icf, f)
-
-    def handle(line) -> (int, str, float):
-        user_id, item_id, _, _, _ = line.strip().split(",")
-        return int(user_id), item_id, 1
-
-    train_path = '/Users/summy/project/python/work/video_rec_recall/data/V0002_20_25.csv'
-    data = read_data(train_path)[:50000]
-    data = pre_process(data, handle)
-    cf = PoolCollFilter(data, 8)
-    ucf = cf.user_cf()
-    icf = cf.item_cf()
-
-
```

### Comparing `coll-filter-1.2.5/coll_filter.egg-info/PKG-INFO` & `coll-filter-1.2.6/coll_filter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: coll-filter
-Version: 1.2.5
+Version: 1.2.6
 Summary: Collaborative Filtering with multi-process parallelism.
 Home-page: https://gitee.com/summry/myai
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: Collaborative Filtering,recommend
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
```

### Comparing `coll-filter-1.2.5/setup.py` & `coll-filter-1.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 
 setup(
     name='coll-filter',
     packages=['cf'],
     description="Collaborative Filtering with multi-process parallelism.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.5',
+    version='1.2.6',
     url='https://gitee.com/summry/myai',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['Collaborative Filtering', 'recommend'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
     include_package_data=True,
-    python_requires='>=3.5',
+    python_requires='>=3.6',
     zip_safe=False
 )
```

