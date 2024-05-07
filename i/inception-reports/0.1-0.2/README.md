# Comparing `tmp/inception_reports-0.1.tar.gz` & `tmp/inception_reports-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inception_reports-0.1.tar", last modified: Tue Apr 30 00:01:38 2024, max compression
+gzip compressed data, was "inception_reports-0.2.tar", last modified: Tue May  7 01:02:34 2024, max compression
```

## Comparing `inception_reports-0.1.tar` & `inception_reports-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-04-30 00:01:38.688906 inception_reports-0.1/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    11357 2023-09-25 12:56:28.000000 inception_reports-0.1/LICENSE
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      752 2023-11-07 13:15:00.000000 inception_reports-0.1/NOTICE.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2073 2024-04-30 00:01:38.688906 inception_reports-0.1/PKG-INFO
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1376 2024-04-29 23:59:37.000000 inception_reports-0.1/README.md
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-04-30 00:01:38.688906 inception_reports-0.1/inception_reports/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      769 2024-04-02 01:14:36.000000 inception_reports-0.1/inception_reports/__init__.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1704 2024-04-29 23:24:38.000000 inception_reports-0.1/inception_reports/__main__.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     7094 2024-04-29 23:24:38.000000 inception_reports-0.1/inception_reports/generate_reports_lead.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    13324 2024-04-29 23:24:38.000000 inception_reports-0.1/inception_reports/generate_reports_manager.py
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-04-30 00:01:38.688906 inception_reports-0.1/inception_reports.egg-info/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2073 2024-04-30 00:01:38.000000 inception_reports-0.1/inception_reports.egg-info/PKG-INFO
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      515 2024-04-30 00:01:38.000000 inception_reports-0.1/inception_reports.egg-info/SOURCES.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)        1 2024-04-30 00:01:38.000000 inception_reports-0.1/inception_reports.egg-info/dependency_links.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       70 2024-04-30 00:01:38.000000 inception_reports-0.1/inception_reports.egg-info/entry_points.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       56 2024-04-30 00:01:38.000000 inception_reports-0.1/inception_reports.egg-info/requires.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       18 2024-04-30 00:01:38.000000 inception_reports-0.1/inception_reports.egg-info/top_level.txt
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      802 2024-04-30 00:01:23.000000 inception_reports-0.1/pyproject.toml
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       38 2024-04-30 00:01:38.688906 inception_reports-0.1/setup.cfg
-drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-04-30 00:01:38.688906 inception_reports-0.1/tests/
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     3551 2024-04-29 23:24:38.000000 inception_reports-0.1/tests/test_generate_reports_lead.py
--rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     3379 2024-04-29 23:24:38.000000 inception_reports-0.1/tests/test_generate_reports_manager.py
+drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-07 01:02:34.953213 inception_reports-0.2/
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    11357 2023-09-25 12:56:28.000000 inception_reports-0.2/LICENSE
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      752 2023-11-07 13:15:00.000000 inception_reports-0.2/NOTICE.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2073 2024-05-07 01:02:34.953213 inception_reports-0.2/PKG-INFO
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1376 2024-04-30 00:10:18.000000 inception_reports-0.2/README.md
+drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-07 01:02:34.953213 inception_reports-0.2/inception_reports/
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      769 2024-04-02 01:14:36.000000 inception_reports-0.2/inception_reports/__init__.py
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     1704 2024-04-29 23:24:38.000000 inception_reports-0.2/inception_reports/__main__.py
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     7094 2024-04-29 23:24:38.000000 inception_reports-0.2/inception_reports/generate_reports_lead.py
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)    14011 2024-05-07 01:00:49.000000 inception_reports-0.2/inception_reports/generate_reports_manager.py
+drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-07 01:02:34.953213 inception_reports-0.2/inception_reports.egg-info/
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     2073 2024-05-07 01:02:34.000000 inception_reports-0.2/inception_reports.egg-info/PKG-INFO
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      515 2024-05-07 01:02:34.000000 inception_reports-0.2/inception_reports.egg-info/SOURCES.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)        1 2024-05-07 01:02:34.000000 inception_reports-0.2/inception_reports.egg-info/dependency_links.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       70 2024-05-07 01:02:34.000000 inception_reports-0.2/inception_reports.egg-info/entry_points.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       56 2024-05-07 01:02:34.000000 inception_reports-0.2/inception_reports.egg-info/requires.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       18 2024-05-07 01:02:34.000000 inception_reports-0.2/inception_reports.egg-info/top_level.txt
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)      802 2024-05-07 01:02:30.000000 inception_reports-0.2/pyproject.toml
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)       38 2024-05-07 01:02:34.953213 inception_reports-0.2/setup.cfg
+drwxr-xr-x   0 basch    (1060118464) domänen-benutzer (1060110849)        0 2024-05-07 01:02:34.953213 inception_reports-0.2/tests/
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     3551 2024-04-29 23:24:38.000000 inception_reports-0.2/tests/test_generate_reports_lead.py
+-rw-r--r--   0 basch    (1060118464) domänen-benutzer (1060110849)     4262 2024-05-07 01:00:49.000000 inception_reports-0.2/tests/test_generate_reports_manager.py
```

### Comparing `inception_reports-0.1/LICENSE` & `inception_reports-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inception_reports-0.1/NOTICE.txt` & `inception_reports-0.2/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `inception_reports-0.1/PKG-INFO` & `inception_reports-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inception_reports
-Version: 0.1
+Version: 0.2
 Summary: Generate plots that report the progress of an INCEpTION project.
 Author-email: Serwar Basch <serwar.basch@tu-darmstadt.de>
 Project-URL: Homepage, https://github.com/inception-project/inception-reporting-dashboard
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -25,15 +25,15 @@
 In its current state, it can be used by the project manager on site to visualize different metrics regarding the progress of the project, and the type of annotations done.
 
 In case the project is part of a bigger project, the project progress can be exported to be sent to a project lead in a centralized location who, in turn, can use the package to get an overview of the progress across the different projects and locations.
 
 ## Getting started
 
 1. Ensure you have python 3.11 or higher (check it using python --version)
-2. Install the package using ``pip install inception_reports``
+2. Install the package using ``pip install inception-reports``
 3. Run the script using ``inception_reports --help`` this will show you the options you have:
     1. Run it with ``inception_reports --manager`` if you have one python project, or are responsible for one location.
     2. Run it with ``inception_reports --lead`` if you're leading multiple projects, or multiple locations.
 4. Regardless of the mode you run the package with, it should open a browser window. Follow the instructions on the page to proceed.
 
 ## Issues
```

