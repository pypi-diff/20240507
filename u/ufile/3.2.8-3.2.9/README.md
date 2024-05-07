# Comparing `tmp/ufile-3.2.8.tar.gz` & `tmp/ufile-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufile-3.2.8.tar", last modified: Tue Oct 17 08:00:39 2023, max compression
+gzip compressed data, was "/Users/user/Public/py/ufile-sdk-python/dist/.tmp-5ggyu0jf/ufile-3.2.9.tar", last modified: Mon May  6 10:40:32 2024, max compression
```

## Comparing `ufile-3.2.8.tar` & `ufile-3.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-10-17 08:00:39.521151 ufile-3.2.8/
--rw-r--r--   0 user       (501) staff       (20)    11357 2023-06-30 08:14:21.000000 ufile-3.2.8/LICENSE
--rw-r--r--   0 user       (501) staff       (20)      942 2023-10-17 08:00:39.520949 ufile-3.2.8/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     6415 2022-12-05 07:14:09.000000 ufile-3.2.8/README.md
--rw-r--r--   0 user       (501) staff       (20)       38 2023-10-17 08:00:39.521192 ufile-3.2.8/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)     1702 2022-12-05 07:14:09.000000 ufile-3.2.8/setup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-10-17 08:00:39.519430 ufile-3.2.8/ufile/
--rw-r--r--   0 user       (501) staff       (20)       84 2023-06-30 08:27:45.000000 ufile-3.2.8/ufile/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3002 2022-12-05 07:14:09.000000 ufile-3.2.8/ufile/auth.py
--rw-r--r--   0 user       (501) staff       (20)     7312 2022-12-05 07:14:09.000000 ufile-3.2.8/ufile/baseufile.py
--rw-r--r--   0 user       (501) staff       (20)     8863 2022-12-05 07:14:09.000000 ufile-3.2.8/ufile/bucketmanager.py
--rw-r--r--   0 user       (501) staff       (20)     1355 2023-08-22 08:42:08.000000 ufile-3.2.8/ufile/compact.py
--rw-r--r--   0 user       (501) staff       (20)     1834 2023-05-30 07:44:43.000000 ufile-3.2.8/ufile/config.py
--rw-r--r--   0 user       (501) staff       (20)    26167 2023-08-22 08:44:00.000000 ufile-3.2.8/ufile/filemanager.py
--rw-r--r--   0 user       (501) staff       (20)    19424 2023-06-30 09:44:45.000000 ufile-3.2.8/ufile/httprequest.py
--rw-r--r--   0 user       (501) staff       (20)      701 2022-12-05 07:14:09.000000 ufile-3.2.8/ufile/logger.py
--rw-r--r--   0 user       (501) staff       (20)    22336 2023-06-30 08:09:02.000000 ufile-3.2.8/ufile/multipartuploadufile.py
--rw-r--r--   0 user       (501) staff       (20)    17939 2023-06-30 06:41:44.000000 ufile-3.2.8/ufile/util.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-10-17 08:00:39.520667 ufile-3.2.8/ufile.egg-info/
--rw-r--r--   0 user       (501) staff       (20)      942 2023-10-17 08:00:39.000000 ufile-3.2.8/ufile.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      379 2023-10-17 08:00:39.000000 ufile-3.2.8/ufile.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-10-17 08:00:39.000000 ufile-3.2.8/ufile.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        9 2023-10-17 08:00:39.000000 ufile-3.2.8/ufile.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        6 2023-10-17 08:00:39.000000 ufile-3.2.8/ufile.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-06 10:40:32.000000 ufile-3.2.9/
+-rw-r--r--   0 user       (501) staff       (20)    11357 2023-06-30 08:14:21.000000 ufile-3.2.9/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)      918 2024-05-06 10:40:32.000000 ufile-3.2.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     6415 2022-12-05 07:14:09.000000 ufile-3.2.9/README.md
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-05-06 10:40:32.000000 ufile-3.2.9/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)     1702 2022-12-05 07:14:09.000000 ufile-3.2.9/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-06 10:40:32.000000 ufile-3.2.9/ufile/
+-rw-r--r--   0 user       (501) staff       (20)       84 2024-04-23 07:21:02.000000 ufile-3.2.9/ufile/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3002 2022-12-05 07:14:09.000000 ufile-3.2.9/ufile/auth.py
+-rw-r--r--   0 user       (501) staff       (20)     7312 2022-12-05 07:14:09.000000 ufile-3.2.9/ufile/baseufile.py
+-rw-r--r--   0 user       (501) staff       (20)     8863 2022-12-05 07:14:09.000000 ufile-3.2.9/ufile/bucketmanager.py
+-rw-r--r--   0 user       (501) staff       (20)     1355 2023-08-22 08:42:08.000000 ufile-3.2.9/ufile/compact.py
+-rw-r--r--   0 user       (501) staff       (20)     1834 2023-05-30 07:44:43.000000 ufile-3.2.9/ufile/config.py
+-rw-r--r--   0 user       (501) staff       (20)    27706 2024-04-22 06:06:51.000000 ufile-3.2.9/ufile/filemanager.py
+-rw-r--r--   0 user       (501) staff       (20)    20906 2024-04-22 03:54:37.000000 ufile-3.2.9/ufile/httprequest.py
+-rw-r--r--   0 user       (501) staff       (20)      701 2022-12-05 07:14:09.000000 ufile-3.2.9/ufile/logger.py
+-rw-r--r--   0 user       (501) staff       (20)    24057 2023-11-21 08:14:19.000000 ufile-3.2.9/ufile/multipartuploadufile.py
+-rw-r--r--   0 user       (501) staff       (20)    19464 2024-04-22 03:47:15.000000 ufile-3.2.9/ufile/util.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-06 10:40:32.000000 ufile-3.2.9/ufile.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)      918 2024-05-06 10:40:32.000000 ufile-3.2.9/ufile.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      379 2024-05-06 10:40:32.000000 ufile-3.2.9/ufile.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-05-06 10:40:32.000000 ufile-3.2.9/ufile.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        9 2024-05-06 10:40:32.000000 ufile-3.2.9/ufile.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        6 2024-05-06 10:40:32.000000 ufile-3.2.9/ufile.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ufile-3.2.8/LICENSE` & `ufile-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ufile-3.2.8/PKG-INFO` & `ufile-3.2.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufile
-Version: 3.2.8
+Version: 3.2.9
 Summary: UCloud UFile Python SDK
 Home-page: https://github.com/ucloud/ufile-sdk-python
 Author-email: leo.li@ucloud.cn
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -16,8 +16,7 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
-Requires-Dist: requests
```

### Comparing `ufile-3.2.8/README.md` & `ufile-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ufile-3.2.8/setup.py` & `ufile-3.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `ufile-3.2.8/ufile/auth.py` & `ufile-3.2.9/ufile/auth.py`

 * *Files identical despite different names*

