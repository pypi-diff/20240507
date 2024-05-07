# Comparing `tmp/myswiki-2.1.3.tar.gz` & `tmp/myswiki-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myswiki-2.1.3.tar", last modified: Tue May  7 18:36:56 2024, max compression
+gzip compressed data, was "myswiki-2.1.4.tar", last modified: Tue May  7 18:53:50 2024, max compression
```

## Comparing `myswiki-2.1.3.tar` & `myswiki-2.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 18:36:56.021047 myswiki-2.1.3/
--rw-rw-rw-   0        0        0     1088 2024-05-07 08:54:42.000000 myswiki-2.1.3/LICENSE
--rw-rw-rw-   0        0        0     2168 2024-05-07 18:36:56.021047 myswiki-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1897 2024-05-07 18:08:52.000000 myswiki-2.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 18:36:56.020051 myswiki-2.1.3/myswiki.egg-info/
--rw-rw-rw-   0        0        0     2168 2024-05-07 18:36:55.000000 myswiki-2.1.3/myswiki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2024-05-07 18:36:55.000000 myswiki-2.1.3/myswiki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 18:36:55.000000 myswiki-2.1.3/myswiki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-07 18:36:55.000000 myswiki-2.1.3/myswiki.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6137 2024-05-07 18:34:32.000000 myswiki-2.1.3/myswiki.py
--rw-rw-rw-   0        0        0       42 2024-05-07 18:36:56.022046 myswiki-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0      412 2024-05-07 18:36:48.000000 myswiki-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:53:50.183237 myswiki-2.1.4/
+-rw-rw-rw-   0        0        0     1088 2024-05-07 08:54:42.000000 myswiki-2.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2158 2024-05-07 18:53:50.182235 myswiki-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1887 2024-05-07 18:53:45.000000 myswiki-2.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 18:53:50.181237 myswiki-2.1.4/myswiki.egg-info/
+-rw-rw-rw-   0        0        0     2158 2024-05-07 18:53:50.000000 myswiki-2.1.4/myswiki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2024-05-07 18:53:50.000000 myswiki-2.1.4/myswiki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 18:53:50.000000 myswiki-2.1.4/myswiki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 18:53:50.000000 myswiki-2.1.4/myswiki.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4894 2024-05-07 18:53:02.000000 myswiki-2.1.4/myswiki.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 18:53:50.183237 myswiki-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      412 2024-05-07 18:53:45.000000 myswiki-2.1.4/setup.py
```

### Comparing `myswiki-2.1.3/LICENSE` & `myswiki-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `myswiki-2.1.3/PKG-INFO` & `myswiki-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myswiki
-Version: 2.1.3
+Version: 2.1.4
 Summary: A program for searching and reading Wikipedia articles in multiple languages
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -33,17 +33,17 @@
 > Выберите статью из результатов поиска.
 > При желании, выберите опцию чтения текста статьи с помощью речи.
 ***
 
 ### Использование в коде
 
 ```python
-from swiki import WikiReader
+from swiki import wiki
 
-WikiReader
+wiki()
 
 ```
 
 ### Сообщения и локализация
 
 > Скрипт поддерживает два языка - русский и английский. Все сообщения и запросы выводятся на выбранном языке.
 ***
```

### Comparing `myswiki-2.1.3/README.md` & `myswiki-2.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 > Выберите статью из результатов поиска.
 > При желании, выберите опцию чтения текста статьи с помощью речи.
 ***
 
 ### Использование в коде
 
 ```python
-from swiki import WikiReader
+from swiki import wiki
 
-WikiReader
+wiki()
 
 ```
 
 ### Сообщения и локализация
 
 > Скрипт поддерживает два языка - русский и английский. Все сообщения и запросы выводятся на выбранном языке.
 ***
```

### Comparing `myswiki-2.1.3/myswiki.egg-info/PKG-INFO` & `myswiki-2.1.4/myswiki.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myswiki
-Version: 2.1.3
+Version: 2.1.4
 Summary: A program for searching and reading Wikipedia articles in multiple languages
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -33,17 +33,17 @@
 > Выберите статью из результатов поиска.
 > При желании, выберите опцию чтения текста статьи с помощью речи.
 ***
 
 ### Использование в коде
 
 ```python
-from swiki import WikiReader
+from swiki import wiki
 
-WikiReader
+wiki()
 
 ```
 
 ### Сообщения и локализация
 
 > Скрипт поддерживает два языка - русский и английский. Все сообщения и запросы выводятся на выбранном языке.
 ***