### Comparing `inception_reports-0.1/README.md` & `inception_reports-0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 In its current state, it can be used by the project manager on site to visualize different metrics regarding the progress of the project, and the type of annotations done.
 
 In case the project is part of a bigger project, the project progress can be exported to be sent to a project lead in a centralized location who, in turn, can use the package to get an overview of the progress across the different projects and locations.
 
 ## Getting started
 
 1. Ensure you have python 3.11 or higher (check it using python --version)
-2. Install the package using ``pip install inception_reports``
+2. Install the package using ``pip install inception-reports``
 3. Run the script using ``inception_reports --help`` this will show you the options you have:
     1. Run it with ``inception_reports --manager`` if you have one python project, or are responsible for one location.
     2. Run it with ``inception_reports --lead`` if you're leading multiple projects, or multiple locations.
 4. Regardless of the mode you run the package with, it should open a browser window. Follow the instructions on the page to proceed.
 
 ## Issues
```

### Comparing `inception_reports-0.1/inception_reports/__init__.py` & `inception_reports-0.2/inception_reports/__init__.py`

 * *Files identical despite different names*

### Comparing `inception_reports-0.1/inception_reports/__main__.py` & `inception_reports-0.2/inception_reports/__main__.py`

 * *Files identical despite different names*

### Comparing `inception_reports-0.1/inception_reports/generate_reports_lead.py` & `inception_reports-0.2/inception_reports/generate_reports_lead.py`

 * *Files identical despite different names*

### Comparing `inception_reports-0.1/inception_reports/generate_reports_manager.py` & `inception_reports-0.2/inception_reports/generate_reports_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 import cassis
 import matplotlib.pyplot as plt
 import numpy as np
 import streamlit as st
 from matplotlib import gridspec
 from pycaprio import Pycaprio
