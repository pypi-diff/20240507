# Comparing `tmp/pybangla-1.0.4.tar.gz` & `tmp/pybangla-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybangla-1.0.4.tar", last modified: Sun May  5 18:27:29 2024, max compression
+gzip compressed data, was "pybangla-1.0.5.tar", last modified: Tue May  7 16:34:44 2024, max compression
```

## Comparing `pybangla-1.0.4.tar` & `pybangla-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:29.479811 pybangla-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:21.000000 pybangla-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-05 18:27:29.479811 pybangla-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15188 2024-05-05 18:27:21.000000 pybangla-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:29.475811 pybangla-1.0.4/pybangla/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:29.479811 pybangla-1.0.4/pybangla/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18100 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/date_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/number_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    18145 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/word_to_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:29.479811 pybangla-1.0.4/pybangla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-05 18:27:29.000000 pybangla-1.0.4/pybangla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-05 18:27:29.000000 pybangla-1.0.4/pybangla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:27:29.000000 pybangla-1.0.4/pybangla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-05 18:27:29.000000 pybangla-1.0.4/pybangla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 18:27:29.000000 pybangla-1.0.4/pybangla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:27:29.479811 pybangla-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-05 18:27:21.000000 pybangla-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:29.479811 pybangla-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-05 18:27:21.000000 pybangla-1.0.4/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:34:44.909571 pybangla-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:34:37.000000 pybangla-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15656 2024-05-07 16:34:44.909571 pybangla-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15098 2024-05-07 16:34:37.000000 pybangla-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:34:44.905571 pybangla-1.0.5/pybangla/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 16:34:37.000000 pybangla-1.0.5/pybangla/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:34:44.909571 pybangla-1.0.5/pybangla/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:34:37.000000 pybangla-1.0.5/pybangla/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18102 2024-05-07 16:34:37.000000 pybangla-1.0.5/pybangla/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-07 16:34:37.000000 pybangla-1.0.5/pybangla/module/date_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-07 16:34:37.000000 pybangla-1.0.5/pybangla/module/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-07 16:34:37.000000 pybangla-1.0.5/pybangla/module/number_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19394 2024-05-07 16:34:37.000000 pybangla-1.0.5/pybangla/module/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-07 16:34:37.000000 pybangla-1.0.5/pybangla/module/word_to_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-05-07 16:34:37.000000 pybangla-1.0.5/pybangla/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:34:44.909571 pybangla-1.0.5/pybangla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15656 2024-05-07 16:34:44.000000 pybangla-1.0.5/pybangla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-07 16:34:44.000000 pybangla-1.0.5/pybangla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:34:44.000000 pybangla-1.0.5/pybangla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 16:34:44.000000 pybangla-1.0.5/pybangla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 16:34:44.000000 pybangla-1.0.5/pybangla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:34:44.909571 pybangla-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-07 16:34:37.000000 pybangla-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:34:44.909571 pybangla-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-07 16:34:37.000000 pybangla-1.0.5/tests/test.py
```

### Comparing `pybangla-1.0.4/PKG-INFO` & `pybangla-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.0.4
+Version: 1.0.5
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -493,17 +493,16 @@
 print(seasons)
 
 # output:
 {'summer': 'গ্রীষ্ম'}
 ```
 # Next Upcomming Features
 
-1. Date extraction from normal text sentence and convert it numerical to word(vice versa)
-2. Bangla lemmatization and stemming algorithm
-3. Bangla Tokenizer
+1. Bangla lemmatization and stemming algorithm
+2. Bangla Tokenizer
 
 
 # Contact
 If you have any suggestion: Email: saifulbrur79@gmail.com
 
 # Contributor
```

### Comparing `pybangla-1.0.4/README.md` & `pybangla-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -477,17 +477,16 @@
 print(seasons)
 
 # output:
 {'summer': 'গ্রীষ্ম'}
 ```
 # Next Upcomming Features
 
-1. Date extraction from normal text sentence and convert it numerical to word(vice versa)
-2. Bangla lemmatization and stemming algorithm
-3. Bangla Tokenizer
+1. Bangla lemmatization and stemming algorithm
+2. Bangla Tokenizer
 
 
 # Contact
 If you have any suggestion: Email: saifulbrur79@gmail.com
 
 # Contributor
```

