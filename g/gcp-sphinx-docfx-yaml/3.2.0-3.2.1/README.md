# Comparing `tmp/gcp-sphinx-docfx-yaml-3.2.0.tar.gz` & `tmp/gcp-sphinx-docfx-yaml-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp-sphinx-docfx-yaml-3.2.0.tar", last modified: Thu May  2 07:11:59 2024, max compression
+gzip compressed data, was "gcp-sphinx-docfx-yaml-3.2.1.tar", last modified: Tue May  7 18:38:23 2024, max compression
```

## Comparing `gcp-sphinx-docfx-yaml-3.2.0.tar` & `gcp-sphinx-docfx-yaml-3.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-02 07:11:59.125235 gcp-sphinx-docfx-yaml-3.2.0/
--rw-rw-r--   0 root         (0)     1003    11358 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/LICENSE
--rw-r--r--   0 root         (0)     1003      796 2024-05-02 07:11:59.125235 gcp-sphinx-docfx-yaml-3.2.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2625 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-02 07:11:59.121235 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/
--rw-rw-r--   0 root         (0)     1003      576 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/__init__.py
--rw-rw-r--   0 root         (0)     1003     1262 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/directives.py
--rw-rw-r--   0 root         (0)     1003    85361 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/extension.py
--rw-rw-r--   0 root         (0)     1003     5154 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/extract_nodes.py
--rw-rw-r--   0 root         (0)     1003    16722 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/markdown_utils.py
--rw-rw-r--   0 root         (0)     1003    20734 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/monkeypatch.py
--rw-rw-r--   0 root         (0)     1003      988 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/nodes.py
--rw-rw-r--   0 root         (0)     1003      727 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/settings.py
--rw-rw-r--   0 root         (0)     1003     1731 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/utils.py
--rw-rw-r--   0 root         (0)     1003    33366 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/writer.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-02 07:11:59.125235 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/
--rw-r--r--   0 root         (0)     1003      796 2024-05-02 07:11:59.000000 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      640 2024-05-02 07:11:59.000000 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-05-02 07:11:59.000000 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-05-02 07:11:59.000000 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      289 2024-05-02 07:11:59.000000 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       11 2024-05-02 07:11:59.000000 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-05-02 07:11:59.125235 gcp-sphinx-docfx-yaml-3.2.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     1756 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-02 07:11:59.125235 gcp-sphinx-docfx-yaml-3.2.0/tests/
--rw-rw-r--   0 root         (0)     1003    15861 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/tests/test_helpers.py
--rw-rw-r--   0 root         (0)     1003     1588 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/tests/test_inspect.py
--rw-rw-r--   0 root         (0)     1003    11616 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/tests/test_markdown.py
--rw-rw-r--   0 root         (0)     1003    32326 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/tests/test_unit.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 18:38:23.597616 gcp-sphinx-docfx-yaml-3.2.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/LICENSE
+-rw-r--r--   0 root         (0)     1003      796 2024-05-07 18:38:23.597616 gcp-sphinx-docfx-yaml-3.2.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2625 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 18:38:23.593610 gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/
+-rw-rw-r--   0 root         (0)     1003      576 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1262 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/directives.py
+-rw-rw-r--   0 root         (0)     1003    87486 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/extension.py
+-rw-rw-r--   0 root         (0)     1003     5154 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/extract_nodes.py
+-rw-rw-r--   0 root         (0)     1003    16891 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/markdown_utils.py
+-rw-rw-r--   0 root         (0)     1003    20734 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/monkeypatch.py
+-rw-rw-r--   0 root         (0)     1003      988 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/nodes.py
+-rw-rw-r--   0 root         (0)     1003      727 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/settings.py
+-rw-rw-r--   0 root         (0)     1003     1731 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/utils.py
+-rw-rw-r--   0 root         (0)     1003    33366 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/writer.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 18:38:23.597616 gcp-sphinx-docfx-yaml-3.2.1/gcp_sphinx_docfx_yaml.egg-info/
+-rw-r--r--   0 root         (0)     1003      796 2024-05-07 18:38:23.000000 gcp-sphinx-docfx-yaml-3.2.1/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      640 2024-05-07 18:38:23.000000 gcp-sphinx-docfx-yaml-3.2.1/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-07 18:38:23.000000 gcp-sphinx-docfx-yaml-3.2.1/gcp_sphinx_docfx_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-07 18:38:23.000000 gcp-sphinx-docfx-yaml-3.2.1/gcp_sphinx_docfx_yaml.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      289 2024-05-07 18:38:23.000000 gcp-sphinx-docfx-yaml-3.2.1/gcp_sphinx_docfx_yaml.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       11 2024-05-07 18:38:23.000000 gcp-sphinx-docfx-yaml-3.2.1/gcp_sphinx_docfx_yaml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-07 18:38:23.597616 gcp-sphinx-docfx-yaml-3.2.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     1756 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 18:38:23.597616 gcp-sphinx-docfx-yaml-3.2.1/tests/
+-rw-rw-r--   0 root         (0)     1003    15861 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/tests/test_helpers.py
+-rw-rw-r--   0 root         (0)     1003     1588 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/tests/test_inspect.py
+-rw-rw-r--   0 root         (0)     1003    11616 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/tests/test_markdown.py
+-rw-rw-r--   0 root         (0)     1003    40229 2024-05-07 18:36:21.000000 gcp-sphinx-docfx-yaml-3.2.1/tests/test_unit.py
```

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/LICENSE` & `gcp-sphinx-docfx-yaml-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/PKG-INFO` & `gcp-sphinx-docfx-yaml-3.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-sphinx-docfx-yaml
-Version: 3.2.0
+Version: 3.2.1
 Summary: Sphinx Python Domain to DocFX YAML Generator
 Home-page: https://github.com/googleapis/sphinx-docfx-yaml
 Author: Google LLC
 Author-email: dandhlee@google.com
 License: Apache 2.0
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/README.rst` & `gcp-sphinx-docfx-yaml-3.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/__init__.py` & `gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/directives.py` & `gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/directives.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/extension.py` & `gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
     if not (repo_metadata := _grab_repo_metadata()):
         print("Failed to retrieve repository metadata.")
         app.env.library_shortname = ""
     else:
         print("Successfully retrieved repository metadata.")
         app.env.library_shortname = repo_metadata["name"]
     print("Running sphinx-build with Markdown first...")
-    markdown_utils.run_sphinx_markdown()
+    markdown_utils.run_sphinx_markdown(app)
     print("Completed running sphinx-build with Markdown files.")
 
     """
     Set up environment data
     """
     if not app.config.docfx_yaml_output:
         raise ExtensionError('You must configure an docfx_yaml_output setting')
@@ -392,19 +392,91 @@
         String lines of left-indented code.
     """
     parts = lines.split("\n")
     parts = [part[tab_space:] for part in parts]
     return "\n".join(parts)
 
 
-def _parse_docstring_summary(summary):
+def _parse_enum_content(parts: Sequence[str]) -> Sequence[Mapping[str, str]]:
+    """Parses the given content for enums.
+
+    Args:
+        parts: The content to parse, given in the form of a sequence of str,
+            which have been split by newlines and are left-indented.
+
+    Returns:
+        Sequence of mapping of enum entries for name and description.
+
+    Raises:
+        ValueError: If the `Values` enum docstring is malformed.
+    """
+    enum_content: MutableSequence[Mapping[str, str]] = []
+    enum_name = ""
+    enum_description = []
+    for part in parts:
+        if (
+            (current_tab_space := len(part) - len(part.lstrip(" "))) > 0
+        ):
+            enum_description.append(indent_code_left(part, current_tab_space))
+            continue
+
+        # Add the new enum and start collecting new entry.
+        if enum_name and enum_description:
+            enum_content.append({
+                "id": enum_name,
+                "description": " ".join(enum_description),
+        })
+
+        enum_description = []
+        # Only collect the name, not the value.
+        enum_name = part.split(" ")[0]
+
+        if not enum_name and not enum_description:
+            raise ValueError(
+                "The enum docstring is not formatted well. Check the"
+                " docstring:\n\n{}".format("\n".join(parts))
+            )
+
+    # Add the last entry.
+    if not enum_name or not enum_description:
+        raise ValueError(
+            "The enum docstring is not formatted well. Check the"
+            " docstring:\n\n{}".format("\n".join(parts))
+        )
+
+    enum_content.append({
+        "id": enum_name,
+        "description": " ".join(enum_description),
+    })
+
+    return enum_content
+
+
+def _parse_docstring_summary(
+    summary: str,
+) -> tuple[str, Mapping[str, str], Mapping[str, str]]:
+    """
+    Parses the docstring tokens found in the summary.
+
+    Looks for tokens such as codeblocks, attributes, notices and enums.
+
+    Args:
+        summary: The content to parse docstring for.
+
+    Returns:
+        A tuple of the following:
+        * str: The content with parsed docstrings.
+        * Mapping[str, str]: Attribute entries if found.
+        * Mapping[str, str]: Enum entries if found.
+    """
     summary_parts = []
     attributes = []
     attribute_type_token = ":type:"
     enum_type_token = "Values:"
+    enums = []
     keyword = name = description = var_type = ""
 
     notice_open_tag = '<aside class="{notice_tag}">\n<b>{notice_name}:</b>'
     notice_close_tag = '</aside>'
 
     # We need to separate in chunks, which is defined by 3 newline breaks.
     # Otherwise when parsing for code and blocks of stuff, we will not be able
@@ -496,22 +568,16 @@
                 parts = [split_part for split_part in part.split("\n") if split_part][1:]
                 if not parts:
                     continue
                 tab_space = len(parts[0]) - len(parts[0].lstrip(" "))
                 if tab_space == 0:
                     raise ValueError("Content in the block should be indented."\
                                      f"Please check the docstring: \n{summary}")
-                parts = "\n".join(
-                    [indent_code_left(part, tab_space) for part in parts]
-                )
-                summary_parts.append(
-                    "Enum values:\n\n```\n"
-                    f"{parts}"
-                    "\n```\n"
-                )
+                parts = [indent_code_left(part, tab_space) for part in parts]
+                enums = _parse_enum_content(parts)
                 continue
 
             try:
                 keyword = extract_keyword(part.lstrip('\n'))
             except ValueError:
                 raise ValueError(f"Please check the docstring: \n{summary}")
             # Works for both code-block and code