### Comparing `ufile-3.2.8/ufile/baseufile.py` & `ufile-3.2.9/ufile/baseufile.py`

 * *Files identical despite different names*

### Comparing `ufile-3.2.8/ufile/bucketmanager.py` & `ufile-3.2.9/ufile/bucketmanager.py`

 * *Files identical despite different names*

### Comparing `ufile-3.2.8/ufile/compact.py` & `ufile-3.2.9/ufile/compact.py`

 * *Files identical despite different names*

### Comparing `ufile-3.2.8/ufile/config.py` & `ufile-3.2.9/ufile/config.py`

 * *Files identical despite different names*

### Comparing `ufile-3.2.8/ufile/filemanager.py` & `ufile-3.2.9/ufile/filemanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 import time
 
 from . import config
 from .baseufile import BaseUFile
 from .compact import b, s, u, url_parse, quote
 from .config import BLOCKSIZE
 from .httprequest import _put_stream, _put_file, _post_file, ResponseInfo, _uploadhit_file, _download_file, \
-    _delete_file, _getfilelist, _head_file, _restore_file, _classswitch_file, _copy_file, _rename_file, _listobjects
+    _delete_file, _getfilelist, _head_file, _restore_file, _classswitch_file, _copy_file, _rename_file, _listobjects, \
+    _op_meta
 from .logger import logger
 from .util import _check_dict, ufile_put_url, ufile_post_url, file_etag, ufile_uploadhit_url, ufile_getfilelist_url, \
     mimetype_from_file, ufile_restore_url, ufile_classswitch_url, ufile_copy_url, ufile_rename_url, \
-    ufile_listobjects_url
+    ufile_listobjects_url, ufile_op_meta_url
 
 
 class FileManager(BaseUFile):
     """
     UCloud UFile普通上传文件类
     """
 
