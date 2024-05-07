# Comparing `tmp/myswiki-1.0.2.tar.gz` & `tmp/myswiki-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myswiki-1.0.2.tar", last modified: Tue May  7 14:10:10 2024, max compression
+gzip compressed data, was "myswiki-2.0.0.tar", last modified: Tue May  7 18:02:53 2024, max compression
```

## Comparing `myswiki-1.0.2.tar` & `myswiki-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 14:10:10.795763 myswiki-1.0.2/
--rw-rw-rw-   0        0        0     1088 2024-05-07 08:54:42.000000 myswiki-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2161 2024-05-07 14:10:10.794762 myswiki-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1890 2024-05-07 14:03:42.000000 myswiki-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 14:10:10.794762 myswiki-1.0.2/myswiki.egg-info/
--rw-rw-rw-   0        0        0     2161 2024-05-07 14:10:10.000000 myswiki-1.0.2/myswiki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2024-05-07 14:10:10.000000 myswiki-1.0.2/myswiki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 14:10:10.000000 myswiki-1.0.2/myswiki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-07 14:10:10.000000 myswiki-1.0.2/myswiki.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4281 2024-05-07 09:04:53.000000 myswiki-1.0.2/myswiki.py
--rw-rw-rw-   0        0        0       42 2024-05-07 14:10:10.795763 myswiki-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      412 2024-05-07 14:09:25.000000 myswiki-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 18:02:53.392605 myswiki-2.0.0/
+-rw-rw-rw-   0        0        0     1088 2024-05-07 08:54:42.000000 myswiki-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2162 2024-05-07 18:02:53.391605 myswiki-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1891 2024-05-07 14:17:59.000000 myswiki-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 18:02:53.390605 myswiki-2.0.0/myswiki.egg-info/
+-rw-rw-rw-   0        0        0     2162 2024-05-07 18:02:53.000000 myswiki-2.0.0/myswiki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2024-05-07 18:02:53.000000 myswiki-2.0.0/myswiki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 18:02:53.000000 myswiki-2.0.0/myswiki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 18:02:53.000000 myswiki-2.0.0/myswiki.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4807 2024-05-07 18:00:48.000000 myswiki-2.0.0/myswiki.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 18:02:53.392605 myswiki-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      412 2024-05-07 18:02:48.000000 myswiki-2.0.0/setup.py
```

### Comparing `myswiki-1.0.2/LICENSE` & `myswiki-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myswiki-1.0.2/PKG-INFO` & `myswiki-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myswiki
-Version: 1.0.2
+Version: 2.0.0
 Summary: A program for searching and reading Wikipedia articles in multiple languages
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -23,15 +23,15 @@
 - Wikipedia: pip install wikipedia
 - pyttsx3: pip install pyttsx3
 
 ***
 
 ### Использование
 
->Запустите скрипт в вашей среде разработки или в терминале.
+> Запустите скрипт в вашей среде разработки или в терминале.
 > Выберите язык (русский или английский), на котором вы хотите искать и читать статьи.
 > Введите запрос для поиска статьи.
 > Выберите статью из результатов поиска.
 > При желании, выберите опцию чтения текста статьи с помощью речи.
 ***
 
 ### Использование в коде
```

### Comparing `myswiki-1.0.2/README.md` & `myswiki-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - Wikipedia: pip install wikipedia
 - pyttsx3: pip install pyttsx3
 
 ***
 
 ### Использование
 
->Запустите скрипт в вашей среде разработки или в терминале.
+> Запустите скрипт в вашей среде разработки или в терминале.
 > Выберите язык (русский или английский), на котором вы хотите искать и читать статьи.
 > Введите запрос для поиска статьи.
 > Выберите статью из результатов поиска.
 > При желании, выберите опцию чтения текста статьи с помощью речи.
 ***
 
 ### Использование в коде
```

### Comparing `myswiki-1.0.2/myswiki.egg-info/PKG-INFO` & `myswiki-2.0.0/myswiki.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myswiki
-Version: 1.0.2
+Version: 2.0.0
 Summary: A program for searching and reading Wikipedia articles in multiple languages
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -23,15 +23,15 @@
 - Wikipedia: pip install wikipedia
 - pyttsx3: pip install pyttsx3
 
 ***
 
 ### Использование
 
