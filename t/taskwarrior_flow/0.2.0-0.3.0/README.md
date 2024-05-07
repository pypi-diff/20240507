# Comparing `tmp/taskwarrior_flow-0.2.0.tar.gz` & `tmp/taskwarrior_flow-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskwarrior_flow-0.2.0.tar", max compression
+gzip compressed data, was "taskwarrior_flow-0.3.0.tar", max compression
```

## Comparing `taskwarrior_flow-0.2.0.tar` & `taskwarrior_flow-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-05-05 11:44:20.536249 taskwarrior_flow-0.2.0/LICENSE
--rw-r--r--   0        0        0     1126 2024-05-05 11:44:20.536249 taskwarrior_flow-0.2.0/README.md
--rw-r--r--   0        0        0      868 2024-05-05 11:44:20.536249 taskwarrior_flow-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      865 2024-05-05 11:44:20.536249 taskwarrior_flow-0.2.0/tools/__init__.py
--rw-r--r--   0        0        0      698 2024-05-05 11:44:20.536249 taskwarrior_flow-0.2.0/tools/main.py
--rw-r--r--   0        0        0    19385 2024-05-05 11:44:20.536249 taskwarrior_flow-0.2.0/tools/utils.py
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 taskwarrior_flow-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-07 05:43:01.918156 taskwarrior_flow-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1452 2024-05-07 05:43:01.918156 taskwarrior_flow-0.3.0/README.md
+-rw-r--r--   0        0        0     1035 2024-05-07 05:43:01.918156 taskwarrior_flow-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      902 2024-05-07 05:43:01.918156 taskwarrior_flow-0.3.0/tools/__init__.py
+-rw-r--r--   0        0        0     1842 2024-05-07 05:43:01.918156 taskwarrior_flow-0.3.0/tools/main.py
+-rw-r--r--   0        0        0    20222 2024-05-07 05:43:01.918156 taskwarrior_flow-0.3.0/tools/utils.py
+-rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 taskwarrior_flow-0.3.0/PKG-INFO
```

### Comparing `taskwarrior_flow-0.2.0/LICENSE` & `taskwarrior_flow-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.2.0/README.md` & `taskwarrior_flow-0.3.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -23,13 +23,20 @@
 
 ### Task template
 
 Allow users to save templates that can be used to create tasks easily
 
 ### Multiple task groups
 
