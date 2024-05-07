# Comparing `tmp/django_admin_keycloak-0.3.1.tar.gz` & `tmp/django_admin_keycloak-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_admin_keycloak-0.3.1.tar", max compression
+gzip compressed data, was "django_admin_keycloak-0.3.2.tar", max compression
```

## Comparing `django_admin_keycloak-0.3.1.tar` & `django_admin_keycloak-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0     1066 2024-02-14 11:36:19.329511 django_admin_keycloak-0.3.1/LICENSE
--rw-r--r--   0        0        0     1495 2024-02-14 11:36:19.329511 django_admin_keycloak-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-02-14 11:36:19.329511 django_admin_keycloak-0.3.1/django_admin_keycloak/__init__.py
--rw-r--r--   0        0        0     2434 2024-02-14 11:36:19.329511 django_admin_keycloak-0.3.1/django_admin_keycloak/admin.py
--rw-r--r--   0        0        0      423 2024-02-14 11:36:19.329511 django_admin_keycloak-0.3.1/django_admin_keycloak/apps.py
--rw-r--r--   0        0        0     2066 2024-02-14 11:36:19.329511 django_admin_keycloak-0.3.1/django_admin_keycloak/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3754 2024-02-14 11:36:19.329511 django_admin_keycloak-0.3.1/django_admin_keycloak/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2024-02-14 11:36:19.329511 django_admin_keycloak-0.3.1/django_admin_keycloak/management/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/management/commands/__init__.py
--rw-r--r--   0        0        0     1633 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/management/commands/update_static_providers.py
--rw-r--r--   0        0        0     2978 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/migrations/0001_initial.py
--rw-r--r--   0        0        0      834 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/migrations/0002_rename_client_secret_key_keycloakprovider_client_secret_and_more.py
--rw-r--r--   0        0        0     1410 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/migrations/0003_keycloaksession.py
--rw-r--r--   0        0        0      315 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/migrations/0004_delete_keycloaksession.py
--rw-r--r--   0        0        0     2082 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/migrations/0005_keycloaksession.py
--rw-r--r--   0        0        0        0 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/migrations/__init__.py
--rw-r--r--   0        0        0     3011 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/models.py
--rw-r--r--   0        0        0     4058 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/oidc.py
--rw-r--r--   0        0        0       89 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/signals.py
--rw-r--r--   0        0        0      689 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/static/admin/css/keycloak.css
--rw-r--r--   0        0        0      675 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/static_settings.py
--rw-r--r--   0        0        0     1107 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/templates/admin/base.html
--rw-r--r--   0        0        0      156 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/templates/admin/login.html
--rw-r--r--   0        0        0      316 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/templates/django_admin_keycloak/auth_link.html
--rw-r--r--   0        0        0      125 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/templates/django_admin_keycloak/login-error.html
--rw-r--r--   0        0        0        0 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/templatetags/__init__.py
--rw-r--r--   0        0        0     1094 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/templatetags/keycloak.py
--rw-r--r--   0        0        0      356 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/urls.py
--rw-r--r--   0        0        0     1029 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/utils.py
--rw-r--r--   0        0        0     2210 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/django_admin_keycloak/views.py
--rw-r--r--   0        0        0      723 2024-02-14 11:36:19.333511 django_admin_keycloak-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2238 1970-01-01 00:00:00.000000 django_admin_keycloak-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1495 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/__init__.py
+-rw-r--r--   0        0        0     3004 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/admin.py
+-rw-r--r--   0        0        0      423 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/apps.py
+-rw-r--r--   0        0        0     2066 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3754 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/management/commands/__init__.py
+-rw-r--r--   0        0        0     1633 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/management/commands/update_static_providers.py
+-rw-r--r--   0        0        0     2978 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/migrations/0001_initial.py
+-rw-r--r--   0        0        0      834 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/migrations/0002_rename_client_secret_key_keycloakprovider_client_secret_and_more.py
+-rw-r--r--   0        0        0     1410 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/migrations/0003_keycloaksession.py
+-rw-r--r--   0        0        0      315 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/migrations/0004_delete_keycloaksession.py
+-rw-r--r--   0        0        0     2082 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/migrations/0005_keycloaksession.py
+-rw-r--r--   0        0        0     2678 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/migrations/0006_keycloakuser.py
+-rw-r--r--   0        0        0      442 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/migrations/0007_keycloakprovider_app_name.py
+-rw-r--r--   0        0        0        0 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/migrations/__init__.py
+-rw-r--r--   0        0        0     4909 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/models.py
+-rw-r--r--   0        0        0     4058 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/oidc.py
+-rw-r--r--   0        0        0       89 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/signals.py
+-rw-r--r--   0        0        0      689 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/static/admin/css/keycloak.css
+-rw-r--r--   0        0        0      675 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/static_settings.py
+-rw-r--r--   0        0        0     1107 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/templates/admin/base.html
+-rw-r--r--   0        0        0      156 2024-05-07 11:10:35.130860 django_admin_keycloak-0.3.2/django_admin_keycloak/templates/admin/login.html
+-rw-r--r--   0        0        0      404 2024-05-07 11:10:35.134861 django_admin_keycloak-0.3.2/django_admin_keycloak/templates/django_admin_keycloak/auth_link.html
+-rw-r--r--   0        0        0      125 2024-05-07 11:10:35.134861 django_admin_keycloak-0.3.2/django_admin_keycloak/templates/django_admin_keycloak/login-error.html
+-rw-r--r--   0        0        0        0 2024-05-07 11:10:35.134861 django_admin_keycloak-0.3.2/django_admin_keycloak/templatetags/__init__.py
+-rw-r--r--   0        0        0     1338 2024-05-07 11:10:35.134861 django_admin_keycloak-0.3.2/django_admin_keycloak/templatetags/keycloak.py
+-rw-r--r--   0        0        0      356 2024-05-07 11:10:35.134861 django_admin_keycloak-0.3.2/django_admin_keycloak/urls.py
+-rw-r--r--   0        0        0     1029 2024-05-07 11:10:35.134861 django_admin_keycloak-0.3.2/django_admin_keycloak/utils.py
+-rw-r--r--   0        0        0     2210 2024-05-07 11:10:35.134861 django_admin_keycloak-0.3.2/django_admin_keycloak/views.py
+-rw-r--r--   0        0        0      723 2024-05-07 11:10:35.134861 django_admin_keycloak-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2238 1970-01-01 00:00:00.000000 django_admin_keycloak-0.3.2/PKG-INFO
```

### Comparing `django_admin_keycloak-0.3.1/LICENSE` & `django_admin_keycloak-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/README.md` & `django_admin_keycloak-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/admin.py` & `django_admin_keycloak-0.3.2/django_admin_keycloak/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django import forms
 from django.contrib import admin
 from django.utils.translation import gettext_lazy as _
 