+from datetime import datetime
 
 # suppress deprecation warnings related to the use of the pyplot
 # can be solved by sending the fig instead of the plt to streamlit
 st.set_option("deprecation.showPyplotGlobalUse", False)
 st.set_page_config(page_title="INCEpTION Reporting Dashboard", layout="centered")
 css = """
 <style>
@@ -55,15 +56,15 @@
 
     Parameters:
         project (dict): A dict containing project information, namely the name, tags, annotations, and logs.
 
     """
 
     # df = project["logs"]
-    project_name = project["name"]
+    project_name = project["name"].strip(".zip")
     project_tags = project["tags"]
     project_annotations = project["annotations"]
     project_documents = project["documents"]
 
     doc_categories = {
         "ANNOTATION_IN_PROGRESS": 0,
         "ANNOTATION_FINISHED": 0,
@@ -156,19 +157,15 @@
     fig.suptitle(
         f'{project_name.split(".")[0]}\nTotal Annotations: {total_annotations}',
         fontsize=16,
     )
     fig.tight_layout()
     st.pyplot()
 
-    # st.title(f"Project: {project_name.split('.')[0]}")
-    if st.button(f"Export data for {project_name.split('.')[0]}"):
-        with open(f"{project_name.split('.')[0]}_data.json", "w") as output_file:
-            output_file.write(json.dumps(project_data, indent=4))
-        st.success(f"{project_name.split('.')[0]} data exported successfully ✅")
+    export_data(project_data)
 
 
 def find_element_by_name(element_list, name):
     """
     Finds an element in the given element list by its name.
 
     Args:
@@ -339,25 +336,48 @@
             st.session_state['method'] = 'API'
             st.session_state['projects_folder'] = f"{os.path.expanduser('~')}/.inception_reports/projects"
 
 
 
 def create_directory_in_home():
     """
-    Creates a directory in the user's home directory for storing Inception reports.
+    Creates a directory in the user's home directory for storing Inception reports imported over the API.
     """
     home_dir = os.path.expanduser("~")
     new_dir_path = os.path.join(home_dir, ".inception_reports")
     try:
         os.makedirs(new_dir_path)
         os.makedirs(os.path.join(new_dir_path, "projects"))
     except FileExistsError:
         pass
 
 
+def export_data(project_data, output_directory=None):
+    """
+    Export project data to a JSON file, and store it in a directory named after the project and the current date.
+
+    Parameters:
+        project_data (dict): The data to be exported.
+    """
+    current_date = datetime.now().strftime("%Y_%m_%d")
+    directory_name = f'exported_data_{current_date}'
+
+    if output_directory is None:
+        output_directory = os.path.join(os.getcwd(), directory_name)
+    else:
+        output_directory = os.path.join(output_directory, directory_name)
+    
+    if not os.path.exists(output_directory):
+        os.makedirs(output_directory)
+
+    project_name = project_data["project_name"]
+    with open(f"{output_directory}/{project_name.split('.')[0]}_data_{current_date}.json", "w") as output_file:
+        json.dump(project_data, output_file, indent=4)
+    st.success(f"{project_name.split('.')[0]} documents status exported successfully ✅")
+
 def main():
     create_directory_in_home()
     
     st.title("INCEpTION Projects Statistics")
 
     if 'initialized' not in st.session_state:
         select_method_to_import_data()
```

### Comparing `inception_reports-0.1/inception_reports.egg-info/PKG-INFO` & `inception_reports-0.2/inception_reports.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inception_reports
-Version: 0.1
+Version: 0.2
 Summary: Generate plots that report the progress of an INCEpTION project.
 Author-email: Serwar Basch <serwar.basch@tu-darmstadt.de>
 Project-URL: Homepage, https://github.com/inception-project/inception-reporting-dashboard
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -25,15 +25,15 @@
 In its current state, it can be used by the project manager on site to visualize different metrics regarding the progress of the project, and the type of annotations done.
 
 In case the project is part of a bigger project, the project progress can be exported to be sent to a project lead in a centralized location who, in turn, can use the package to get an overview of the progress across the different projects and locations.
 
 ## Getting started
 
 1. Ensure you have python 3.11 or higher (check it using python --version)
-2. Install the package using ``pip install inception_reports``
+2. Install the package using ``pip install inception-reports``
 3. Run the script using ``inception_reports --help`` this will show you the options you have:
     1. Run it with ``inception_reports --manager`` if you have one python project, or are responsible for one location.
     2. Run it with ``inception_reports --lead`` if you're leading multiple projects, or multiple locations.
 4. Regardless of the mode you run the package with, it should open a browser window. Follow the instructions on the page to proceed.
 
 ## Issues
```

### Comparing `inception_reports-0.1/inception_reports.egg-info/SOURCES.txt` & `inception_reports-0.2/inception_reports.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inception_reports-0.1/pyproject.toml` & `inception_reports-0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inception_reports"
 description = "Generate plots that report the progress of an INCEpTION project."
-version = "0.1"
+version = "0.2"
 authors = [
     { name = "Serwar Basch", email = "serwar.basch@tu-darmstadt.de" }
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
     "streamlit",
```

### Comparing `inception_reports-0.1/tests/test_generate_reports_lead.py` & `inception_reports-0.2/tests/test_generate_reports_lead.py`

 * *Files identical despite different names*

### Comparing `inception_reports-0.1/tests/test_generate_reports_manager.py` & `inception_reports-0.2/tests/test_generate_reports_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
 import json
 import os
 import tempfile
 import zipfile
 from unittest.mock import Mock, patch
+from datetime import datetime
 
-from inception_reports.generate_reports_manager import find_element_by_name, read_dir
+from inception_reports.generate_reports_manager import find_element_by_name, read_dir, export_data
 
 
 def test_find_element_by_name():
     MockElement_1 = Mock()
     MockElement_1.configure_mock(**{"name": "element1", "uiName": "UI Element 1"})
     MockElement_2 = Mock()
     MockElement_2.configure_mock(**{"name": "element2", "uiName": "UI Element 2"})
@@ -69,7 +71,32 @@
         print(project['annotations'])
         assert project['name'] == zip_name, "Project name should match the zip file name"
         assert set(project['tags']) == {"tag1", "tag2"}, "Should extract correct tags from project metadata"
         assert project['documents'] == ["doc1.txt", "doc2.txt"], "Should list all source documents"
         assert 'doc1' in project['annotations'], "Should include annotations in the project data"
         assert project['annotations']['doc1'] == "MockCASObject", "Should load CAS objects for annotations"
 
+
+def test_export_data(tmpdir):
+    project_data = {
+        "project_name": "project1",
+        "project_tags": ["tag1", "tag2"],
+        "doc_categories": {
+            "NEW": 10,
+            "ANNOTATION_IN_PROGRESS": 5,
+            "ANNOTATION_FINISHED": 15,
+            "CURATION_IN_PROGRESS": 3,
+            "CURATION_FINISHED": 7,
+        },
+    }
+
+    current_date = datetime.now().strftime("%Y_%m_%d")
+    output_directory = tmpdir.mkdir("output")
+    export_data(project_data, output_directory)
+
+    expected_file_path = os.path.join(output_directory, f"exported_data_{current_date}/{project_data['project_name']}_data_{current_date}.json")
+    assert os.path.exists(expected_file_path)
+
+    with open(expected_file_path, "r") as output_file:
+        exported_data = json.load(output_file)
+
+    assert exported_data == project_data
```

