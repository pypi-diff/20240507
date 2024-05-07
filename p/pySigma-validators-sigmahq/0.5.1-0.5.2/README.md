# Comparing `tmp/pysigma_validators_sigmahq-0.5.1.tar.gz` & `tmp/pysigma_validators_sigmahq-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_validators_sigmahq-0.5.1.tar", max compression
+gzip compressed data, was "pysigma_validators_sigmahq-0.5.2.tar", max compression
```

## Comparing `pysigma_validators_sigmahq-0.5.1.tar` & `pysigma_validators_sigmahq-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    26526 2024-05-04 06:04:48.727126 pysigma_validators_sigmahq-0.5.1/LICENSE
--rw-r--r--   0        0        0     3187 2024-05-04 06:04:48.727126 pysigma_validators_sigmahq-0.5.1/README.md
--rw-r--r--   0        0        0      644 2024-05-04 06:04:48.727126 pysigma_validators_sigmahq-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      830 2024-05-04 06:04:48.727126 pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/__init__.py
--rw-r--r--   0        0        0    52850 2024-05-04 06:04:48.727126 pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/config.py
--rw-r--r--   0        0        0     7066 2024-05-04 06:04:48.727126 pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/field.py
--rw-r--r--   0        0        0     2772 2024-05-04 06:04:48.727126 pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/filename.py
--rw-r--r--   0        0        0      917 2024-05-04 06:04:48.727126 pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/logsource.py
--rw-r--r--   0        0        0     7349 2024-05-04 06:04:48.727126 pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/metadata.py
--rw-r--r--   0        0        0     2914 2024-05-04 06:04:48.727126 pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/title.py
--rw-r--r--   0        0        0     3980 1970-01-01 00:00:00.000000 pysigma_validators_sigmahq-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3292 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/README.md
+-rw-r--r--   0        0        0      644 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      830 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/__init__.py
+-rw-r--r--   0        0        0    53521 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/config.py
+-rw-r--r--   0        0        0     7066 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/field.py
+-rw-r--r--   0        0        0     2772 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/filename.py
+-rw-r--r--   0        0        0     1516 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/logsource.py
+-rw-r--r--   0        0        0     7349 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/metadata.py
+-rw-r--r--   0        0        0     2914 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/title.py
+-rw-r--r--   0        0        0     4085 1970-01-01 00:00:00.000000 pysigma_validators_sigmahq-0.5.2/PKG-INFO
```

### Comparing `pysigma_validators_sigmahq-0.5.1/LICENSE` & `pysigma_validators_sigmahq-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_validators_sigmahq-0.5.1/README.md` & `pysigma_validators_sigmahq-0.5.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 | sigmahq_filename                      | Check rule filename match SigmaHQ standard.                  |
 | sigmahq_filename_prefix               | Check rule filename match SigmaHQ prefix standard.           |
 | sigmahq_invalid_all_modifier          | Check All modifier used with a single value.                 |
 | sigmahq_invalid_field_source          | Check field Source use with Eventlog.                        |
 | sigmahq_invalid_fieldname             | Check field name do not exist in the logsource.              |
 | sigmahq_level_existence               | Checks if rule has a level.                                  |
 | sigmahq_link_description              | Checks if rule description use a link instead of references. |
-| sigmahq_logsource_valid               | Checks if rule has valid logsource.                          |
+| sigmahq_logsource_coherent            | Checks if rule has Coherent logsource.                       |
+| sigmahq_logsource_known               | Checks if rule has known logsource.                          |
 | sigmahq_space_fieldname               | Check field name have a space.                               |
 | sigmahq_status_deprecated             | Checks if rule has a status DEPRECATED.                      |
 | sigmahq_status_existence              | Checks if rule has a status.                                 |
 | sigmahq_status_unsupported            | Checks if rule has a status UNSUPPORTED.                     |
 | sigmahq_title_case                    | Checks if rule title use capitalization.                     |
 | sigmahq_title_end                     | Checks if rule title end with a dot(.).                      |
 | sigmahq_title_length                  | Checks if rule has a title too long.                         |
