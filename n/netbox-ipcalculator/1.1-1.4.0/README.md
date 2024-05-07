# Comparing `tmp/netbox_ipcalculator-1.1.tar.gz` & `tmp/netbox_ipcalculator-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_ipcalculator-1.1.tar", last modified: Tue Jan  4 11:54:20 2022, max compression
+gzip compressed data, was "netbox_ipcalculator-1.4.0.tar", last modified: Tue May  7 13:33:54 2024, max compression
```

## Comparing `netbox_ipcalculator-1.1.tar` & `netbox_ipcalculator-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 11:54:20.064436 netbox_ipcalculator-1.1/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-01-04 11:54:05.000000 netbox_ipcalculator-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-01-04 11:54:20.064436 netbox_ipcalculator-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-01-04 11:54:05.000000 netbox_ipcalculator-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 11:54:20.064436 netbox_ipcalculator-1.1/netbox_ipcalculator/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-01-04 11:54:05.000000 netbox_ipcalculator-1.1/netbox_ipcalculator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 11:54:20.064436 netbox_ipcalculator-1.1/netbox_ipcalculator/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-04 11:54:05.000000 netbox_ipcalculator-1.1/netbox_ipcalculator/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-01-04 11:54:05.000000 netbox_ipcalculator-1.1/netbox_ipcalculator/navigation.py
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-01-04 11:54:05.000000 netbox_ipcalculator-1.1/netbox_ipcalculator/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 11:54:20.060436 netbox_ipcalculator-1.1/netbox_ipcalculator/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 11:54:20.064436 netbox_ipcalculator-1.1/netbox_ipcalculator/templates/netbox_ipcalculator/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 11:54:20.064436 netbox_ipcalculator-1.1/netbox_ipcalculator/templates/netbox_ipcalculator/core/
--rw-r--r--   0 runner    (1001) docker     (121)    13546 2022-01-04 11:54:05.000000 netbox_ipcalculator-1.1/netbox_ipcalculator/templates/netbox_ipcalculator/core/ipcalc.html
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-01-04 11:54:05.000000 netbox_ipcalculator-1.1/netbox_ipcalculator/templates/netbox_ipcalculator/ipcalcbase.html
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-01-04 11:54:05.000000 netbox_ipcalculator-1.1/netbox_ipcalculator/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-01-04 11:54:05.000000 netbox_ipcalculator-1.1/netbox_ipcalculator/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-04 11:54:20.064436 netbox_ipcalculator-1.1/netbox_ipcalculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-01-04 11:54:20.000000 netbox_ipcalculator-1.1/netbox_ipcalculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-01-04 11:54:20.000000 netbox_ipcalculator-1.1/netbox_ipcalculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-04 11:54:20.000000 netbox_ipcalculator-1.1/netbox_ipcalculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-04 11:54:19.000000 netbox_ipcalculator-1.1/netbox_ipcalculator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-04 11:54:20.000000 netbox_ipcalculator-1.1/netbox_ipcalculator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-04 11:54:20.064436 netbox_ipcalculator-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-01-04 11:54:05.000000 netbox_ipcalculator-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:33:54.758665 netbox_ipcalculator-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 13:33:49.000000 netbox_ipcalculator-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 13:33:49.000000 netbox_ipcalculator-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-07 13:33:54.758665 netbox_ipcalculator-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-07 13:33:49.000000 netbox_ipcalculator-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:33:54.758665 netbox_ipcalculator-1.4.0/netbox_ipcalculator/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 13:33:49.000000 netbox_ipcalculator-1.4.0/netbox_ipcalculator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:33:54.758665 netbox_ipcalculator-1.4.0/netbox_ipcalculator/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:33:49.000000 netbox_ipcalculator-1.4.0/netbox_ipcalculator/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-07 13:33:49.000000 netbox_ipcalculator-1.4.0/netbox_ipcalculator/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-07 13:33:49.000000 netbox_ipcalculator-1.4.0/netbox_ipcalculator/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:33:54.754665 netbox_ipcalculator-1.4.0/netbox_ipcalculator/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:33:54.758665 netbox_ipcalculator-1.4.0/netbox_ipcalculator/templates/netbox_ipcalculator/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:33:54.758665 netbox_ipcalculator-1.4.0/netbox_ipcalculator/templates/netbox_ipcalculator/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-05-07 13:33:49.000000 netbox_ipcalculator-1.4.0/netbox_ipcalculator/templates/netbox_ipcalculator/core/ipcalc.html
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-07 13:33:49.000000 netbox_ipcalculator-1.4.0/netbox_ipcalculator/templates/netbox_ipcalculator/ipcalcbase.html
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 13:33:49.000000 netbox_ipcalculator-1.4.0/netbox_ipcalculator/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 13:33:49.000000 netbox_ipcalculator-1.4.0/netbox_ipcalculator/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:33:54.758665 netbox_ipcalculator-1.4.0/netbox_ipcalculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-07 13:33:54.000000 netbox_ipcalculator-1.4.0/netbox_ipcalculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-07 13:33:54.000000 netbox_ipcalculator-1.4.0/netbox_ipcalculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:33:54.000000 netbox_ipcalculator-1.4.0/netbox_ipcalculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:33:54.000000 netbox_ipcalculator-1.4.0/netbox_ipcalculator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 13:33:54.000000 netbox_ipcalculator-1.4.0/netbox_ipcalculator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:33:54.758665 netbox_ipcalculator-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-07 13:33:49.000000 netbox_ipcalculator-1.4.0/setup.py
```

### Comparing `netbox_ipcalculator-1.1/netbox_ipcalculator/template_content.py` & `netbox_ipcalculator-1.4.0/netbox_ipcalculator/template_content.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from extras.plugins import PluginTemplateExtension
+from netbox.plugins import PluginTemplateExtension
 import json
 
 class IPCalcAggregate(PluginTemplateExtension):
     model = 'ipam.aggregate'
 
     def right_page(self):
         output=self.render('netbox_ipcalculator/core/ipcalc.html', extra_context={
```

### Comparing `netbox_ipcalculator-1.1/netbox_ipcalculator/templates/netbox_ipcalculator/core/ipcalc.html` & `netbox_ipcalculator-1.4.0/netbox_ipcalculator/templates/netbox_ipcalculator/core/ipcalc.html`

 * *Files 4% similar despite different names*

```diff
@@ -51,19 +51,23 @@
                     bit
                 }*/
                 return this.calccidr();
             }
         
             this.setcidr=function(newcidr) {
                 var m;
-                m = newcidr.match(/^[0-9a-fA-F\:\.]+\/\d+$/); //at least match 'something/number'
+                m = newcidr.match(/^[0-9a-fA-F\:\.]+\/[\d\.]+$/); //at least match 'something/number'
                 if (m) { 
                     m=m[0].split('/');
                     this.ip=m[0];
-                    this.pl=parseInt(m[1]);
+                    if (m[1].match(/^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}?(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$/)) {
+                        this.pl=this.netmask2cidr(m[1]) 
+                    } else {
+                        this.pl=parseInt(m[1]);
+                    }
                     return this.calccidr();
                 }
                 return false;
             }
         
             this.calccidr=function() {
                 // ipver, ip and pl must be known.
@@ -227,14 +231,26 @@
                         m = (t.length > m.length) ? t : m;
                         return t;
                     }).replace(m || ' ', '::');
                 } else { // Invalid length
                     return false;
                 }
             }
+
+            this.netmask2cidr = function(nm) {
+                var m = nm.match(/^(?:\d{1,3}(?:\.|$)){4}/); // IPv4
+                if (m) {
+                    nmcidr = 0
+                    m = m[0].split('.');
+                    for (i = 0; i < m.length; i++) {
+                        nmcidr += parseInt(m[i]).toString(2).replace(/0/g,"").length
+                    }                    
+                    return nmcidr
+                }
+            }
         }
         
         
         
         </script>        
         <table cellpadding="2" id='cidrout'>
             <colgroup><col align="left" span="4"></colgroup>
```

### Comparing `netbox_ipcalculator-1.1/netbox_ipcalculator.egg-info/SOURCES.txt` & `netbox_ipcalculator-1.4.0/netbox_ipcalculator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 netbox_ipcalculator/__init__.py
 netbox_ipcalculator/navigation.py
 netbox_ipcalculator/template_content.py
 netbox_ipcalculator/urls.py
```