@@ -569,15 +635,15 @@
         if notice_body:
             parts = [indent_code_left(part, tab_space) for part in notice_body]
             summary_parts.append("\n\n".join(parts))
         if summary_parts[-1] != notice_close_tag:
             summary_parts.append(notice_close_tag)
 
     # Requires 2 newline chars to properly show on cloud site.
-    return "\n".join(summary_parts), attributes
+    return "\n".join(summary_parts), attributes, enums
 
 
 # Given documentation docstring, parse them into summary_info.
 def _extract_docstring_info(summary_info, summary, name):
     top_summary = ""
     # Return clean summary if returning early.
     parsed_text = summary
@@ -1010,15 +1076,17 @@
         summary = app.docfx_transform_string('\n'.join(_refact_example_in_module_summary(lines)))
 
         # Extract summary info into respective sections.
         if summary:
             summary = reformat_summary(summary)
             top_summary = _extract_docstring_info(summary_info, summary, name)
             try:
-                datam['summary'], datam['attributes'] = _parse_docstring_summary(top_summary)
+                datam['summary'], datam['attributes'], datam['enum'] = (
+                    _parse_docstring_summary(top_summary)
+                )
             except ValueError:
                 debug_line = []
                 if path:
                     debug_line.append(f"In file {path}\n")
                 debug_line.append(f"For module {module}, type {_type}:\n")
                 debug_line.append(f"Failed to parse docstring on {name}.")
                 raise ValueError("".join(debug_line))