->Запустите скрипт в вашей среде разработки или в терминале.
+> Запустите скрипт в вашей среде разработки или в терминале.
 > Выберите язык (русский или английский), на котором вы хотите искать и читать статьи.
 > Введите запрос для поиска статьи.
 > Выберите статью из результатов поиска.
 > При желании, выберите опцию чтения текста статьи с помощью речи.
 ***
 
 ### Использование в коде
```

### Comparing `myswiki-1.0.2/myswiki.py` & `myswiki-2.0.0/myswiki.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,94 +1,96 @@
 import wikipedia
 import pyttsx3
 
-messages = {
-    'ru': {
-        'choose_language': 'Выберите язык для поиска и прочтения статьи (ru/en): ',
-        'invalid_language': 'Пожалуйста, выберите корректный язык (ru/en).',
-        'enter_query': 'Что вы хотите узнать?\n',
-        'no_results': 'Ничего не найдено. Пожалуйста, попробуйте другой запрос.',
-        'input_article_number': '\nВведите номер статьи для прочтения (или 0 для выхода): ',
-        'invalid_article_number': 'Пожалуйста, введите корректный номер статьи.',
-        'read_text': 'Хотите чтобы я вам прочитал текст?\n(yes/no) ',
-        'http_error': 'Ошибка: превышено время ожидания запроса к Википедии.'
-    },
-    'en': {
-        'choose_language': 'Choose language for searching and reading articles (ru/en): ',
-        'invalid_language': 'Please choose a valid language (ru/en).',
-        'enter_query': 'What do you want to know?\n',
-        'no_results': 'Nothing found. Please try another query.',
-        'input_article_number': '\nEnter the article number to read (or 0 to exit): ',
-        'invalid_article_number': 'Please enter a valid article number.',
-        'read_text': 'Do you want me to read the text?\n(yes/no) ',
-        'http_error': 'Error: Wikipedia request timeout.'
-    }
-}
-
-
-def wrap_text(text, line_length=150):
-    wrapped_text = ""
-    words = text.split()
-    line = ""
-    for word in words:
-        if len(line) + len(word) <= line_length:
-            line += word + " "
-        else:
-            wrapped_text += line.strip() + '\n'
-            line = word + " "
-    wrapped_text += line.strip()
-    return wrapped_text
-
-
-def get_article_summary(query, language):
-    wikipedia.set_lang(language)
-    try:
-        summary = wikipedia.summary(query)
-        return wrap_text(summary)
-    except wikipedia.exceptions.DisambiguationError:
-        return "Неоднозначный запрос. Пожалуйста, уточните ваш запрос."
-    except wikipedia.exceptions.PageError:
-        return "Страница не найдена. Пожалуйста, попробуйте другой запрос."
-
-
-def main():
-    language = input(messages['en']['choose_language']).lower()
-    while language not in ('ru', 'en'):
-        print(messages['en']['invalid_language'])
-        language = input(messages['en']['choose_language']).lower()
 
