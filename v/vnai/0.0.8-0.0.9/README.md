# Comparing `tmp/vnai-0.0.8.tar.gz` & `tmp/vnai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnai-0.0.8.tar", last modified: Mon May  6 17:41:47 2024, max compression
+gzip compressed data, was "vnai-0.0.9.tar", last modified: Tue May  7 13:05:00 2024, max compression
```

## Comparing `vnai-0.0.8.tar` & `vnai-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 17:41:47.198375 vnai-0.0.8/
--rw-r--r--   0 mrthinh    (501) staff       (20)      573 2024-05-06 17:41:47.198274 vnai-0.0.8/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)      140 2024-05-06 15:49:50.000000 vnai-0.0.8/pyproject.toml
--rw-r--r--   0 mrthinh    (501) staff       (20)      568 2024-05-06 17:41:47.198666 vnai-0.0.8/setup.cfg
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 17:41:47.196383 vnai-0.0.8/vnai/
--rw-r--r--   0 mrthinh    (501) staff       (20)    16992 2024-05-06 17:40:52.000000 vnai-0.0.8/vnai/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-06 17:41:47.197717 vnai-0.0.8/vnai.egg-info/
--rw-r--r--   0 mrthinh    (501) staff       (20)      573 2024-05-06 17:41:47.000000 vnai-0.0.8/vnai.egg-info/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)      180 2024-05-06 17:41:47.000000 vnai-0.0.8/vnai.egg-info/SOURCES.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-05-06 17:41:47.000000 vnai-0.0.8/vnai.egg-info/dependency_links.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)       47 2024-05-06 17:41:47.000000 vnai-0.0.8/vnai.egg-info/requires.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)        5 2024-05-06 17:41:47.000000 vnai-0.0.8/vnai.egg-info/top_level.txt
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-07 13:05:00.385245 vnai-0.0.9/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      573 2024-05-07 13:05:00.385183 vnai-0.0.9/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)      140 2024-05-06 15:49:50.000000 vnai-0.0.9/pyproject.toml
+-rw-r--r--   0 mrthinh    (501) staff       (20)      568 2024-05-07 13:05:00.385498 vnai-0.0.9/setup.cfg
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-07 13:05:00.383847 vnai-0.0.9/vnai/
+-rw-r--r--   0 mrthinh    (501) staff       (20)    17531 2024-05-07 13:01:44.000000 vnai-0.0.9/vnai/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-07 13:05:00.384877 vnai-0.0.9/vnai.egg-info/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      573 2024-05-07 13:05:00.000000 vnai-0.0.9/vnai.egg-info/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)      180 2024-05-07 13:05:00.000000 vnai-0.0.9/vnai.egg-info/SOURCES.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-05-07 13:05:00.000000 vnai-0.0.9/vnai.egg-info/dependency_links.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)       47 2024-05-07 13:05:00.000000 vnai-0.0.9/vnai.egg-info/requires.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)        5 2024-05-07 13:05:00.000000 vnai-0.0.9/vnai.egg-info/top_level.txt
```

### Comparing `vnai-0.0.8/PKG-INFO` & `vnai-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnai
-Version: 0.0.8
+Version: 0.0.9
 Author: Vnstock HQ
 Author-email: support@vnstock.site
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vnai-0.0.8/setup.cfg` & `vnai-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnai
-version = 0.0.8
+version = 0.0.9
 author = Vnstock HQ
 author_email = support@vnstock.site
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
```

### Comparing `vnai-0.0.8/vnai/__init__.py` & `vnai-0.0.9/vnai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,47 +16,47 @@
 
 HOME_DIR = pathlib.Path.home()
 PROJECT_DIR = HOME_DIR / ".vnstock"
 ID_DIR = PROJECT_DIR / 'id'
 TG = b'gAAAAABmOPXPmFYXs94INEralMxhR38geFp91TZRLP29C41OoO0k7D7QiXIR2nWl5PCEoQCKECZw8b-Xeek3oqT6LcpcpJsAPyOGOBTX5cw_r5Mv0o8SBLa53jOeuVAwCAhId_BpMtOO'
 TC_PATH = ID_DIR / "terms_agreement.txt"
 