@@ -531,7 +532,39 @@
                                     marker if isinstance(marker, str) else marker.encode('utf-8')),
                                 '' if maxkeys is None else ', maxkeys: {0}'.format(maxkeys),
                                 '' if prefix is None else ', prefix: {0}'.format(prefix),
                                 '' if delimiter is None else ', delimiter: {0}'.format(delimiter)])
         logger.info(info_message)
         url = ufile_listobjects_url(bucket, upload_suffix=self.__upload_suffix)
         return _listobjects(url, header, param)
+
+    def opMeta(self, bucket, key, metak, metav, op="set", header=None):
+        """
+        获取文件元数据
+
+        :param bucket: string 类型，空间名称
+        :param key: string 类型，文件在空间中的名称
+        :param metak: string 类型，元数据的key
+        :param metav: string 类型，元数据的value
+        :param op: string 类型，操作类型，目前只支持set
+        :param header: dict类型，http 请求header，键值对类型分别为string，比如{'User-Agent': 'Google Chrome'}
+        :return: ret: 如果http状态码为[200, 204, 206]之一则返回None，否则如果服务器返回json信息则返回dict类型，键值对类型分别为string, unicode string类型，否则返回空的dict
+        :return:  ResponseInfo: 响应的具体信息，UCloud UFile 服务器返回信息或者网络链接异常
+        """
+        if header is None:
+            header = dict()
+        else:
+            _check_dict(header)
+
+        if 'User-Agent' not in header:
+            header['User-Agent'] = config.get_default('user_agent')
+        header['Content-Type'] = 'application/json'
+
+        auth = self.authorization('post', bucket, key, header, action="opmeta")
+        header['Authorization'] = auth
+        data = {
+            'op': op,
+            'metak': metak,
+            'metav': metav
+        }
+        url = ufile_op_meta_url(bucket, key, upload_suffix=self.__upload_suffix)
+        return _op_meta(url, json.dumps(data), header)
```

### Comparing `ufile-3.2.8/ufile/httprequest.py` & `ufile-3.2.9/ufile/httprequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,14 +323,45 @@
     try:
         response = requests.get(url, headers=header, params=param)
     except RequestException as e:
         return None, ResponseInfo(None, e)
     return __return_wraper(response)
 
 
+def _get_multi_upload_part(url, header):
+    """
+    UCloud UFile 获取分片上传列表信息请求
+
+    :param url: String类型，获取分片上传列表信息请求的url
+    :param header: dict类型，键值对类型分别为string类型，HTTP请求头信息
+    :return: ret: 如果http状态码不为[200, 204, 206]之一则返回None，否则如果服务器返回json信息则返回dict类型，键值对类型分别为string, unicode string类型，否则返回空的dict
+    :return:  ResponseInfo: 响应的具体信息，UCloud UFile 服务器返回信息或者网络链接异常
+    """
+    try:
+        response = requests.get(url, headers=header)
+    except RequestException as e:
+        return None, ResponseInfo(None, e)
+    return __return_wraper(response)
+
+
+def _op_meta(url, body, header):
+    """
+    UCloud UFile 文件元数据操作请求
+
+    :param url: String类型，文件元数据操作请求的url
+    :param body: dict类型，键值对类型分别为string类型，HTTP请求的body信息
+    :param header: dict类型，键值对类型分别为string类型，HTTP请求头信息
+    """
+    try:
+        response = requests.post(url, headers=header, data=body, timeout=config.get_default('connection_timeout'))
+    except RequestException as e:
+        return None, ResponseInfo(None, e)
+    return __return_wraper(response)
+
+
 class ResponseInfo(object):
     """
     UCloud UFile 服务器返回信息,解析UCloud UFile服务器返回信息以及网络连接问题
 
     Attributes:
         content: 服务器返回信息的二级制数据块，如果出现网络连接问题则为None
         status_code: Integer类型，服务器返回信息状态码，如果出现网络连接问题则为-1
@@ -362,22 +393,24 @@
             self.etag = None
             self.content_type = None
             self.content_length = None
             self.content_range = None
             self.ret_code = None
             self.content = None
             self.md5 = None
+            self.x_ufile_restore = None
         else:
             self.status_code = response.status_code
             self.x_session_id = response.headers.get('X-SessionId')
             self.content_type = response.headers.get('Content-Type')
             self.md5 = response.headers.get('Content-MD5')
             self.content_length = response.headers.get('Content-Length')
             content_length = response.headers.get('content-range')
             self.content = None if content_consumed else response.content
+            self.x_ufile_restore = response.headers.get('X-Ufile-restore')
             if content_length is not None:
                 byteslist = re.split('[- /]', content_length)
                 self.content_range = (int(byteslist[1]), int(byteslist[2]))
             else:
                 self.content_range = None
             self.etag = response.headers.get('Etag')
             if self.status_code not in [200, 204, 206]:
```

### Comparing `ufile-3.2.8/ufile/logger.py` & `ufile-3.2.9/ufile/logger.py`

 * *Files identical despite different names*

### Comparing `ufile-3.2.8/ufile/multipartuploadufile.py` & `ufile-3.2.9/ufile/multipartuploadufile.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import os
 import threading
 import time
 
 from . import config
 from .baseufile import BaseUFile
 from .compact import s
-from .httprequest import ResponseInfo, _initialsharding, _finishsharding, _shardingupload
+from .httprequest import ResponseInfo, _initialsharding, _finishsharding, _shardingupload, _get_multi_upload_part
 from .logger import logger
 from .util import _check_dict, initialsharding_url, finishsharding_url, shardingupload_url, _file_iter, \
-    mimetype_from_file, mimetype_from_buffer, deprecated
+    mimetype_from_file, mimetype_from_buffer, deprecated, ufile_listparts_url
 
 
 class MultipartUploadUFile(BaseUFile):
     """
     分片上传UFile类
 
     Attributes:
@@ -111,16 +111,17 @@
         for data in _file_iter(self.__stream, self.blocksize):
             sem.acquire()  # 控制最大并发线程数
             if self.__errresp:  # 如果有分片上传失败，停止后续分片上传
                 sem.release()
                 break
             self.etaglist.append("")
             thread1 = threading.Thread(target=self.__partthread, args=(
-            sem, self.__bucket, self.__key, self.uploadid, partnumber, self.__header, data, retrycount, retryinterval,
-            self.etaglist, self.__upload_suffix))
+                sem, self.__bucket, self.__key, self.uploadid, partnumber, self.__header, data, retrycount,
+                retryinterval,
+                self.etaglist, self.__upload_suffix))
             self.__threaddict[partnumber] = thread1
             thread1.start()
             partnumber += 1
 
         for thread in list(self.__threaddict.values()):  # 转为list是因为遍历字典时长度变化会报错
             thread.join()
 
@@ -393,14 +394,16 @@
         :param header: dict类型，HTTP请求头部
         :param upload_suffix: string类型, 如果传入此参数, 则会忽略 config 中配置的 upload_suffix 字段
         :return: (dict, ResponseInfo) tuple类型，dict为返回的json信息，ResponseInfo为请求的返回信息
         """
         self.__bucket = bucket
         self.__key = key
         self.__header = header if header else dict()
+        if 'User-Agent' not in self.__header:
+            self.__header['User-Agent'] = config.get_default('user_agent')
         self.__upload_suffix = upload_suffix if upload_suffix else config.get_default('upload_suffix')
         ret, resp = self.__initialsharding()
         if resp.ok:
             self.uploadid = ret.get('UploadId')
             self.blocksize = ret.get('BlkSize')
         return ret, resp
 
@@ -427,17 +430,40 @@
         :return:  ResponseInfo: 响应的具体信息，UCloud UFile 服务器返回信息或者网络链接异常
         """
         self.__mimetype = mime_type
         self.__upload_suffix = config.get_default("upload_suffix") if upload_suffix is None else upload_suffix
         self.__header.update({"X-Ufile-Copy-Source": "/%s/%s" % (source_bucket, source_key)})
         self.__header.update({"Content-Type": self.__mimetype})
         self.__header.update({"X-Ufile-Copy-Source-Range": "bytes=%d-%d" % (offset, size - 1)})
-
+        if 'User-Agent' not in self.__header:
+            self.__header['User-Agent'] = config.get_default('user_agent')
         authorization = self.authorization('put', self.__bucket, self.__key, self.__header)
         self.__header.update({"Authorization": authorization})
 
         url = shardingupload_url(self.__bucket, self.__key, self.uploadid, part_number,
                                  upload_suffix=self.__upload_suffix)
         ret, resp = _shardingupload(url, None, self.__header)
         if resp.ok:
             self.etaglist.append(resp.etag)
         return ret, resp