```

### Comparing `myswiki-2.1.3/myswiki.py` & `myswiki-2.1.4/myswiki.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,128 +1,102 @@
+__all__ = ['wiki']
 import wikipedia
 import pyttsx3
 
+messages = {
+    'ru': {
+        'choose_language': 'Выберите язык для поиска и прочтения статьи (ru/en): ',
+        'invalid_language': 'Пожалуйста, выберите корректный язык (ru/en).',
+        'enter_query': 'Что вы хотите узнать?\n',
+        'no_results': 'Ничего не найдено. Пожалуйста, попробуйте другой запрос.',
+        'input_article_number': '\nВведите номер статьи для прочтения (или 0 для выхода): ',
+        'invalid_article_number': 'Пожалуйста, введите корректный номер статьи.',
+        'read_text': 'Хотите чтобы я вам прочитал текст?\n(yes/no) ',
+        'http_error': 'Ошибка: превышено время ожидания запроса к Википедии.'
+    },
+    'en': {
+        'choose_language': 'Choose language for searching and reading articles (ru/en): ',
+        'invalid_language': 'Please choose a valid language (ru/en).',
+        'enter_query': 'What do you want to know?\n',
+        'no_results': 'Nothing found. Please try another query.',
+        'input_article_number': '\nEnter the article number to read (or 0 to exit): ',
+        'invalid_article_number': 'Please enter a valid article number.',
+        'read_text': 'Do you want me to read the text?\n(yes/no) ',
+        'http_error': 'Error: Wikipedia request timeout.'
+    }
+}
+
+
+def wrap_text(text, line_length=150):
+    wrapped_text = ""
+    words = text.split()
+    line = ""
+    for word in words:
+        if len(line) + len(word) <= line_length:
+            line += word + " "
+        else:
+            wrapped_text += line.strip() + '\n'
+            line = word + " "
+    wrapped_text += line.strip()
+    return wrapped_text
+
+
+def get_article_summary(query, language):
+    wikipedia.set_lang(language)
+    try:
+        summary = wikipedia.summary(query)
+        return wrap_text(summary)
+    except wikipedia.exceptions.DisambiguationError:
+        return "Неоднозначный запрос. Пожалуйста, уточните ваш запрос."
+    except wikipedia.exceptions.PageError:
+        return "Страница не найдена. Пожалуйста, попробуйте другой запрос."
 
-class WikiReader:
-    """
-    Класс для чтения статей из Википедии.
 
-    :param language: Язык статьи (ru или en).
-    :param query: Запрос для поиска статьи.
+def wiki():
     """
+    Запускает процесс чтения статей из Википедии.
 
