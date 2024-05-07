# Comparing `tmp/cow_transfer-0.0.4.tar.gz` & `tmp/cow_transfer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cow_transfer-0.0.4.tar", last modified: Mon Nov 27 16:56:21 2023, max compression
+gzip compressed data, was "cow_transfer-0.0.5.tar", last modified: Tue May  7 14:52:36 2024, max compression
```

## Comparing `cow_transfer-0.0.4.tar` & `cow_transfer-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-11-27 16:56:21.460327 cow_transfer-0.0.4/
--rw-rw-rw-   0        0        0     2223 2023-11-27 16:56:21.460327 cow_transfer-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1695 2023-11-27 16:53:02.000000 cow_transfer-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-11-27 16:56:21.444707 cow_transfer-0.0.4/cow_transfer/
--rw-rw-rw-   0        0        0        0 2023-10-06 16:40:32.000000 cow_transfer-0.0.4/cow_transfer/__init__.py
--rw-rw-rw-   0        0        0     4502 2023-11-27 16:53:02.000000 cow_transfer-0.0.4/cow_transfer/cow_download.py
--rw-rw-rw-   0        0        0    17779 2023-10-06 16:40:32.000000 cow_transfer-0.0.4/cow_transfer/cow_upload.py
--rw-rw-rw-   0        0        0     2541 2023-11-27 16:53:02.000000 cow_transfer-0.0.4/cow_transfer/main.py
-drwxrwxrwx   0        0        0        0 2023-11-27 16:56:21.460327 cow_transfer-0.0.4/cow_transfer.egg-info/
--rw-rw-rw-   0        0        0     2223 2023-11-27 16:56:21.000000 cow_transfer-0.0.4/cow_transfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-11-27 16:56:21.000000 cow_transfer-0.0.4/cow_transfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-27 16:56:21.000000 cow_transfer-0.0.4/cow_transfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-11-27 16:56:21.000000 cow_transfer-0.0.4/cow_transfer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-11-27 16:56:21.000000 cow_transfer-0.0.4/cow_transfer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-11-27 16:56:21.000000 cow_transfer-0.0.4/cow_transfer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-27 16:56:21.460327 cow_transfer-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      954 2023-11-27 16:18:55.000000 cow_transfer-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:52:36.060862 cow_transfer-0.0.5/
+-rw-rw-rw-   0        0        0     2175 2024-05-07 14:52:36.060862 cow_transfer-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1647 2024-05-06 17:44:19.000000 cow_transfer-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 14:52:36.045460 cow_transfer-0.0.5/cow_transfer/
+-rw-rw-rw-   0        0        0        0 2023-10-06 16:40:32.000000 cow_transfer-0.0.5/cow_transfer/__init__.py
+-rw-rw-rw-   0        0        0     4715 2024-05-06 17:44:19.000000 cow_transfer-0.0.5/cow_transfer/cow_download.py
+-rw-rw-rw-   0        0        0    17557 2024-05-06 18:00:33.000000 cow_transfer-0.0.5/cow_transfer/cow_upload.py
+-rw-rw-rw-   0        0        0     2845 2024-05-06 18:02:50.000000 cow_transfer-0.0.5/cow_transfer/main.py
+-rw-rw-rw-   0        0        0      407 2024-05-06 17:44:19.000000 cow_transfer-0.0.5/cow_transfer/util.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:52:36.060862 cow_transfer-0.0.5/cow_transfer.egg-info/
+-rw-rw-rw-   0        0        0     2175 2024-05-07 14:52:35.000000 cow_transfer-0.0.5/cow_transfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2024-05-07 14:52:35.000000 cow_transfer-0.0.5/cow_transfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:52:35.000000 cow_transfer-0.0.5/cow_transfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-07 14:52:35.000000 cow_transfer-0.0.5/cow_transfer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-05-07 14:52:35.000000 cow_transfer-0.0.5/cow_transfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-07 14:52:35.000000 cow_transfer-0.0.5/cow_transfer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 14:52:36.060862 cow_transfer-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      954 2024-05-06 17:17:28.000000 cow_transfer-0.0.5/setup.py
```

### Comparing `cow_transfer-0.0.4/PKG-INFO` & `cow_transfer-0.0.5/cow_transfer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cow_transfer
-Version: 0.0.4
+Name: cow-transfer
+Version: 0.0.5
 Summary: Easily downlaod file from CowTransfer
 Home-page: https://github.com/xiyoucloud/cow_transfer.git
 Author: txb
 Author-email: txb.sdn@gmail.com
 License: MIT
 Keywords: python,DownloadKit,cow_transfer
 Platform: UNKNOWN
