# Comparing `tmp/gmailbox-0.0.6.tar.gz` & `tmp/gmailbox-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmailbox-0.0.6.tar", last modified: Tue May  7 08:39:31 2024, max compression
+gzip compressed data, was "gmailbox-0.0.7.tar", last modified: Tue May  7 15:05:13 2024, max compression
```

## Comparing `gmailbox-0.0.6.tar` & `gmailbox-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 08:39:31.760769 gmailbox-0.0.6/
-drwxrwxrwx   0        0        0        0 2024-05-07 08:39:31.739781 gmailbox-0.0.6/GmailBox/
--rw-rw-rw-   0        0        0     3267 2024-05-07 08:12:03.000000 gmailbox-0.0.6/GmailBox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 08:39:31.758772 gmailbox-0.0.6/GmailBox.egg-info/
--rw-rw-rw-   0        0        0     1480 2024-05-07 08:39:31.000000 gmailbox-0.0.6/GmailBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-07 08:39:31.000000 gmailbox-0.0.6/GmailBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 08:39:31.000000 gmailbox-0.0.6/GmailBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-07 08:39:31.000000 gmailbox-0.0.6/GmailBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-07 08:39:31.000000 gmailbox-0.0.6/GmailBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1480 2024-05-07 08:39:31.759771 gmailbox-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      839 2024-05-07 08:29:09.000000 gmailbox-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-07 08:39:31.760769 gmailbox-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-05-07 08:18:24.000000 gmailbox-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:05:13.781983 gmailbox-0.0.7/
+drwxrwxrwx   0        0        0        0 2024-05-07 15:05:13.759998 gmailbox-0.0.7/GmailBox/
+-rw-rw-rw-   0        0        0     3304 2024-05-07 12:19:14.000000 gmailbox-0.0.7/GmailBox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:05:13.779984 gmailbox-0.0.7/GmailBox.egg-info/
+-rw-rw-rw-   0        0        0     1480 2024-05-07 15:05:13.000000 gmailbox-0.0.7/GmailBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-07 15:05:13.000000 gmailbox-0.0.7/GmailBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 15:05:13.000000 gmailbox-0.0.7/GmailBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-07 15:05:13.000000 gmailbox-0.0.7/GmailBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 15:05:13.000000 gmailbox-0.0.7/GmailBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1480 2024-05-07 15:05:13.780983 gmailbox-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2024-05-07 08:29:09.000000 gmailbox-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 15:05:13.782982 gmailbox-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      828 2024-05-07 15:00:05.000000 gmailbox-0.0.7/setup.py
```

### Comparing `gmailbox-0.0.6/GmailBox/__init__.py` & `gmailbox-0.0.7/GmailBox/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,21 +55,22 @@
         for hamoo in hamo:
             messageID = hamoo['messageID']
             json_data = {
                 'email': f'{email}',
                 'messageID': f'{messageID}',
             }
             response = self.request.post('https://www.emailnator.com/message-list', headers=headers, json=json_data).text
+
             soup = BeautifulSoup(response, 'html.parser')
             formatted_html = soup.prettify()
             soup = BeautifulSoup(formatted_html, 'html.parser')
-            match = re.search(r"Time:.*\n\n(.*)", soup.text.strip(), re.DOTALL)
-            if match:
-                message = match.group(1)
-            else:
+            try:
+                tim = re.search(r"Time:\s*\n\s*\n(.+)", soup.text.strip()).group(1)
+                message = (soup.text.strip().split(f'{tim}',1)[1]).strip()
+            except:
                 message = soup.text.strip()
             sender = hamoo['from']
             try:
                 email_sender = re.findall(r'<(.*?)>', sender)[0]
             except:
                 email_sender = sender
             try:
```

### Comparing `gmailbox-0.0.6/GmailBox.egg-info/PKG-INFO` & `gmailbox-0.0.7/GmailBox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GmailBox
-Version: 0.0.6
+Version: 0.0.7
 Summary: With this library, you can create random Gmail and receive messages
 Author: Hamo
 License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox,email,Tempmail,Tempgmail
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GmailBox Version: 0.0.6 Summary: With this library,
+Metadata-Version: 2.1 Name: GmailBox Version: 0.0.7 Summary: With this library,
 you can create random Gmail and receive messages Author: Hamo License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox,email,Tempmail,Tempgmail Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
 (LGPLv3) Classifier: Programming Language :: Python :: 3 Classifier: Operating
 System :: OS Independent Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: beautifulsoup4
```

### Comparing `gmailbox-0.0.6/PKG-INFO` & `gmailbox-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GmailBox
-Version: 0.0.6
+Version: 0.0.7
 Summary: With this library, you can create random Gmail and receive messages
 Author: Hamo
 License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox,email,Tempmail,Tempgmail
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GmailBox Version: 0.0.6 Summary: With this library,
+Metadata-Version: 2.1 Name: GmailBox Version: 0.0.7 Summary: With this library,
 you can create random Gmail and receive messages Author: Hamo License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox,email,Tempmail,Tempgmail Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
 (LGPLv3) Classifier: Programming Language :: Python :: 3 Classifier: Operating
 System :: OS Independent Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: beautifulsoup4
```

### Comparing `gmailbox-0.0.6/README.md` & `gmailbox-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gmailbox-0.0.6/setup.py` & `gmailbox-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
 	name= "GmailBox",
-	version= "0.0.6",
+	version= "0.0.7",
 	author= "Hamo",
     keywords=["gmail","mail","GmailBox","inbox","email","Tempmail","Tempgmail"],
     install_requires=['requests','beautifulsoup4'],
     long_description=readme,
     long_description_content_type="text/markdown",
 	description= "With this library, you can create random Gmail and receive messages",
 	packages=setuptools.find_packages(),
```