-    def __init__(self):
-        """
-        Инициализация объекта WikiReader.
-
-        :param language: Язык статьи (ru или en).
-        :param query: Запрос для поиска статьи.
-        """
-        self.messages = {
-            'ru': {
-                'choose_language': 'Выберите язык для поиска и прочтения статьи (ru/en): ',
-                'invalid_language': 'Пожалуйста, выберите корректный язык (ru/en).',
-                'enter_query': 'Что вы хотите узнать?\n',
-                'no_results': 'Ничего не найдено. Пожалуйста, попробуйте другой запрос.',
-                'input_article_number': '\nВведите номер статьи для прочтения (или 0 для выхода): ',
-                'invalid_article_number': 'Пожалуйста, введите корректный номер статьи.',
-                'read_text': 'Хотите чтобы я вам прочитал текст?\n(yes/no) ',
-                'http_error': 'Ошибка: превышено время ожидания запроса к Википедии.'
-            },
-            'en': {
-                'choose_language': 'Choose language for searching and reading articles (ru/en): ',
-                'invalid_language': 'Please choose a valid language (ru/en).',
-                'enter_query': 'What do you want to know?\n',
-                'no_results': 'Nothing found. Please try another query.',
-                'input_article_number': '\nEnter the article number to read (or 0 to exit): ',
-                'invalid_article_number': 'Please enter a valid article number.',
-                'read_text': 'Do you want me to read the text?\n(yes/no) ',
-                'http_error': 'Error: Wikipedia request timeout.'
-            }
-        }
-
-        self.language = input(self.messages['en']['choose_language']).lower()
-        while self.language not in ('ru', 'en'):
-            print(self.messages['en']['invalid_language'])
-            self.language = input(self.messages['en']['choose_language']).lower()
+    Эта функция запрашивает у пользователя язык и тему для поиска статей на Википедии.
+    Затем она выводит результаты поиска и предлагает выбрать одну из статей для чтения.
+    Если пользователь согласится, то функция прочитает краткое описание выбранной статьи.
+    """
+    language = input(messages['en']['choose_language']).lower()
+    while language not in ('ru', 'en'):
+        print(messages['en']['invalid_language'])
+        language = input(messages['en']['choose_language']).lower()
 
-        self.query = input(self.messages[self.language]['enter_query'])
-        try:
-            wikipedia.set_lang(self.language)
-            search_results = wikipedia.search(self.query)
-            if not search_results:
-                print(self.messages[self.language]['no_results'])
-                return
-            article_idx = self.select_article(search_results, self.language)
-            if article_idx is None:
-                return
-            print("\n")
-            if input(self.messages[self.language]['read_text']).lower() == 'yes':
-                say = pyttsx3.init()
-                say.say(self.get_article_summary(search_results[article_idx], self.language))
-                print("\n")
-                print(self.get_article_summary(search_results[article_idx], self.language))
-                say.runAndWait()
-            else:
-                print(self.get_article_summary(search_results[article_idx], self.language))
-        except wikipedia.exceptions.HTTPTimeoutError:
-            print(self.messages[self.language]['http_error'])
-
-    def wrap_text(self, text, line_length=150):
-        """
-        Обертывает текст для вывода с заданной длиной строки.
-
-        :param text: Текст для обертывания.
-        :param line_length: Максимальная длина строки.
-        :return: Обернутый текст.
-        """
-        wrapped_text = ""
-        words = text.split()
-        line = ""
-        for word in words:
-            if len(line) + len(word) <= line_length:
-                line += word + " "
-            else:
-                wrapped_text += line.strip() + '\n'
-                line = word + " "
-        wrapped_text += line.strip()
-        return wrapped_text
-
-    def get_article_summary(self, query, language):
-        """
-        Получает краткое описание статьи из Википедии.
-
-        :param query: Запрос для поиска статьи.
-        :return: Краткое описание статьи.
-        """
+    query = input(messages[language]['enter_query'])
+    try:
         wikipedia.set_lang(language)
+        search_results = wikipedia.search(query)
+        if not search_results:
+            print(messages[language]['no_results'])
+            return
+        article_idx = select_article(search_results, language)  # Passing language to select_article
+        if article_idx is None:
+            return
+        print("\n")
+        if input(messages[language]['read_text']).lower() == 'yes':
+            say = pyttsx3.init()
+            say.say(get_article_summary(search_results[article_idx], language))
+            print("\n")
+            print(get_article_summary(search_results[article_idx], language))
+            say.runAndWait()
+        else:
+            print(get_article_summary(search_results[article_idx], language))
+    except wikipedia.exceptions.HTTPTimeoutError:
+        print(messages[language]['http_error'])
+
+def select_article(search_results, language):  # Added 'language' as parameter
+    for idx, result in enumerate(search_results, start=1):
+        print(f"{idx}. {result}")
+    while True:
         try:
-            summary = wikipedia.summary(query)
-            return self.wrap_text(summary)
-        except wikipedia.exceptions.DisambiguationError:
-            return "Неоднозначный запрос. Пожалуйста, уточните ваш запрос."
-        except wikipedia.exceptions.PageError:
-            return "Страница не найдена. Пожалуйста, попробуйте другой запрос."
-
-    def select_article(self, search_results, language):
-        """
-        Позволяет пользователю выбрать статью из списка результатов.
-
-        :param search_results: Список результатов поиска.
-        :return: Индекс выбранной статьи.
-        """
-        for idx, result in enumerate(search_results, start=1):
-            print(f"{idx}. {result}")
-        while True:
-            try:
-                choice = int(input(self.messages[language]['input_article_number']))
-                if choice == 0:
-                    return None
-                elif choice < 1 or choice > len(search_results):
-                    print(self.messages[language]['invalid_article_number'])
-                else:
-                    return choice - 1
-            except ValueError:
-                print("Please enter the number.")
-
-
-WikiReader()
+            choice = int(input(messages[language]['input_article_number']))  # Using 'language' variable
+            if choice == 0:
+                return None
+            elif choice < 1 or choice > len(search_results):
+                print(messages[language]['invalid_article_number'])
+            else:
+                return choice - 1
+        except ValueError:
+            print("Please enter the number.")
```