@@ -31,27 +31,26 @@
 ```
 Usage: cow download [OPTIONS]
 
 Options:
   -u, --urlcode TEXT     urlcode for download file  [required]       
   -t, --threads INTEGER  set threads for download file  [default: 20]
   -p, --path PATH        set save path for download file
-  -c, --cookie_path PATH cookie file path
+  -h, --header_file_path PATH header file path
   --help                 Show this message and exit.
 ```
 
 ### 文件上传
 ```
 Usage: cow upload [OPTIONS]
 
   CowTransfer - 奶牛快传
 
 Options:
-  --authorization TEXT  用户 authorization  [required]
-  --remember_mev2 TEXT  用户 remember-mev2  [required]
+  --header_file_path PATH header file path
   --upload_path TEXT    待上传文件或目录路径  [required]
   --folder_name TEXT    文件夹名称
   --title TEXT          传输标题
   --message TEXT        传输描述
   --valid_days INTEGER  传输有效期（天）  [default: 7]
   --chunk_size INTEGER  分块大小（字节）  [default: 2097152]
   --threads INTEGER     上传并发数  [default: 5]
@@ -60,14 +59,15 @@
 
 默认情况下会开启 20 个线程对文件进行下载，这会大大加快下载速度，不过下载速度还受到网络带宽的限制，即下载速度最快不会超过网络带宽。
 
 ## 打包源码
 ```
 # 安装依赖
 pip install wheel
