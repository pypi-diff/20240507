# Comparing `tmp/kjutils-1.6-py3-none-any.whl.zip` & `tmp/kjutils-1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5802 bytes, number of entries: 7
+Zip file size: 6422 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx     9677 b- defN 23-Sep-01 03:34 kjutils/PriceStock.py
 -rw-rw-r--  2.0 unx      111 b- defN 23-Aug-16 01:35 kjutils/__init__.py
--rw-rw-r--  2.0 unx     6192 b- defN 23-Aug-28 07:57 kjutils/kjutils.py
--rw-rw-r--  2.0 unx      234 b- defN 23-Sep-01 03:38 kjutils-1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Sep-01 03:38 kjutils-1.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Sep-01 03:38 kjutils-1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      516 b- defN 23-Sep-01 03:38 kjutils-1.6.dist-info/RECORD
-7 files, 16830 bytes uncompressed, 4892 bytes compressed:  70.9%
+-rw-rw-r--  2.0 unx     8543 b- defN 24-May-07 03:16 kjutils/kjutils.py
+-rw-rw-r--  2.0 unx      220 b- defN 24-May-07 03:23 kjutils-1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-07 03:23 kjutils-1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 24-May-07 03:23 kjutils-1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      516 b- defN 24-May-07 03:23 kjutils-1.7.dist-info/RECORD
+7 files, 19167 bytes uncompressed, 5512 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: kjutils/__init__.py
 Comment: 
 
 Filename: kjutils/kjutils.py
 Comment: 
 
-Filename: kjutils-1.6.dist-info/METADATA
+Filename: kjutils-1.7.dist-info/METADATA
 Comment: 
 
-Filename: kjutils-1.6.dist-info/WHEEL
+Filename: kjutils-1.7.dist-info/WHEEL
 Comment: 
 
-Filename: kjutils-1.6.dist-info/top_level.txt
+Filename: kjutils-1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: kjutils-1.6.dist-info/RECORD
+Filename: kjutils-1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kjutils/kjutils.py

