# Comparing `tmp/npdtools-fx-1.0.1.tar.gz` & `tmp/npdtools_fx-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npdtools-fx-1.0.1.tar", last modified: Tue May  7 02:40:43 2024, max compression
+gzip compressed data, was "npdtools_fx-1.0.2.tar", last modified: Tue May  7 12:22:31 2024, max compression
```

## Comparing `npdtools-fx-1.0.1.tar` & `npdtools_fx-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 02:40:43.889871 npdtools-fx-1.0.1/
--rw-rw-rw-   0        0        0    17098 2024-05-07 02:18:22.000000 npdtools-fx-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    11878 2024-05-07 02:40:43.889871 npdtools-fx-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    11305 2024-05-07 02:37:33.000000 npdtools-fx-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 02:40:43.842597 npdtools-fx-1.0.1/npdtools/
--rw-rw-rw-   0        0        0       53 2024-05-07 02:18:22.000000 npdtools-fx-1.0.1/npdtools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:40:43.858213 npdtools-fx-1.0.1/npdtools/errors/
--rw-rw-rw-   0        0        0      510 2024-05-07 02:18:22.000000 npdtools-fx-1.0.1/npdtools/errors/FNSError.py
--rw-rw-rw-   0        0        0       47 2024-05-07 02:18:22.000000 npdtools-fx-1.0.1/npdtools/errors/__init__.py
--rw-rw-rw-   0        0        0      154 2024-05-07 02:18:22.000000 npdtools-fx-1.0.1/npdtools/helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:40:43.858213 npdtools-fx-1.0.1/npdtools/modules/
--rw-rw-rw-   0        0        0      410 2024-05-07 02:18:22.000000 npdtools-fx-1.0.1/npdtools/modules/__init__.py
--rw-rw-rw-   0        0        0     5376 2024-05-07 02:36:49.000000 npdtools-fx-1.0.1/npdtools/modules/base.py
--rw-rw-rw-   0        0        0     7944 2024-05-07 02:20:47.000000 npdtools-fx-1.0.1/npdtools/modules/income.py
--rw-rw-rw-   0        0        0    11898 2024-05-07 02:18:22.000000 npdtools-fx-1.0.1/npdtools/modules/invoice.py
--rw-rw-rw-   0        0        0      117 2024-05-07 02:18:22.000000 npdtools-fx-1.0.1/npdtools/settings.py
--rw-rw-rw-   0        0        0     3719 2024-05-07 02:24:01.000000 npdtools-fx-1.0.1/npdtools/token_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:40:43.873844 npdtools-fx-1.0.1/npdtools/types/
--rw-rw-rw-   0        0        0      403 2024-05-07 02:18:22.000000 npdtools-fx-1.0.1/npdtools/types/__init__.py
--rw-rw-rw-   0        0        0     4169 2024-05-07 02:18:22.000000 npdtools-fx-1.0.1/npdtools/types/entity.py
--rw-rw-rw-   0        0        0     8799 2024-05-07 02:18:22.000000 npdtools-fx-1.0.1/npdtools/types/income.py
--rw-rw-rw-   0        0        0     9832 2024-05-07 02:18:22.000000 npdtools-fx-1.0.1/npdtools/types/invoice.py
--rw-rw-rw-   0        0        0     1243 2024-05-07 02:18:22.000000 npdtools-fx-1.0.1/npdtools/types/service.py
-drwxrwxrwx   0        0        0        0 2024-05-07 02:40:43.889871 npdtools-fx-1.0.1/npdtools_fx.egg-info/
--rw-rw-rw-   0        0        0    11878 2024-05-07 02:40:43.000000 npdtools-fx-1.0.1/npdtools_fx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2024-05-07 02:40:43.000000 npdtools-fx-1.0.1/npdtools_fx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 02:40:43.000000 npdtools-fx-1.0.1/npdtools_fx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-07 02:40:43.000000 npdtools-fx-1.0.1/npdtools_fx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-07 02:40:43.000000 npdtools-fx-1.0.1/npdtools_fx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 02:40:43.889871 npdtools-fx-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1146 2024-05-07 02:36:08.000000 npdtools-fx-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:22:31.046722 npdtools_fx-1.0.2/
+-rw-rw-rw-   0        0        0    17098 2024-05-07 02:18:22.000000 npdtools_fx-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    12141 2024-05-07 12:22:31.044211 npdtools_fx-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11411 2024-05-07 12:19:52.000000 npdtools_fx-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 12:22:31.008562 npdtools_fx-1.0.2/npdtools/
+-rw-rw-rw-   0        0        0       53 2024-05-07 02:18:22.000000 npdtools_fx-1.0.2/npdtools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:22:31.010432 npdtools_fx-1.0.2/npdtools/errors/
+-rw-rw-rw-   0        0        0      510 2024-05-07 02:18:22.000000 npdtools_fx-1.0.2/npdtools/errors/FNSError.py
+-rw-rw-rw-   0        0        0       47 2024-05-07 02:18:22.000000 npdtools_fx-1.0.2/npdtools/errors/__init__.py
+-rw-rw-rw-   0        0        0      154 2024-05-07 02:18:22.000000 npdtools_fx-1.0.2/npdtools/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:22:31.014197 npdtools_fx-1.0.2/npdtools/modules/
+-rw-rw-rw-   0        0        0      410 2024-05-07 02:18:22.000000 npdtools_fx-1.0.2/npdtools/modules/__init__.py
+-rw-rw-rw-   0        0        0     5383 2024-05-07 12:17:35.000000 npdtools_fx-1.0.2/npdtools/modules/base.py
+-rw-rw-rw-   0        0        0     7944 2024-05-07 02:20:47.000000 npdtools_fx-1.0.2/npdtools/modules/income.py
+-rw-rw-rw-   0        0        0    11898 2024-05-07 02:18:22.000000 npdtools_fx-1.0.2/npdtools/modules/invoice.py
+-rw-rw-rw-   0        0        0      117 2024-05-07 02:18:22.000000 npdtools_fx-1.0.2/npdtools/settings.py
+-rw-rw-rw-   0        0        0     3719 2024-05-07 02:24:01.000000 npdtools_fx-1.0.2/npdtools/token_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:22:31.020217 npdtools_fx-1.0.2/npdtools/types/
+-rw-rw-rw-   0        0        0      403 2024-05-07 02:18:22.000000 npdtools_fx-1.0.2/npdtools/types/__init__.py
+-rw-rw-rw-   0        0        0     4169 2024-05-07 02:18:22.000000 npdtools_fx-1.0.2/npdtools/types/entity.py
+-rw-rw-rw-   0        0        0     8799 2024-05-07 02:18:22.000000 npdtools_fx-1.0.2/npdtools/types/income.py
+-rw-rw-rw-   0        0        0     9832 2024-05-07 02:18:22.000000 npdtools_fx-1.0.2/npdtools/types/invoice.py
+-rw-rw-rw-   0        0        0     1243 2024-05-07 02:18:22.000000 npdtools_fx-1.0.2/npdtools/types/service.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:22:31.041390 npdtools_fx-1.0.2/npdtools_fx.egg-info/
+-rw-rw-rw-   0        0        0    12141 2024-05-07 12:22:30.000000 npdtools_fx-1.0.2/npdtools_fx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2024-05-07 12:22:30.000000 npdtools_fx-1.0.2/npdtools_fx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 12:22:30.000000 npdtools_fx-1.0.2/npdtools_fx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-07 12:22:30.000000 npdtools_fx-1.0.2/npdtools_fx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 12:22:30.000000 npdtools_fx-1.0.2/npdtools_fx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 12:22:31.046903 npdtools_fx-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2024-05-07 12:20:29.000000 npdtools_fx-1.0.2/setup.py
```

### Comparing `npdtools-fx-1.0.1/LICENSE` & `npdtools_fx-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `npdtools-fx-1.0.1/PKG-INFO` & `npdtools_fx-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 Metadata-Version: 2.1
 Name: npdtools-fx
-Version: 1.0.1
+Version: 1.0.2
 Summary: tool for work with FNS API
 Home-page: https://gitlab.com/whiteapfel/npdtools
 Author: WhiteApfel
 Author-email: white@pfel.ru
 License: MPL 2.0
 Project-URL: Документация, https://npd-tools.readthedocs.io/en/latest/
 Project-URL: Исходники, https://gitlab.com/whiteapfel/npdtools/
 Project-URL: По вопросам, https://t.me/apfel
 Keywords: FNS API wrapper nalog налог ФНС самозанятость
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing>=3.7.4.3; python_version < "3.5"
+Requires-Dist: httpx~=0.27.0
+Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: pydantic>=2.0.2
 
 # NPDTools
 
 Исправления:
+* Исправлено название ключа `refreshToken`
 * Использование стандартного `json` модуля
 * Установка модуля `typing` только для python<3.5 (возможно стоит совсем убрать)
 * Обновлен модуль `httpx` до 0.27.0
+* Обновлен юзерагент
 * Удалены print'ы
 
 Ищешь инструмент для удобного декларирования доходов? 
 Хочешь автоматизировать выдачу чеков клиентам?
 Надоело заходить в Мой налог? Надоедает проверять, что каждый приход зарегистрирован в налоговой?
 Боишься ошибиться и получить безжалостный удар от ФНС кнутом без пряника?
```

