# Comparing `tmp/leanblueprint-0.0.8.tar.gz` & `tmp/leanblueprint-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leanblueprint-0.0.8.tar", last modified: Tue Apr 30 16:12:54 2024, max compression
+gzip compressed data, was "leanblueprint-0.0.9.tar", last modified: Mon May  6 23:38:18 2024, max compression
```

## Comparing `leanblueprint-0.0.8.tar` & `leanblueprint-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 16:12:54.934962 leanblueprint-0.0.8/
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    11357 2024-03-02 23:37:31.000000 leanblueprint-0.0.8/LICENSE
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      158 2024-03-02 23:37:31.000000 leanblueprint-0.0.8/MANIFEST.in
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       36 2024-03-02 23:37:31.000000 leanblueprint-0.0.8/NOTICE
--rw-r--r--   0 pmassot   (1000) pmassot   (1000)     9361 2024-04-30 16:12:54.934962 leanblueprint-0.0.8/PKG-INFO
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     8690 2024-04-30 01:47:25.000000 leanblueprint-0.0.8/README.md
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 16:12:54.930962 leanblueprint-0.0.8/leanblueprint/
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 16:12:54.930962 leanblueprint-0.0.8/leanblueprint/Packages/
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        0 2024-03-02 23:37:31.000000 leanblueprint-0.0.8/leanblueprint/Packages/__init__.py
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    11578 2024-04-30 16:07:36.000000 leanblueprint-0.0.8/leanblueprint/Packages/blueprint.py
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 16:12:54.930962 leanblueprint-0.0.8/leanblueprint/Packages/renderer_templates/
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       49 2024-03-02 22:17:10.000000 leanblueprint-0.0.8/leanblueprint/Packages/renderer_templates/blueprint.jinja2s
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        0 2020-05-23 12:35:34.000000 leanblueprint-0.0.8/leanblueprint/__init__.py
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    15180 2024-04-30 02:43:23.000000 leanblueprint-0.0.8/leanblueprint/client.py
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 16:12:54.930962 leanblueprint-0.0.8/leanblueprint/static/
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      103 2024-01-05 14:42:04.000000 leanblueprint-0.0.8/leanblueprint/static/blueprint.css
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 16:12:54.934962 leanblueprint-0.0.8/leanblueprint/templates/
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       34 2024-04-29 19:18:12.000000 leanblueprint-0.0.8/leanblueprint/templates/blueprint.sty
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     2825 2024-04-30 01:49:45.000000 leanblueprint-0.0.8/leanblueprint/templates/blueprint.yml
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      364 2024-03-02 23:37:31.000000 leanblueprint-0.0.8/leanblueprint/templates/content.tex
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      483 2024-03-02 23:37:31.000000 leanblueprint-0.0.8/leanblueprint/templates/extra_styles.css
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      182 2024-03-02 23:37:31.000000 leanblueprint-0.0.8/leanblueprint/templates/latexmkrc
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 16:12:54.934962 leanblueprint-0.0.8/leanblueprint/templates/macros/
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      143 2024-03-02 23:37:31.000000 leanblueprint-0.0.8/leanblueprint/templates/macros/common.tex
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     1077 2024-04-29 19:18:12.000000 leanblueprint-0.0.8/leanblueprint/templates/macros/print.tex
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      261 2024-03-02 23:37:31.000000 leanblueprint-0.0.8/leanblueprint/templates/macros/web.tex
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      340 2024-03-02 23:37:31.000000 leanblueprint-0.0.8/leanblueprint/templates/plastex.cfg
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     1125 2024-03-02 23:37:31.000000 leanblueprint-0.0.8/leanblueprint/templates/print.tex
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      643 2024-03-02 23:37:31.000000 leanblueprint-0.0.8/leanblueprint/templates/web.tex
-drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-04-30 16:12:54.934962 leanblueprint-0.0.8/leanblueprint.egg-info/
--rw-r--r--   0 pmassot   (1000) pmassot   (1000)     9361 2024-04-30 16:12:54.000000 leanblueprint-0.0.8/leanblueprint.egg-info/PKG-INFO
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      942 2024-04-30 16:12:54.000000 leanblueprint-0.0.8/leanblueprint.egg-info/SOURCES.txt
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        1 2024-04-30 16:12:54.000000 leanblueprint-0.0.8/leanblueprint.egg-info/dependency_links.txt
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       64 2024-04-30 16:12:54.000000 leanblueprint-0.0.8/leanblueprint.egg-info/entry_points.txt
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        1 2024-01-30 23:24:22.000000 leanblueprint-0.0.8/leanblueprint.egg-info/not-zip-safe
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      113 2024-04-30 16:12:54.000000 leanblueprint-0.0.8/leanblueprint.egg-info/requires.txt
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       14 2024-04-30 16:12:54.000000 leanblueprint-0.0.8/leanblueprint.egg-info/top_level.txt
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      797 2024-04-30 16:12:54.934962 leanblueprint-0.0.8/setup.cfg
--rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       70 2024-03-02 23:37:31.000000 leanblueprint-0.0.8/setup.py
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-05-06 23:38:18.435917 leanblueprint-0.0.9/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    11357 2024-03-02 23:37:31.000000 leanblueprint-0.0.9/LICENSE
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      158 2024-03-02 23:37:31.000000 leanblueprint-0.0.9/MANIFEST.in
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       36 2024-03-02 23:37:31.000000 leanblueprint-0.0.9/NOTICE
+-rw-r--r--   0 pmassot   (1000) pmassot   (1000)    11294 2024-05-06 23:38:18.435917 leanblueprint-0.0.9/PKG-INFO
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    10623 2024-05-06 23:02:33.000000 leanblueprint-0.0.9/README.md
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-05-06 23:38:18.431916 leanblueprint-0.0.9/leanblueprint/
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-05-06 23:38:18.435917 leanblueprint-0.0.9/leanblueprint/Packages/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        0 2024-03-02 23:37:31.000000 leanblueprint-0.0.9/leanblueprint/Packages/__init__.py
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    11578 2024-04-30 16:07:36.000000 leanblueprint-0.0.9/leanblueprint/Packages/blueprint.py
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-05-06 23:38:18.435917 leanblueprint-0.0.9/leanblueprint/Packages/renderer_templates/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       49 2024-03-02 22:17:10.000000 leanblueprint-0.0.9/leanblueprint/Packages/renderer_templates/blueprint.jinja2s
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        0 2020-05-23 12:35:34.000000 leanblueprint-0.0.9/leanblueprint/__init__.py
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)    15180 2024-04-30 02:43:23.000000 leanblueprint-0.0.9/leanblueprint/client.py
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-05-06 23:38:18.435917 leanblueprint-0.0.9/leanblueprint/static/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      103 2024-01-05 14:42:04.000000 leanblueprint-0.0.9/leanblueprint/static/blueprint.css
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-05-06 23:38:18.435917 leanblueprint-0.0.9/leanblueprint/templates/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       34 2024-04-29 19:18:12.000000 leanblueprint-0.0.9/leanblueprint/templates/blueprint.sty
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     2825 2024-04-30 01:49:45.000000 leanblueprint-0.0.9/leanblueprint/templates/blueprint.yml
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      364 2024-03-02 23:37:31.000000 leanblueprint-0.0.9/leanblueprint/templates/content.tex
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      483 2024-03-02 23:37:31.000000 leanblueprint-0.0.9/leanblueprint/templates/extra_styles.css
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      182 2024-03-02 23:37:31.000000 leanblueprint-0.0.9/leanblueprint/templates/latexmkrc
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-05-06 23:38:18.435917 leanblueprint-0.0.9/leanblueprint/templates/macros/
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      143 2024-03-02 23:37:31.000000 leanblueprint-0.0.9/leanblueprint/templates/macros/common.tex
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     1102 2024-05-06 23:34:32.000000 leanblueprint-0.0.9/leanblueprint/templates/macros/print.tex
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      261 2024-03-02 23:37:31.000000 leanblueprint-0.0.9/leanblueprint/templates/macros/web.tex
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      340 2024-03-02 23:37:31.000000 leanblueprint-0.0.9/leanblueprint/templates/plastex.cfg
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)     1125 2024-03-02 23:37:31.000000 leanblueprint-0.0.9/leanblueprint/templates/print.tex
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      643 2024-03-02 23:37:31.000000 leanblueprint-0.0.9/leanblueprint/templates/web.tex
+drwxrwxr-x   0 pmassot   (1000) pmassot   (1000)        0 2024-05-06 23:38:18.435917 leanblueprint-0.0.9/leanblueprint.egg-info/
+-rw-r--r--   0 pmassot   (1000) pmassot   (1000)    11294 2024-05-06 23:38:18.000000 leanblueprint-0.0.9/leanblueprint.egg-info/PKG-INFO
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      942 2024-05-06 23:38:18.000000 leanblueprint-0.0.9/leanblueprint.egg-info/SOURCES.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        1 2024-05-06 23:38:18.000000 leanblueprint-0.0.9/leanblueprint.egg-info/dependency_links.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       64 2024-05-06 23:38:18.000000 leanblueprint-0.0.9/leanblueprint.egg-info/entry_points.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)        1 2024-01-30 23:24:22.000000 leanblueprint-0.0.9/leanblueprint.egg-info/not-zip-safe
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      113 2024-05-06 23:38:18.000000 leanblueprint-0.0.9/leanblueprint.egg-info/requires.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       14 2024-05-06 23:38:18.000000 leanblueprint-0.0.9/leanblueprint.egg-info/top_level.txt
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)      797 2024-05-06 23:38:18.435917 leanblueprint-0.0.9/setup.cfg
+-rw-rw-r--   0 pmassot   (1000) pmassot   (1000)       70 2024-03-02 23:37:31.000000 leanblueprint-0.0.9/setup.py
```

### Comparing `leanblueprint-0.0.8/LICENSE` & `leanblueprint-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `leanblueprint-0.0.8/PKG-INFO` & `leanblueprint-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-Metadata-Version: 2.1
-Name: leanblueprint
-Version: 0.0.8
-Summary: Lean prover blueprint plasTeX plugin.
-Home-page: https://github.com/PatrickMassot/leanblueprint
-Author: Patrick Massot
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-Requires-Dist: plasTeX>=3.1
-Requires-Dist: plastexshowmore>=0.0.2
-Requires-Dist: plastexdepgraph>=0.0.4
-Requires-Dist: click
-Requires-Dist: rich
-Requires-Dist: rich-click
-Requires-Dist: Jinja2>=3.1.0
-Requires-Dist: GitPython>=3.1.28
-
 # Lean blueprints
 
 This is a [plasTeX](https://github.com/plastex/plastex/) plugin allowing
 to write blueprints for Lean 4 projects.
+You can learn what those blueprints are about by reading
+Terence Tao’s excellent [blog post about it](https://terrytao.wordpress.com/2023/11/18/formalizing-the-proof-of-pfr-in-lean4-using-blueprint-a-short-tour/).
+
+This infrastructure was originally created in 2020 for the
+[Sphere Eversion Project](https://leanprover-community.github.io/sphere-eversion/).
+Since then, it has been used by many projects. The list below will give you many
+examples but is not intended to be exhaustive.
+It is in approximate chronological order.
+
+* [Sphere eversion project](https://leanprover-community.github.io/sphere-eversion/blueprint/index.html).
+* [Liquid tensor experiment](https://leanprover-community.github.io/liquid/)
+* [Fermat’s last theorem for regular primes](https://leanprover-community.github.io/flt-regular/blueprint/)
+* [Arithmetic Progressions - Almost Periodicity](https://yaeldillies.github.io/LeanAPAP/blueprint/)
+* [Polynomial Freiman-Ruzsa Conjecture](https://teorth.github.io/pfr/blueprint/)
+* [Lower bounds for hypothesis testing based on information theory](https://remydegenne.github.io/testing-lower-bounds/blueprint/)
+* [Prime number theorem and…](https://alexkontorovich.github.io/PrimeNumberTheoremAnd/web/)
+* [Fermat's Last Theorem for 3](https://pitmonticone.github.io/FLT3/blueprint)
+* [Fermat’s last theorem](https://imperialcollegelondon.github.io/FLT/blueprint/)
 
 ## Installation
 
 This package depends on `plastexdepgraph` which requires graphviz and its development libraries. 
 If you have a user-friendly OS, it is as simple as 
 `sudo apt install graphviz libgraphviz-dev`. 
 See https://pygraphviz.github.io/documentation/stable/install.html otherwise.
@@ -53,15 +49,15 @@
 particular the creation of a blueprint for your Lean project. This tool is not
 mandatory in any way. Its goal is to make it easy to create a blueprint without
 worrying about choosing a file layout or a continuous integration and deployment
 setup. As every one–size-fits-all tool, it is fairly opinionated. It assumes in
 particular that your project repository is hosted on Github and you want to host
 its blueprint on github.io.
 
-If you don’t want to use the `leanblueprint` command line tool, you can use use
+If you don’t want to use the `leanblueprint` command line tool, you can use
 this plugin as any other plasTeX plugin, using
 `plastex --plugins leanblueprint my_file.tex` (not recommended).
 
 In order to use the `leanblueprint` tool, you need to already have a Lean
 project created using lake. In addition, your blueprint will be easier to
 configure if you have at least one commit in the git repository of your project
 and you have already configured its GitHub git remote (GitHub displays
@@ -107,15 +103,15 @@
   in the blueprint exist in the project (or in a dependency of the project such
   as Mathlib). This requires a compiled Lean project, so make sure to run `lake build` beforehand.
 * `leanblueprint all` to run the previous three commands.
 * `leanblueprint serve` to start a local webserver showing your local blueprint
   (this sounds silly but web browsers paranoia makes it impossible to simply
   open the generated html pages without serving them). The url you should use
   in your browser will be displayed and will probably be `http://0.0.0.0:8000/`,