-    query = input(messages[language]['enter_query'])
-    try:
-        wikipedia.set_lang(language)
-        search_results = wikipedia.search(query)
-        if not search_results:
-            print(messages[language]['no_results'])
-            return
-        article_idx = select_article(search_results, language)  # Passing language to select_article
-        if article_idx is None:
-            return
-        print("\n")
-        if input(messages[language]['read_text']).lower() == 'yes':
-            say = pyttsx3.init()
-            say.say(get_article_summary(search_results[article_idx], language))
-            print("\n")
-            print(get_article_summary(search_results[article_idx], language))
-            say.runAndWait()
-        else:
-            print(get_article_summary(search_results[article_idx], language))
-    except wikipedia.exceptions.HTTPTimeoutError:
-        print(messages[language]['http_error'])
-
-def select_article(search_results, language):  # Added 'language' as parameter
-    for idx, result in enumerate(search_results, start=1):
-        print(f"{idx}. {result}")
-    while True:
+class WikiReader:
+    def __init__(self):
+        self.messages = {
+            'ru': {
+                'choose_language': 'Выберите язык для поиска и прочтения статьи (ru/en): ',
+                'invalid_language': 'Пожалуйста, выберите корректный язык (ru/en).',
+                'enter_query': 'Что вы хотите узнать?\n',
+                'no_results': 'Ничего не найдено. Пожалуйста, попробуйте другой запрос.',
+                'input_article_number': '\nВведите номер статьи для прочтения (или 0 для выхода): ',
+                'invalid_article_number': 'Пожалуйста, введите корректный номер статьи.',
+                'read_text': 'Хотите чтобы я вам прочитал текст?\n(yes/no) ',
+                'http_error': 'Ошибка: превышено время ожидания запроса к Википедии.'
+            },
+            'en': {
+                'choose_language': 'Choose language for searching and reading articles (ru/en): ',
+                'invalid_language': 'Please choose a valid language (ru/en).',
+                'enter_query': 'What do you want to know?\n',
+                'no_results': 'Nothing found. Please try another query.',
+                'input_article_number': '\nEnter the article number to read (or 0 to exit): ',
+                'invalid_article_number': 'Please enter a valid article number.',
+                'read_text': 'Do you want me to read the text?\n(yes/no) ',
+                'http_error': 'Error: Wikipedia request timeout.'
+            }
+        }
+
+        self.language = input(self.messages['en']['choose_language']).lower()
+        while self.language not in ('ru', 'en'):
+            print(self.messages['en']['invalid_language'])
+            self.language = input(self.messages['en']['choose_language']).lower()
+
+        self.query = input(self.messages[self.language]['enter_query'])
         try:
-            choice = int(input(messages[language]['input_article_number']))  # Using 'language' variable
-            if choice == 0:
-                return None
-            elif choice < 1 or choice > len(search_results):
-                print(messages[language]['invalid_article_number'])
+            wikipedia.set_lang(self.language)
+            search_results = wikipedia.search(self.query)
+            if not search_results:
+                print(self.messages[self.language]['no_results'])
+                return
+            article_idx = self.select_article(search_results, self.language)
+            if article_idx is None:
+                return
+            print("\n")
+            if input(self.messages[self.language]['read_text']).lower() == 'yes':
+                say = pyttsx3.init()
+                say.say(self.get_article_summary(search_results[article_idx], self.language))
+                print("\n")
+                print(self.get_article_summary(search_results[article_idx], self.language))
+                say.runAndWait()
+            else:
+                print(self.get_article_summary(search_results[article_idx], self.language))
+        except wikipedia.exceptions.HTTPTimeoutError:
+            print(self.messages[self.language]['http_error'])
+
+    def wrap_text(self, text, line_length=150):
+        wrapped_text = ""
+        words = text.split()
+        line = ""
+        for word in words:
+            if len(line) + len(word) <= line_length:
+                line += word + " "
             else:
-                return choice - 1
-        except ValueError:
-            print("Please enter the number.")
+                wrapped_text += line.strip() + '\n'
+                line = word + " "
+        wrapped_text += line.strip()
+        return wrapped_text
+
+    def get_article_summary(self, query, language):
+        wikipedia.set_lang(language)
+        try:
+            summary = wikipedia.summary(query)
+            return self.wrap_text(summary)
+        except wikipedia.exceptions.DisambiguationError:
+            return "Неоднозначный запрос. Пожалуйста, уточните ваш запрос."
+        except wikipedia.exceptions.PageError:
+            return "Страница не найдена. Пожалуйста, попробуйте другой запрос."
+
+    def select_article(self, search_results, language):
+        for idx, result in enumerate(search_results, start=1):
+            print(f"{idx}. {result}")
+        while True:
+            try:
+                choice = int(input(self.messages[language]['input_article_number']))
+                if choice == 0:
+                    return None
+                elif choice < 1 or choice > len(search_results):
+                    print(self.messages[language]['invalid_article_number'])
+                else:
+                    return choice - 1
+            except ValueError:
+                print("Please enter the number.")
+
+
+WikiReader()
```

