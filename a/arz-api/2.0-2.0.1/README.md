# Comparing `tmp/arz_api-2.0.tar.gz` & `tmp/arz_api-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arz_api-2.0.tar", last modified: Sat May  4 17:17:07 2024, max compression
+gzip compressed data, was "arz_api-2.0.1.tar", last modified: Tue May  7 14:18:17 2024, max compression
```

## Comparing `arz_api-2.0.tar` & `arz_api-2.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 17:17:07.107349 arz_api-2.0/
--rw-rw-rw-   0        0        0     1089 2023-11-08 20:12:48.000000 arz_api-2.0/LICENSE
--rw-rw-rw-   0        0        0     1737 2024-05-04 17:17:07.106350 arz_api-2.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-11-08 20:15:07.000000 arz_api-2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 17:17:07.058795 arz_api-2.0/arz_api/
--rw-rw-rw-   0        0        0     3604 2023-08-04 21:34:31.000000 arz_api-2.0/arz_api/__init__.py
--rw-rw-rw-   0        0        0    29414 2024-05-04 16:59:06.000000 arz_api-2.0/arz_api/api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 17:17:07.090105 arz_api-2.0/arz_api/bypass_antibot/
--rw-rw-rw-   0        0        0       21 2023-05-31 18:16:38.000000 arz_api-2.0/arz_api/bypass_antibot/__init__.py
--rw-rw-rw-   0        0        0    35306 2023-05-31 19:17:18.000000 arz_api-2.0/arz_api/bypass_antibot/script.py
--rw-rw-rw-   0        0        0      247 2024-05-03 19:46:30.000000 arz_api-2.0/arz_api/consts.py
--rw-rw-rw-   0        0        0      563 2023-07-08 19:21:59.000000 arz_api-2.0/arz_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-04 17:17:07.101366 arz_api-2.0/arz_api/models/
--rw-rw-rw-   0        0        0      112 2023-05-31 18:48:38.000000 arz_api-2.0/arz_api/models/__init__.py
--rw-rw-rw-   0        0        0     4126 2024-05-03 20:23:22.000000 arz_api-2.0/arz_api/models/category_object.py
--rw-rw-rw-   0        0        0     4794 2024-05-03 18:06:11.000000 arz_api-2.0/arz_api/models/member_object.py
--rw-rw-rw-   0        0        0      512 2023-07-08 10:56:45.000000 arz_api-2.0/arz_api/models/other.py
--rw-rw-rw-   0        0        0     5600 2024-05-03 18:16:32.000000 arz_api-2.0/arz_api/models/post_object.py
--rw-rw-rw-   0        0        0     5513 2024-05-03 20:50:47.000000 arz_api-2.0/arz_api/models/thread_object.py
-drwxrwxrwx   0        0        0        0 2024-05-04 17:17:07.104359 arz_api-2.0/arz_api.egg-info/
--rw-rw-rw-   0        0        0     1737 2024-05-04 17:17:06.000000 arz_api-2.0/arz_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2024-05-04 17:17:06.000000 arz_api-2.0/arz_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 17:17:06.000000 arz_api-2.0/arz_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-04 17:17:06.000000 arz_api-2.0/arz_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-04 17:17:06.000000 arz_api-2.0/arz_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 17:17:07.110337 arz_api-2.0/setup.cfg
--rw-rw-rw-   0        0        0     1847 2024-05-04 17:16:40.000000 arz_api-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:18:17.752351 arz_api-2.0.1/
+-rw-rw-rw-   0        0        0     1089 2023-11-08 20:12:48.000000 arz_api-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1739 2024-05-07 14:18:17.750356 arz_api-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-11-08 20:15:07.000000 arz_api-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 14:18:17.690699 arz_api-2.0.1/arz_api/
+-rw-rw-rw-   0        0        0     3604 2023-08-04 21:34:31.000000 arz_api-2.0.1/arz_api/__init__.py
+-rw-rw-rw-   0        0        0    29486 2024-05-07 14:11:54.000000 arz_api-2.0.1/arz_api/api.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:18:17.728186 arz_api-2.0.1/arz_api/bypass_antibot/
+-rw-rw-rw-   0        0        0       21 2023-05-31 18:16:38.000000 arz_api-2.0.1/arz_api/bypass_antibot/__init__.py
+-rw-rw-rw-   0        0        0    35306 2023-05-31 19:17:18.000000 arz_api-2.0.1/arz_api/bypass_antibot/script.py
+-rw-rw-rw-   0        0        0      247 2024-05-03 19:46:30.000000 arz_api-2.0.1/arz_api/consts.py
+-rw-rw-rw-   0        0        0      563 2023-07-08 19:21:59.000000 arz_api-2.0.1/arz_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:18:17.744370 arz_api-2.0.1/arz_api/models/
+-rw-rw-rw-   0        0        0      112 2023-05-31 18:48:38.000000 arz_api-2.0.1/arz_api/models/__init__.py
+-rw-rw-rw-   0        0        0     4126 2024-05-03 20:23:22.000000 arz_api-2.0.1/arz_api/models/category_object.py
+-rw-rw-rw-   0        0        0     4794 2024-05-03 18:06:11.000000 arz_api-2.0.1/arz_api/models/member_object.py
+-rw-rw-rw-   0        0        0      512 2023-07-08 10:56:45.000000 arz_api-2.0.1/arz_api/models/other.py
+-rw-rw-rw-   0        0        0     5600 2024-05-03 18:16:32.000000 arz_api-2.0.1/arz_api/models/post_object.py
+-rw-rw-rw-   0        0        0     5513 2024-05-03 20:50:47.000000 arz_api-2.0.1/arz_api/models/thread_object.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:18:17.748355 arz_api-2.0.1/arz_api.egg-info/
+-rw-rw-rw-   0        0        0     1739 2024-05-07 14:18:17.000000 arz_api-2.0.1/arz_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-05-07 14:18:17.000000 arz_api-2.0.1/arz_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:18:17.000000 arz_api-2.0.1/arz_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-07 14:18:17.000000 arz_api-2.0.1/arz_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 14:18:17.000000 arz_api-2.0.1/arz_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 14:18:17.755360 arz_api-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1849 2024-05-07 14:17:31.000000 arz_api-2.0.1/setup.py
```

### Comparing `arz_api-2.0/LICENSE` & `arz_api-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arz_api-2.0/PKG-INFO` & `arz_api-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arz_api
-Version: 2.0
+Version: 2.0.1
 Summary: Модуль для взаимодействия с форумом без Xenforo ключей
 Home-page: https://github.com/TastyBread123/Arizona-API/
 Author: TastyBread123
 Author-email: ermakovglebyt@gmail.com
 Project-URL: Documentation, https://tastybread123.github.io/Arizona-API/arz_api.html
 Keywords: python xenforo arizona roleplay samp gta
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `arz_api-2.0/arz_api/__init__.py` & `arz_api-2.0.1/arz_api/__init__.py`

 * *Files identical despite different names*