-class VnstockInitializer:
-    def __init__(self, target):
-        self.TERMS_AND_CONDITIONS = """
+TERMS_AND_CONDITIONS = """
         Vui lòng nhập 'Tôi đồng ý' hoặc nhấn Enter để chấp nhận các điều khoản, điều kiện và tiếp tục sử dụng phần mềm. 
 
         Bạn cũng có thể tự động chấp nhận điều khoản và ẩn thông báo này với câu lệnh mẫu bên dưới:
+
         ```
         import os
         if "ACCEPT_TC" not in os.environ:
         os.environ["ACCEPT_TC"] = "tôi đồng ý"
         ```
 
         THOẢ THUẬN & GIẤY PHÉP SỬ DỤNG PHẦN MỀM VNSTOCK3
         ------------------------------------------------
 
         (*) Gói thư viện Python Vnstock thế hệ thứ 3 được phát hành vào tháng 5 năm 2024, được đề cập đến trong giấy phép này với tên gọi tắt là Vnstock3.
 
-        Khi bạn truy cập, sử dụng nội dung mã nguồn Vnstock3, hoặc cài đặt Vnstock3 trên thiết bị của mình, bạn xác nhận rằng mình đã đọc, hiểu rõ, và chấp nhận điều khoản sử dụng phần mềm như mô tả dưới đây. Bạn cần xác nhận điều khoản & điều kiện trong lần đầu tiên chạy thư viện Vnstock để có thể sử dụng.
+        Khi bạn truy cập, sử dụng nội dung mã nguồn Vnstock3, hoặc cài đặt Vnstock3 trên thiết bị của mình, bạn xác nhận rằng mình đã đọc, hiểu rõ, và chấp nhận điều khoản sử dụng phần mềm như mô tả dưới đây. 
+        Bạn cần xác nhận điều khoản & điều kiện trong lần đầu tiên chạy thư viện Vnstock để có thể sử dụng.
 
         I. ĐIỀU KHOẢN CHUNG
         -------------------
 
-        Cấp Phép: Thư viện này chỉ dành cho mục đích cá nhân và không được phân phối lại hoặc sử dụng cho mục đích thương mại mà không có sự đồng ý bằng văn bản chính thức từ tác giả. Tất cả bản quyền và sở hữu trí tuệ thuộc về tác giả. Bất kỳ hành vi vi phạm bản quyền hoặc sở hữu trí tuệ sẽ bị xử lý theo pháp luật.
+        Cấp Phép: Thư viện này chỉ dành cho mục đích cá nhân và không được phân phối lại hoặc sử dụng cho mục đích thương mại mà không có sự đồng ý bằng văn bản chính thức từ tác giả. Tất cả bản quyền và sở hữu trí tuệ thuộc về tác giả. Bất kỳ hành vi vi phạm bản quyền hoặc sở hữu trí tuệ sẽ chịu trách nhiệm trước pháp luật.
 
