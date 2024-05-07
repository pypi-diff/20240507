# Comparing `tmp/nbappinator-0.1.3.tar.gz` & `tmp/nbappinator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbappinator-0.1.3.tar", last modified: Tue May  7 02:38:23 2024, max compression
+gzip compressed data, was "nbappinator-0.1.4.tar", last modified: Tue May  7 11:13:14 2024, max compression
```

## Comparing `nbappinator-0.1.3.tar` & `nbappinator-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:23.308660 nbappinator-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 02:37:32.000000 nbappinator-0.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-07 02:38:23.308660 nbappinator-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-07 02:37:32.000000 nbappinator-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:23.304660 nbappinator-0.1.3/nbappinator/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 02:37:32.000000 nbappinator-0.1.3/nbappinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 02:37:32.000000 nbappinator-0.1.3/nbappinator/aggridhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-07 02:37:32.000000 nbappinator-0.1.3/nbappinator/appinator.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 02:37:32.000000 nbappinator-0.1.3/nbappinator/browser_title.py
--rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-05-07 02:37:32.000000 nbappinator-0.1.3/nbappinator/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:37:32.000000 nbappinator-0.1.3/nbappinator/jinjamagic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:23.308660 nbappinator-0.1.3/nbappinator/nbappinator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-07 02:38:23.000000 nbappinator-0.1.3/nbappinator/nbappinator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-07 02:38:23.000000 nbappinator-0.1.3/nbappinator/nbappinator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:38:23.000000 nbappinator-0.1.3/nbappinator/nbappinator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 02:38:23.000000 nbappinator-0.1.3/nbappinator/nbappinator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 02:38:23.000000 nbappinator-0.1.3/nbappinator/nbappinator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-07 02:37:32.000000 nbappinator-0.1.3/nbappinator/plotly_charts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 02:37:32.000000 nbappinator-0.1.3/nbappinator/treew.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-07 02:37:32.000000 nbappinator-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:38:23.308660 nbappinator-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:23.308660 nbappinator-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-07 02:37:32.000000 nbappinator-0.1.3/tests/test_fails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 02:37:32.000000 nbappinator-0.1.3/tests/test_nb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:13:14.050385 nbappinator-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 11:12:18.000000 nbappinator-0.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-05-07 11:13:14.050385 nbappinator-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-07 11:12:18.000000 nbappinator-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:13:14.046385 nbappinator-0.1.4/nbappinator/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/aggridhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/appinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/browser_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15437 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/jinjamagic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:13:14.050385 nbappinator-0.1.4/nbappinator/nbappinator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-05-07 11:13:14.000000 nbappinator-0.1.4/nbappinator/nbappinator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-07 11:13:14.000000 nbappinator-0.1.4/nbappinator/nbappinator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:13:14.000000 nbappinator-0.1.4/nbappinator/nbappinator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 11:13:14.000000 nbappinator-0.1.4/nbappinator/nbappinator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 11:13:14.000000 nbappinator-0.1.4/nbappinator/nbappinator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/plotly_charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/treew.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-07 11:12:18.000000 nbappinator-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:13:14.050385 nbappinator-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:13:14.050385 nbappinator-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-07 11:12:18.000000 nbappinator-0.1.4/tests/test_fails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 11:12:18.000000 nbappinator-0.1.4/tests/test_nb.py
```

### Comparing `nbappinator-0.1.3/LICENSE.md` & `nbappinator-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.3/PKG-INFO` & `nbappinator-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbappinator
-Version: 0.1.3
+Version: 0.1.4
 Summary: Jupyter Notebook Application Builder
 Author-email: Paul T <paul@iqmo.com>
 Maintainer-email: Paul T <paul@iqmo.com>
 Project-URL: Homepage, https://github.com/iqmo-org/nbappinator
 Project-URL: Repository, https://github.com/iqmo-org/nbappinator
 Project-URL: Issues, https://github.com/iqmo-org/nbappinator/issues
 Requires-Python: >=3.9
