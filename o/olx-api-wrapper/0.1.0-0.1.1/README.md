# Comparing `tmp/olx-api-wrapper-0.1.0.tar.gz` & `tmp/olx-api-wrapper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olx-api-wrapper-0.1.0.tar", last modified: Mon May  6 19:17:27 2024, max compression
+gzip compressed data, was "olx-api-wrapper-0.1.1.tar", last modified: Tue May  7 07:11:07 2024, max compression
```

## Comparing `olx-api-wrapper-0.1.0.tar` & `olx-api-wrapper-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 19:17:27.510775 olx-api-wrapper-0.1.0/
--rw-rw-rw-   0        0        0     1071 2024-05-06 17:28:53.000000 olx-api-wrapper-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     8762 2024-05-06 19:17:27.509774 olx-api-wrapper-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8254 2024-05-06 17:30:11.000000 olx-api-wrapper-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 19:17:27.488615 olx-api-wrapper-0.1.0/olx/
--rw-rw-rw-   0        0        0      488 2024-05-06 16:20:24.000000 olx-api-wrapper-0.1.0/olx/__init__.py
--rw-rw-rw-   0        0        0     1121 2024-05-06 16:01:53.000000 olx-api-wrapper-0.1.0/olx/advert_logo.py
--rw-rw-rw-   0        0        0      907 2024-05-06 15:48:15.000000 olx-api-wrapper-0.1.0/olx/advert_statistics.py
--rw-rw-rw-   0        0        0     4448 2024-05-06 15:34:57.000000 olx-api-wrapper-0.1.0/olx/adverts.py
--rw-rw-rw-   0        0        0     1420 2024-05-06 09:14:13.000000 olx-api-wrapper-0.1.0/olx/auth.py
--rw-rw-rw-   0        0        0     1740 2024-05-06 11:21:31.000000 olx-api-wrapper-0.1.0/olx/categories_attributes.py
--rw-rw-rw-   0        0        0     2743 2024-05-06 11:21:42.000000 olx-api-wrapper-0.1.0/olx/cities_districts.py
--rw-rw-rw-   0        0        0      777 2024-05-06 10:58:19.000000 olx-api-wrapper-0.1.0/olx/languages_currencies.py
--rw-rw-rw-   0        0        0     5372 2024-05-06 16:23:34.000000 olx-api-wrapper-0.1.0/olx/models.py
--rw-rw-rw-   0        0        0     5917 2024-05-06 16:19:01.000000 olx-api-wrapper-0.1.0/olx/olx.py
--rw-rw-rw-   0        0        0        0 2024-05-06 13:04:48.000000 olx-api-wrapper-0.1.0/olx/packets.py
--rw-rw-rw-   0        0        0     1295 2024-05-06 14:32:48.000000 olx-api-wrapper-0.1.0/olx/paid_features.py
--rw-rw-rw-   0        0        0     1654 2024-05-06 16:25:10.000000 olx-api-wrapper-0.1.0/olx/payments.py
--rw-rw-rw-   0        0        0     3278 2024-05-06 14:32:48.000000 olx-api-wrapper-0.1.0/olx/threads_messages.py
--rw-rw-rw-   0        0        0      500 2024-05-06 16:13:13.000000 olx-api-wrapper-0.1.0/olx/user_business.py
--rw-rw-rw-   0        0        0     1178 2024-05-06 09:56:07.000000 olx-api-wrapper-0.1.0/olx/users.py
-drwxrwxrwx   0        0        0        0 2024-05-06 19:17:27.508773 olx-api-wrapper-0.1.0/olx_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0     8762 2024-05-06 19:17:27.000000 olx-api-wrapper-0.1.0/olx_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      523 2024-05-06 19:17:27.000000 olx-api-wrapper-0.1.0/olx_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 19:17:27.000000 olx-api-wrapper-0.1.0/olx_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-06 19:17:27.000000 olx-api-wrapper-0.1.0/olx_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-06 19:17:27.000000 olx-api-wrapper-0.1.0/olx_api_wrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 19:17:27.510775 olx-api-wrapper-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      769 2024-05-06 19:16:36.000000 olx-api-wrapper-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:07.413425 olx-api-wrapper-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-07 07:11:07.413425 olx-api-wrapper-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:07.413425 olx-api-wrapper-0.1.1/olx/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/advert_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/advert_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/adverts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/categories_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/cities_districts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/languages_currencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/olx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/paid_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/threads_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/user_business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/olx/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:11:07.413425 olx-api-wrapper-0.1.1/olx_api_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-07 07:11:07.000000 olx-api-wrapper-0.1.1/olx_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 07:11:07.000000 olx-api-wrapper-0.1.1/olx_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:11:07.000000 olx-api-wrapper-0.1.1/olx_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 07:11:07.000000 olx-api-wrapper-0.1.1/olx_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 07:11:07.000000 olx-api-wrapper-0.1.1/olx_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:11:07.413425 olx-api-wrapper-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-07 07:10:59.000000 olx-api-wrapper-0.1.1/setup.py
```

### Comparing `olx-api-wrapper-0.1.0/LICENSE` & `olx-api-wrapper-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2024 Paweł Stawikowski
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2024 Paweł Stawikowski
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `olx-api-wrapper-0.1.0/olx/advert_logo.py` & `olx-api-wrapper-0.1.1/olx/advert_logo.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from .olx import Olx
-from .models import AdvertLogoType
-from dacite import from_dict
-from typing import List
-
-
-class AdvertLogo(Olx):
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-
-    def get_advert_logos(self, advert_id: int) -> List[AdvertLogoType]:
-        endpoint = self.endpoints["advert_logo"]["get_advert_logos"].format(
-            id=advert_id
-        )
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(AdvertLogoType, obj) for obj in data]
-
-    def add_logo(self, advert_id: int, url: str) -> AdvertLogoType:
-        endpoint = self.endpoints["advert_logo"]["add_logo"].format(id=advert_id)
-        payload = {"url": url}
-        response = self.post(endpoint, json=payload)
-        data = response.json()
-        return from_dict(AdvertLogo, data)
-
-    def delete_logo(self, advert_id: int, logo_id: int):
-        endpoint = self.endpoints["advert_logo"]["delete_logo"].format(
-            id=advert_id, logo_id=logo_id
-        )
-        self.delete(endpoint, wanted_status=204)
+from .olx import Olx
+from .models import AdvertLogoType
+from dacite import from_dict
+from typing import List
+
+
+class AdvertLogo(Olx):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+    def get_advert_logos(self, advert_id: int) -> List[AdvertLogoType]:
+        endpoint = self.endpoints["advert_logo"]["get_advert_logos"].format(
+            id=advert_id
+        )
+        response = self.get(endpoint)
+        data = response.json()["data"]
+        return [from_dict(AdvertLogoType, obj) for obj in data]
+
+    def add_logo(self, advert_id: int, url: str) -> AdvertLogoType:
+        endpoint = self.endpoints["advert_logo"]["add_logo"].format(id=advert_id)
+        payload = {"url": url}
+        response = self.post(endpoint, json=payload)
+        data = response.json()
+        return from_dict(AdvertLogo, data)
+
+    def delete_logo(self, advert_id: int, logo_id: int):
+        endpoint = self.endpoints["advert_logo"]["delete_logo"].format(
+            id=advert_id, logo_id=logo_id
+        )
+        self.delete(endpoint, wanted_status=204)
```