-  unless the port 8000 is already is use.
+  unless the port 8000 is already in use.
 
 Note: plasTeX does not call BibTeX. If you have a bibliography, you should use
 `leanblueprint pdf` before `leanblueprint web` to get it to work in the web
 version (and redo it when you add a reference).
 
 ## Editing the blueprint
 
@@ -167,14 +163,26 @@
   This obviously follows from what we did so far.
 \end
 ```
 
 Note that the proof above is abbreviated in this documentation. 
 Be nice to you and your collaborators and include more details in your blueprint proofs!
 
+By default, the dependency graph will collect the environments definition,
+lemma, proposition, theorem and corollary. You can change this list using the
+`thms` option which expects a list of environment names separated by `+` signs. 
+For instance you can write
+```latex
+\usepackage[thms=dfn+lem+prop+thm+cor]{blueprint}
+```
+if you like short environment names. See the 
+[plastexdepgraph documentation](https://github.com/PatrickMassot/plastexdepgraph/blob/master/README.md) 
+for other dependency graph options having nothing to do with Lean.
+
+
 The above macros are by far the most important, but there are a couple more.
 
 * `\notready` which claims the surrounding environment is not ready to be formalized,
   typically because it requires more blueprint work.
 * `\discussion` gives a GitHub issue number where the surrounding definition or
   statement is discussed.
 * `\proves` inside a proof environment gives the LaTeX label of the LaTeX
```