+
+    def get_multi_upload_part(self, bucket, upload_id, max_parts=None, part_number_marker=None, header=None, upload_suffix=None):
+        """
+        获取未完成分片上传的对象的已上传成功的分片列表。
+
+        :param bucket: string类型，空间名称
+        :param upload_id: string类型，初始化分片上传时返回的uploadid
+        :param max_parts: int类型，返回的最大条目数，默认为1000
+        :param part_number_marker: int类型，返回的起始条目，默认为0
+        :param header: dict类型，HTTP请求头部
+        :param upload_suffix: string类型, 如果传入此参数, 则会忽略 config 中配置的 upload_suffix 字段
+        :return: (dict, ResponseInfo) tuple类型，dict为返回的json信息，ResponseInfo为请求的返回信息
+        """
+        self.__header = header if header else dict()
+        if 'User-Agent' not in self.__header:
+            self.__header['User-Agent'] = config.get_default('user_agent')
+        if upload_suffix is not None:
+            self.__upload_suffix = upload_suffix
+        authorization = self.authorization('get', bucket, "", self.__header, action='muploadpart')
+        self.__header.update({"Authorization": authorization})
+        url = ufile_listparts_url(bucket, self.__upload_suffix, upload_id, max_parts, part_number_marker)
+        return _get_multi_upload_part(url, self.__header)
```

### Comparing `ufile-3.2.8/ufile/util.py` & `ufile-3.2.9/ufile/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # -*- coding: utf-8 -*-
 
-from .compact import *
-from . import config
-
 import base64
 import hashlib
+import mimetypes
 import os
 import struct
-
-import mimetypes
-from os import path
 import warnings