-        Hạn Chế Sử Dụng Thương Mại: Sử dụng Vnstock3 cho mục đích thương mại bởi bất kỳ tổ chức nào là không được phép. Điều này bao gồm, nhưng không giới hạn, các hoạt động mà Vnstock3 trực tiếp hoặc gián tiếp góp phần tạo ra doanh thu hoặc dòng tiền cho một tổ chức mà không có sự chấp thuận bằng văn bản từ tác giả. Tuy nhiên, việc sử dụng Vnstock3 cho mục đích cá nhân, nghiên cứu vẫn được duy trì miễn phí.
+        Hạn Chế Sử Dụng Thương Mại: Sử dụng Vnstock3 cho mục đích thương mại bởi bất kỳ tổ chức nào là không được phép nếu không có sự đồng ý bằng văn bản của tác giả. Điều này bao gồm, nhưng không giới hạn, các hoạt động mà Vnstock3 trực tiếp hoặc gián tiếp góp phần tạo ra doanh thu hoặc dòng tiền cho một tổ chức mà không có sự chấp thuận từ tác giả. Tuy nhiên, việc sử dụng Vnstock3 cho mục đích cá nhân, nghiên cứu vẫn được duy trì miễn phí với điều kiện bạn phải tuân thủ việc công khai trích dẫn thông tin dự án trong sản phẩm của mình. Trong trường hợp tổ chức của bạn cần sử dụng Vnstock3 cho mục đích thương mại, vui lòng liên hệ với tác giả để được hỗ trợ và cấp phép sử dụng chính thức.
 
         Các Mục Đích Sử Dụng Bị Cấm: Bạn không được sử dụng Vnstock cho các mục đích bất hợp pháp, phi đạo đức, hoặc trái với quy định pháp luật hiện hành.
 
         Từ Chối Trách Nhiệm: Tác giả không chịu trách nhiệm cho bất kỳ thiệt hại, mất mát, hoặc hậu quả nào phát sinh từ việc sử dụng thư viện này, đặc biệt trong hoạt động đầu tư hoặc bất kỳ hoạt động nào có rủi ro. Bạn tự chịu trách nhiệm cho các quyết định đầu tư của mình.
 
         Tuân Thủ Luật Pháp: Bạn đồng ý tuân thủ mọi luật pháp, quy định, và hướng dẫn liên quan khi sử dụng thư viện này.
 
-        Bảo Mật Dữ Liệu: Vnstock có thể lưu trữ dữ liệu ẩn danh của thiết bị để tối ưu tính năng và cải thiện hiệu năng phần mềm. Thông tin này sẽ được bảo mật và không được chia sẻ với bên thứ ba mà không có sự đồng ý của bạn.
+        Bảo Mật Dữ Liệu: Bạn đồng ý cho phép Vnstock3 thu thập và lưu trữ dữ liệu ẩn danh của thiết bị nhằm mục đích phân tích và tối ưu hiệu năng, trải nghiệm sử dụng của phần mềm. Thông tin này được bảo mật và sẽ không được chia sẻ với bên thứ ba mà không có sự đồng ý của bạn.
 
         II. BẢN QUYỀN VÀ SỞ HỮU
         -----------------------
 
         Bản quyền (c) 2024 Thinh Vu @ Vnstock. Tất cả các quyền được bảo lưu.
 
         Sử Dụng và Phân Phối Không Được Phép: Việc sao chép, phân phối, hoặc khai thác thương mại Vnstock3, hoặc bất kỳ phần nào của nó là không được phép. Giới hạn này bao gồm bất kỳ hình thức tạo ra doanh thu hoặc sử dụng cho tổ chức mà không được sự cho phép rõ ràng của tác giả. Tuy nhiên, việc sử dụng cá nhân, chỉnh sửa, và nghiên cứu học thuật không liên quan đến lợi ích thương mại vẫn được duy trì. Người dùng tham gia vào các hoạt động được cho phép nên tôn trọng mục đích của phần mềm này như một công cụ cho việc thúc đẩy phát triển cá nhân và mục đích giáo dục, chứ không phải để lợi dụng tính chất mở của phần mềm cho mục đích sinh lợi trong khi tổ chức vốn có nguồn tiềm lực về tài chính và con người nhưng không chia sẻ với tác giả và đội ngũ phát triển. Vi phạm các điều khoản này tương đương với việc đánh cắp quyền sở hữu trí tuệ và phi đạo đức, có thể dẫn đến các rắc rối pháp lý kèm theo.
@@ -67,17 +67,21 @@
         Thỏa thuận này có hiệu lực cho đến khi được chấm dứt. Nó sẽ tự động chấm dứt ngay lập tức mà không cần thông báo từ tác giả nếu bạn không tuân thủ bất kỳ điều khoản nào của thỏa thuận này. Sau khi chấm dứt, bạn phải hủy bỏ tất cả các bản sao của Vnstock3 và tất cả các bộ phận thành phần của nó.
 
         IV. ĐIỀU KHOẢN THI HÀNH
         -----------------------
 
         Thỏa thuận này sẽ được điều chỉnh và giải thích theo luật pháp của quốc gia mà tác giả cư trú, không kể đến các quy định xung đột của pháp luật.
 