```

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/extract_nodes.py` & `gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/extract_nodes.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/markdown_utils.py` & `gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/markdown_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -481,26 +481,28 @@
             os.remove(f"{outdir}/{page}")
         except FileNotFoundError:
             # This shouldn't happen, but in case we fail, ignore the failure
             # and continue deleting other files.
             print(f"Could not delete {page}.")
 
 
-def run_sphinx_markdown() -> None:
+def run_sphinx_markdown(app: sphinx.application) -> None:
     """Runs sphinx-build with Markdown builder in the plugin."""
     cwd = os.getcwd()
+    relative_srcdir = app.srcdir.removeprefix(f"{cwd}/")
+    relative_outdir = app.outdir.removeprefix(f"{cwd}/").removesuffix("/html")
     # Skip running sphinx-build for Markdown for some unit tests.
     # Not required other than to output DocFX YAML.
     if "docs" in cwd:
         return
 
     return shell.run(
         [
             "sphinx-build",
             "-M",
             "markdown",
-            "docs/",
-            "docs/_build",
+            relative_srcdir,
+            relative_outdir,
         ],
         hide_output=False
     )
```

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/monkeypatch.py` & `gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/nodes.py` & `gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/settings.py` & `gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/settings.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/utils.py` & `gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/utils.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/writer.py` & `gcp-sphinx-docfx-yaml-3.2.1/docfx_yaml/writer.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO` & `gcp-sphinx-docfx-yaml-3.2.1/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-sphinx-docfx-yaml
-Version: 3.2.0
+Version: 3.2.1
 Summary: Sphinx Python Domain to DocFX YAML Generator
 Home-page: https://github.com/googleapis/sphinx-docfx-yaml
 Author: Google LLC
 Author-email: dandhlee@google.com
 License: Apache 2.0
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt` & `gcp-sphinx-docfx-yaml-3.2.1/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/setup.py` & `gcp-sphinx-docfx-yaml-3.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 import codecs
 import setuptools
 
 name = 'gcp-sphinx-docfx-yaml'
 description = 'Sphinx Python Domain to DocFX YAML Generator'
-version = '3.2.0'
+version = '3.2.1'
 dependencies = [
     'black',
     'gcp-docuploader',
     'PyYAML',
     'recommonmark',
     'sphinxcontrib-applehelp==1.0.4',
     'sphinxcontrib-devhelp==1.0.2',
```

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/tests/test_helpers.py` & `gcp-sphinx-docfx-yaml-3.2.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/tests/test_inspect.py` & `gcp-sphinx-docfx-yaml-3.2.1/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.2.0/tests/test_markdown.py` & `gcp-sphinx-docfx-yaml-3.2.1/tests/test_markdown.py`

 * *Files identical despite different names*