```

### Comparing `pysigma_validators_sigmahq-0.5.1/pyproject.toml` & `pysigma_validators_sigmahq-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-validators-sigmahq"
-version = "0.5.1"
+version = "0.5.2"
 description = "pySigma SigmaHQ validators"
 authors = ["François Hubaut <frack113@users.noreply.github.com>"]
 license = "LGPL-2.1-only"
 readme = "README.md"
 repository = "https://github.com/frack113/pySigma_validators_sigmaHQ"
 packages = [
     { include = "sigma" }
```

### Comparing `pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/__init__.py` & `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/__init__.py`

 * *Files identical despite different names*

### Comparing `pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/config.py` & `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,16 +296,18 @@
     {"category": None, "product": "aws", "service": "cloudtrail"},
     {"category": None, "product": "azure", "service": "activitylogs"},
     {"category": None, "product": "azure", "service": "auditlogs"},
     {"category": None, "product": "azure", "service": "pim"},
     {"category": None, "product": "azure", "service": "pim"},
     {"category": None, "product": "azure", "service": "riskdetection"},
     {"category": None, "product": "azure", "service": "signinlogs"},
+    {"category": None, "product": "bitbucket", "service": "audit"},
     {"category": None, "product": "cisco", "service": "aaa"},
     {"category": None, "product": "cisco", "service": "bgp"},
+    {"category": None, "product": "cisco", "service": "duo"},
     {"category": None, "product": "cisco", "service": "ldp"},
     {"category": None, "product": "cisco", "service": "syslog"},
     {"category": None, "product": "fortios", "service": "sslvpnd"},
     {"category": None, "product": "gcp", "service": "gcp.audit"},
     {"category": None, "product": "gcp", "service": "google_workspace.admin"},
     {"category": None, "product": "github", "service": "audit"},
     {"category": None, "product": "huawei", "service": "bgp"},
@@ -391,19 +393,22 @@
     {"category": None, "product": "zeek", "service": "dns"},
     {"category": None, "product": "zeek", "service": "http"},
     {"category": None, "product": "zeek", "service": "kerberos"},
     {"category": None, "product": "zeek", "service": "rdp"},
     {"category": None, "product": "zeek", "service": "smb_files"},
     {"category": None, "product": "zeek", "service": "x509"},
     {"category": "antivirus", "product": None, "service": None},
+    {"category": "appliance", "product": "paloalto", "service": "globalprotect"},
     {"category": "application", "product": "django", "service": None},
     {"category": "application", "product": "jvm", "service": None},
+    {"category": "application", "product": "kubernetes", "service": "audit"},
     {"category": "application", "product": "modsecurity", "service": None},
     {"category": "application", "product": "nodejs", "service": None},
     {"category": "application", "product": "python", "service": None},
+    {"category": "application", "product": "opencanary", "service": None},
     {"category": "application", "product": "qualys", "service": None},
     {"category": "application", "product": "rpc_firewall", "service": None},
     {"category": "application", "product": "ruby_on_rails", "service": None},
     {"category": "application", "product": "spring", "service": None},
     {"category": "application", "product": "sql", "service": None},
     {"category": "application", "product": "velocity", "service": None},
     {"category": "create_remote_thread", "product": "windows", "service": None},
@@ -416,14 +421,15 @@
     {"category": "file_access", "product": "windows", "service": None},
     {"category": "file_change", "product": "windows", "service": None},
     {"category": "file_delete", "product": "macos", "service": None},
     {"category": "file_delete", "product": "windows", "service": None},
     {"category": "file_event", "product": "linux", "service": None},
     {"category": "file_event", "product": "macos", "service": None},
     {"category": "file_event", "product": "macos", "service": None},
+    {"category": "file_event", "product": "paloalto", "service": "globalprotect"},
     {"category": "file_event", "product": "windows", "service": None},
     {"category": "file_executable_detected", "product": "windows", "service": None},
     {"category": "file_rename", "product": "windows", "service": None},
     {"category": "firewall", "product": None, "service": None},
     {"category": "firewall", "product": None, "service": None},
     {"category": "image_load", "product": "windows", "service": None},
     {"category": "network_connection", "product": "linux", "service": None},
@@ -1596,15 +1602,23 @@
             field = v["field"]
             self.sigmahq_logsource_cast[SigmaLogSource.from_dict(v["log"])] = field
 
             if "Hashes" in field or "Hash" in field:
                 field.extend(["Imphash", "md5", "sha1", "sha256"])
 
             if v["log"]["product"] == "windows":
-                field.extend(["EventID", "Provider_Name"])
+                field.extend(
+                    [
+                        "EventID",
+                        "Provider_Name",
+                        "Channel",
+                        "Computer",
+                        "Security_UserID",
+                    ]
+                )
 
             self.sigmahq_logsource_unicast[SigmaLogSource.from_dict(v["log"])] = [
                 x.lower() for x in field
             ]
 
         # Valid logsource list
         for v in Data_SigmaHQ_logsource:
```

### Comparing `pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/field.py` & `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/field.py`

 * *Files identical despite different names*

### Comparing `pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/filename.py` & `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/filename.py`

 * *Files identical despite different names*

### Comparing `pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/logsource.py` & `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/logsource.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,21 +10,38 @@
 
 from .config import ConfigHq
 
 config = ConfigHq()
 
 
 @dataclass
-class SigmahqLogsourceValidIssue(SigmaValidationIssue):
-    description: ClassVar[str] = "Rule has an invalid logsource"
+class SigmahqLogsourceKnownIssue(SigmaValidationIssue):
+    description: ClassVar[str] = "Rule has an unknown logsource"
     severity: ClassVar[SigmaValidationIssueSeverity] = SigmaValidationIssueSeverity.HIGH
     logsource: SigmaLogSource
 
 
-class SigmahqLogsourceValidValidator(SigmaRuleValidator):
-    """Checks if rule has valid logsource."""
+class SigmahqLogsourceKnownValidator(SigmaRuleValidator):
+    """Checks if rule has known logsource."""
 
     def validate(self, rule: SigmaRule) -> List[SigmaValidationIssue]:
-        if rule.logsource and not rule.logsource in config.sigmahq_logsource_list:
-            return [SigmahqLogsourceValidIssue(rule, rule.logsource)]
+        if not rule.logsource in config.sigmahq_logsource_list:
+            return [SigmahqLogsourceKnownIssue(rule, rule.logsource)]
+        else:
+            return []
+
+
+@dataclass
+class SigmahqLogsourceCoherentIssue(SigmaValidationIssue):
+    description: ClassVar[str] = "Rule has an incoherent logsource"
+    severity: ClassVar[SigmaValidationIssueSeverity] = SigmaValidationIssueSeverity.HIGH
+    logsource: SigmaLogSource
+
+
+class SigmahqLogsourceCoherentValidator(SigmaRuleValidator):
+    """Checks if rule has Coherent logsource."""
+
+    def validate(self, rule: SigmaRule) -> List[SigmaValidationIssue]:
+        if rule.logsource.service and not rule.logsource.product:
+            return [SigmahqLogsourceCoherentIssue(rule, rule.logsource)]
         else:
             return []
```

### Comparing `pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/metadata.py` & `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/metadata.py`

 * *Files identical despite different names*

### Comparing `pysigma_validators_sigmahq-0.5.1/sigma/validators/sigmahq/title.py` & `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/title.py`

 * *Files identical despite different names*

### Comparing `pysigma_validators_sigmahq-0.5.1/PKG-INFO` & `pysigma_validators_sigmahq-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySigma-validators-sigmahq
-Version: 0.5.1
+Version: 0.5.2
 Summary: pySigma SigmaHQ validators
 Home-page: https://github.com/frack113/pySigma_validators_sigmaHQ
 License: LGPL-2.1-only
 Author: François Hubaut
 Author-email: frack113@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
@@ -42,15 +42,16 @@
 | sigmahq_filename                      | Check rule filename match SigmaHQ standard.                  |
 | sigmahq_filename_prefix               | Check rule filename match SigmaHQ prefix standard.           |
 | sigmahq_invalid_all_modifier          | Check All modifier used with a single value.                 |
 | sigmahq_invalid_field_source          | Check field Source use with Eventlog.                        |
 | sigmahq_invalid_fieldname             | Check field name do not exist in the logsource.              |
 | sigmahq_level_existence               | Checks if rule has a level.                                  |
 | sigmahq_link_description              | Checks if rule description use a link instead of references. |
-| sigmahq_logsource_valid               | Checks if rule has valid logsource.                          |
+| sigmahq_logsource_coherent            | Checks if rule has Coherent logsource.                       |
+| sigmahq_logsource_known               | Checks if rule has known logsource.                          |
 | sigmahq_space_fieldname               | Check field name have a space.                               |
 | sigmahq_status_deprecated             | Checks if rule has a status DEPRECATED.                      |
 | sigmahq_status_existence              | Checks if rule has a status.                                 |
 | sigmahq_status_unsupported            | Checks if rule has a status UNSUPPORTED.                     |
 | sigmahq_title_case                    | Checks if rule title use capitalization.                     |
 | sigmahq_title_end                     | Checks if rule title end with a dot(.).                      |
 | sigmahq_title_length                  | Checks if rule has a title too long.                         |
```