-from .config import BLOCKSIZE 
+from os import path
+
+from . import config
+from .compact import *
+from .config import BLOCKSIZE
 
 _EXTRA_TYPES_MAP = {
     ".js": "application/javascript",
     ".xlsx": "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
     ".xltx": "application/vnd.openxmlformats-officedocument.spreadsheetml.template",
     ".potx": "application/vnd.openxmlformats-officedocument.presentationml.template",
     ".ppsx": "application/vnd.openxmlformats-officedocument.presentationml.slideshow",
@@ -424,25 +423,29 @@
 
     :param bucket: string类型, 待创建的空间名称
     :param key:  string类型, 在空间中的文件名
     :param uploadid: string类型, 初始化分片上传获得的uploadid字符串
     :param part_number: integer类型, 分片上传的编号,从0开始
     :return: string类型, 结束分片上传UFile的url
     """
-    return 'http://{0}{1}/{2}?uploadId={3}&partNumber={4}'.format(bucket, upload_suffix or config.get_default('upload_suffix'), key, uploadid, s(str(part_number)))
+    return 'http://{0}{1}/{2}?uploadId={3}&partNumber={4}'.format(bucket,
+                                                                  upload_suffix or config.get_default('upload_suffix'),
+                                                                  key, uploadid, s(str(part_number)))
+
 
 def ufile_getfilelist_url(bucket, upload_suffix=None):
     """
     获取文件列表的url
 
     :param bucket: string 类型，获取的空间名称
     :return: string类型，获取文件列表的url
     """
     return 'http://{0}{1}/?list'.format(bucket, upload_suffix or config.get_default('upload_suffix'))
 
+
 def mimetype_from_file(file):
     """
     获取文件的mimetype
 
     :param bucket: string 类型，获取的文件名称
     :return: string类型，获取文件的mimetype
     """
@@ -450,76 +453,115 @@
     if ext in _EXTRA_TYPES_MAP:
         return _EXTRA_TYPES_MAP[ext]
     elif mimetypes.guess_type(file)[0] is not None:
         return mimetypes.guess_type(file)[0]
 
     return 'application/unknowntype'
 
+
 def mimetype_from_buffer(stream):
     """
     获取流对象的mimetype
 
     :param bucket: string 类型，获取的流对象名称
     :return: string类型，获取流对象的mimetype
     """
     return 'application/octet-stream'
 
+
 def ufile_restore_url(bucket, key, upload_suffix=None):
     """
     解冻冷存文件的url
 
     :param bucket: string类型, 待创建的空间名称
     :param key:  string类型, 在空间中的文件名
     :return: string类型, 解冻文件的url
     """
     return 'http://{0}{1}/{2}?restore'.format(bucket, upload_suffix or config.get_default('upload_suffix'), key)
 
+
 def ufile_classswitch_url(bucket, key, upload_suffix=None):
     """
     文件存储类型转换的url
 
     :param bucket: string类型, 待创建的空间名称
     :param key:  string类型, 在空间中的文件名
     :return: string类型, 类型转换的url
     """
     return 'http://{0}{1}/{2}'.format(bucket, upload_suffix or config.get_default('upload_suffix'), key)
 
+
 def ufile_copy_url(bucket, key, upload_suffix=None):
     """
     拷贝文件的url
 
     :param bucket: string类型, 待创建的空间名称
     :param key:  string类型, 在空间中的目标文件名
     :return: string类型, 拷贝文件的url
     """
     return 'http://{0}{1}/{2}'.format(bucket, upload_suffix or config.get_default('upload_suffix'), key)
 
+
 def ufile_rename_url(bucket, key, upload_suffix=None):
     """
     重命名文件的url
 
     :param bucket: string类型, 待创建的空间名称
     :param key:  string类型, 在空间中的源文件名
     :param newkey:  string类型, 在空间中的目标文件名
     :return: string类型, 重命名文件的url
     """
     return 'http://{0}{1}/{2}'.format(bucket, upload_suffix or config.get_default('upload_suffix'), key)
 
+
 def ufile_listobjects_url(bucket, upload_suffix=None):
     """
     获取目录文件列表的url
 
     :param bucket: string 类型，获取的空间名称
     :return: string类型，获取目录文件列表的url
     """
     return 'http://{0}{1}/?listobjects'.format(bucket, upload_suffix or config.get_default('upload_suffix'))
 
+
+def ufile_listparts_url(bucket, upload_suffix, upload_id, max_parts=None, part_number_marker=None):
+    """
+    获取未完成分片上传的对象的已上传成功的分片列表。
+
+    :param bucket: string类型, 空间名称
+    :param upload_suffix: string类型, 域名后缀
+    :param upload_id: string类型, 初始化分片上传获得的uploadid字符串
+    :param max_parts: integer类型, 规定在US3响应中的最大Part数目。
+    :param part_number_marker: integer类型, 指定List的起始位置，只有Part Number数目大于该参数的Part会被列出
+    """
+    url = 'http://{0}{1}/?muploadpart&uploadId={2}'.format(bucket, upload_suffix or config.get_default('upload_suffix'),
+                                                           upload_id)
+    if max_parts is not None:
+        url += '&max-parts={}'.format(max_parts)
+    if part_number_marker is not None:
+        url += '&part-number-marker={}'.format(part_number_marker)
+    return url
+
+
+def ufile_op_meta_url(bucket, key, upload_suffix=None):
+    """
+    文件元数据的url
+
+    :param bucket: string类型, 待创建的空间名称
+    :param key:  string类型, 在空间中的文件名
+    :return: string类型, 获取文件元数据的url
+    """
+    return 'http://{0}{1}/{2}?opmeta'.format(bucket, upload_suffix or config.get_default('upload_suffix'), key)
+
+
 def deprecated(message):
-  def deprecated_decorator(func):
-      def deprecated_func(*args, **kwargs):
-          warnings.warn("Call to deprecated function {} . -- {}".format(func.__name__, message),
-                        category=DeprecationWarning,
-                        stacklevel=2)
-          warnings.simplefilter('default', DeprecationWarning)
-          return func(*args, **kwargs)
-      return deprecated_func
-  return deprecated_decorator
+    def deprecated_decorator(func):
+        def deprecated_func(*args, **kwargs):
+            warnings.warn("Call to deprecated function {} . -- {}".format(func.__name__, message),
+                          category=DeprecationWarning,
+                          stacklevel=2)
+            warnings.simplefilter('default', DeprecationWarning)
+            return func(*args, **kwargs)
+
+        return deprecated_func
+
+    return deprecated_decorator
```

### Comparing `ufile-3.2.8/ufile.egg-info/PKG-INFO` & `ufile-3.2.9/ufile.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufile
-Version: 3.2.8
+Version: 3.2.9
 Summary: UCloud UFile Python SDK
 Home-page: https://github.com/ucloud/ufile-sdk-python
 Author-email: leo.li@ucloud.cn
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -16,8 +16,7 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
-Requires-Dist: requests
```