### Comparing `pybangla-1.0.4/pybangla/module/config.py` & `pybangla-1.0.5/pybangla/module/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             "seasons"  : ["গ্রীষ্ম","বর্ষা", "শরৎ", "হেমন্ত", "শীত", "বসন্ত"],
             "number_mapping": {'০':'শূন্য', '১':'এক', '২':'দুই', '৩':'তিন', '৪':'চার', '৫':'পাঁচ', '৬':'ছয়', '৭':'সাত', '৮':'আট', '৯':'নয়'}
 
             }
     }
     bn_number_word_mapping = {'০':'শূন্য', '১':'এক', '২':'দুই', '৩':'তিন', '৪':'চার', '৫':'পাঁচ', '৬':'ছয়', '৭':'সাত', '৮':'আট', '৯':'নয়'}
 
-    bn_regex = r'[০-৯]+'
+    bn_regex = r'[০-৯.,]+'
     en_regex = r'[0-9]+'
     samples = ["-", ",", "/", " "]
     _currency = {"৳" : "টাকা", "$" : "ডলার", "£" : "পাউন্ড", "€" : "ইউরো", "¥" : "ইয়েন", "₹" : "রুপি", "₽" : "রুবেল", "₺" : "লিরা"}
     en_to_bn_digits_mapping = {e : b for e, b in zip(data["en"]["number"], data["bn"]["number"])}
     bn_to_en_digits_mapping = {v : k for k, v in en_to_bn_digits_mapping.items()}
     en_month_shortname = [i[:3] for i in data["en"]["months"]]
```

### Comparing `pybangla-1.0.4/pybangla/module/date_extractor.py` & `pybangla-1.0.5/pybangla/module/date_extractor.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.4/pybangla/module/main.py` & `pybangla-1.0.5/pybangla/module/main.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.4/pybangla/module/number_parser.py` & `pybangla-1.0.5/pybangla/module/number_parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.4/pybangla/module/parser.py` & `pybangla-1.0.5/pybangla/module/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import datetime
+import string
 from .config import Config as cfg
 from num2words import num2words
 from .date_extractor import DateExtractor
 # from .number_parser import Word2NumberMap
 
 
 dt = DateExtractor()
@@ -26,14 +27,18 @@
         self.bangla_numeric_words = bangla_numeric_words
         self.en_regex = cfg.en_regex
         self.bn_regex = cfg.bn_regex
 
     def is_english_digit_string(s):
         # Check if all characters in the string are digits (0-9)
         return all(char.isdigit() for char in s)
+    
+    def contains_only_english(self, input_string):
+        # Check if all characters in the string are English (ASCII) characters
+        return all(ord(char) < 128 for char in input_string)
 
     def number_to_words_converting_process(self, number_string:str, lang = "bn"):
         number_string = number_string.strip()
         num = int("".join([self.english_digits[bangla_digit] if lang =="bn" else bangla_digit for bangla_digit in number_string]))
         try:
             eng_in_num_to_words = num2words(num, lang='en_IN')
             if lang =="bn":
@@ -67,14 +72,16 @@
         return " ".join(number.split())
     
     def digit_number_to_digit_word(self, number, language="bn"):
 
         number = re.sub(_whitespace_re, " ", number)
         s_n = ""
         for i in number:
+            # print("language : ", language, i)
+
             n = data[language]["number_mapping"][i]
             s_n += " "+n
         return s_n.strip()
     
     def year_in_number(self, year_in_number:str, language="bn"):
         """ Converts a Bangla year in numeric form to literal words.
 
@@ -158,14 +165,16 @@
         # print("d, y : ", d, y)
         
         if d:
             date_[0] = self._digit_converter(date_[0], language="bn")
         if y:
             date_[2] = self._digit_converter(date_[2], language="bn")
 
+        # print("date_", date_)
+
         current_date_object = datetime.datetime(int(date_[2]), int(date_[1]), int(date_[0]))
         if language in data:
             weekday = data[language]["weekdays"][current_date_object.weekday()]
         else:
             print("language not handel")
             weekday = ""
         return weekday
@@ -200,35 +209,53 @@
         start  = text.find(word)
         end = start+len(word)
         return [start, end]
 
     def replace_text_at_position(self, text:str, replacement:str, start_pos:int, end_pos:int)->str:
         """
         Replance text using text position