-Instead of having one task database (i.e. $HOME/.task/), using `twf task -g [GROUP]` will allow users to use different task databases (i.e. $HOME/.task_[GROUP])
+Instead of having one task database (i.e. $HOME/.task/), using `twf [GROUP] [Taskwarrior commands]` will allow users to use different task databases (i.e. $HOME/.task_[GROUP])
+
+### Natural date parsing
+
+Users can specify dates in natural language, such as "tomorrow", "next week", "last year", etc.
+
+- In the template, users can define fields to be date, this enables natural date parsing
+- In task group, users can use a special syntax to specify dates, such as `due:@tomorrow at 2pm@`
 
 ## Related tools
 
 - This CLI is a complementary tool for [taskwarrior](https://taskwarrior.org)
 - This CLI is designed to work well with my [taskwarrior Neovim Plugin](https://github.com/huantrinh1802/m_taskwarrior_d.nvim)
```

### Comparing `taskwarrior_flow-0.2.0/pyproject.toml` & `taskwarrior_flow-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [tool.poetry]
 name = "taskwarrior_flow"
-version = "0.2.0"
+version = "0.3.0"
 description = "Set of helpers for improving Taskwarrior workflow"
 authors = ["Ben Trinh <huantrinh1802@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "tools" }]
 
 [tool.poetry.scripts]
 twf = 'tools.main:app'
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = "^0.12.3"
 python-dateutil = "^2.8.2"
 questionary = "^2.0.1"
+dateparser = "^1.2.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.3"
 mypy = "^1.6.1"
 types-python-dateutil = "^2.8.19.14"
 pytest = "^8.2.0"
+types-dateparser = "^1.2.0.20240420"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 120
@@ -32,7 +34,13 @@
 [tool.ruff.lint]
 select = ["E4", "E5", "E7", "E9", "F", "I"]
 ignore = []
 
 [project.urls]
 Homepage = "https://github.com/huantrinh1802/taskwarrior_flow"
 Issues = "https://github.com/huantrinh1802/taskwarrior_flow/issues"
+
+[tool.pytest.ini_options]
+log_cli = true
+log_level = "INFO"
+testpaths = ["tests"]
+addopts = "--capture=no"
```

### Comparing `taskwarrior_flow-0.2.0/tools/__init__.py` & `taskwarrior_flow-0.3.0/tools/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 import os
 
 config_file = os.environ.get("TW_CONFIG", f'{os.path.expanduser("~")}/.local/share/nvim/m_taskwarrior_d.json')
 if os.path.isfile(config_file):
-    with open(config_file, 'r') as f:
+    with open(config_file, "r") as f:
         tw_config = json.load(f)
 else:
-    with open(config_file, 'w') as f:
+    with open(config_file, "w") as f:
         tw_config = {
             "use_mtwd": False,
             "flow_config": {"task": {"data": "~/.task", "config": "~/.taskrc"}},
-            "add_templates": {"data": []},
+            "add_templates": {"date_fields": ["due", "scheduled"], "data": []},
             "saved_queries": {"name_max_length": 0, "data": []},
         }
         f.write(json.dumps(tw_config))
 group_mappings = {key: f'TASKDATA={value["data"]}' for key, value in tw_config["flow_config"].items()}
 
 
 def group_mappings_completion():
```

### Comparing `taskwarrior_flow-0.2.0/tools/utils.py` & `taskwarrior_flow-0.3.0/tools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import os
 import re
 import shutil
 import subprocess
 from typing import Annotated, Callable, TypedDict
 
+import dateparser
 import questionary
 import typer
 from prompt_toolkit.shortcuts import CompleteStyle
 from rich import print as rprint
 
 from tools import config_file, group_mappings, group_mappings_completion, tw_config
 
@@ -40,14 +41,25 @@
 
 
 class FunctionsGroup(TypedDict):
     func: Callable
     help: str
 
 
+class DateValidator(questionary.Validator):
+    def validate(self, document):
+        if dateparser.parse(document.text) or len(document.text) == 0:
+            return True
+        else:
+            raise questionary.ValidationError(
+                message="Invalid date",
+                cursor_position=len(document.text),
+            )
+
+
 def safe_ask(question):
     try:
         response = question.unsafe_ask()
         return response
     except KeyboardInterrupt:
         print("Cancelled by user")
         return None
@@ -110,26 +122,33 @@
     )
     if chosen_template is None:
         return
     questions = {}
     for name, field in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
         if name in preset_questions:
             questions[name] = preset_questions[name]
+        elif name in tw_config['add_templates']['date_fields']:
+            questions[name] = questionary.text(f"Enter {name}", style=question_style, validate=DateValidator)
         else:
             questions[name] = questionary.text(f"Enter {name}", instruction="Use ';' for list\n", style=question_style)
     answers = safe_ask(questionary.form(**questions))
     if answers is None:
         return
     parts = ""
     annotations: None | list[str] = None
     for name, field in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
         value = answers.get(name, "")
         if len(value) != 0 or answers[name] != " ":
             if name in "annotations":
                 annotations = [annotation for annotation in answers[name].split(";")]
+            elif name in tw_config['add_templates']['date_fields']:
+                date_str = dateparser.parse(answers[name])
+                if date_str is not None:
+                    date_str = date_str.strftime("%Y-%m-%dT%H:%M:%S")
+                    parts += " " + field.replace("%s", date_str)
             else:
                 parts += " " + " ".join(
                     field.replace("%s", item) if item != "" else "" for item in answers[name].split(";")
                 )
     command = tw_config["add_templates"]["data"][chosen_template]["command"].replace("%s", parts)
     confirm = safe_ask(questionary.confirm("Add task?", instruction=f"\n{command}\n", style=question_style))
     if confirm:
@@ -161,15 +180,15 @@
             data=questionary.text("Enter data location", style=question_style),
             config=questionary.text("Enter config location", style=question_style),
         )
     )
     if result is None:
         return
     if result["name"] != "" and result["data"] != "" and result["config"] != "":
-        tw_config["flow_config"].update({result["name"]: {'data': result["data"], 'config': result["config"]}})
+        tw_config["flow_config"].update({result["name"]: {"data": result["data"], "config": result["config"]}})
     with open(config_file, "w") as f:
         f.write(json.dumps(tw_config))
 
 
 create_groups: dict[str, FunctionsGroup] = {
     "task": {"help": "Add a new task based on template", "func": create_task},
     "template": {"help": "Add a new task template", "func": create_template},
```

### Comparing `taskwarrior_flow-0.2.0/PKG-INFO` & `taskwarrior_flow-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: taskwarrior_flow
-Version: 0.2.0
+Version: 0.3.0
 Summary: Set of helpers for improving Taskwarrior workflow
 Author: Ben Trinh
 Author-email: huantrinh1802@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dateparser (>=1.2.0,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
 # Taskwarrior Flow (TWF)
 
@@ -39,14 +40,21 @@
 
 ### Task template
 
 Allow users to save templates that can be used to create tasks easily
 
 ### Multiple task groups
 
-Instead of having one task database (i.e. $HOME/.task/), using `twf task -g [GROUP]` will allow users to use different task databases (i.e. $HOME/.task_[GROUP])
+Instead of having one task database (i.e. $HOME/.task/), using `twf [GROUP] [Taskwarrior commands]` will allow users to use different task databases (i.e. $HOME/.task_[GROUP])
+
+### Natural date parsing
+
+Users can specify dates in natural language, such as "tomorrow", "next week", "last year", etc.
+
+- In the template, users can define fields to be date, this enables natural date parsing
+- In task group, users can use a special syntax to specify dates, such as `due:@tomorrow at 2pm@`
 
 ## Related tools
 
 - This CLI is a complementary tool for [taskwarrior](https://taskwarrior.org)
 - This CLI is designed to work well with my [taskwarrior Neovim Plugin](https://github.com/huantrinh1802/m_taskwarrior_d.nvim)
```