### Comparing `npdtools-fx-1.0.1/README.md` & `npdtools_fx-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # NPDTools
 
 Исправления:
+* Исправлено название ключа `refreshToken`
 * Использование стандартного `json` модуля
 * Установка модуля `typing` только для python<3.5 (возможно стоит совсем убрать)
 * Обновлен модуль `httpx` до 0.27.0
+* Обновлен юзерагент
 * Удалены print'ы
 
 Ищешь инструмент для удобного декларирования доходов? 
 Хочешь автоматизировать выдачу чеков клиентам?
 Надоело заходить в Мой налог? Надоедает проверять, что каждый приход зарегистрирован в налоговой?
 Боишься ошибиться и получить безжалостный удар от ФНС кнутом без пряника?
```

### Comparing `npdtools-fx-1.0.1/npdtools/modules/base.py` & `npdtools_fx-1.0.2/npdtools/modules/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,36 +122,35 @@
         auth_data = {
             "deviceInfo": {
                 "appVersion": "1.0.0",
                 "sourceDeviceId": tokens.device,
                 "sourceType": "WEB",
                 "metaDetails": {
                     "userAgent": (
-                        "Mozilla/5.0 (X11; rv:109.0) Gecko/20100101 Firefox/109.0"
-                        " npdtools"
+                        "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36"
                     )
                 },
             },
         }
 
         if refresh_token is not None:
             auth_data |= {
-                "refresh_token": refresh_token,
+                "refreshToken": refresh_token,
             }
         else:
             auth_data |= {
                 "username": inn,
                 "password": password,
             }
 
         response = await self._request(
             method="POST",
             url="/auth/token" if refresh_token is not None else "/auth/lkfl",
             json=auth_data,
-            headers={"referer": "https://lknpd.nalog.ru/Sales"},
+            headers={"referer": "https://lknpd.nalog.ru/sales"},
             auth_required=False,
         )
 
         r_data = response.json()
         tokens.access = (
             r_data["token"],
             datetime.strptime(
```

### Comparing `npdtools-fx-1.0.1/npdtools/modules/income.py` & `npdtools_fx-1.0.2/npdtools/modules/income.py`

 * *Files identical despite different names*

### Comparing `npdtools-fx-1.0.1/npdtools/modules/invoice.py` & `npdtools_fx-1.0.2/npdtools/modules/invoice.py`

 * *Files identical despite different names*

### Comparing `npdtools-fx-1.0.1/npdtools/token_manager.py` & `npdtools_fx-1.0.2/npdtools/token_manager.py`

 * *Files identical despite different names*

### Comparing `npdtools-fx-1.0.1/npdtools/types/entity.py` & `npdtools_fx-1.0.2/npdtools/types/entity.py`

 * *Files identical despite different names*

### Comparing `npdtools-fx-1.0.1/npdtools/types/income.py` & `npdtools_fx-1.0.2/npdtools/types/income.py`

 * *Files identical despite different names*

### Comparing `npdtools-fx-1.0.1/npdtools/types/invoice.py` & `npdtools_fx-1.0.2/npdtools/types/invoice.py`

 * *Files identical despite different names*

### Comparing `npdtools-fx-1.0.1/npdtools/types/service.py` & `npdtools_fx-1.0.2/npdtools/types/service.py`

 * *Files identical despite different names*

### Comparing `npdtools-fx-1.0.1/npdtools_fx.egg-info/PKG-INFO` & `npdtools_fx-1.0.2/npdtools_fx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 Metadata-Version: 2.1
 Name: npdtools-fx
-Version: 1.0.1
+Version: 1.0.2
 Summary: tool for work with FNS API
 Home-page: https://gitlab.com/whiteapfel/npdtools
 Author: WhiteApfel
 Author-email: white@pfel.ru
 License: MPL 2.0
 Project-URL: Документация, https://npd-tools.readthedocs.io/en/latest/
 Project-URL: Исходники, https://gitlab.com/whiteapfel/npdtools/
 Project-URL: По вопросам, https://t.me/apfel
 Keywords: FNS API wrapper nalog налог ФНС самозанятость
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing>=3.7.4.3; python_version < "3.5"
+Requires-Dist: httpx~=0.27.0
+Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: pydantic>=2.0.2
 
 # NPDTools
 
 Исправления:
+* Исправлено название ключа `refreshToken`
 * Использование стандартного `json` модуля
 * Установка модуля `typing` только для python<3.5 (возможно стоит совсем убрать)
 * Обновлен модуль `httpx` до 0.27.0
+* Обновлен юзерагент
 * Удалены print'ы
 
 Ищешь инструмент для удобного декларирования доходов? 
 Хочешь автоматизировать выдачу чеков клиентам?
 Надоело заходить в Мой налог? Надоедает проверять, что каждый приход зарегистрирован в налоговой?
 Боишься ошибиться и получить безжалостный удар от ФНС кнутом без пряника?
```

### Comparing `npdtools-fx-1.0.1/npdtools_fx.egg-info/SOURCES.txt` & `npdtools_fx-1.0.2/npdtools_fx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `npdtools-fx-1.0.1/setup.py` & `npdtools_fx-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 def requirements():
     with open("requirements.txt", "r") as req:
         return [r for r in req.read().split("\n") if r]
 
 
 setup(
     name="npdtools-fx",
-    version=environ.get("CI_COMMIT_TAG", "1.0.1").replace("v", ""),
+    version=environ.get("CI_COMMIT_TAG", "1.0.2").replace("v", ""),
     packages=["npdtools", "npdtools.types", "npdtools.errors", "npdtools.modules"],
     url="https://gitlab.com/whiteapfel/npdtools",
     license="MPL 2.0",
     author="WhiteApfel",
     author_email="white@pfel.ru",
     description="tool for work with FNS API",
     install_requires=requirements(),
```