### Comparing `arz_api-2.0/arz_api/api.py` & `arz_api-2.0.1/arz_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,39 +51,39 @@
         """Получить токен CSRF"""
         return BeautifulSoup(self.session.get(f"{MAIN_URL}/help/terms/").content, 'lxml').find('html')['data-csrf']
 
 
     def get_category(self, category_id: int) -> Category:
         """Найти раздел по ID"""
 
-        request = self.session.get(f"{MAIN_URL}/forums/{category_id}?&_xfResponseType=json&_xfToken={self.token}").json()
+        request = self.session.get(f"{MAIN_URL}/forums/{category_id}?_xfResponseType=json&_xfToken={self.token}").json()
         if request['status'] == 'error':
             return None
 
         content = unescape(request['html']['content'])
         content = BeautifulSoup(content, 'lxml')
 
-        title = request['html']['title']
+        title = unescape(request['html']['title'])
         try: pages_count = int(content.find_all('li', {'class': 'pageNav-page'})[-1].text)
         except IndexError: pages_count = 1
 
         return Category(self, category_id, title, pages_count)
     
     
     def get_member(self, user_id: int) -> Member:
         """Найти пользователя по ID (возвращает либо Member, либо None (если профиль закрыт / не существует))"""
 
-        request = self.session.get(f"{MAIN_URL}/members/{user_id}?&_xfResponseType=json&_xfToken={self.token}").json()
+        request = self.session.get(f"{MAIN_URL}/members/{user_id}?_xfResponseType=json&_xfToken={self.token}").json()
         if request['status'] == 'error':
             return None
 
         content = unescape(request['html']['content'])
         content = BeautifulSoup(content, 'lxml')
 
-        username = request['html']['title']
+        username = unescape(request['html']['title'])
 
         roles = []
         for i in content.find('div', {'class': 'memberHeader-banners'}).children:
             if i.text != '\n': roles.append(i.text)
 
         try: user_title = content.find('span', {'class': 'userTitle'}).text
         except AttributeError: user_title = None
@@ -94,15 +94,15 @@
         reactions_count = int(content.find('dl', {'class': 'pairs pairs--rows pairs--rows--centered'}).find('dd').text.strip().replace(',', ''))
         trophies_count = int(content.find('a', {'href': f'/members/{user_id}/trophies'}).text.strip().replace(',', ''))
         
         return Member(self, user_id, username, user_title, avatar, roles, messages_count, reactions_count, trophies_count)
     
 
     def get_thread(self, thread_id: int):
-        request = self.session.get(f"{MAIN_URL}/threads/{thread_id}/page-1?&_xfResponseType=json&_xfToken={self.token}").json()
+        request = self.session.get(f"{MAIN_URL}/threads/{thread_id}/page-1?_xfResponseType=json&_xfToken={self.token}").json()
         if request['status'] == 'error':
             return None
         
         if request.get('redirect') is not None:
             return self.get_thread(request['redirect'].strip(MAIN_URL).split('/')[1])
 
         content = unescape(request['html']['content'])
