# Comparing `tmp/swiki-2.0.1.tar.gz` & `tmp/swiki-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiki-2.0.1.tar", last modified: Tue May  7 08:23:14 2024, max compression
+gzip compressed data, was "swiki-2.0.2.tar", last modified: Tue May  7 08:29:39 2024, max compression
```

## Comparing `swiki-2.0.1.tar` & `swiki-2.0.2.tar`

### file list

```diff
@@ -1,12 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 08:23:14.098867 swiki-2.0.1/
--rw-rw-rw-   0        0        0     2326 2024-05-07 08:23:14.098867 swiki-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1895 2024-05-06 23:42:59.000000 swiki-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-07 08:23:14.099865 swiki-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1410 2024-05-07 08:23:10.000000 swiki-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 08:23:14.097866 swiki-2.0.1/swiki.egg-info/
--rw-rw-rw-   0        0        0     2326 2024-05-07 08:23:14.000000 swiki-2.0.1/swiki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-05-07 08:23:14.000000 swiki-2.0.1/swiki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 08:23:14.000000 swiki-2.0.1/swiki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-07 08:23:14.000000 swiki-2.0.1/swiki.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-05-07 08:23:14.000000 swiki-2.0.1/swiki.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 08:23:14.000000 swiki-2.0.1/swiki.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 08:29:39.327495 swiki-2.0.2/
+-rw-rw-rw-   0        0        0     2276 2024-05-07 08:29:39.326496 swiki-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1895 2024-05-06 23:42:59.000000 swiki-2.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 08:29:39.327495 swiki-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2024-05-07 08:29:10.000000 swiki-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:29:39.324495 swiki-2.0.2/swiki.egg-info/
+-rw-rw-rw-   0        0        0     2276 2024-05-07 08:29:39.000000 swiki-2.0.2/swiki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      134 2024-05-07 08:29:39.000000 swiki-2.0.2/swiki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 08:29:39.000000 swiki-2.0.2/swiki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 08:29:39.000000 swiki-2.0.2/swiki.egg-info/top_level.txt
```

### Comparing `swiki-2.0.1/PKG-INFO` & `swiki-2.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: swiki
-Version: 2.0.1
+Version: 2.0.2
 Summary: A program for searching and reading Wikipedia articles in multiple languages
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: wikipedia
-Requires-Dist: pyttsx3
 
     # Программа для поиска и чтения статей из Википедии
 
 Этот скрипт позволяет пользователю искать и читать статьи из Википедии на разных языках. Пользователь выбирает язык для
 поиска и чтения статей, вводит запрос, выбирает статью из результатов поиска и может запросить чтение текста статьи с
 помощью речи.
 ***
```

### Comparing `swiki-2.0.1/README.md` & `swiki-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `swiki-2.0.1/setup.py` & `swiki-2.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='swiki',  # Уникальное имя вашего пакета
-    version='2.0.1',  # Версия вашего пакета
+    version='2.0.2',  # Версия вашего пакета
     author='k0ng999',  # Ваше имя или имя вашего проекта
     author_email='baydar_14@mail.ru',  # Ваш адрес электронной почты
     description='A program for searching and reading Wikipedia articles in multiple languages',  # Краткое описание вашего пакета
     long_description=open('README.md', encoding='utf-8').read(),  # Длинное описание вашего пакета из файла README.md
     long_description_content_type='text/markdown',  # Тип длинного описания (markdown)
     packages=find_packages(),  # Список пакетов Python, которые должны быть включены в ваш пакет
-    entry_points={
-        'console_scripts': [
-            'swiki = swikipedia:search',  # Точка входа для вашего скрипта
-        ],
-    },
-    install_requires=[
-        'wikipedia',  # Зависимости вашего пакета
-        'pyttsx3',
-    ],
+
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

### Comparing `swiki-2.0.1/swiki.egg-info/PKG-INFO` & `swiki-2.0.2/swiki.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: swiki
-Version: 2.0.1
+Version: 2.0.2
 Summary: A program for searching and reading Wikipedia articles in multiple languages
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: wikipedia
-Requires-Dist: pyttsx3
 
     # Программа для поиска и чтения статей из Википедии
 
 Этот скрипт позволяет пользователю искать и читать статьи из Википедии на разных языках. Пользователь выбирает язык для
 поиска и чтения статей, вводит запрос, выбирает статью из результатов поиска и может запросить чтение текста статьи с
 помощью речи.
 ***
```