### Comparing `leanblueprint-0.0.8/README.md` & `leanblueprint-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,51 @@
+Metadata-Version: 2.1
+Name: leanblueprint
+Version: 0.0.9
+Summary: Lean prover blueprint plasTeX plugin.
+Home-page: https://github.com/PatrickMassot/leanblueprint
+Author: Patrick Massot
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+Requires-Dist: plasTeX>=3.1
+Requires-Dist: plastexshowmore>=0.0.2
+Requires-Dist: plastexdepgraph>=0.0.4
+Requires-Dist: click
+Requires-Dist: rich
+Requires-Dist: rich-click
+Requires-Dist: Jinja2>=3.1.0
+Requires-Dist: GitPython>=3.1.28
+
 # Lean blueprints
 
 This is a [plasTeX](https://github.com/plastex/plastex/) plugin allowing
 to write blueprints for Lean 4 projects.
+You can learn what those blueprints are about by reading
+Terence Tao’s excellent [blog post about it](https://terrytao.wordpress.com/2023/11/18/formalizing-the-proof-of-pfr-in-lean4-using-blueprint-a-short-tour/).
+
+This infrastructure was originally created in 2020 for the
+[Sphere Eversion Project](https://leanprover-community.github.io/sphere-eversion/).
+Since then, it has been used by many projects. The list below will give you many
+examples but is not intended to be exhaustive.
+It is in approximate chronological order.
+
+* [Sphere eversion project](https://leanprover-community.github.io/sphere-eversion/blueprint/index.html).
+* [Liquid tensor experiment](https://leanprover-community.github.io/liquid/)
+* [Fermat’s last theorem for regular primes](https://leanprover-community.github.io/flt-regular/blueprint/)
+* [Arithmetic Progressions - Almost Periodicity](https://yaeldillies.github.io/LeanAPAP/blueprint/)
+* [Polynomial Freiman-Ruzsa Conjecture](https://teorth.github.io/pfr/blueprint/)
+* [Lower bounds for hypothesis testing based on information theory](https://remydegenne.github.io/testing-lower-bounds/blueprint/)
+* [Prime number theorem and…](https://alexkontorovich.github.io/PrimeNumberTheoremAnd/web/)
+* [Fermat's Last Theorem for 3](https://pitmonticone.github.io/FLT3/blueprint)
+* [Fermat’s last theorem](https://imperialcollegelondon.github.io/FLT/blueprint/)
 
 ## Installation
 
 This package depends on `plastexdepgraph` which requires graphviz and its development libraries. 
 If you have a user-friendly OS, it is as simple as 
 `sudo apt install graphviz libgraphviz-dev`. 
 See https://pygraphviz.github.io/documentation/stable/install.html otherwise.
@@ -31,15 +71,15 @@
 particular the creation of a blueprint for your Lean project. This tool is not
 mandatory in any way. Its goal is to make it easy to create a blueprint without
 worrying about choosing a file layout or a continuous integration and deployment
 setup. As every one–size-fits-all tool, it is fairly opinionated. It assumes in
 particular that your project repository is hosted on Github and you want to host
 its blueprint on github.io.
 
-If you don’t want to use the `leanblueprint` command line tool, you can use use
+If you don’t want to use the `leanblueprint` command line tool, you can use
 this plugin as any other plasTeX plugin, using
 `plastex --plugins leanblueprint my_file.tex` (not recommended).
 
 In order to use the `leanblueprint` tool, you need to already have a Lean
 project created using lake. In addition, your blueprint will be easier to
 configure if you have at least one commit in the git repository of your project
 and you have already configured its GitHub git remote (GitHub displays
@@ -85,15 +125,15 @@
   in the blueprint exist in the project (or in a dependency of the project such
   as Mathlib). This requires a compiled Lean project, so make sure to run `lake build` beforehand.
 * `leanblueprint all` to run the previous three commands.
 * `leanblueprint serve` to start a local webserver showing your local blueprint
   (this sounds silly but web browsers paranoia makes it impossible to simply
   open the generated html pages without serving them). The url you should use
   in your browser will be displayed and will probably be `http://0.0.0.0:8000/`,
-  unless the port 8000 is already is use.
+  unless the port 8000 is already in use.
 
 Note: plasTeX does not call BibTeX. If you have a bibliography, you should use
 `leanblueprint pdf` before `leanblueprint web` to get it to work in the web
 version (and redo it when you add a reference).
 
 ## Editing the blueprint
 
@@ -145,14 +185,26 @@
   This obviously follows from what we did so far.
 \end
 ```
 
 Note that the proof above is abbreviated in this documentation. 
 Be nice to you and your collaborators and include more details in your blueprint proofs!
 
+By default, the dependency graph will collect the environments definition,
+lemma, proposition, theorem and corollary. You can change this list using the
+`thms` option which expects a list of environment names separated by `+` signs. 
+For instance you can write
+```latex
+\usepackage[thms=dfn+lem+prop+thm+cor]{blueprint}
+```
+if you like short environment names. See the 
+[plastexdepgraph documentation](https://github.com/PatrickMassot/plastexdepgraph/blob/master/README.md) 
+for other dependency graph options having nothing to do with Lean.
+
+
 The above macros are by far the most important, but there are a couple more.
 
 * `\notready` which claims the surrounding environment is not ready to be formalized,
   typically because it requires more blueprint work.
 * `\discussion` gives a GitHub issue number where the surrounding definition or
   statement is discussed.
 * `\proves` inside a proof environment gives the LaTeX label of the LaTeX
```

### Comparing `leanblueprint-0.0.8/leanblueprint/Packages/blueprint.py` & `leanblueprint-0.0.9/leanblueprint/Packages/blueprint.py`

 * *Files identical despite different names*

### Comparing `leanblueprint-0.0.8/leanblueprint/client.py` & `leanblueprint-0.0.9/leanblueprint/client.py`

 * *Files identical despite different names*

### Comparing `leanblueprint-0.0.8/leanblueprint/templates/blueprint.yml` & `leanblueprint-0.0.9/leanblueprint/templates/blueprint.yml`

 * *Files identical despite different names*

### Comparing `leanblueprint-0.0.8/leanblueprint/templates/macros/print.tex` & `leanblueprint-0.0.9/leanblueprint/templates/macros/print.tex`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 
 % Dummy macros that make sense only for web version.
 \newcommand{\lean}[1]{}
 \newcommand{\discussion}[1]{}
 \newcommand{\leanok}{}
 \newcommand{\mathlibok}{}
+\newcommand{\notready}{}
 % Make sure that arguments of \uses and \proves are real labels, by using invisible refs:
 % latex prints a warning if the label is not defined, but nothing is shown in the pdf file.
 % It uses LaTeX3 programming, this is why we use the expl3 package.
 \ExplSyntaxOn
 \NewDocumentCommand{\uses}{m}
  {\clist_map_inline:nn{#1}{\vphantom{\ref{##1}}}%
   \ignorespaces}
```

### Comparing `leanblueprint-0.0.8/leanblueprint/templates/print.tex` & `leanblueprint-0.0.9/leanblueprint/templates/print.tex`

 * *Files identical despite different names*

### Comparing `leanblueprint-0.0.8/leanblueprint/templates/web.tex` & `leanblueprint-0.0.9/leanblueprint/templates/web.tex`

 * *Files identical despite different names*

### Comparing `leanblueprint-0.0.8/leanblueprint.egg-info/PKG-INFO` & `leanblueprint-0.0.9/leanblueprint.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leanblueprint
-Version: 0.0.8
+Version: 0.0.9
 Summary: Lean prover blueprint plasTeX plugin.
 Home-page: https://github.com/PatrickMassot/leanblueprint
 Author: Patrick Massot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -20,14 +20,32 @@
 Requires-Dist: Jinja2>=3.1.0
 Requires-Dist: GitPython>=3.1.28
 
 # Lean blueprints
 
 This is a [plasTeX](https://github.com/plastex/plastex/) plugin allowing
 to write blueprints for Lean 4 projects.
+You can learn what those blueprints are about by reading
+Terence Tao’s excellent [blog post about it](https://terrytao.wordpress.com/2023/11/18/formalizing-the-proof-of-pfr-in-lean4-using-blueprint-a-short-tour/).
+
+This infrastructure was originally created in 2020 for the
+[Sphere Eversion Project](https://leanprover-community.github.io/sphere-eversion/).
+Since then, it has been used by many projects. The list below will give you many
+examples but is not intended to be exhaustive.
+It is in approximate chronological order.
+
+* [Sphere eversion project](https://leanprover-community.github.io/sphere-eversion/blueprint/index.html).
+* [Liquid tensor experiment](https://leanprover-community.github.io/liquid/)
+* [Fermat’s last theorem for regular primes](https://leanprover-community.github.io/flt-regular/blueprint/)
+* [Arithmetic Progressions - Almost Periodicity](https://yaeldillies.github.io/LeanAPAP/blueprint/)
+* [Polynomial Freiman-Ruzsa Conjecture](https://teorth.github.io/pfr/blueprint/)
+* [Lower bounds for hypothesis testing based on information theory](https://remydegenne.github.io/testing-lower-bounds/blueprint/)
+* [Prime number theorem and…](https://alexkontorovich.github.io/PrimeNumberTheoremAnd/web/)
+* [Fermat's Last Theorem for 3](https://pitmonticone.github.io/FLT3/blueprint)
+* [Fermat’s last theorem](https://imperialcollegelondon.github.io/FLT/blueprint/)
 
 ## Installation
 
 This package depends on `plastexdepgraph` which requires graphviz and its development libraries. 
 If you have a user-friendly OS, it is as simple as 
 `sudo apt install graphviz libgraphviz-dev`. 
 See https://pygraphviz.github.io/documentation/stable/install.html otherwise.
@@ -53,15 +71,15 @@
 particular the creation of a blueprint for your Lean project. This tool is not
 mandatory in any way. Its goal is to make it easy to create a blueprint without
 worrying about choosing a file layout or a continuous integration and deployment
 setup. As every one–size-fits-all tool, it is fairly opinionated. It assumes in
 particular that your project repository is hosted on Github and you want to host
 its blueprint on github.io.
 
-If you don’t want to use the `leanblueprint` command line tool, you can use use
+If you don’t want to use the `leanblueprint` command line tool, you can use
 this plugin as any other plasTeX plugin, using
 `plastex --plugins leanblueprint my_file.tex` (not recommended).
 
 In order to use the `leanblueprint` tool, you need to already have a Lean
 project created using lake. In addition, your blueprint will be easier to
 configure if you have at least one commit in the git repository of your project
 and you have already configured its GitHub git remote (GitHub displays
@@ -107,15 +125,15 @@
   in the blueprint exist in the project (or in a dependency of the project such
   as Mathlib). This requires a compiled Lean project, so make sure to run `lake build` beforehand.
 * `leanblueprint all` to run the previous three commands.
 * `leanblueprint serve` to start a local webserver showing your local blueprint
   (this sounds silly but web browsers paranoia makes it impossible to simply
   open the generated html pages without serving them). The url you should use
   in your browser will be displayed and will probably be `http://0.0.0.0:8000/`,
-  unless the port 8000 is already is use.
+  unless the port 8000 is already in use.
 
 Note: plasTeX does not call BibTeX. If you have a bibliography, you should use
 `leanblueprint pdf` before `leanblueprint web` to get it to work in the web
 version (and redo it when you add a reference).
 
 ## Editing the blueprint
 
@@ -167,14 +185,26 @@
   This obviously follows from what we did so far.
 \end
 ```
 
 Note that the proof above is abbreviated in this documentation. 
 Be nice to you and your collaborators and include more details in your blueprint proofs!
 
+By default, the dependency graph will collect the environments definition,
+lemma, proposition, theorem and corollary. You can change this list using the
+`thms` option which expects a list of environment names separated by `+` signs. 
+For instance you can write
+```latex
+\usepackage[thms=dfn+lem+prop+thm+cor]{blueprint}
+```
+if you like short environment names. See the 
+[plastexdepgraph documentation](https://github.com/PatrickMassot/plastexdepgraph/blob/master/README.md) 
+for other dependency graph options having nothing to do with Lean.
+
+
 The above macros are by far the most important, but there are a couple more.
 
 * `\notready` which claims the surrounding environment is not ready to be formalized,
   typically because it requires more blueprint work.
 * `\discussion` gives a GitHub issue number where the surrounding definition or
   statement is discussed.
 * `\proves` inside a proof environment gives the LaTeX label of the LaTeX
```

### Comparing `leanblueprint-0.0.8/leanblueprint.egg-info/SOURCES.txt` & `leanblueprint-0.0.9/leanblueprint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leanblueprint-0.0.8/setup.cfg` & `leanblueprint-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = leanblueprint
 description = Lean prover blueprint plasTeX plugin.
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.0.8
+version = 0.0.9
 author = Patrick Massot
 url = https://github.com/PatrickMassot/leanblueprint
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

