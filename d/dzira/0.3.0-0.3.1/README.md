# Comparing `tmp/dzira-0.3.0.tar.gz` & `tmp/dzira-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dzira-0.3.0.tar", last modified: Wed May  1 19:47:15 2024, max compression
+gzip compressed data, was "dzira-0.3.1.tar", last modified: Tue May  7 16:30:04 2024, max compression
```

## Comparing `dzira-0.3.0.tar` & `dzira-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-01 19:47:15.611689 dzira-0.3.0/
--rw-r--r--   0 piotr     (1000) piotr     (1000)     1072 2023-05-08 16:48:33.000000 dzira-0.3.0/LICENSE
--rw-r--r--   0 piotr     (1000) piotr     (1000)     7574 2024-05-01 19:47:15.611689 dzira-0.3.0/PKG-INFO
--rw-r--r--   0 piotr     (1000) piotr     (1000)     6532 2024-05-01 19:20:29.000000 dzira-0.3.0/README.md
--rw-r--r--   0 piotr     (1000) piotr     (1000)     1110 2024-05-01 19:33:00.000000 dzira-0.3.0/pyproject.toml
--rw-r--r--   0 piotr     (1000) piotr     (1000)       38 2024-05-01 19:47:15.611689 dzira-0.3.0/setup.cfg
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-01 19:47:15.608355 dzira-0.3.0/src/
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-01 19:47:15.608355 dzira-0.3.0/src/dzira/
--rw-r--r--   0 piotr     (1000) piotr     (1000)        0 2024-02-11 20:24:51.000000 dzira-0.3.0/src/dzira/__init__.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)     4204 2024-05-01 19:20:29.000000 dzira-0.3.0/src/dzira/api.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)     1198 2024-05-01 19:20:29.000000 dzira-0.3.0/src/dzira/betterdict.py
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-01 19:47:15.611689 dzira-0.3.0/src/dzira/cli/
--rw-r--r--   0 piotr     (1000) piotr     (1000)    25671 2024-05-01 19:20:29.000000 dzira-0.3.0/src/dzira/cli/commands.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)     1538 2024-05-01 19:20:29.000000 dzira-0.3.0/src/dzira/cli/config.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)     3544 2024-05-01 19:20:29.000000 dzira-0.3.0/src/dzira/cli/output.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)     1072 2024-05-01 19:03:08.000000 dzira-0.3.0/src/dzira/data.py
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-01 19:47:15.611689 dzira-0.3.0/src/dzira.egg-info/
--rw-r--r--   0 piotr     (1000) piotr     (1000)     7574 2024-05-01 19:47:15.000000 dzira-0.3.0/src/dzira.egg-info/PKG-INFO
--rw-r--r--   0 piotr     (1000) piotr     (1000)      470 2024-05-01 19:47:15.000000 dzira-0.3.0/src/dzira.egg-info/SOURCES.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)        1 2024-05-01 19:47:15.000000 dzira-0.3.0/src/dzira.egg-info/dependency_links.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)       50 2024-05-01 19:47:15.000000 dzira-0.3.0/src/dzira.egg-info/entry_points.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)       39 2024-05-01 19:47:15.000000 dzira-0.3.0/src/dzira.egg-info/requires.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)        6 2024-05-01 19:47:15.000000 dzira-0.3.0/src/dzira.egg-info/top_level.txt
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-01 19:47:15.611689 dzira-0.3.0/tests/
--rw-r--r--   0 piotr     (1000) piotr     (1000)     9608 2024-05-01 19:20:29.000000 dzira-0.3.0/tests/test_api.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)     2288 2024-05-01 19:20:29.000000 dzira-0.3.0/tests/test_betterdict.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)     1882 2024-02-17 22:14:30.000000 dzira-0.3.0/tests/test_data.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)      941 2024-05-01 19:20:29.000000 dzira-0.3.0/tests/test_readme.py
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-07 16:30:04.590531 dzira-0.3.1/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1072 2023-05-08 16:48:33.000000 dzira-0.3.1/LICENSE
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     7574 2024-05-07 16:30:04.590531 dzira-0.3.1/PKG-INFO
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     6532 2024-05-01 19:20:29.000000 dzira-0.3.1/README.md
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1110 2024-05-07 16:22:36.000000 dzira-0.3.1/pyproject.toml
+-rw-r--r--   0 piotr     (1000) piotr     (1000)       38 2024-05-07 16:30:04.590531 dzira-0.3.1/setup.cfg
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-07 16:30:04.587198 dzira-0.3.1/src/
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-07 16:30:04.590531 dzira-0.3.1/src/dzira/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)        0 2024-02-11 20:24:51.000000 dzira-0.3.1/src/dzira/__init__.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     4321 2024-05-07 10:45:08.000000 dzira-0.3.1/src/dzira/api.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1198 2024-05-01 19:20:29.000000 dzira-0.3.1/src/dzira/betterdict.py
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-07 16:30:04.590531 dzira-0.3.1/src/dzira/cli/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)    25757 2024-05-07 10:45:08.000000 dzira-0.3.1/src/dzira/cli/commands.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1538 2024-05-01 19:20:29.000000 dzira-0.3.1/src/dzira/cli/config.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     3544 2024-05-07 10:30:17.000000 dzira-0.3.1/src/dzira/cli/output.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1072 2024-05-01 19:03:08.000000 dzira-0.3.1/src/dzira/data.py
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-07 16:30:04.590531 dzira-0.3.1/src/dzira.egg-info/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     7574 2024-05-07 16:30:04.000000 dzira-0.3.1/src/dzira.egg-info/PKG-INFO
+-rw-r--r--   0 piotr     (1000) piotr     (1000)      470 2024-05-07 16:30:04.000000 dzira-0.3.1/src/dzira.egg-info/SOURCES.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)        1 2024-05-07 16:30:04.000000 dzira-0.3.1/src/dzira.egg-info/dependency_links.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)       50 2024-05-07 16:30:04.000000 dzira-0.3.1/src/dzira.egg-info/entry_points.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)       39 2024-05-07 16:30:04.000000 dzira-0.3.1/src/dzira.egg-info/requires.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)        6 2024-05-07 16:30:04.000000 dzira-0.3.1/src/dzira.egg-info/top_level.txt
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-07 16:30:04.590531 dzira-0.3.1/tests/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)    10082 2024-05-07 10:45:08.000000 dzira-0.3.1/tests/test_api.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     2288 2024-05-01 19:20:29.000000 dzira-0.3.1/tests/test_betterdict.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1882 2024-02-17 22:14:30.000000 dzira-0.3.1/tests/test_data.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)      941 2024-05-01 19:20:29.000000 dzira-0.3.1/tests/test_readme.py
```

### Comparing `dzira-0.3.0/LICENSE` & `dzira-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dzira-0.3.0/PKG-INFO` & `dzira-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dzira
-Version: 0.3.0
+Version: 0.3.1
 Summary: A cli wrapper for jira API to track sprints and manage worklogs
 Author-email: Piotr Kaznowski <piotr@kazno.dev>
 Project-URL: Homepage, https://github.com/caseneuve/dzira
 Project-URL: Issues, https://github.com/caseneuve/dzira/issues
 Project-URL: Changelog, https://github.com/caseneuve/dzira/blob/master/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dzira-0.3.0/README.md` & `dzira-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dzira-0.3.0/pyproject.toml` & `dzira-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dzira"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
     "click >= 8.1",
     "jira",
     "python-dotenv",
     "tabulate",
 ]
 authors = [
```

### Comparing `dzira-0.3.0/src/dzira/api.py` & `dzira-0.3.1/src/dzira/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,36 +73,46 @@
 
 
 def get_worklog(jira: JIRA, issue: str, worklog_id: str) -> Worklog:
     return jira.worklog(issue=issue, id=worklog_id)
 
 
 def get_issues_by_work_logged_on_date(
-        jira: JIRA, report_date: datetime | None = None, fields="worklog,summary"
+        jira: JIRA,
+        project_key: str,
+        report_date: datetime | None = None,
+        fields: str = "worklog,summary",
 ):
     if report_date is not None:
-        query = f"worklogDate = {report_date:%Y-%m-%d}"
+        date_query = f"worklogDate = {report_date:%Y-%m-%d}"
     else:
-        query = f"worklogDate >= startOfDay()"
+        date_query = f"worklogDate >= startOfDay()"
+    query = f"{date_query} AND project = {project_key!r}"
     return jira.search_issues(query, fields=fields)
 
 
 def get_issue_worklogs_by_user_and_date(
         jira: JIRA, issue: Issue, user_email: str, report_date: datetime
 ) -> list:
-    # can't use `issue.fields.worklog.worklogs` as it fetches only up to 20 worklogs per issue
-    # so we need an extra call to api
-    # issue.fields.worklog.maxResult
-    if len(issue.fields.worklog.worklogs) < 20:
+    matching = []
+
+    try:
+        worklog_count = len(issue.fields.worklog.worklogs)
+    except (AttributeError, TypeError):
+        worklog_count = 0
+
+    if worklog_count == 0:
+        return matching
+    elif worklog_count < 20:
         worklogs = issue.fields.worklog.worklogs
     else:
         worklogs = jira.worklogs(issue.id)
+
     report_date = report_date.astimezone()
 
-    matching = []
     for worklog in worklogs:
         started = datetime.strptime(worklog.started, "%Y-%m-%dT%H:%M:%S.%f%z")
         if worklog.author.emailAddress == user_email and (
                 report_date <= started < report_date + timedelta(days=1)
         ):
             matching.append(worklog)
```

### Comparing `dzira-0.3.0/src/dzira/betterdict.py` & `dzira-0.3.1/src/dzira/betterdict.py`

 * *Files identical despite different names*

### Comparing `dzira-0.3.0/src/dzira/cli/commands.py` & `dzira-0.3.1/src/dzira/cli/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,16 +595,20 @@
 
 @spinner.run("Getting user id")
 def get_user_id(jira: JIRA) -> Result:
     return Result(result=api.get_current_user_id(jira))
 
 
 @spinner.run("Getting issues")
-def get_issues_with_work_logged_on_date(jira: JIRA, report_date: datetime | None) -> Result:
-    issues = api.get_issues_by_work_logged_on_date(jira, report_date)
+def get_issues_with_work_logged_on_date(
+        jira: JIRA,
+        project_key: str,
+        report_date: datetime | None,
+) -> Result:
+    issues = api.get_issues_by_work_logged_on_date(jira, project_key, report_date)
     if report_date is None:
         report_date = datetime.combine(date.today(), datetime.min.time())
     return Result(
         result=issues,
         data=D(report_date=report_date),
         stdout=(
             f"Found {len(issues)} issue{'s' if len(issues) != 1 else ''} "
@@ -758,15 +762,15 @@
         ],
         "total_time": "1h 15m",
         "total_seconds": 4500
       }
     """
     config = get_config(config=ctx.obj)
     jira = get_jira(config).result
-    issues = get_issues_with_work_logged_on_date(jira, report_date)
+    issues = get_issues_with_work_logged_on_date(jira, config["JIRA_PROJECT_KEY"], report_date)
     if issues.result:
         worklogs = get_user_worklogs_from_date(jira, config["JIRA_EMAIL"], issues).result
     else:
         worklogs = D()
 
     show_report(worklogs, format=format)
```

### Comparing `dzira-0.3.0/src/dzira/cli/config.py` & `dzira-0.3.1/src/dzira/cli/config.py`

 * *Files identical despite different names*

### Comparing `dzira-0.3.0/src/dzira/cli/output.py` & `dzira-0.3.1/src/dzira/cli/output.py`

 * *Files identical despite different names*

### Comparing `dzira-0.3.0/src/dzira/data.py` & `dzira-0.3.1/src/dzira/data.py`

 * *Files identical despite different names*

### Comparing `dzira-0.3.0/src/dzira.egg-info/PKG-INFO` & `dzira-0.3.1/src/dzira.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dzira
-Version: 0.3.0
+Version: 0.3.1
 Summary: A cli wrapper for jira API to track sprints and manage worklogs
 Author-email: Piotr Kaznowski <piotr@kazno.dev>
 Project-URL: Homepage, https://github.com/caseneuve/dzira
 Project-URL: Issues, https://github.com/caseneuve/dzira/issues
 Project-URL: Changelog, https://github.com/caseneuve/dzira/blob/master/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dzira-0.3.0/tests/test_api.py` & `dzira-0.3.1/tests/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,29 +154,36 @@
 
     assert result == mock_jira.worklog.return_value
     mock_jira.worklog.assert_called_once_with(issue=sentinel.issue, id=sentinel.worklog_id)
 
 
 def test_get_issues_by_work_logged_on_date_uses_date_and_default_fields(mock_jira):
     report_date = datetime(2024, 2, 11, 10, 24)
+    project_key = "FOO"
 
-    result = get_issues_by_work_logged_on_date(mock_jira, report_date)
+    result = get_issues_by_work_logged_on_date(
+        mock_jira, project_key, report_date
+    )
 
     assert result == mock_jira.search_issues.return_value
     mock_jira.search_issues.assert_called_once_with(
-        "worklogDate = 2024-02-11", fields="worklog,summary"
+        "worklogDate = 2024-02-11 AND project = 'FOO'", fields="worklog,summary"
     )
 
 
 def test_get_issues_by_work_logged_on_date_uses_today_as_fallback(mock_jira):
-    result = get_issues_by_work_logged_on_date(mock_jira, fields=sentinel.fields)
+    project_key = "FOO"
+
+    result = get_issues_by_work_logged_on_date(
+        mock_jira, project_key, fields=sentinel.fields
+    )
 
     assert result == mock_jira.search_issues.return_value
     mock_jira.search_issues.assert_called_once_with(
-        "worklogDate >= startOfDay()", fields=sentinel.fields
+        "worklogDate >= startOfDay() AND project = 'FOO'", fields=sentinel.fields
     )
 
 
 def test_get_issue_worklogs_by_user_and_date_from_the_issue(mock_jira):
     os.environ["TZ"] = "CET"
     time.tzset()
 
@@ -246,14 +253,25 @@
     report_date = datetime(2023, 11, 26, 0, 0).astimezone()
 
     result = get_issue_worklogs_by_user_and_date(mock_jira, mock_issue, email_address, report_date)
 
     assert result == mock_jira.worklogs.return_value
 
 
+def test_get_issue_worklogs_by_user_and_date_exists_early_when_no_worklogs_found(mock_jira):
+    mock_issue = Mock(fields=Mock())
+
+    result = get_issue_worklogs_by_user_and_date(
+        mock_jira, mock_issue, sentinel.email_address, sentinel.report_date
+    )
+
+    assert result == []
+    assert not mock_jira.worklogs.called
+
+
 def test_search_issues_with_sprint_info_uses_sprint_id(mock_jira):
     sprint_id = "123"
 
     result = search_issues_with_sprint_info(
         mock_jira, project_key=Mock(), sprint_id=sprint_id
     )
```

### Comparing `dzira-0.3.0/tests/test_betterdict.py` & `dzira-0.3.1/tests/test_betterdict.py`

 * *Files identical despite different names*

### Comparing `dzira-0.3.0/tests/test_data.py` & `dzira-0.3.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `dzira-0.3.0/tests/test_readme.py` & `dzira-0.3.1/tests/test_readme.py`

 * *Files identical despite different names*

