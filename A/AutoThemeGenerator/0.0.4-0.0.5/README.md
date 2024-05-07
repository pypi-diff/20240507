# Comparing `tmp/autothemegenerator-0.0.4.tar.gz` & `tmp/autothemegenerator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autothemegenerator-0.0.4.tar", last modified: Tue May  7 12:33:49 2024, max compression
+gzip compressed data, was "autothemegenerator-0.0.5.tar", last modified: Tue May  7 13:00:37 2024, max compression
```

## Comparing `autothemegenerator-0.0.4.tar` & `autothemegenerator-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 12:33:49.277277 autothemegenerator-0.0.4/
-drwxrwxrwx   0        0        0        0 2024-05-07 12:33:49.256958 autothemegenerator-0.0.4/AutoThemeGenerator/
--rw-rw-rw-   0        0        0    29700 2024-05-07 12:33:14.000000 autothemegenerator-0.0.4/AutoThemeGenerator/AutoThemeGenerator.py
--rw-rw-rw-   0        0        0       86 2024-05-07 12:19:43.000000 autothemegenerator-0.0.4/AutoThemeGenerator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 12:33:49.276275 autothemegenerator-0.0.4/AutoThemeGenerator.egg-info/
--rw-rw-rw-   0        0        0     3960 2024-05-07 12:33:49.000000 autothemegenerator-0.0.4/AutoThemeGenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-07 12:33:49.000000 autothemegenerator-0.0.4/AutoThemeGenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 12:33:49.000000 autothemegenerator-0.0.4/AutoThemeGenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-07 12:33:49.000000 autothemegenerator-0.0.4/AutoThemeGenerator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-07 12:33:49.000000 autothemegenerator-0.0.4/AutoThemeGenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      368 2024-05-07 12:32:58.000000 autothemegenerator-0.0.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2024-05-07 12:08:17.000000 autothemegenerator-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-05-07 12:08:18.000000 autothemegenerator-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3960 2024-05-07 12:33:49.276275 autothemegenerator-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3079 2024-05-07 12:08:19.000000 autothemegenerator-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-07 12:33:49.277277 autothemegenerator-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1320 2024-05-07 12:32:37.000000 autothemegenerator-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:00:37.253498 autothemegenerator-0.0.5/
+drwxrwxrwx   0        0        0        0 2024-05-07 13:00:37.240275 autothemegenerator-0.0.5/AutoThemeGenerator/
+-rw-rw-rw-   0        0        0    29815 2024-05-07 12:57:56.000000 autothemegenerator-0.0.5/AutoThemeGenerator/AutoThemeGenerator.py
+-rw-rw-rw-   0        0        0       86 2024-05-07 12:19:43.000000 autothemegenerator-0.0.5/AutoThemeGenerator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:00:37.252492 autothemegenerator-0.0.5/AutoThemeGenerator.egg-info/
+-rw-rw-rw-   0        0        0     4366 2024-05-07 13:00:37.000000 autothemegenerator-0.0.5/AutoThemeGenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-07 13:00:37.000000 autothemegenerator-0.0.5/AutoThemeGenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 13:00:37.000000 autothemegenerator-0.0.5/AutoThemeGenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-07 13:00:37.000000 autothemegenerator-0.0.5/AutoThemeGenerator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 13:00:37.000000 autothemegenerator-0.0.5/AutoThemeGenerator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      524 2024-05-07 12:58:41.000000 autothemegenerator-0.0.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2024-05-07 12:08:17.000000 autothemegenerator-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-07 12:08:18.000000 autothemegenerator-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4366 2024-05-07 13:00:37.253498 autothemegenerator-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3489 2024-05-07 12:55:19.000000 autothemegenerator-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 13:00:37.253498 autothemegenerator-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1320 2024-05-07 12:58:46.000000 autothemegenerator-0.0.5/setup.py
```

### Comparing `autothemegenerator-0.0.4/AutoThemeGenerator/AutoThemeGenerator.py` & `autothemegenerator-0.0.5/AutoThemeGenerator/AutoThemeGenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -527,14 +527,17 @@
     """
     Save the analysis results to a JSON file.
 
     Parameters:
     results (list): The analysis results to save.
     file_path (str): The path where the JSON file will be saved.
     """