-from django_admin_keycloak.models import KeycloakProvider, KeycloakSession
+from django_admin_keycloak.models import KeycloakProvider, KeycloakSession, KeycloakUser
 
 
 class KeycloakProviderModelForm(forms.ModelForm):
     class Meta:
         model = KeycloakProvider
         fields = '__all__'
         widgets = {
@@ -31,14 +31,15 @@
         if obj and getattr(obj, 'is_static', False):
             server_fields.remove('client_secret')
         return (
             (None, {'fields': (
                 'active',
                 'slug',
                 'name',
+                'app_name',
             )}),
             (_('Server'), {'fields': server_fields}),
             (_('Other Info'), {'fields': (
                 'redirect_uri',
                 'role_super_user',
                 'role_staff_user',
                 'options',
@@ -77,7 +78,27 @@
     list_filter = ('provider__name',)
 
     def has_add_permission(self, request):
         return False
 
     def has_change_permission(self, request, obj=None):
         return False
+
+
+@admin.register(KeycloakUser)
+class KeycloakUserAdmin(admin.ModelAdmin):
+    list_display = (
+        'preferred_username',
+        'given_name',
+        'family_name',
+        'email',
+        'user',
+        'provider',
+    )
+    search_fields = ('preferred_username', 'given_name', 'family_name', 'email', 'user__username', 'provider__name')
+    list_filter = ('provider__name',)
+
+    def has_change_permission(self, request, obj=None):
+        return False
+
+    def has_add_permission(self, request):
+        return False
```

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/locale/ru/LC_MESSAGES/django.mo` & `django_admin_keycloak-0.3.2/django_admin_keycloak/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/locale/ru/LC_MESSAGES/django.po` & `django_admin_keycloak-0.3.2/django_admin_keycloak/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/management/commands/update_static_providers.py` & `django_admin_keycloak-0.3.2/django_admin_keycloak/management/commands/update_static_providers.py`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/migrations/0001_initial.py` & `django_admin_keycloak-0.3.2/django_admin_keycloak/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/migrations/0002_rename_client_secret_key_keycloakprovider_client_secret_and_more.py` & `django_admin_keycloak-0.3.2/django_admin_keycloak/migrations/0002_rename_client_secret_key_keycloakprovider_client_secret_and_more.py`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/migrations/0003_keycloaksession.py` & `django_admin_keycloak-0.3.2/django_admin_keycloak/migrations/0003_keycloaksession.py`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/migrations/0005_keycloaksession.py` & `django_admin_keycloak-0.3.2/django_admin_keycloak/migrations/0005_keycloaksession.py`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/oidc.py` & `django_admin_keycloak-0.3.2/django_admin_keycloak/oidc.py`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/static/admin/css/keycloak.css` & `django_admin_keycloak-0.3.2/django_admin_keycloak/static/admin/css/keycloak.css`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/static_settings.py` & `django_admin_keycloak-0.3.2/django_admin_keycloak/static_settings.py`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/templates/admin/base.html` & `django_admin_keycloak-0.3.2/django_admin_keycloak/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/templatetags/keycloak.py` & `django_admin_keycloak-0.3.2/django_admin_keycloak/templatetags/keycloak.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,24 +15,32 @@
     for provider in KeycloakProvider.objects.filter(active=True).iterator():
         yield {
             'name': provider.name,
             'url': get_auth_url(provider, request)
         }
 
 
+def _has_providers() -> bool:
+    return KeycloakProvider.objects.filter(active=True).exists()
+
+
 @register.inclusion_tag('django_admin_keycloak/auth_link.html', takes_context=True)
 def keycloak_authorization_links(context):
     request = context['request']
     return {
         'providers': _get_providers(request),
+        'has_providers': _has_providers(),
     }
 
 
 @register.simple_tag(name='sso_account', takes_context=True)
 def get_account_link(context):
     request = context['request']
     try:
         provider = KeycloakProvider.objects.get(pk=request.session['keycloak_pk'])
     except (KeycloakProvider.DoesNotExist, KeyError):
         return
 
-    return provider.get_account_link()
+    return provider.get_account_link(
+        referrer=provider.app_name,
+        referrer_uri=request.build_absolute_uri(request.path),
+    )
```

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/utils.py` & `django_admin_keycloak-0.3.2/django_admin_keycloak/utils.py`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/django_admin_keycloak/views.py` & `django_admin_keycloak-0.3.2/django_admin_keycloak/views.py`

 * *Files identical despite different names*

### Comparing `django_admin_keycloak-0.3.1/pyproject.toml` & `django_admin_keycloak-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-admin-keycloak"
-version = "0.3.1"
+version = "0.3.2"
 description = "Django Admin Keycloak"
 authors = ["Mikhail Badrazhan <mikhail@devilweb.ru>"]
 readme = "README.md"
 repository = "https://github.com/migelbd/django-admin-keycloak"
 keywords = ["keycloak", "django"]
 classifiers = [
     "Framework :: Django :: 4",
```

### Comparing `django_admin_keycloak-0.3.1/PKG-INFO` & `django_admin_keycloak-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-keycloak
-Version: 0.3.1
+Version: 0.3.2
 Summary: Django Admin Keycloak
 Home-page: https://github.com/migelbd/django-admin-keycloak
 Keywords: keycloak,django
 Author: Mikhail Badrazhan
 Author-email: mikhail@devilweb.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Framework :: Django :: 4
```

