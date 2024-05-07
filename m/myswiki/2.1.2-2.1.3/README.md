# Comparing `tmp/myswiki-2.1.2.tar.gz` & `tmp/myswiki-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myswiki-2.1.2.tar", last modified: Tue May  7 18:21:10 2024, max compression
+gzip compressed data, was "myswiki-2.1.3.tar", last modified: Tue May  7 18:36:56 2024, max compression
```

## Comparing `myswiki-2.1.2.tar` & `myswiki-2.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 18:21:10.669614 myswiki-2.1.2/
--rw-rw-rw-   0        0        0     1088 2024-05-07 08:54:42.000000 myswiki-2.1.2/LICENSE
--rw-rw-rw-   0        0        0     2168 2024-05-07 18:21:10.668615 myswiki-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1897 2024-05-07 18:08:52.000000 myswiki-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 18:21:10.668615 myswiki-2.1.2/myswiki.egg-info/
--rw-rw-rw-   0        0        0     2168 2024-05-07 18:21:10.000000 myswiki-2.1.2/myswiki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2024-05-07 18:21:10.000000 myswiki-2.1.2/myswiki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 18:21:10.000000 myswiki-2.1.2/myswiki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-07 18:21:10.000000 myswiki-2.1.2/myswiki.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6177 2024-05-07 18:20:40.000000 myswiki-2.1.2/myswiki.py
--rw-rw-rw-   0        0        0       42 2024-05-07 18:21:10.669614 myswiki-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      412 2024-05-07 18:20:55.000000 myswiki-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:36:56.021047 myswiki-2.1.3/
+-rw-rw-rw-   0        0        0     1088 2024-05-07 08:54:42.000000 myswiki-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2168 2024-05-07 18:36:56.021047 myswiki-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1897 2024-05-07 18:08:52.000000 myswiki-2.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 18:36:56.020051 myswiki-2.1.3/myswiki.egg-info/
+-rw-rw-rw-   0        0        0     2168 2024-05-07 18:36:55.000000 myswiki-2.1.3/myswiki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2024-05-07 18:36:55.000000 myswiki-2.1.3/myswiki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 18:36:55.000000 myswiki-2.1.3/myswiki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 18:36:55.000000 myswiki-2.1.3/myswiki.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6137 2024-05-07 18:34:32.000000 myswiki-2.1.3/myswiki.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 18:36:56.022046 myswiki-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      412 2024-05-07 18:36:48.000000 myswiki-2.1.3/setup.py
```

### Comparing `myswiki-2.1.2/LICENSE` & `myswiki-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `myswiki-2.1.2/PKG-INFO` & `myswiki-2.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myswiki
-Version: 2.1.2
+Version: 2.1.3
 Summary: A program for searching and reading Wikipedia articles in multiple languages
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `myswiki-2.1.2/README.md` & `myswiki-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `myswiki-2.1.2/myswiki.egg-info/PKG-INFO` & `myswiki-2.1.3/myswiki.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myswiki
-Version: 2.1.2
+Version: 2.1.3
 Summary: A program for searching and reading Wikipedia articles in multiple languages
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `myswiki-2.1.2/myswiki.py` & `myswiki-2.1.3/myswiki.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import wikipedia
 import pyttsx3
 
 
 class WikiReader:
+    """
+    Класс для чтения статей из Википедии.
+
+    :param language: Язык статьи (ru или en).
+    :param query: Запрос для поиска статьи.
+    """
+
     def __init__(self):
         """
-        Класс для чтения статей из Википедии.
+        Инициализация объекта WikiReader.
+
+        :param language: Язык статьи (ru или en).
+        :param query: Запрос для поиска статьи.
         """
         self.messages = {
             'ru': {
                 'choose_language': 'Выберите язык для поиска и прочтения статьи (ru/en): ',
                 'invalid_language': 'Пожалуйста, выберите корректный язык (ru/en).',
                 'enter_query': 'Что вы хотите узнать?\n',
                 'no_results': 'Ничего не найдено. Пожалуйста, попробуйте другой запрос.',
@@ -57,20 +67,17 @@
         except wikipedia.exceptions.HTTPTimeoutError:
             print(self.messages[self.language]['http_error'])
 
     def wrap_text(self, text, line_length=150):
         """
         Обертывает текст для вывода с заданной длиной строки.
 
-        Args:
-            text (str): Текст для обертывания.
-            line_length (int): Максимальная длина строки.
-
-        Returns:
-            str: Обернутый текст.
+        :param text: Текст для обертывания.
+        :param line_length: Максимальная длина строки.
+        :return: Обернутый текст.
         """
         wrapped_text = ""
         words = text.split()
         line = ""
         for word in words:
             if len(line) + len(word) <= line_length:
                 line += word + " "
@@ -80,44 +87,32 @@
         wrapped_text += line.strip()
         return wrapped_text
 
     def get_article_summary(self, query, language):
         """
         Получает краткое описание статьи из Википедии.
 
-        Args:
-            query (str): Запрос для поиска статьи.
-            language (str): Язык статьи (ru или en).
-
-        Returns:
-            str: Краткое описание статьи.
-
-        Raises:
-            WikipediaException: Если не удалось получить описание статьи.
+        :param query: Запрос для поиска статьи.
+        :return: Краткое описание статьи.
         """
         wikipedia.set_lang(language)
         try:
             summary = wikipedia.summary(query)
             return self.wrap_text(summary)
         except wikipedia.exceptions.DisambiguationError:
             return "Неоднозначный запрос. Пожалуйста, уточните ваш запрос."
         except wikipedia.exceptions.PageError:
             return "Страница не найдена. Пожалуйста, попробуйте другой запрос."
 
     def select_article(self, search_results, language):
         """
         Позволяет пользователю выбрать статью из списка результатов.
 
-        Args:
-            search_results (list): Список результатов поиска.
-            language (str): Язык статьи (ru или en).
-
-        Returns:
-            int: Индекс выбранной статьи.
-
+        :param search_results: Список результатов поиска.
+        :return: Индекс выбранной статьи.
         """
         for idx, result in enumerate(search_results, start=1):
             print(f"{idx}. {result}")
         while True:
             try:
                 choice = int(input(self.messages[language]['input_article_number']))
                 if choice == 0:
```