+    directory = os.path.dirname(file_path)
+    if not os.path.exists(directory):
+        os.makedirs(directory)
     with open(file_path, 'w', encoding = 'utf-8') as file:
         json.dump(results, file, ensure_ascii = False, indent = 0)
 
 
 def load_results_from_json(file_path):
     """
     Load the analysis results from a JSON file.
```

### Comparing `autothemegenerator-0.0.4/AutoThemeGenerator.egg-info/PKG-INFO` & `autothemegenerator-0.0.5/AutoThemeGenerator.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThemeGenerator
-Version: 0.0.4
+Version: 0.0.5
 Summary: Performing thematic analysis with OpenAI's GPT-4 models
 Author: Charles Alba
 Author-email: alba@wustl.edu
 Keywords: GPT models,Thematic analysis,OpenAI,Qualitiative studies,transcripts,interviews
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,17 @@
 Requires-Dist: nltk==3.8.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: python-docx
 Requires-Dist: tqdm
 
 `AutoThemeGenerator` is a package that allows you to perform qualitative analysis using OpenAI's GPT models.
 
+## User inputs
+Users are only required to specify the folder location where their interview transcripts are stored. Accepted formats of transcripts include `PDF`, `.docx`, and `.txt` (prefered).`AutoThemeGenerator` assumes that each document is a transcript of one interviewed participant.
+
 ## Requirements
 ### Required packages
 To use `AutoThemeGenerator`, you are required to have the following packages installed:  
 - `openai`  
 - `docx`    
 - `tqdm`    
 - `nltk`    
@@ -40,27 +43,32 @@
 If you do not have this packages installed in python, you can do the following:
 ```bash
 pip install openai docx tqdm nltk nltk.tokenize python-docx textract zipfile shutil requests json
 ```
 ### OpenAI API key
 You also need an OpenAI key to be able to use this package. If you do not have one, you can apply for an OpenAI API key at [platform.openai.com/api-keys](https://platform.openai.com/api-keys). 
 
-
 ## Installation
 To install in python, simply do the following: 
-
 ```bash
 pip install AutoThemeGenerator
 ```
 
 ## Quick Start
-Here we provide a quick example on how you can execute GPT4QualitativeAnalysis to conveniently perform qualitative analysis from your transcript. For details towards each of the package's functions and parameters, refer to the [documention](documention.md). 
-
+Here we provide a quick example on how you can execute `AutoThemeGenerator` to conveniently perform qualitative analysis from your transcript. For details towards each of the package's functions and parameters, refer to the [documention](documention.md). 
 ```python
-from AutoThemeGenerator import *
+from AutoThemeGenerator import analyze_and_synthesize_transcripts
+
+# Specify the folders containing your transcript
+# This is the folder containing transcripts in .docx, .PDF or .txt format
+directory_path = "my_transcript_folder"
+# specify your OpenAI API key
+api_key = "<insert your API key>"
+# specify the folder you wish to save your themes. 
+save_results_path = "folder_of_my_saved_results"
 
 # specify the context of your study
 context = (
     "Physical inactivity is a major risk factor for developing several chronic illness. "
     "However, university students and staff in the UK are found to be more physically inactive "
     "compared the general UK population. "
     )
@@ -75,36 +83,23 @@
 survey_script = (
     "Knowledge\n "
     "What do you know about physical activity? How might you define physical activity? "
     "... ..." # note: truncated to save space
     "... ..." 
     )
 
-
-
-# Specify the folders containing your transcript
-directory_path = "my_transcript_folder"
-# specify your OpenAI API key
-api_key = "<insert your API key>"
-# specify the folder you wish to save your themes. 
-save_results_path = "folder_of_my_saved_results"
-
-
 # Analyze and synthesize transcripts
 initial_themes, individual_synthesized_themes, overall_synthesized_themes = \
 analyze_and_synthesize_transcripts(
     directory_path = directory_path, context = context,
     research_questions = research_questions, script = survey_script,
     api_key = api_key, save_results_path = save_results_path)
 
-
-# optional (load your saved themes)
-overall_synthesized_themes = load_results_from_json(
-    os.path.join(save_results_path, "themes_overall.json"))
-
 # display your study-level themes
 print(overall_synthesized_themes)
 ```
-
 You can now view the themes in the form of a topic sentence, a detailed explaination and a relevant quote
 
 
+## Citation
+
+Y Yang, C Alba, W Xi, M Li, C Wang, A Jami, R An. "GPT Models Can Perform Thematic Analysis in Public Health Studies, Akin to Qualitative Researchers" Working paper.
```

### Comparing `autothemegenerator-0.0.4/LICENSE.txt` & `autothemegenerator-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autothemegenerator-0.0.4/PKG-INFO` & `autothemegenerator-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThemeGenerator
-Version: 0.0.4
+Version: 0.0.5
 Summary: Performing thematic analysis with OpenAI's GPT-4 models
 Author: Charles Alba
 Author-email: alba@wustl.edu
 Keywords: GPT models,Thematic analysis,OpenAI,Qualitiative studies,transcripts,interviews
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,17 @@
 Requires-Dist: nltk==3.8.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: python-docx
 Requires-Dist: tqdm
 
 `AutoThemeGenerator` is a package that allows you to perform qualitative analysis using OpenAI's GPT models.
 
+## User inputs
+Users are only required to specify the folder location where their interview transcripts are stored. Accepted formats of transcripts include `PDF`, `.docx`, and `.txt` (prefered).`AutoThemeGenerator` assumes that each document is a transcript of one interviewed participant.
+
 ## Requirements
 ### Required packages
 To use `AutoThemeGenerator`, you are required to have the following packages installed:  
 - `openai`  
 - `docx`    
 - `tqdm`    
 - `nltk`    
@@ -40,27 +43,32 @@
 If you do not have this packages installed in python, you can do the following:
 ```bash
 pip install openai docx tqdm nltk nltk.tokenize python-docx textract zipfile shutil requests json
 ```
 ### OpenAI API key
 You also need an OpenAI key to be able to use this package. If you do not have one, you can apply for an OpenAI API key at [platform.openai.com/api-keys](https://platform.openai.com/api-keys). 
 
-
 ## Installation
 To install in python, simply do the following: 
-
 ```bash
 pip install AutoThemeGenerator
 ```
 
 ## Quick Start
-Here we provide a quick example on how you can execute GPT4QualitativeAnalysis to conveniently perform qualitative analysis from your transcript. For details towards each of the package's functions and parameters, refer to the [documention](documention.md). 
-
+Here we provide a quick example on how you can execute `AutoThemeGenerator` to conveniently perform qualitative analysis from your transcript. For details towards each of the package's functions and parameters, refer to the [documention](documention.md). 
 ```python
-from AutoThemeGenerator import *
+from AutoThemeGenerator import analyze_and_synthesize_transcripts
+
+# Specify the folders containing your transcript
+# This is the folder containing transcripts in .docx, .PDF or .txt format
+directory_path = "my_transcript_folder"
+# specify your OpenAI API key
+api_key = "<insert your API key>"
+# specify the folder you wish to save your themes. 
+save_results_path = "folder_of_my_saved_results"
 
 # specify the context of your study
 context = (
     "Physical inactivity is a major risk factor for developing several chronic illness. "
     "However, university students and staff in the UK are found to be more physically inactive "
     "compared the general UK population. "
     )
@@ -75,36 +83,23 @@
 survey_script = (
     "Knowledge\n "
     "What do you know about physical activity? How might you define physical activity? "
     "... ..." # note: truncated to save space
     "... ..." 
     )
 
-
-
-# Specify the folders containing your transcript
-directory_path = "my_transcript_folder"
-# specify your OpenAI API key
-api_key = "<insert your API key>"
-# specify the folder you wish to save your themes. 
-save_results_path = "folder_of_my_saved_results"
-
-
 # Analyze and synthesize transcripts
 initial_themes, individual_synthesized_themes, overall_synthesized_themes = \
 analyze_and_synthesize_transcripts(
     directory_path = directory_path, context = context,
     research_questions = research_questions, script = survey_script,
     api_key = api_key, save_results_path = save_results_path)
 
-
-# optional (load your saved themes)
-overall_synthesized_themes = load_results_from_json(
-    os.path.join(save_results_path, "themes_overall.json"))
-
 # display your study-level themes
 print(overall_synthesized_themes)
 ```
-
 You can now view the themes in the form of a topic sentence, a detailed explaination and a relevant quote
 
 
+## Citation
+
+Y Yang, C Alba, W Xi, M Li, C Wang, A Jami, R An. "GPT Models Can Perform Thematic Analysis in Public Health Studies, Akin to Qualitative Researchers" Working paper.
```

### Comparing `autothemegenerator-0.0.4/README.md` & `autothemegenerator-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 `AutoThemeGenerator` is a package that allows you to perform qualitative analysis using OpenAI's GPT models.
 
+## User inputs
+Users are only required to specify the folder location where their interview transcripts are stored. Accepted formats of transcripts include `PDF`, `.docx`, and `.txt` (prefered).`AutoThemeGenerator` assumes that each document is a transcript of one interviewed participant.
+
 ## Requirements
 ### Required packages
 To use `AutoThemeGenerator`, you are required to have the following packages installed:  
 - `openai`  
 - `docx`    
 - `tqdm`    
 - `nltk`    
@@ -18,27 +21,32 @@
 If you do not have this packages installed in python, you can do the following:
 ```bash
 pip install openai docx tqdm nltk nltk.tokenize python-docx textract zipfile shutil requests json
 ```
 ### OpenAI API key
 You also need an OpenAI key to be able to use this package. If you do not have one, you can apply for an OpenAI API key at [platform.openai.com/api-keys](https://platform.openai.com/api-keys). 
 
-
 ## Installation
 To install in python, simply do the following: 
-
 ```bash
 pip install AutoThemeGenerator
 ```
 
 ## Quick Start
-Here we provide a quick example on how you can execute GPT4QualitativeAnalysis to conveniently perform qualitative analysis from your transcript. For details towards each of the package's functions and parameters, refer to the [documention](documention.md). 
-
+Here we provide a quick example on how you can execute `AutoThemeGenerator` to conveniently perform qualitative analysis from your transcript. For details towards each of the package's functions and parameters, refer to the [documention](documention.md). 
 ```python
-from AutoThemeGenerator import *
+from AutoThemeGenerator import analyze_and_synthesize_transcripts
+
+# Specify the folders containing your transcript
+# This is the folder containing transcripts in .docx, .PDF or .txt format
+directory_path = "my_transcript_folder"
+# specify your OpenAI API key
+api_key = "<insert your API key>"
+# specify the folder you wish to save your themes. 
+save_results_path = "folder_of_my_saved_results"
 
 # specify the context of your study
 context = (
     "Physical inactivity is a major risk factor for developing several chronic illness. "
     "However, university students and staff in the UK are found to be more physically inactive "
     "compared the general UK population. "
     )
@@ -53,36 +61,23 @@
 survey_script = (
     "Knowledge\n "
     "What do you know about physical activity? How might you define physical activity? "
     "... ..." # note: truncated to save space
     "... ..." 
     )
 
-
-
-# Specify the folders containing your transcript
-directory_path = "my_transcript_folder"
-# specify your OpenAI API key
-api_key = "<insert your API key>"
-# specify the folder you wish to save your themes. 
-save_results_path = "folder_of_my_saved_results"
-
-
 # Analyze and synthesize transcripts
 initial_themes, individual_synthesized_themes, overall_synthesized_themes = \
 analyze_and_synthesize_transcripts(
     directory_path = directory_path, context = context,
     research_questions = research_questions, script = survey_script,
     api_key = api_key, save_results_path = save_results_path)
 
-
-# optional (load your saved themes)
-overall_synthesized_themes = load_results_from_json(
-    os.path.join(save_results_path, "themes_overall.json"))
-
 # display your study-level themes
 print(overall_synthesized_themes)
 ```
-
 You can now view the themes in the form of a topic sentence, a detailed explaination and a relevant quote
 
 
+## Citation
+
+Y Yang, C Alba, W Xi, M Li, C Wang, A Jami, R An. "GPT Models Can Perform Thematic Analysis in Public Health Studies, Akin to Qualitative Researchers" Working paper.
```

### Comparing `autothemegenerator-0.0.4/setup.py` & `autothemegenerator-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 readme_path = os.path.join(here, "README.md")
 with codecs.open(readme_path, encoding="utf-8") as fh:
     long_description = fh.read()
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Performing thematic analysis with OpenAI\'s GPT-4 models'
 LONG_DESCRIPTION = 'A package uses openAI\'s GPT-4 model to perform thematic analysis using interview transcripts from qualititative studies'
 
 # Setting up
 setup(
     name="AutoThemeGenerator",
     version=VERSION,
```