+pip install twine
 # 打包
 python setup.py bdist_wheel sdist
 
 # 上传打包后的 python 包到 https://pypi.org
 twine upload dist/*
 ```
```

### Comparing `cow_transfer-0.0.4/README.md` & `cow_transfer-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,27 +15,26 @@
 ```
 Usage: cow download [OPTIONS]
 
 Options:
   -u, --urlcode TEXT     urlcode for download file  [required]       
   -t, --threads INTEGER  set threads for download file  [default: 20]
   -p, --path PATH        set save path for download file
-  -c, --cookie_path PATH cookie file path
+  -h, --header_file_path PATH header file path
   --help                 Show this message and exit.
 ```
 
 ### 文件上传
 ```
 Usage: cow upload [OPTIONS]
 
   CowTransfer - 奶牛快传
 
 Options:
-  --authorization TEXT  用户 authorization  [required]
-  --remember_mev2 TEXT  用户 remember-mev2  [required]
+  --header_file_path PATH header file path
   --upload_path TEXT    待上传文件或目录路径  [required]
   --folder_name TEXT    文件夹名称
   --title TEXT          传输标题
   --message TEXT        传输描述
   --valid_days INTEGER  传输有效期（天）  [default: 7]
   --chunk_size INTEGER  分块大小（字节）  [default: 2097152]
   --threads INTEGER     上传并发数  [default: 5]
@@ -44,13 +43,14 @@
 
 默认情况下会开启 20 个线程对文件进行下载，这会大大加快下载速度，不过下载速度还受到网络带宽的限制，即下载速度最快不会超过网络带宽。
 
 ## 打包源码
 ```
 # 安装依赖
 pip install wheel
+pip install twine
 # 打包
 python setup.py bdist_wheel sdist
 
 # 上传打包后的 python 包到 https://pypi.org
 twine upload dist/*
 ```
```

### Comparing `cow_transfer-0.0.4/cow_transfer/cow_download.py` & `cow_transfer-0.0.5/cow_transfer/cow_download.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from DownloadKit import DownloadKit
 import os
 import sys
 import requests
 
+from cow_transfer.util import get_str_arr_split_by_new_line_from_file, build_request_header
+
 dirname = os.path.dirname(__file__)
 # 创建下载器对象
 d = DownloadKit(roads=20)
 # 线程数
 # 大文件分块大小，默认 20MB
 d.block_size = '50M'
 # 设置文件保存路径
@@ -70,22 +72,21 @@
     rate = float(num) / total
     rate_num = int(100 * rate)
     r = '\r[{}{}]{}%'.format('*' * rate_num, ' ' * (100 - rate_num), rate_num)
     sys.stdout.write(r)
     sys.stdout.flush()
 
 
-def download_file(unique_url, target=None, threads=20, cookie_file_path=None):
-    if cookie_file_path is None:
-        cookie_file_path = './cookie'
-    cookie = get_str_from_file(cookie_file_path)
+def download_file(unique_url, target=None, threads=20, header_file_path=None):
+    if header_file_path is None:
+        header_file_path = './header.txt'
+    if not os.path.exists(header_file_path):
+        raise SyntaxError("请添加header.txt文件")
     global common_header
-    common_header = {
-        'cookie': cookie
-    }
+    common_header = build_request_header(get_str_arr_split_by_new_line_from_file(header_file_path))
     get_permission_info(unique_url)
     file_details = get_file_details(unique_url)
     download_url = get_download_url(file_details)
     if target is None:
         target = dirname
     else:
         if os.path.exists(target) and os.path.isdir(target):
@@ -113,22 +114,22 @@
     arg_len = len(sys.argv)
     if arg_len <= 1:
         raise SyntaxError("不合法的参数，help显示帮助，download下载文件")
     command = sys.argv[1]
     if command == 'download':
         unique_url = None
         save_target = None
-        cookie_file_path = None
+        header_file_path = None
         if arg_len == 4:
             unique_url = sys.argv[2]
-            cookie_file_path = sys.argv[3]
+            header_file_path = sys.argv[3]
         elif arg_len == 5:
             unique_url = sys.argv[2]
             save_target = sys.argv[3]
-            cookie_file_path = sys.argv[4]
+            header_file_path = sys.argv[4]
         else:
             raise SyntaxError("不合法的参数个数")
-        download_file(unique_url, save_target, cookie_file_path)
+        download_file(unique_url, save_target, header_file_path=header_file_path)
     elif command == 'help':
         show_help()
     else:
         raise SyntaxError("不合法的命令")
```

### Comparing `cow_transfer-0.0.4/cow_transfer/cow_upload.py` & `cow_transfer-0.0.5/cow_transfer/cow_upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 import time
 import requests
 import threading
 from tqdm import tqdm
 from oss2.models import PartInfo
 from concurrent.futures import ThreadPoolExecutor
 
+from cow_transfer.util import build_request_header, get_str_arr_split_by_new_line_from_file
+
 requests.adapters.DEFAULT_RETRIES = 3
 
 debug = False
 
 
 def log(text: str) -> str:
     if debug:
         print(text)
     return text
 
 
 class CowUploader(threading.Thread):
 
     def __init__(self,
-                 authorization: str,
-                 remember_mev2: str,
+                 header_file_path: str,
                  upload_path: str,
                  folder_name: str = "",
                  title: str = "",
                  message: str = "",
                  valid_days: int = 7,
                  chunk_size: int = 2097152,
                  threads: int = 5):
@@ -41,16 +42,15 @@
         :param valid_days: 传输有效期（单位：天数，默认 7 天）
         :param chunk_size: 分块大小（单位：字节，默认 2097152 字节，即 2 MB）
         :param threads: 上传线程数（默认 5）
         """
         super(CowUploader, self).__init__()
 
         # 参数
-        self.authorization = authorization
-        self.remember_mev2 = remember_mev2
+        self.header_file_path = header_file_path
         self.upload_path = upload_path
         self.folder_name = folder_name
         self.title = title
         self.message = message
         self.valid_days = valid_days
         self.chunk_size = chunk_size
         self.threads = threads
@@ -59,19 +59,15 @@
         self.err = ""
         self.status = "work"
         self.file_dict = {}
         self.upload_info = {
             "complete": False
         }
         self.transfer_info = {}
-        self.auth_headers = {
-            "cookie": f"{self.remember_mev2}; cow-auth-token={self.authorization}",
-            "authorization": self.authorization,
-            "Connection": "close"
-        }
+        self.auth_headers = build_request_header(get_str_arr_split_by_new_line_from_file(header_file_path))
 
         # 对象
         self.executor = None
         self.progress_bar_curr = None
         self.progress_bar_total = None
 
     # 执行
@@ -133,19 +129,14 @@
             if not self.action():
                 return False
         return True
 
     def check(self) -> bool:
         """检查"""
 
-        # 缺少 remember_mev2 或 authorization
-        if not all([self.remember_mev2, self.authorization]):
-            self.err = "错误：缺少 remember_mev2 或 authorization"
-            return False
-
         # 待上传文件或目录
         if not os.path.exists(self.upload_path):
             self.err = "错误：待上传文件或目录不存在"
             return False
 
         return True
 
@@ -176,15 +167,16 @@
                 "enablePreview": True,  # 允许预览
                 "enableSaveTo": True  # 允许转存
             }
             req_resp = requests.post(url=req_url, headers=self.auth_headers, json=req_json)
             resp_json = req_resp.json()
             if "code" in resp_json and resp_json["code"] == "0000":
                 self.transfer_info.update(resp_json["data"])
-                self.upload_info["transfer_url"] = self.upload_info["url_prefix"] + resp_json["data"]["uniqueUrl"]  # 传输链接
+                self.upload_info["transfer_url"] = self.upload_info["url_prefix"] + resp_json["data"][
+                    "uniqueUrl"]  # 传输链接
                 self.upload_info["transfer_code"] = resp_json["data"]["downloadCode"]  # 传输取件码
                 return True
             else:
                 self.err = f"返回：{resp_json}"
         except Exception as exc:
             self.err = f"异常：{exc}"
             return False
@@ -199,15 +191,16 @@
 
         # 判断上传目标类型
         if os.path.isfile(self.upload_path):
             # 单文件
             self.upload_info["mode"] = "single"
             self.file_dict["1"] = {
                 "file_name": os.path.basename(self.upload_path),
-                "file_format": os.path.basename(self.upload_path).split(".")[-1] if "." in os.path.basename(self.upload_path) else "unknow",
+                "file_format": os.path.basename(self.upload_path).split(".")[-1] if "." in os.path.basename(
+                    self.upload_path) else "unknow",
                 "rel_path": "\\" + os.path.basename(self.upload_path),
                 "abs_path": os.path.abspath(self.upload_path),
                 "file_size": os.path.getsize(self.upload_path),
                 "folder_id": "0",
                 "uploaded": False,
                 "uploaded_size": 0
             }
@@ -219,15 +212,16 @@
 
             # 遍历获取所有待上传文件信息
             root_path = os.path.abspath(self.upload_path)
             for root, dirs, files in os.walk(self.upload_path):
                 for file in files:
                     self.file_dict[str(len(self.file_dict) + 1)] = {
                         "file_name": os.path.basename(file),
-                        "file_format": os.path.basename(file).split(".")[-1] if "." in os.path.basename(file) else "unknow",
+                        "file_format": os.path.basename(file).split(".")[-1] if "." in os.path.basename(
+                            file) else "unknow",
                         "rel_path": os.path.abspath(os.path.join(root, file)).replace(root_path, ""),
                         "abs_path": os.path.abspath(os.path.join(root, file)),
                         "file_size": os.path.getsize(os.path.join(root, file)),
                         "folder_id": "0",
                         "uploaded": False,
                         "uploaded_size": 0
                     }
```

### Comparing `cow_transfer-0.0.4/cow_transfer/main.py` & `cow_transfer-0.0.5/cow_transfer/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,31 +8,37 @@
 import argparse
 import click
 
 
 @click.group()
 def cli():
     """upload and download - v0.1.5"""
-    pass
 
 
 @cli.command()
-@click.option("--authorization", type=str, prompt="用户 authorization", help="用户 authorization", required=True)
-@click.option("--remember_mev2", type=str, prompt="用户 remember-mev2", help="用户 remember-mev2", required=True)
+@click.option("-h", "--header_file_path", type=click.Path(exists=True), help="header file path",
+              default="./header.txt")
 @click.option("--upload_path", type=str, prompt="待上传文件或目录路径", help="待上传文件或目录路径", required=True)
 @click.option("--folder_name", type=str, help="文件夹名称", default="")
 @click.option("--title", type=str, help="传输标题", default="")
 @click.option("--message", type=str, help="传输描述", default="")
 @click.option("--valid_days", type=int, help="传输有效期（天）", default=7, show_default=True)
 @click.option("--chunk_size", type=int, help="分块大小（字节）", default=2097152, show_default=True)
 @click.option("--threads", type=int, help="上传并发数", default=5, show_default=True)
-def upload(authorization, remember_mev2, upload_path, folder_name, title, message, valid_days, chunk_size, threads):
+def upload(header_file_path, upload_path, folder_name, title, message, valid_days,
+           chunk_size, threads):
     """CowTransfer - 奶牛快传"""
-    # 如果传入特殊字符，就获取 xiyouyun 的 author 和 remember
-    thread = CowUploader(authorization, remember_mev2, upload_path, folder_name,
+    upload_file(header_file_path, upload_path, folder_name, title, message, valid_days,
+                chunk_size, threads)
+
+
+def upload_file(header_file_path, upload_path, folder_name, title, message, valid_days,
+                chunk_size, threads):
+    # TODO 如果传入特殊字符，就获取 xiyou 的 author 和 remember
+    thread = CowUploader(header_file_path, upload_path, folder_name,
                          title, message, valid_days, chunk_size, threads)
     if thread.start_upload():
         click.echo(f"链接：{thread.upload_info.get('transfer_url')}\n"
                    f"口令：{thread.upload_info.get('transfer_code')}")
     else:
         click.echo(f"上传失败，{thread.err}")
     return thread
@@ -42,15 +48,17 @@
 # 列表，必须
 @click.option('-u', '--urlcode', help="urlcode for download file", required=True)
 # int，可选，默认值
 @click.option("-t", "--threads", default=20, help="set threads for download file", show_default=True)
 # 可选，默认值
 @click.option("-p", "--path", type=click.Path(exists=True), help="set save path for download file", default=".")
 # 可选，默认值
-@click.option("-c", "--cookie_path", type=click.Path(exists=True), help="cookie file path",
-              default="./cookie")
-def download(urlcode, threads, path, cookie_path):
-    download_file(urlcode, target=path, threads=threads, cookie_file_path=cookie_path)
+@click.option("-h", "--header_file_path", type=click.Path(exists=True), help="header file path",
+              default="./header.txt")
+def download(urlcode, threads, path, header_file_path):
+    download_file(urlcode, target=path, threads=threads, header_file_path=header_file_path)
 
 
 if __name__ == "__main__":
+    # download_file('bdae5a8fc3444b', ".", 20, "./header.txt")
+    # upload_file("./header.txt", "./DSCF0001123.jpg", "", "", "", 1, 2097152, 5)
     cli()
```

### Comparing `cow_transfer-0.0.4/cow_transfer.egg-info/PKG-INFO` & `cow_transfer-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cow-transfer
-Version: 0.0.4
+Name: cow_transfer
+Version: 0.0.5
 Summary: Easily downlaod file from CowTransfer
 Home-page: https://github.com/xiyoucloud/cow_transfer.git
 Author: txb
 Author-email: txb.sdn@gmail.com
 License: MIT
 Keywords: python,DownloadKit,cow_transfer
 Platform: UNKNOWN
@@ -31,27 +31,26 @@
 ```
 Usage: cow download [OPTIONS]
 
 Options:
   -u, --urlcode TEXT     urlcode for download file  [required]       
   -t, --threads INTEGER  set threads for download file  [default: 20]
   -p, --path PATH        set save path for download file
-  -c, --cookie_path PATH cookie file path
+  -h, --header_file_path PATH header file path
   --help                 Show this message and exit.
 ```
 
 ### 文件上传
 ```
 Usage: cow upload [OPTIONS]
 
   CowTransfer - 奶牛快传
 
 Options:
-  --authorization TEXT  用户 authorization  [required]
-  --remember_mev2 TEXT  用户 remember-mev2  [required]
+  --header_file_path PATH header file path
   --upload_path TEXT    待上传文件或目录路径  [required]
   --folder_name TEXT    文件夹名称
   --title TEXT          传输标题
   --message TEXT        传输描述
   --valid_days INTEGER  传输有效期（天）  [default: 7]
   --chunk_size INTEGER  分块大小（字节）  [default: 2097152]
   --threads INTEGER     上传并发数  [default: 5]
@@ -60,14 +59,15 @@
 
 默认情况下会开启 20 个线程对文件进行下载，这会大大加快下载速度，不过下载速度还受到网络带宽的限制，即下载速度最快不会超过网络带宽。
 
 ## 打包源码
 ```
 # 安装依赖
 pip install wheel
+pip install twine
 # 打包
 python setup.py bdist_wheel sdist
 
 # 上传打包后的 python 包到 https://pypi.org
 twine upload dist/*
 ```
```