@@ -112,17 +112,21 @@
 
         creator_id = content.find('a', {'class': 'username'})
         try: creator = self.get_member(int(creator_id['data-user-id']))
         except: creator = Member(self, int(creator_id['data-user-id']), content.find('a', {'class': 'username'}).text, None, None, None, None, None, None)
         
         create_date = int(content.find('time')['data-time'])
         
-        title = request['html']['title']
-        try: prefix = content_h1.find('span', {'class': 'label'}).text
-        except: prefix = ""
+        try:
+            prefix = content_h1.find('span', {'class': 'label'}).text
+            title = content_h1.text.strip(prefix).strip()
+
+        except AttributeError:
+            prefix = ""
+            title = content_h1.text
         thread_content_html = content.find('div', {'class': 'bbWrapper'})
         thread_content = thread_content_html.text
         
         try: pages_count = int(content.find_all('li', {'class': 'pageNav-page'})[-1].text)
         except IndexError: pages_count = 1
 
         is_closed = False
@@ -539,31 +543,30 @@
         """
 
         content = BeautifulSoup(self.session.get(f"{MAIN_URL}/threads/{thread_id}/page-1").content, 'lxml')
         thread_post_id = content.find('article', {'id': compile('js-post-*')})['id'].strip('js-post-')
         return self.session.post(f"{MAIN_URL}/posts/{thread_post_id}/edit", {"message_html": message_html, "message": message_html, "_xfToken": self.token})
     
 
-    def edit_thread_info(self, thread_id: int, title: str = None, prefix_id: int = None, sticky: bool = True, opened: bool = True) -> Response:
-        """Изменить заголовок и/или префикс темы
+    def edit_thread_info(self, thread_id: int, title: str, prefix_id: int = None, sticky: bool = True, opened: bool = True) -> Response:
+        """Изменить статус темы, ее префикс и название
 
         Attributes:
             thread_id (int): ID темы
             title (str): Новое название
             prefix_id (int): Новый ID префикса
             sticky (bool): Закрепить (True - закреп / False - не закреп)
             opened (bool): Открыть/закрыть тему (True - открыть / False - закрыть)
         
         Returns:
             Объект Response модуля requests
         """
         
-        data = {"_xfToken": self.token}
+        data = {"_xfToken": self.token, 'title': title}
 
-        if title is not None: data.update({'title': title})
         if prefix_id is not None: data.update({'prefix_id': prefix_id})
         if opened: data.update({"discussion_open": 1})
         if sticky: data.update({"sticky": 1})
 
         return self.session.post(f"{MAIN_URL}/threads/{thread_id}/edit", data)
```

### Comparing `arz_api-2.0/arz_api/bypass_antibot/script.py` & `arz_api-2.0.1/arz_api/bypass_antibot/script.py`

 * *Files identical despite different names*

### Comparing `arz_api-2.0/arz_api/exceptions.py` & `arz_api-2.0.1/arz_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `arz_api-2.0/arz_api/models/category_object.py` & `arz_api-2.0.1/arz_api/models/category_object.py`

 * *Files identical despite different names*

### Comparing `arz_api-2.0/arz_api/models/member_object.py` & `arz_api-2.0.1/arz_api/models/member_object.py`

 * *Files identical despite different names*

### Comparing `arz_api-2.0/arz_api/models/other.py` & `arz_api-2.0.1/arz_api/models/other.py`

 * *Files identical despite different names*

### Comparing `arz_api-2.0/arz_api/models/post_object.py` & `arz_api-2.0.1/arz_api/models/post_object.py`

 * *Files identical despite different names*

### Comparing `arz_api-2.0/arz_api/models/thread_object.py` & `arz_api-2.0.1/arz_api/models/thread_object.py`

 * *Files identical despite different names*

### Comparing `arz_api-2.0/arz_api.egg-info/PKG-INFO` & `arz_api-2.0.1/arz_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arz_api
-Version: 2.0
+Version: 2.0.1
 Summary: Модуль для взаимодействия с форумом без Xenforo ключей
 Home-page: https://github.com/TastyBread123/Arizona-API/
 Author: TastyBread123
 Author-email: ermakovglebyt@gmail.com
 Project-URL: Documentation, https://tastybread123.github.io/Arizona-API/arz_api.html
 Keywords: python xenforo arizona roleplay samp gta
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `arz_api-2.0/arz_api.egg-info/SOURCES.txt` & `arz_api-2.0.1/arz_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arz_api-2.0/setup.py` & `arz_api-2.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name='arz_api',
-  version='2.0',
+  version='2.0.1',
   author='TastyBread123',
   author_email='ermakovglebyt@gmail.com',
   description='Модуль для взаимодействия с форумом без Xenforo ключей',
   long_description="""# Arizona-API
 API для взаимодействия с ресурсами Arizona без необходимости в получении API ключа xenforo у администраторов форума. Вы можете просто найти ваши куки (рекомендую для этого отдельные расширения) и начинать разработку!
 
 # Описание проекта
```