-        
+    
         """
-        return text[:start_pos] + replacement + text[end_pos:]
+        rep_text = text[:start_pos] + replacement + text[end_pos:]
+        return rep_text
+    
+    def fraction_number_conversion(self, number, language="bn"):
+        n_n = ""
+        for i in number:
+            if i in cfg._english2bangla2_digits_mapping:
+                n_n+=cfg._english2bangla2_digits_mapping[i]
+            else:
+                n_n+=i
+                
+        s_m = n_n.split(".")
+        before_dot_word, after_dot_word = self.number_to_words(s_m[0]), self.digit_number_to_digit_word(s_m[1], language=language)
+        word =  before_dot_word+" দশমিক "+after_dot_word
+        return word
     
     def number_processing(self, text):
+        pattern = r'[\d,\.]+'
+        matches = re.findall(pattern, text)
+        for n in matches:
+            status = self.contains_only_english(n)
+            m_re = n.replace(",", "")
+            if status:
+                if "." in m_re:
+                    bn_m= self.fraction_number_conversion(m_re)
+                else:
+                    bn_m= self.number_to_words(self._digit_converter(m_re))
+                
+                text = text.replace(n, bn_m)
+            else:
+                if "." in m_re:
+                    bn_m= self.fraction_number_conversion(m_re, language="bn")
+                else:
+                    bn_m= self.number_to_words(m_re)
+                print(n, m_re, bn_m)
+                text = text.replace(n, bn_m)
 
-        # bn_regex, en_regex = r'[০-৯]+', r'[0-9]+'
-        bn_matches, en_matches = list(re.finditer(self.bn_regex, text, re.UNICODE)), \
-            list(re.finditer(self.en_regex, text, re.UNICODE))
-        if en_matches:
-            for m in en_matches:
-                m = m[0].replace(",", "")
-                if m:
-                    bn_m= self.number_to_words(self._digit_converter(m))
-                    text = text.replace(m[0], bn_m)
-        if bn_matches:
-            for m in bn_matches:
-                m = m[0].replace(",", "")
-                if m[0]:
-                    bn_m= self.number_to_words(m)
-                    text = text.replace(m[0], bn_m)
         return text
 
 class DateParser:
     def __init__(self):
         self.samples = cfg.samples
 
         self.npr = NumberParser()
@@ -255,16 +282,17 @@
         elif key in data["en"]["option_name"]:
             index = data["en"]["option_name"].index(key)+1
         elif key in data["en"]["number"]:
             index = data["en"]["number"].index(key)+1
         elif key in data["bn"]["number"]:
             index = data["bn"]["number"].index(key)+1
         else:
-            print("else : ", key)
-            index = key
+            key = key.strip()
+            if key[-1] in string.punctuation:
+                index = key[:-1]
         return index
 
 
     def format_non_punctuation(self, split_date):
         """
         
         """
@@ -416,51 +444,63 @@
         # print(matches)
         """
         Need to correct year format extraction
         """
         for i in matches:
             text = text.replace(i, self.npr.year_in_number(i))
         return text
+    
+
 
     def extract_currency_amounts(self, text):
 
         matches = re.findall(self.currency_pattern, text)
         pattern = r'[৳$£€¥₹₽₺]'
 
         for m in matches:
-            # print("m : ", m)
             # Use findall to extract matches
             currency = re.findall(pattern, m)
 
             # print(currency)
             if currency:
                 # print("m : ", m)
                 n_m = m.replace(currency[0], "")
                 n_m = n_m.replace(",", "")
+                language = "en" if self.npr.contains_only_english(n_m) else "bn"
                 if "." in n_m:
-                    s_m = n_m.split(".")
-                    before_dot_word, after_dot_word = self.npr.number_to_words(s_m[0]), self.npr.digit_number_to_digit_word(s_m[1])
-                    word =  before_dot_word+" দশমিক "+after_dot_word+ " "+_currency[currency[0]]
-                    text = text.replace(m, word)
-                    # print(s_m, before_dot_word, after_dot_word)
+                    word = self.npr.fraction_number_conversion(n_m, language=language)
+                    r_word =  word+" "+_currency[currency[0]]
+                    text = text.replace(m, r_word)
                 else:
                     word = self.npr.number_to_words(n_m)
                     n_word = word + " "+_currency[currency[0]]
                     text = text.replace(m, n_word)
         return text
     
+    def date_formate_validation(self, date):
+        n_data = date.strip().split(" ")
+        month_name = data["en"]["months"]+ data["en"]["months"] + data["en"]["option_name"] + data["bn"]["option_name"]
+        for n_d in n_data:
+            if n_d in month_name:
+                return True
+        return False
+
+
+    
     def replance_date_processing(self, text):
         dates = dt.get_dates(text)
         for date in dates:
-            position = self.npr.find_word_index(text, date)
-            formated_date = self.dp.date_processing(date)
-            # print(formated_date)
-            f_d_string = formated_date["txt_date"]+" "+formated_date["month"]+" "+formated_date["txt_year"]
-            # print(f_d_string)
-            text = self.npr.replace_text_at_position(text, f_d_string, position[0], position[1])
+            status = True
+            if " " in date:
+                status = self.date_formate_validation(date)
+            if status:
+                position = self.npr.find_word_index(text, date)
+                formated_date = self.dp.date_processing(date)
+                f_d_string = formated_date["txt_date"]+" "+formated_date["month"]+" "+formated_date["txt_year"]
+                text = self.npr.replace_text_at_position(text, f_d_string, position[0], position[1])
         return text
 
     
 
     def processing(self, text):
         text = self.collapse_whitespace(text)
         text = self.expand_symbols(text)
```

### Comparing `pybangla-1.0.4/pybangla/module/word_to_number.py` & `pybangla-1.0.5/pybangla/module/word_to_number.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.4/pybangla/test.py` & `pybangla-1.0.5/pybangla/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import time
 from module.main import Normalizer
 
 if __name__ == "__main__":
 
 
     # # Testing Date format
-    # date_list = [
-    #     "সেপ্টেম্বর ০৫ ২০২৩",
-    #     "এপ্রিল ২০২৩" 
-    #     "2023-04-05",  
-    #     "06-04-2023", 
-    #     "04/01/2023",  
-    #     "07 April, 2023", 
-    #     "Apr 1, 2023",  
-    #     "2023/04/01", 
-    #     "01-Apr-2023", 
-    #     "01-Apr/2023",  
-    #     "20230401",  
-    #     "20042024",
-    #     ["1", "4", "2025"]
-    # ]
+    date_list = [
+        "সেপ্টেম্বর ০৫ ২০২৩",
+        "এপ্রিল ২০২৩" 
+        "2023-04-05",  
+        "06-04-2023", 
+        "04/01/2023",  
+        "07 April, 2023", 
+        "Apr 1, 2023",  
+        "2023/04/01", 
+        "01-Apr-2023", 
+        "01-Apr/2023",  
+        "20230401",  
+        "20042024",
+        ["1", "4", "2025"]
+    ]
     # # # number = "123456" or "২০২৩"
     # number = "২০২৩"
     nrml = Normalizer()
     # # print("++++++++++++++++++++ Date testing ++++++++++++++++++++++")
-    # # print("Date format Testing : ", end ="", flush=True)
-    # for date_ in date_list:
-    #     start_time = time.time()
-    #     formated_date = nrml.date_format(date_, language="bn")
-    #     print(formated_date)
-    # print("++++++++++++++++++++ end of Date testing ++++++++++++++++++++++")
+    # print("Date format Testing : ", end ="", flush=True)
+    for date_ in date_list:
+        start_time = time.time()
+        formated_date = nrml.date_format(date_, language="bn")
+        print(formated_date)
+    print("++++++++++++++++++++ end of Date testing ++++++++++++++++++++++")
 
     # print("++++++++++++++++++++ en number to bn number convert ++++++++++++++++++++++")
     # number = nrml.number_convert(number, language="bn")
     
     
     # number = nrml.number_convert(number, language="bn")
 
@@ -163,10 +163,15 @@
         print("output : ", text)
         print("="*40)
     text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২,০২৩"
     formated_date = nrml.date_extraction(text)
 
     print(formated_date)
 
+    # text = "৫ বছরে নন-ক্যাডার পদে ৭,৪৪৭ জনকে নিয়োগের সুপারিশ করা হয়েছে 1,230"
+    text = "৫ বছরে নন-ক্যাডার পদে ৭,৪৪৭ জনকে নিয়োগের সুপারিশ করা হয়েছে"
+
+    # text = "The numbers are 10 নন-ক্যাডার 20.5  30, and 40.75. সুপারিশ ২০৩০.৩০ 12 23 45"
+
     text = nrml.text_normalizer(text)
     print(text)
```

### Comparing `pybangla-1.0.4/pybangla.egg-info/PKG-INFO` & `pybangla-1.0.5/pybangla.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.0.4
+Version: 1.0.5
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -493,17 +493,16 @@
 print(seasons)
 
 # output:
 {'summer': 'গ্রীষ্ম'}
 ```
 # Next Upcomming Features
 
-1. Date extraction from normal text sentence and convert it numerical to word(vice versa)
-2. Bangla lemmatization and stemming algorithm
-3. Bangla Tokenizer
+1. Bangla lemmatization and stemming algorithm
+2. Bangla Tokenizer
 
 
 # Contact
 If you have any suggestion: Email: saifulbrur79@gmail.com
 
 # Contributor
```

### Comparing `pybangla-1.0.4/setup.py` & `pybangla-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import codecs
 from setuptools import setup, find_packages
 
 setup(
     name='pybangla',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(),
     # entry_points={
     #     'console_scripts': [
     #         'pybangla = pybangla.main:Normalizer'
     #     ]
     # },
     author='saiful',
```

### Comparing `pybangla-1.0.4/tests/test.py` & `pybangla-1.0.5/tests/test.py`

 * *Files identical despite different names*