-        Bằng cách sử dụng Vnstock3, bạn đồng ý rằng mình sẽ bị ràng buộc bởi các điều khoản của Thỏa thuận này. Nếu bạn không đồng ý với các điều khoản của Thỏa thuận này, vui lòng không cài đặt hoặc sử dụng Vnstock3.
+        Bằng cách sử dụng Vnstock3, bạn đồng ý rằng mình sẽ bị ràng buộc bởi các điều khoản của Thỏa thuận này. 
+        Nếu bạn không đồng ý với các điều khoản của Thỏa thuận này, vui lòng không cài đặt hoặc sử dụng Vnstock3.
         """
 
+class VnstockInitializer:
+    def __init__(self, target, tc=TERMS_AND_CONDITIONS):
+        self.terms_and_conditions = tc
         self.home_dir = HOME_DIR
         self.project_dir = PROJECT_DIR
         self.id_dir = ID_DIR
         self.terms_file_path = TC_PATH
         self.RH = 'asejruyy^&%$#W2vX>NfwrevDRESWR'
         self.LH = 'YMAnhuytr%$59u90y7j-mjhgvyFTfbiuUYH'
 
@@ -167,15 +171,15 @@
 
         return info
 
     def show_terms_and_conditions(self):
         """
         Displays terms and conditions and asks for acceptance.
         """
-        print(self.TERMS_AND_CONDITIONS)
+        print(self.terms_and_conditions)
         
         # check if os.environ[TC_VAR] exist and equal to tôi đồng ý
         if TC_VAR in os.environ and os.environ[TC_VAR] == TC_VAL:
             response = TC_VAL
         else:
             response = input("Nhập 'Tôi đồng ý' hoặc nhấn Enter để chấp nhận: ")
             if not response.strip():
@@ -189,18 +193,19 @@
             HARDWARE = self.system_info()
             # VERSION = pkg_resources.get_distribution('vnstock').version
             
             VERSION = None
             try:
                 VERSION = importlib.metadata.version('vnstock')
             except importlib.metadata.PackageNotFoundError:
-                print("Package 'vnstock' not found")
+                # print("Package 'vnstock' not found")
+                pass
 
             # parse HARDWARE to string to store in the file
-            signed_aggreement = f"PHIÊN BẢN: {VERSION}\nMÔ TẢ:\nNgười dùng có mã nhận dạng {HARDWARE['uuid']} đã chấp nhận điều khoản & điều kiện sử dụng Vnstock lúc {now}\n---\n\nTHÔNG TIN THIẾT BỊ: {str(HARDWARE)}\n\nĐính kèm bản sao nội dung bạn đã đọc, hiểu rõ và đồng ý dưới đây:\n{self.TERMS_AND_CONDITIONS}"
+            signed_aggreement = f"MÔ TẢ:\nNgười dùng có mã nhận dạng {HARDWARE['uuid']} đã chấp nhận điều khoản & điều kiện sử dụng Vnstock lúc {now}\n---\n\nTHÔNG TIN THIẾT BỊ: {str(HARDWARE)}\n\nĐính kèm bản sao nội dung bạn đã đọc, hiểu rõ và đồng ý dưới đây:\n{self.terms_and_conditions}"
             
             # Store the acceptance
             with open(self.terms_file_path, "w", encoding="utf-8") as f:
                 f.write(signed_aggreement)
 
             print("---\nCảm ơn bạn đã chấp nhận điều khoản và điều kiện!\nBạn đã có thể tiếp tục sử dụng Vnstock!")
             return True
```

### Comparing `vnai-0.0.8/vnai.egg-info/PKG-INFO` & `vnai-0.0.9/vnai.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnai
-Version: 0.0.8
+Version: 0.0.9
 Author: Vnstock HQ
 Author-email: support@vnstock.site
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