```diff
@@ -90,36 +90,77 @@
         """
         patter = re.compile(r",")
         info = {_: re.sub(patter, '', val) for _, val in self.result.items() if _ in self.comma_fields}
         self.result.update(info)
 
         # pprint(self.result)
 
+    def filter_kuohao(self):
+        """
+        去除specs字段中存在的中英文括号
+        @return:
+        """
+        patters = [r"\（.*?\）", r"\(.*?\)$"]
+        for patter in patters:
+            for _, val in self.result.items():
+                if _ in self.lower_fields:
+                    specs_val = re.sub(patter, "", val)
+                    if specs_val != val:
+                        info = {_: specs_val}
+                        self.result.update(info)
+                        break
+                    else:
+                        continue
+
+
     def filter_int(self):
         """
         规格及货号数据取整
         去除小数点后面的只有一位的0
         @return:
         """
         try:
             if self.filter_str:
-                patter = re.compile(r'\d+')
-                # patter1 = re.compile(r"[a-zA-Z]") # 不能匹配 μ
-                val = patter.findall(self.result.get('specs'))
-                val = [s for s in val if int(s) >= 0]
-                val = '.'.join(val)
-                # print(val)
-                unit = self.result.get('specs').split(val.strip())[-1]
-                if "." in val:
-                    first_val = val.strip().split('.')[0]
-                    val = val.strip().split('.')[-1] if "." in val else val.strip()
-                    # val = first_val + "." + val if val != str(0) else first_val
-                    val = first_val + "." + val if int(val) else first_val
-
-                specs = str(val) + ''.join(unit)
+                self.result.update({"specs": self.result.get('specs').replace(",", ".")})
+                specunits = ["kg", "KG", 'mg', 'MG', "μg", "g", "G", 'ml', "ML", "μmol", 'l', 'L']
+                specs_flag = False  # 默认没有匹配到现有的规格单位
+
+                specs = ""
+                for end_unit in specunits:
+                    # 遍历所有的规格单位，如果是以当前单位结尾的，则提取值和单位
+                    specs = self.result.get("specs")
+                    # specs = "".join(specs.split("（")[:-1])
+                    # specs = "".join(specs.split("(")[:-1]) if len(specs.split("(")) > 1 else "".join(specs.split("("))
+                    # print(specs)
+                    if specs.endswith(end_unit):
+                        specs_flag = True
+                        value = re.match(r"\d+.\d+|\d+", specs)
+                        spec_value = value.group(0) if value else ""
+                        spec_unit = end_unit.lower()
+                        specs = str(spec_value) + str(spec_unit)
+                        break
+                    else:
+                        continue
+                if not specs_flag:
+                    specs = self.result.get('specs')
+                # self.result.update({"specs":self.result.get('specs').replace(",",".")})
+                # patter = re.compile(r'\d+')
+                # # patter1 = re.compile(r"[a-zA-Z]") # 不能匹配 μ
+                # val = patter.findall(self.result.get('specs'))  # 规格的组成只能是两部份整数和浮点数
+                # val = [s for s in val if int(s) >= 0]
+                # val = '.'.join(val[:2]) if len(val) >= 3 else '.'.join(val)
+                # # print(val)
+                # unit = self.result.get('specs').split(val.strip())[-1]
+                # if "." in val:
+                #     first_val = val.strip().split('.')[0]
+                #     val = val.strip().split('.')[-1] if "." in val else val.strip()
+                #     # val = first_val + "." + val if val != str(0) else first_val
+                #     val = first_val + "." + val if int(val) else first_val
+                #
+                # specs = str(val) + ''.join(unit)
                 goods_id = '-'.join(self.result.get("goods_id").split('-')[0:-1])
                 info = {"specs": specs, 'goods_id': goods_id + "-" + specs.lower()}
                 # info = {"specs": specs}
                 self.result.update(info)
             else:
                 pass
         except ValueError:
@@ -135,34 +176,41 @@
         self.result.update(
             {_: val.lower() for _, val in self.result.items() if _ in self.lower_fields and self.filter_str})
         self.result.update({_: val.replace('/', '') for _, val in self.result.items() if _ in self.lower_fields})
 
         # pprint(self.result)
 
     def int_to_str(self):
+        # 数字转字符串
         self.result = {_: str(val).strip() for _, val in self.result.items() if val}
 
     def process_item(self):
         self.int_to_str()  # 数字转字符串
+        self.filter_kuohao()  # 去除括号
         self.filter_l_r()  # 去除左右空格
         self.filter_vals()  # 去除所有的空格
         self.filter_comma()  # 去除逗号
         self.filter_int()  # specs去除小数点后的0
         self.filter_lower()  # 转成小写
 
         return self.result
 
 
-if __name__ == '__main__':
+# if __name__ == '__main__':
     # value = {'goods_id': '0109160017-10 mM * 1 mL in DMSO ', 'productname': "3-bromo-[1,1'-biphenyl]-4-ol", 'cas': '92-03-5',
     #          'purity': ' 95% ', 'specs': '  50MG(COLL)   ', 'price': '$58.00', 'stock': '8700mg',
     #          'source': 'otavachemicals',
     #          'mdl': 'MFCD00053297',
     #          'source_url': 'https://search.otavachemicals.com/#!/compound/609a502cf1270034218f8004',
     #          'companyname': 'OTAVAchemicals', 'create_time': '2023-06-25 14:26:48',
     #          'update_time': '2023-06-25 14:26:48', 'spider': 'otava'}
-    value = {'goods_id': 'AB118589-500 g', 'cas': '98-98-6', 'price': '€124.00', 'purity': '99%', 'productname': '2-Picolinic acid, 99%; .', 'specs': '500 g', 'mdl': 'MFCD00006293', 'stock': '', 'source_url': 'https://abcr.com/de_en/ab118589', 'source': 'abcr', 'companyname': 'abcr', 'create_time': '2023-08-28 15:38:50', 'update_time': '2023-08-28 15:38:50', 'spider': 'abc'}
-
+    # value = {'goods_id': 'EN300-24210107-5.0g', 'productname': 'potassium trifluoro(5-formylpyridin-3-yl)boranuide',
+    #          'cas': '1245906-60-8', 'purity': '', 'stock': 'Out of Stock',
+    #          'specs': '	250 mg (757.5 mM * 500 μL in Water)', 'price': '$1240.0',
+    #          'source': 'enaminestore', 'mdl': 'MFCD09993069',
+    #          'source_url': 'https://new.enaminestore.com/catalog/EN300-24210107?cat=BB&cas=1245906-60-8',
+    #          'companyname': 'Enamine', 'create_time': '2023-09-15 14:38:04', 'update_time': '2023-09-15 14:38:04',
+    #          'spider': 'enamin'}
 
     # kjutils().filter_lower(value=value)
-    ff = Kjutils(string=value).process_item()
-    pprint(ff)
+    # ff = Kjutils(string=value).process_item()
+    # pprint(ff)
```

## Comparing `kjutils-1.6.dist-info/RECORD` & `kjutils-1.7.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 kjutils/PriceStock.py,sha256=gbnAJAusgWzWYLRB_78FG0c124WLhvpivExMtb5kalY,9677
 kjutils/__init__.py,sha256=4981gBVz1AJoLILfckEfHL9at4jnvbSoB6eO34c0g74,111
-kjutils/kjutils.py,sha256=-EgE7_ye-g_0Ga9NICN6SduGSPLqgC9PM2YD_aD3NUY,6192
-kjutils-1.6.dist-info/METADATA,sha256=K1AL8-aEfSBAKkh0BJdAihbsUjWhq721b79cIldLELc,234
-kjutils-1.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-kjutils-1.6.dist-info/top_level.txt,sha256=Irxi4AKcpZEdgz0YATi6hx9fr1yfuv1Puzn3aTiZNLk,8
-kjutils-1.6.dist-info/RECORD,,
+kjutils/kjutils.py,sha256=MjqyMSr_P8_eXHMljQ7s4E_nUs3diuupiOVVTt5Pvj8,8543
+kjutils-1.7.dist-info/METADATA,sha256=J7zeoEzphN0JxNXdnrD6I3z91LMn43Qt0gRAnmm9eHk,220
+kjutils-1.7.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+kjutils-1.7.dist-info/top_level.txt,sha256=Irxi4AKcpZEdgz0YATi6hx9fr1yfuv1Puzn3aTiZNLk,8
+kjutils-1.7.dist-info/RECORD,,
```