### Comparing `olx-api-wrapper-0.1.0/olx/advert_statistics.py` & `olx-api-wrapper-0.1.1/olx/advert_statistics.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from .olx import Olx
-from .models import AdvertStatistic
-from dacite import from_dict
-from typing import Literal
-
-
-class AdvertsStatistics(Olx):
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-
-    def get_advert_statistics(self, advert_id: int) -> AdvertStatistic:
-        endpoint = self.endpoints["advert_statistics"]["get_advert_statistics"].format(
-            id=advert_id
-        )
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(AdvertStatistic, data)
-
-    def clear_statistics(
-        self, advert_id: int, statistic_name: Literal["phone-views", "advert-views"]
-    ) -> None:
-        endpoint = self.endpoints["advert_statistics"]["clear_statistics"].format(
-            id=advert_id, statistic_name=statistic_name
-        )
-        self.delete(endpoint, wanted_status=204)
+from .olx import Olx
+from .models import AdvertStatistic
+from dacite import from_dict
+from typing import Literal
+
+
+class AdvertsStatistics(Olx):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+    def get_advert_statistics(self, advert_id: int) -> AdvertStatistic:
+        endpoint = self.endpoints["advert_statistics"]["get_advert_statistics"].format(
+            id=advert_id
+        )
+        response = self.get(endpoint)
+        data = response.json()["data"]
+        return from_dict(AdvertStatistic, data)
+
+    def clear_statistics(
+        self, advert_id: int, statistic_name: Literal["phone-views", "advert-views"]
+    ) -> None:
+        endpoint = self.endpoints["advert_statistics"]["clear_statistics"].format(
+            id=advert_id, statistic_name=statistic_name
+        )
+        self.delete(endpoint, wanted_status=204)
```

### Comparing `olx-api-wrapper-0.1.0/olx/adverts.py` & `olx-api-wrapper-0.1.1/olx/adverts.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-from .olx import Olx
-from .models import Advert
-from dacite import from_dict
-from typing import List, Literal
-
-
-class Adverts(Olx):
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-
-    def get_user_adverts(
-        self,
-        offset: int = None,
-        limit: int = None,
-        external_id: str = None,
-        category_ids: str = None,
-    ) -> List[Advert]:
-        endpoint = self.endpoints["adverts"]["get_user_adverts"]
-        params = dict()
-        if offset:
-            params["offset"] = offset
-        params = dict()
-        if limit:
-            params["limit"] = limit
-        params = dict()
-        if external_id:
-            params["external_id"] = external_id
-        params = dict()
-        if category_ids:
-            params["category_ids"] = category_ids
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        return [from_dict(Advert, obj) for obj in data]
-
-    def build_payload_for_create_or_update(
-        self,
-        title: str,
-        description: str,
-        category_id: str,
-        advertiser_type: Literal["private", "business"],
-        contact: dict,  # models.AdvertContact
-        location: dict,  # models.AdvertLocation
-        attributes: List[dict],  # models.AdvertAttribute
-        price: dict,  # models.AdvertPrice
-        images: List[dict] = None,  # models.AdvertImage
-        salary: dict = None,  # models.AdvertSalary
-        external_url: str = None,
-        external_id: str = None,
-        courier: bool = None,
-    ):
-        payload = {
-            "title": title,
-            "description": description,
-            "category_id": category_id,
-            "advertiser_type": advertiser_type,
-            "contact": contact,
-            "price": price,
-            "location": location,
-            "attributes": attributes,
-        }
-        if images:
-            payload["images"] = images
-        if salary:
-            payload["salary"] = salary
-        if external_url:
-            payload["external_url"] = external_url
-        if external_id:
-            payload["external_id"] = external_id
-        if courier:
-            payload["courier"] = courier
-
-        return payload
-
-    def create_advert(self, *args, **kwargs) -> Advert:
-        endpoint = self.endpoints["adverts"]["create_advert"]
-        payload = self.build_payload_for_create_or_update(*args, **kwargs)
-        response = self.post(endpoint, json=payload)
-        return from_dict(Advert, response.json())
-
-    def get_advert(self, advert_id) -> Advert:
-        endpoint = self.endpoints["adverts"]["get_advert"].format(id=advert_id)
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(Advert, data)
-
-    def update_advert(self, advert_id, *args, **kwargs) -> Advert:
-        endpoint = self.endpoints["adverts"]["update_advert"].format(id=advert_id)
-        payload = self.build_payload_for_create_or_update(*args, **kwargs)
-        response = self.put(endpoint, json=payload)
-        data = response.json()["data"]
-        return from_dict(Advert, data)
-
-    def delete_advert(self, advert_id: int) -> None:
-        endpoint = self.endpoints["adverts"]["delete_advert"].format(id=advert_id)
-        self.delete(endpoint, wanted_status=204)
-
-    def take_action_on_advert(
-        self,
-        advert_id: int,
-        command: Literal["activate", "deactivate", "finish", "refresh"],
-        is_success: bool = None,
-    ):
-        endpoint = self.endpoints["adverts"]["take_action_on_advert"].format(
-            id=advert_id
-        )
-        payload = {"command": command}
-        if command == "deactivate":
-            assert is_success is not None
-            payload["is_success"] = is_success
-        self.post(endpoint, json=payload, wanted_status=204)
-
-    def activate_advert(self, advert_id: int):
-        return self.take_action_on_advert(advert_id, "activate")
-
-    def deactivate_advert(self, advert_id: int, is_success: bool):
-        return self.take_action_on_advert(advert_id, "deactivate", is_success)
-
-    def finish_advert(self, advert_id: int):
-        return self.take_action_on_advert(advert_id, "finish")
-
-    def refresh_advert(self, advert_id: int):
-        return self.take_action_on_advert(advert_id, "refresh")
+from .olx import Olx
+from .models import Advert
+from dacite import from_dict
+from typing import List, Literal
+
+
+class Adverts(Olx):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+    def get_user_adverts(
+        self,
+        offset: int = None,
+        limit: int = None,
+        external_id: str = None,
+        category_ids: str = None,
+    ) -> List[Advert]:
+        endpoint = self.endpoints["adverts"]["get_user_adverts"]
+        params = dict()
+        if offset:
+            params["offset"] = offset
+        params = dict()
+        if limit:
+            params["limit"] = limit
+        params = dict()
+        if external_id:
+            params["external_id"] = external_id
+        params = dict()
+        if category_ids:
+            params["category_ids"] = category_ids
+        response = self.get(endpoint, params=params)
+        data = response.json()["data"]
+        return [from_dict(Advert, obj) for obj in data]
+
+    def build_payload_for_create_or_update(
+        self,
+        title: str,
+        description: str,
+        category_id: str,
+        advertiser_type: Literal["private", "business"],
+        contact: dict,  # models.AdvertContact
+        location: dict,  # models.AdvertLocation
+        attributes: List[dict],  # models.AdvertAttribute
+        price: dict,  # models.AdvertPrice
+        images: List[dict] = None,  # models.AdvertImage
+        salary: dict = None,  # models.AdvertSalary
+        external_url: str = None,
+        external_id: str = None,
+        courier: bool = None,
+    ):
+        payload = {
+            "title": title,
+            "description": description,
+            "category_id": category_id,
+            "advertiser_type": advertiser_type,
+            "contact": contact,
+            "price": price,
+            "location": location,
+            "attributes": attributes,
+        }
+        if images:
+            payload["images"] = images
+        if salary:
+            payload["salary"] = salary
+        if external_url:
+            payload["external_url"] = external_url
+        if external_id:
+            payload["external_id"] = external_id
+        if courier:
+            payload["courier"] = courier
+
+        return payload
+
+    def create_advert(self, *args, **kwargs) -> Advert:
+        endpoint = self.endpoints["adverts"]["create_advert"]
+        payload = self.build_payload_for_create_or_update(*args, **kwargs)
+        response = self.post(endpoint, json=payload)
+        return from_dict(Advert, response.json())
+
+    def get_advert(self, advert_id) -> Advert:
+        endpoint = self.endpoints["adverts"]["get_advert"].format(id=advert_id)
+        response = self.get(endpoint)
+        data = response.json()["data"]
+        return from_dict(Advert, data)
+
+    def update_advert(self, advert_id, *args, **kwargs) -> Advert:
+        endpoint = self.endpoints["adverts"]["update_advert"].format(id=advert_id)
+        payload = self.build_payload_for_create_or_update(*args, **kwargs)
+        response = self.put(endpoint, json=payload)
+        data = response.json()["data"]
+        return from_dict(Advert, data)
+
+    def delete_advert(self, advert_id: int) -> None:
+        endpoint = self.endpoints["adverts"]["delete_advert"].format(id=advert_id)
+        self.delete(endpoint, wanted_status=204)
+
+    def take_action_on_advert(
+        self,
+        advert_id: int,
+        command: Literal["activate", "deactivate", "finish", "refresh"],
+        is_success: bool = None,
+    ):
+        endpoint = self.endpoints["adverts"]["take_action_on_advert"].format(
+            id=advert_id
+        )
+        payload = {"command": command}
+        if command == "deactivate":
+            assert is_success is not None
+            payload["is_success"] = is_success
+        self.post(endpoint, json=payload, wanted_status=204)
+
+    def activate_advert(self, advert_id: int):
+        return self.take_action_on_advert(advert_id, "activate")
+
+    def deactivate_advert(self, advert_id: int, is_success: bool):
+        return self.take_action_on_advert(advert_id, "deactivate", is_success)
+
+    def finish_advert(self, advert_id: int):
+        return self.take_action_on_advert(advert_id, "finish")
+
+    def refresh_advert(self, advert_id: int):
+        return self.take_action_on_advert(advert_id, "refresh")
```

### Comparing `olx-api-wrapper-0.1.0/olx/categories_attributes.py` & `olx-api-wrapper-0.1.1/olx/categories_attributes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-from .olx import Olx
-from .models import Category, CategoryAttribute, CategorySuggestion
-from dacite import from_dict
-from typing import List
-
-
-class CategoriesAttributes(Olx):
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-
-    def get_categories(self, parent_id: int = None) -> List[Category]:
-        endpoint = self.endpoints["categories_attributes"]["get_categories"]
-        params = dict()
-        if parent_id:
-            params["parent_id"] = parent_id
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        return [from_dict(Category, obj) for obj in data]
-
-    def get_category(self, category_id: int) -> Category:
-        endpoint = self.endpoints["categories_attributes"]["get_category"].format(
-            id=category_id
-        )
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(Category, data)
-
-    def get_category_attributes(self, category_id: int) -> List[CategoryAttribute]:
-        endpoint = self.endpoints["categories_attributes"][
-            "get_category_attributes"
-        ].format(id=category_id)
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(CategoryAttribute, obj) for obj in data]
-
-    def get_category_suggestions(self, ad_title: str) -> List[CategorySuggestion]:
-        endpoint = self.endpoints["categories_attributes"]["get_category_suggestions"]
-        params = {"q": ad_title}
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        print(data)
-        return [from_dict(CategorySuggestion, obj) for obj in data]
+from .olx import Olx
+from .models import Category, CategoryAttribute, CategorySuggestion
+from dacite import from_dict
+from typing import List
+
+
+class CategoriesAttributes(Olx):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+    def get_categories(self, parent_id: int = None) -> List[Category]:
+        endpoint = self.endpoints["categories_attributes"]["get_categories"]
+        params = dict()
+        if parent_id:
+            params["parent_id"] = parent_id
+        response = self.get(endpoint, params=params)
+        data = response.json()["data"]
+        return [from_dict(Category, obj) for obj in data]
+
+    def get_category(self, category_id: int) -> Category:
+        endpoint = self.endpoints["categories_attributes"]["get_category"].format(
+            id=category_id
+        )
+        response = self.get(endpoint)
+        data = response.json()["data"]
+        return from_dict(Category, data)
+
+    def get_category_attributes(self, category_id: int) -> List[CategoryAttribute]:
+        endpoint = self.endpoints["categories_attributes"][
+            "get_category_attributes"
+        ].format(id=category_id)
+        response = self.get(endpoint)
+        data = response.json()["data"]
+        return [from_dict(CategoryAttribute, obj) for obj in data]
+
+    def get_category_suggestions(self, ad_title: str) -> List[CategorySuggestion]:
+        endpoint = self.endpoints["categories_attributes"]["get_category_suggestions"]
+        params = {"q": ad_title}
+        response = self.get(endpoint, params=params)
+        data = response.json()["data"]
+        return [from_dict(CategorySuggestion, obj) for obj in data]
```

### Comparing `olx-api-wrapper-0.1.0/olx/cities_districts.py` & `olx-api-wrapper-0.1.1/olx/threads_messages.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,92 @@
-from .olx import Olx
-from .models import Region, City, District, Location
-from dacite import from_dict
-from typing import List
-
-
-class CitiesDistricts(Olx):
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-
-    def list_of_country_regions(self) -> List[Region]:
-        endpoint = self.endpoints["cities_and_districts"]["list_of_country_regions"]
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(Region, obj) for obj in data]
-
-    def get_region(self, region_id: int) -> Region:
-        endpoint = self.endpoints["cities_and_districts"]["get_region"].format(
-            id=region_id
-        )
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(Region, data)
-
-    def get_cities(self, offset: int = None, limit: int = None) -> List[City]:
-        endpoint = self.endpoints["cities_and_districts"]["get_cities"]
-        params = dict()
-        if offset:
-            params["offset"] = offset
-        if limit:
-            params["limit"] = limit
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        return [from_dict(City, obj) for obj in data]
-
-    def get_city(self, city_id: int) -> City:
-        endpoint = self.endpoints["cities_and_districts"]["get_city"].format(id=city_id)
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(City, data)
-
-    def get_city_districts(self, city_id) -> List[District]:
-        endpoint = self.endpoints["cities_and_districts"]["get_city_districts"].format(
-            id=city_id
-        )
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(District, obj) for obj in data]
-
-    def get_districts(self) -> List[District]:
-        endpoint = self.endpoints["cities_and_districts"]["get_districts"]
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(District, obj) for obj in data]
-
-    def get_district(self, district_id) -> District:
-        endpoint = self.endpoints["cities_and_districts"]["get_district"].format(
-            id=district_id
-        )
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(District, data)
-
-    def get_locations(self, lat, lon):
-        endpoint = self.endpoints["cities_and_districts"]["get_locations"]
-        params = {"latitude": lat, "longitude": lon}
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        return [from_dict(Location, obj) for obj in data]
+from .olx import Olx
+from .models import Thread, Message
+from dacite import from_dict
+from typing import List, Literal
+
+
+class ThreadsMessages(Olx):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+    def get_threads(
+        self,
+        advert_id: int = None,
+        interlocutor_id: int = None,
+        offset: int = None,
+        limit: int = None,
+    ) -> List[Thread]:
+        endpoint = self.endpoints["threads_messages"]["get_threads"]
+        params = dict()
+        if advert_id:
+            params["advert_id"] = advert_id
+        if interlocutor_id:
+            params["interlocutor_id"] = interlocutor_id
+        if offset:
+            params["offset"] = offset
+        if limit:
+            params["limit"] = limit
+
+        response = self.get(endpoint, params=params)
+        data = response.json()["data"]
+        return [from_dict(Thread, obj) for obj in data]
+
+    def get_thread(self, thread_id) -> Thread:
+        endpoint = self.endpoints["threads_messages"]["get_thread"].format(id=thread_id)
+        response = self.get(endpoint)
+        data = response.json()["data"]
+        return from_dict(Thread, data)
+
+    def get_messages(
+        self, thread_id: int, offset: int = None, limit: int = None
+    ) -> List[Message]:
+        endpoint = self.endpoints["threads_messages"]["get_messages"].format(
+            id=thread_id
+        )
+        params = dict()
+        if offset:
+            params["offset"] = offset
+        if limit:
+            params["limit"] = limit
+
+        response = self.get(endpoint, params=params)
+        data = response.json()["data"]
+        return [from_dict(Message, obj) for obj in data]
+
+    def post_message(self, thread_id: int, text: str, attachments: List[str] = None):
+        endpoint = self.endpoints["threads_messages"]["post_message"].format(
+            id=thread_id
+        )
+        payload = {"text": text}
+        if attachments:
+            payload["attachments"] = attachments
+        response = self.post(endpoint, json=payload)
+        data = response.json()["data"]
+        return from_dict(Message, data)
+
+    def get_message(self, thread_id: int, message_id: int):
+        endpoint = self.endpoints["threads_messages"]["get_message"].format(
+            thread_id=thread_id, message_id=message_id
+        )
+        response = self.get(endpoint)
+        data = response.json()["data"]
+        return from_dict(Message, data)
+
+    def action_on_thread(
+        self,
+        thread_id: int,
+        action: Literal["set-favourite", "mark-as-read"],
+        is_favourite: bool = None,
+    ):
+        endpoint = self.endpoints["threads_messages"]["take_action_on_thread"].format(
+            id=thread_id
+        )
+        payload = {"command": action}
+        if action == "set-favourite":
+            payload["is_favourite"] = is_favourite
+        self.post(endpoint, json=payload, wanted_status=204)
+
+    def mark_thread_as_read(self, thread_id: int):
+        return self.action_on_thread(thread_id, "mark-as-read")
+
+    def set_favourite(self, thread_id: int, action: bool):
+        return self.action_on_thread(thread_id, "set-favourite", is_favourite=action)
```

### Comparing `olx-api-wrapper-0.1.0/olx/languages_currencies.py` & `olx-api-wrapper-0.1.1/olx/languages_currencies.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from .olx import Olx
-from .models import Language, Currency
-from dacite import from_dict
-from typing import List
-
-
-class LanguagesCurrencies(Olx):
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-
-    def get_languages(self) -> List[Language]:
-        endpoint = self.endpoints["languages_currencies"]["get_languages"]
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(Language, obj) for obj in data]
-
-    def get_currencies(self) -> List[Currency]:
-        endpoint = self.endpoints["languages_currencies"]["get_currencies"]
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(Currency, obj) for obj in data]
+from .olx import Olx
+from .models import Language, Currency
+from dacite import from_dict
+from typing import List
+
+
+class LanguagesCurrencies(Olx):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+    def get_languages(self) -> List[Language]:
+        endpoint = self.endpoints["languages_currencies"]["get_languages"]
+        response = self.get(endpoint)
+        data = response.json()["data"]
+        return [from_dict(Language, obj) for obj in data]
+
+    def get_currencies(self) -> List[Currency]:
+        endpoint = self.endpoints["languages_currencies"]["get_currencies"]
+        response = self.get(endpoint)
+        data = response.json()["data"]
+        return [from_dict(Currency, obj) for obj in data]
```

### Comparing `olx-api-wrapper-0.1.0/olx/olx.py` & `olx-api-wrapper-0.1.1/olx/olx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-import requests
-
-
-class Olx:
-    def __init__(self, country_code: str = "pl", access_token: str = None) -> None:
-        self.url = f"https://www.olx.{country_code}"
-        self.endpoints = {
-            "auth": "/api/open/oauth/token/",
-            "users": {
-                "me": "/api/partner/users/me",
-                "get_user": "/api/partner/users/{id}",
-                "account_balance": "/api/partner/users/me/account-balance",
-                "payment_methods": "/api/partner/users/me/payment-methods",
-            },
-            "cities_and_districts": {
-                "list_of_country_regions": "/api/partner/regions",
-                "get_region": "/api/partner/regions/{id}",
-                "get_cities": "/api/partner/cities",
-                "get_city": "/api/partner/cities/{id}",
-                "get_city_districts": "/api/partner/cities/{id}/districts",
-                "get_districts": "/api/partner/districts",
-                "get_district": "/api/partner/districts/{id}",
-                "get_locations": "/api/partner/locations",
-            },
-            "languages_currencies": {
-                "get_languages": "/api/partner/languages",
-                "get_currencies": "/api/partner/currencies",
-            },
-            "categories_attributes": {
-                "get_categories": "/api/partner/categories",
-                "get_category": "/api/partner/categories/{id}",
-                "get_category_attributes": "/api/partner/categories/{id}/attributes",
-                "get_category_suggestions": "/api/partner/categories/suggestion",
-            },
-            "threads_messages": {
-                "get_threads": "/api/partner/threads",
-                "get_thread": "/api/partner/threads/{id}",
-                "get_messages": "/api/partner/threads/{id}/messages",
-                "post_message": "/api/partner/threads/{id}/messages",
-                "get_message": "/api/partner/threads/{thread_id}/messages/{message_id}",
-                "take_action_on_thread": "/api/partner/threads/{id}/commands",
-            },
-            "paid_features": {
-                "get_available_paid_features": "/api/partner/paid-features",
-                "get_active_paid_features": "/api/partner/adverts/{advert_id}/paid-features",
-                "purchase_paid_feature": "/api/partner/adverts/{id}",
-            },
-            "adverts": {
-                "get_user_adverts": "/api/partner/adverts",
-                "create_advert": "/api/partner/adverts",
-                "get_advert": "/api/partner/adverts/{id}",
-                "update_advert": "/api/partner/adverts/{id}",
-                "delete_advert": "/api/partner/adverts/{id}",
-                "take_action_on_advert": "/api/partner/adverts/{id}/commands",
-            },
-            "advert_statistics": {
-                "get_advert_statistics": "/api/partner/adverts/{id}/statistics",
-                "clear_statistics": "/api/partner/adverts/{id}/statistics/{statistic_name}",
-            },
-            "advert_logo": {
-                "get_advert_logos": "/api/partner/adverts/{id}/logos",
-                "add_logo": "/api/partner/adverts/{id}/logos",
-                "delete_logo": "/api/partner/adverts/{id}/logos/{logo_id}",
-            },
-            "users_business": {
-                "get_user_business_data": "/api/partner/user-business/me",
-                "update_user_business_data": "/api/partner/user-business/me",
-                "get_user_business_logos": "/api/partner/user-business/me/logos",
-                "set_user_business_logos": "/api/partner/user-business/me/logos",
-                "remove_user_business_logo": "/api/partner/user-business/me/logos/{logo_id}",
-                "get_user_business_banners": "/api/partner/user-business/me/banners",
-                "set_user_business_banner": "/api/partner/user-business/me/banners",
-                "remove_user_business_banner": "/api/partner/user-business/me/banners/{banner_id}",
-            },
-            "payments": {
-                "get_billing": "/api/partner/user/me/billing",
-                "get_prepaid_invoices": "/api/partner/user/me/prepaid-invoices",
-                "get_postpaid_invoices": "/api/partner/user/me/postpaid-invoices",
-            },
-        }
-        self.default_scope = "read write v2"
-        self.headers = {"Version": "2.0", "Content-Type": "application/json"}
-
-        if access_token:
-            self.headers["Authorization"] = "Bearer " + access_token
-
-    def get(self, endpoint, wanted_status=200, **kwargs):
-        response = requests.get(url=self.url + endpoint, headers=self.headers, **kwargs)
-        if response.status_code != wanted_status:
-            print(response.json())
-            print("ERROR")  # TODO:
-            return None
-        return response
-
-    def post(self, endpoint, wanted_status=200, **kwargs):
-        response = requests.post(
-            url=self.url + endpoint, headers=self.headers, **kwargs
-        )
-        if response.status_code != wanted_status:
-            print(response.json())
-            print("ERROR")  # TODO:
-            return None
-        return response
-
-    def put(self, endpoint, wanted_status=200, **kwargs):
-        response = requests.put(url=self.url + endpoint, headers=self.headers, **kwargs)
-        if response.status_code != wanted_status:
-            print(response.json())
-            print("ERROR")  # TODO:
-            return None
-        return response
-
-    def delete(self, endpoint, wanted_status=200, **kwargs):
-        response = requests.delete(
-            url=self.url + endpoint, headers=self.headers, **kwargs
-        )
-        if response.status_code != wanted_status:
-            print(response.json())
-            print("ERROR")  # TODO:
-            return None
-        return response
+import requests
+
+
+class Olx:
+    def __init__(self, country_code: str = "pl", access_token: str = None) -> None:
+        self.url = f"https://www.olx.{country_code}"
+        self.endpoints = {
+            "auth": "/api/open/oauth/token/",
+            "users": {
+                "get_authenticated_user": "/api/partner/users/me",
+                "get_user": "/api/partner/users/{id}",
+                "account_balance": "/api/partner/users/me/account-balance",
+                "payment_methods": "/api/partner/users/me/payment-methods",
+            },
+            "cities_and_districts": {
+                "list_of_country_regions": "/api/partner/regions",
+                "get_region": "/api/partner/regions/{id}",
+                "get_cities": "/api/partner/cities",
+                "get_city": "/api/partner/cities/{id}",
+                "get_city_districts": "/api/partner/cities/{id}/districts",
+                "get_districts": "/api/partner/districts",
+                "get_district": "/api/partner/districts/{id}",
+                "get_locations": "/api/partner/locations",
+            },
+            "languages_currencies": {
+                "get_languages": "/api/partner/languages",
+                "get_currencies": "/api/partner/currencies",
+            },
+            "categories_attributes": {
+                "get_categories": "/api/partner/categories",
+                "get_category": "/api/partner/categories/{id}",
+                "get_category_attributes": "/api/partner/categories/{id}/attributes",
+                "get_category_suggestions": "/api/partner/categories/suggestion",
+            },
+            "threads_messages": {
+                "get_threads": "/api/partner/threads",
+                "get_thread": "/api/partner/threads/{id}",
+                "get_messages": "/api/partner/threads/{id}/messages",
+                "post_message": "/api/partner/threads/{id}/messages",
+                "get_message": "/api/partner/threads/{thread_id}/messages/{message_id}",
+                "take_action_on_thread": "/api/partner/threads/{id}/commands",
+            },
+            "paid_features": {
+                "get_available_paid_features": "/api/partner/paid-features",
+                "get_active_paid_features": "/api/partner/adverts/{advert_id}/paid-features",
+                "purchase_paid_feature": "/api/partner/adverts/{id}",
+            },
+            "adverts": {
+                "get_user_adverts": "/api/partner/adverts",
+                "create_advert": "/api/partner/adverts",
+                "get_advert": "/api/partner/adverts/{id}",
+                "update_advert": "/api/partner/adverts/{id}",
+                "delete_advert": "/api/partner/adverts/{id}",
+                "take_action_on_advert": "/api/partner/adverts/{id}/commands",
+            },
+            "advert_statistics": {
+                "get_advert_statistics": "/api/partner/adverts/{id}/statistics",
+                "clear_statistics": "/api/partner/adverts/{id}/statistics/{statistic_name}",
+            },
+            "advert_logo": {
+                "get_advert_logos": "/api/partner/adverts/{id}/logos",
+                "add_logo": "/api/partner/adverts/{id}/logos",
+                "delete_logo": "/api/partner/adverts/{id}/logos/{logo_id}",
+            },
+            "users_business": {
+                "get_user_business_data": "/api/partner/user-business/me",
+                "update_user_business_data": "/api/partner/user-business/me",
+                "get_user_business_logos": "/api/partner/user-business/me/logos",
+                "set_user_business_logos": "/api/partner/user-business/me/logos",
+                "remove_user_business_logo": "/api/partner/user-business/me/logos/{logo_id}",
+                "get_user_business_banners": "/api/partner/user-business/me/banners",
+                "set_user_business_banner": "/api/partner/user-business/me/banners",
+                "remove_user_business_banner": "/api/partner/user-business/me/banners/{banner_id}",
+            },
+            "payments": {
+                "get_billing": "/api/partner/user/me/billing",
+                "get_prepaid_invoices": "/api/partner/user/me/prepaid-invoices",
+                "get_postpaid_invoices": "/api/partner/user/me/postpaid-invoices",
+            },
+        }
+        self.default_scope = "read write v2"
+        self.headers = {"Version": "2.0", "Content-Type": "application/json"}
+
+        if access_token:
+            self.headers["Authorization"] = "Bearer " + access_token
+
+    def get(self, endpoint, wanted_status=200, **kwargs):
+        response = requests.get(url=self.url + endpoint, headers=self.headers, **kwargs)
+        if response.status_code != wanted_status:
+            print(response.json())
+            print("ERROR")  # TODO:
+            return None
+        return response
+
+    def post(self, endpoint, wanted_status=200, **kwargs):
+        response = requests.post(
+            url=self.url + endpoint, headers=self.headers, **kwargs
+        )
+        if response.status_code != wanted_status:
+            print(response.json())
+            print("ERROR")  # TODO:
+            return None
+        return response
+
+    def put(self, endpoint, wanted_status=200, **kwargs):
+        response = requests.put(url=self.url + endpoint, headers=self.headers, **kwargs)
+        if response.status_code != wanted_status:
+            print(response.json())
+            print("ERROR")  # TODO:
+            return None
+        return response
+
+    def delete(self, endpoint, wanted_status=200, **kwargs):
+        response = requests.delete(
+            url=self.url + endpoint, headers=self.headers, **kwargs
+        )
+        if response.status_code != wanted_status:
+            print(response.json())
+            print("ERROR")  # TODO:
+            return None
+        return response
```

### Comparing `olx-api-wrapper-0.1.0/olx/paid_features.py` & `olx-api-wrapper-0.1.1/olx/paid_features.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from .olx import Olx
-from .models import PaidFeature, ActivePaidFeature
-from dacite import from_dict
-from typing import List, Literal
-
-
-class PaidFeatures(Olx):
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-
-    def get_available_paid_features(self) -> List[PaidFeature]:
-        endpoint = self.endpoints["paid_features"]["get_available_paid_features"]
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(PaidFeature, obj) for obj in data]
-
-    def get_active_paid_features(self, advert_id) -> List[ActivePaidFeature]:
-        endpoint = self.endpoints["paid_features"]["get_active_paid_features"].format(
-            advert_id=advert_id
-        )
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(ActivePaidFeature, obj) for obj in data]
-
-    def purchase_paid_feature(
-        self, advert_id: int, payment_method: Literal["account", "postpaid"], code: str
-    ):
-        endpoint = self.endpoints["paid_features"]["purchase_paid_feature"].format(
-            id=advert_id
-        )
-        payload = {"payment_method": payment_method, "code": code}
-        self.post(endpoint, wanted_status=204, json=payload)
+from .olx import Olx
+from .models import PaidFeature, ActivePaidFeature
+from dacite import from_dict
+from typing import List, Literal
+
+
+class PaidFeatures(Olx):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+    def get_available_paid_features(self) -> List[PaidFeature]:
+        endpoint = self.endpoints["paid_features"]["get_available_paid_features"]
+        response = self.get(endpoint)
+        data = response.json()["data"]
+        return [from_dict(PaidFeature, obj) for obj in data]
+
+    def get_active_paid_features(self, advert_id) -> List[ActivePaidFeature]:
+        endpoint = self.endpoints["paid_features"]["get_active_paid_features"].format(
+            advert_id=advert_id
+        )
+        response = self.get(endpoint)
+        data = response.json()["data"]
+        return [from_dict(ActivePaidFeature, obj) for obj in data]
+
+    def purchase_paid_feature(
+        self, advert_id: int, payment_method: Literal["account", "postpaid"], code: str
+    ):
+        endpoint = self.endpoints["paid_features"]["purchase_paid_feature"].format(
+            id=advert_id
+        )
+        payload = {"payment_method": payment_method, "code": code}
+        self.post(endpoint, wanted_status=204, json=payload)
```