@@ -27,33 +27,25 @@
 
 <!--[![Coverage badge](https://raw.githubusercontent.com/iqmo-org/nbappinator/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/iqmo-org/nbappinator/blob/python-coverage-comment-action-data/htmlcov/index.html)-->
 
 [![Coverage badge2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/iqmo-org/nbappinator/python-coverage-comment-action-data/endpoint.json)](https://htmlpreview.github.io/?https://github.com/iqmo-org/nbappinator/blob/python-coverage-comment-action-data/htmlcov/index.html)
 
 # Introduction
 
-nbappinator's goal is to make interactive Jupyter apps easier to develop and maintain, and reduce the learning curve involved with building & deploying Voila applications.
+nbappinator streamlines Jupyter and Voila app development through a structured, opinionated framework for UI construction. Adding a button to a page is as simple as using app.page[0].add_button(...).
 
-nbappinator provides an opinionated model for adding apps consisting of interaction widgets, such as buttons and dropdowns, along with display widgets including charts and grid / dataframe rendering.
+nbappinator has three goals:
 
-A secondary goal is to make it easy to swap UI extensions, support different deployment environments, and insulate the developer from implementation decisions relating to web technologies.
+- Simplify UI development for Notebook developers by reducing the surface area of APIs to learn.
+- Abstract the underlying UI components, allowing nbappinator to plug in different frameworks to achieve equivalent behavior.
+- Provide a foundation to develop reusable and portable themes to improve app styling.
 
-By creating a TabbedUiModel, you can easily add new display widgets to each page/tab, and set interactions as function calls for each action.
+# Example
 
-# Foundation
-
-nbappinator builds on a few great projects that provide useful building blocks in Jupyter, which themselves build on other great web technologies. Yet, nbappinator is intended to be implementation agnostic - a core goal is to allow any of these components to be swapped out.
-
-- [ipyvuetify](https://ipyvuetify.readthedocs.io/en/latest/): Provides the underlying UI widgets, bringing modern VUE components to Jupyter.
-- [ipyaggrid](https://github.com/widgetti/ipyaggrid): Wraps the excellent [AG Grid](https://ag-grid.com/) javascript grid library. AG Grid provides some great enterprise features too.
-- [ipytree](https://github.com/jupyter-widgets-contrib/ipytree): A tree widget for Jupyter
-
-[Plotly](https://plotly.com/) is given first class support, although any matplotlib charting library works too, such as Seaborn.
-
-This all builds on [Jupyter](https://jupyter.org/) and [ipywidgets](https://ipywidgets.readthedocs.io/en/stable/), of course.
+![Example](readme_example.png)
 
 # Getting Started
 
 ```py
 import nbappinator as nbapp
 
 def my_action(component, action, args, app: nbapp.UiModel, caller: str):
@@ -66,27 +58,42 @@
         chosen_value = app.get_values(caller)
         print(f"You chose {chosen_value}")
         app.get_page(1).add_textstatic(f"You chose {chosen_value}")
 
 # Create a Tabbed UI comprised of three sections:
 # "Config" Header,  Tabbed Pages: "First Tab" and "Second Tab", and a "Messages" Footer
 myapp = nbapp.TabbedUiModel(pages=["First Tab", "Second Tab"], log_footer = "Messages", headers=["Config"])
-myapp.get_page("Config").add_textstatic("This is some static text in the Config section of the page. You could add global settings, buttons and other widgets here.")
+myapp.get_page("Config").add_textstatic("This is static text in the Config section of the page. You could add global settings, buttons and other widgets here.")
 
 # Add a button to First Tab
+myapp.get_page(0).add_textstatic("This is the first tab")
 myapp.get_page(0).add_button(name="but1", label="Some button", action=my_action)
 myapp.get_page(0).add_textstatic("Click the button")
 
 # Add a dropdown selection to Second Tab
 myapp.get_page(1).add_select(name="choose1", label="Choose A Number", options=list(range(10)), action=choose_action)
 
 # Render the app:
 myapp.display()
 ```
 
-# Testing Notes
+# Deployment and BQuant
+
+nbappinator was originally designed to simplify developing applications within Bloomberg's BQuant environment, which provides a managed but locked down Jupyter environment with a Voila-based deployment of applications.
+
+# Acknowledgements
 
-A significant portion of the tests are Notebook smoketests designed to exercise the code base in its entirety.
+nbappinator builds on some great projects that provide useful building blocks in Jupyter, which themselves build on other great web technologies. At the same time, nbappinator is implementation agnostic - a core goal is to allow any of these components to be swapped out.
+
+[ipyvuetify](https://ipyvuetify.readthedocs.io/en/latest/) provides the underlying UI widgets, bringing modern VUE components to Jupyter.
+
+[AG Grid](https://ag-grid.com/) is an excellent javascript grid library, which [ipyaggrid](https://github.com/widgetti/ipyaggrid) provides as an Jupyter extension.
+
+[Plotly](https://plotly.com/) is given first class support, although any matplotlib charting library works, such as Seaborn.
+
+This all builds on [Jupyter](https://jupyter.org/) and [ipywidgets](https://ipywidgets.readthedocs.io/en/stable/).
+
+# Testing Notes
 
-The coverage report primarily reflects the percentage of the code base that the Notebooks exercise: but manual verification of the Notebook behavior is still required.
+A significant portion of the tests are Notebook smoketests designed to exercise the code base in its entirety. The coverage report primarily reflects the percentage of the code base that the Notebooks exercise: but manual verification of the Notebook behavior is still required.
 
 Some assertions are baked into the Notebooks, but largely its intended to ensure that all the features are exercised.
```

### Comparing `nbappinator-0.1.3/README.md` & `nbappinator-0.1.4/nbappinator/nbappinator.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,51 @@
+Metadata-Version: 2.1
+Name: nbappinator
+Version: 0.1.4
+Summary: Jupyter Notebook Application Builder
+Author-email: Paul T <paul@iqmo.com>
+Maintainer-email: Paul T <paul@iqmo.com>
+Project-URL: Homepage, https://github.com/iqmo-org/nbappinator
+Project-URL: Repository, https://github.com/iqmo-org/nbappinator
+Project-URL: Issues, https://github.com/iqmo-org/nbappinator/issues
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: ipywidgets~=7.8.0
+Requires-Dist: plotly
+Requires-Dist: ipyvuetify>=1.9
+Requires-Dist: ipyaggrid
+Requires-Dist: ipytree
+Requires-Dist: pandas>=1.5.3
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-xdist; extra == "test"
+
 [![PyPI Version](https://badge.fury.io/py/nbappinator.svg)](https://pypi.python.org/pypi/nbappinator)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/nbappinator/badges/version.svg)](https://anaconda.org/conda-forge/nbappinator)
 [![Tests](https://github.com/iqmo-org/nbappinator/actions/workflows/build_release.yml/badge.svg)](https://github.com/iqmo-org/nbappinator/actions/workflows/build_release.yml)
 [![Tests](https://github.com/iqmo-org/nbappinator/actions/workflows/test_coverage.yml/badge.svg)](https://github.com/iqmo-org/nbappinator/actions/workflows/test_coverage.yml)
 
 <!--[![Coverage badge](https://raw.githubusercontent.com/iqmo-org/nbappinator/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/iqmo-org/nbappinator/blob/python-coverage-comment-action-data/htmlcov/index.html)-->
 
 [![Coverage badge2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/iqmo-org/nbappinator/python-coverage-comment-action-data/endpoint.json)](https://htmlpreview.github.io/?https://github.com/iqmo-org/nbappinator/blob/python-coverage-comment-action-data/htmlcov/index.html)
 
 # Introduction
 
-nbappinator's goal is to make interactive Jupyter apps easier to develop and maintain, and reduce the learning curve involved with building & deploying Voila applications.
-
-nbappinator provides an opinionated model for adding apps consisting of interaction widgets, such as buttons and dropdowns, along with display widgets including charts and grid / dataframe rendering.
-
-A secondary goal is to make it easy to swap UI extensions, support different deployment environments, and insulate the developer from implementation decisions relating to web technologies.
-
-By creating a TabbedUiModel, you can easily add new display widgets to each page/tab, and set interactions as function calls for each action.
+nbappinator streamlines Jupyter and Voila app development through a structured, opinionated framework for UI construction. Adding a button to a page is as simple as using app.page[0].add_button(...).
 
-# Foundation
+nbappinator has three goals:
 
-nbappinator builds on a few great projects that provide useful building blocks in Jupyter, which themselves build on other great web technologies. Yet, nbappinator is intended to be implementation agnostic - a core goal is to allow any of these components to be swapped out.
+- Simplify UI development for Notebook developers by reducing the surface area of APIs to learn.
+- Abstract the underlying UI components, allowing nbappinator to plug in different frameworks to achieve equivalent behavior.
+- Provide a foundation to develop reusable and portable themes to improve app styling.
 
-- [ipyvuetify](https://ipyvuetify.readthedocs.io/en/latest/): Provides the underlying UI widgets, bringing modern VUE components to Jupyter.
-- [ipyaggrid](https://github.com/widgetti/ipyaggrid): Wraps the excellent [AG Grid](https://ag-grid.com/) javascript grid library. AG Grid provides some great enterprise features too.
-- [ipytree](https://github.com/jupyter-widgets-contrib/ipytree): A tree widget for Jupyter
+# Example
 
-[Plotly](https://plotly.com/) is given first class support, although any matplotlib charting library works too, such as Seaborn.
-
-This all builds on [Jupyter](https://jupyter.org/) and [ipywidgets](https://ipywidgets.readthedocs.io/en/stable/), of course.
+![Example](readme_example.png)
 
 # Getting Started
 
 ```py
 import nbappinator as nbapp
 
 def my_action(component, action, args, app: nbapp.UiModel, caller: str):
@@ -44,27 +58,42 @@
         chosen_value = app.get_values(caller)
         print(f"You chose {chosen_value}")
         app.get_page(1).add_textstatic(f"You chose {chosen_value}")
 
 # Create a Tabbed UI comprised of three sections:
 # "Config" Header,  Tabbed Pages: "First Tab" and "Second Tab", and a "Messages" Footer
 myapp = nbapp.TabbedUiModel(pages=["First Tab", "Second Tab"], log_footer = "Messages", headers=["Config"])
-myapp.get_page("Config").add_textstatic("This is some static text in the Config section of the page. You could add global settings, buttons and other widgets here.")
+myapp.get_page("Config").add_textstatic("This is static text in the Config section of the page. You could add global settings, buttons and other widgets here.")
 
 # Add a button to First Tab
+myapp.get_page(0).add_textstatic("This is the first tab")
 myapp.get_page(0).add_button(name="but1", label="Some button", action=my_action)
 myapp.get_page(0).add_textstatic("Click the button")
 
 # Add a dropdown selection to Second Tab
 myapp.get_page(1).add_select(name="choose1", label="Choose A Number", options=list(range(10)), action=choose_action)
 
 # Render the app:
 myapp.display()
 ```
 
-# Testing Notes
+# Deployment and BQuant
+
+nbappinator was originally designed to simplify developing applications within Bloomberg's BQuant environment, which provides a managed but locked down Jupyter environment with a Voila-based deployment of applications.
 
-A significant portion of the tests are Notebook smoketests designed to exercise the code base in its entirety.
+# Acknowledgements
+
+nbappinator builds on some great projects that provide useful building blocks in Jupyter, which themselves build on other great web technologies. At the same time, nbappinator is implementation agnostic - a core goal is to allow any of these components to be swapped out.
+
+[ipyvuetify](https://ipyvuetify.readthedocs.io/en/latest/) provides the underlying UI widgets, bringing modern VUE components to Jupyter.
+
+[AG Grid](https://ag-grid.com/) is an excellent javascript grid library, which [ipyaggrid](https://github.com/widgetti/ipyaggrid) provides as an Jupyter extension.
+
+[Plotly](https://plotly.com/) is given first class support, although any matplotlib charting library works, such as Seaborn.
+
+This all builds on [Jupyter](https://jupyter.org/) and [ipywidgets](https://ipywidgets.readthedocs.io/en/stable/).
+
+# Testing Notes
 
-The coverage report primarily reflects the percentage of the code base that the Notebooks exercise: but manual verification of the Notebook behavior is still required.
+A significant portion of the tests are Notebook smoketests designed to exercise the code base in its entirety. The coverage report primarily reflects the percentage of the code base that the Notebooks exercise: but manual verification of the Notebook behavior is still required.
 
 Some assertions are baked into the Notebooks, but largely its intended to ensure that all the features are exercised.
```

### Comparing `nbappinator-0.1.3/nbappinator/aggridhelper.py` & `nbappinator-0.1.4/nbappinator/aggridhelper.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.3/nbappinator/appinator.py` & `nbappinator-0.1.4/nbappinator/appinator.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.3/nbappinator/browser_title.py` & `nbappinator-0.1.4/nbappinator/browser_title.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.3/nbappinator/datagrid.py` & `nbappinator-0.1.4/nbappinator/datagrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 
 import ipyaggrid as ag
 from typing import List, Dict, Literal, Optional
 from typing import Any, Callable, Tuple, Union
 
 logger = logging.getLogger(__name__)
 
+# Set this to enable Enterprise features
+LICENSE = "community"
+
+
+def get_license():
+    return LICENSE
+
 
 @dataclass
 class ColMd:
     name: str
     label: Optional[str] = None
     format: str = "default"  # percent, decimal, mag_si (convert to K/M/G suffixes)
     pinned: bool = False
@@ -185,18 +192,18 @@
         showindex: bool = False,
         js_post_grid: List = [],
         js_pre_grid: List = [],
         grid_options: Dict = {},
         num_toppinned_rows=0,
         flatten_columns=True,
         default_precision=2,
-        license="e",
         *argv,
         **kargv,
     ):
+        license = get_license()
         # if pathcol is not None:
         #    pathcol = pathcol.title()
         sortcols = False
         if isinstance(grid_data, pd.DataFrame) and flatten_columns:
             input_df = grid_data.copy()
             input_df.columns = [str(col) for col in input_df.columns]
         else:
```

### Comparing `nbappinator-0.1.3/nbappinator/nbappinator.egg-info/SOURCES.txt` & `nbappinator-0.1.4/nbappinator/nbappinator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.3/nbappinator/plotly_charts.py` & `nbappinator-0.1.4/nbappinator/plotly_charts.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.3/nbappinator/treew.py` & `nbappinator-0.1.4/nbappinator/treew.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.3/pyproject.toml` & `nbappinator-0.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nbappinator"
-version = "0.1.3"
+version = "0.1.4"
 description = "Jupyter Notebook Application Builder"
 authors = [{ name = "Paul T", email = "paul@iqmo.com" }]
 maintainers =  [{ name = "Paul T", email = "paul@iqmo.com" }]
 dependencies = ["ipywidgets~=7.8.0", "plotly", "ipyvuetify>=1.9", "ipyaggrid", "ipytree", "pandas>=1.5.3"]
 requires-python = ">=3.9"
 
 [project.readme]
```

### Comparing `nbappinator-0.1.3/tests/test_fails.py` & `nbappinator-0.1.4/tests/test_fails.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.3/tests/test_nb.py` & `nbappinator-0.1.4/tests/test_nb.py`

 * *Files identical despite different names*

