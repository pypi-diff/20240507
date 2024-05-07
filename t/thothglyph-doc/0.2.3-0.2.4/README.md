# Comparing `tmp/thothglyph_doc-0.2.3.tar.gz` & `tmp/thothglyph_doc-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thothglyph_doc-0.2.3.tar", max compression
+gzip compressed data, was "thothglyph_doc-0.2.4.tar", max compression
```

## Comparing `thothglyph_doc-0.2.3.tar` & `thothglyph_doc-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1065 2023-09-03 08:30:24.832210 thothglyph_doc-0.2.3/LICENSE
--rw-r--r--   0        0        0      899 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/README.md
--rw-r--r--   0        0        0      697 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/__init__.py
--rw-r--r--   0        0        0        0 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/app/__init__.py
--rw-r--r--   0        0        0     2500 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/app/converter.py
--rw-r--r--   0        0        0     3115 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/data/tglyph.svg
--rw-r--r--   0        0        0     7412 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/data/tglyph_256.png
--rw-r--r--   0        0        0     1651 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/data/tglyph_64.png
--rw-r--r--   0        0        0       43 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/error.py
--rw-r--r--   0        0        0     3079 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/ext/blockdiag.py
--rw-r--r--   0        0        0     1179 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/ext/graphviz.py
--rw-r--r--   0        0        0     2243 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/ext/math.py
--rw-r--r--   0        0        0     2185 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/ext/mermaid.py
--rw-r--r--   0        0        0     2342 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/ext/plantuml.py
--rw-r--r--   0        0        0     1292 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/ext/wavedrom.py
--rw-r--r--   0        0        0      580 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/node/logging.py
--rw-r--r--   0        0        0    17283 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/node/nd.py
--rw-r--r--   0        0        0      485 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.3/thothglyph/reader/__init__.py
--rw-r--r--   0        0        0    26011 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/reader/md.py
--rw-r--r--   0        0        0     7344 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/reader/reader.py
--rw-r--r--   0        0        0    52416 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/reader/tglyph.py
--rw-r--r--   0        0        0     1557 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/common/check_dis.pdf
--rw-r--r--   0        0        0      627 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/common/check_dis.svg
--rw-r--r--   0        0        0     1597 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/common/check_en.pdf
--rw-r--r--   0        0        0      748 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/common/check_en.svg
--rw-r--r--   0        0        0     1638 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/common/check_im.pdf
--rw-r--r--   0        0        0      735 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/common/check_im.svg
--rw-r--r--   0        0        0    52673 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/docx/default/style.docx
--rw-r--r--   0        0        0     5439 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.3/thothglyph/template/html/default/index.html
--rw-r--r--   0        0        0     4322 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.3/thothglyph/template/html/preview/index.html
--rw-r--r--   0        0        0     6793 2024-05-04 04:58:45.492809 thothglyph_doc-0.2.3/thothglyph/template/latex/default/document-ja.tex
--rw-r--r--   0        0        0     1428 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/util/svg.py
--rw-r--r--   0        0        0      363 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/writer/__init__.py
--rw-r--r--   0        0        0    18936 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/writer/docx.py
--rw-r--r--   0        0        0    17349 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/writer/html.py
--rw-r--r--   0        0        0    18962 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/writer/latex.py
--rw-r--r--   0        0        0     4528 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/writer/pdf.py
--rw-r--r--   0        0        0     5474 2024-05-03 06:04:24.989564 thothglyph_doc-0.2.3/thothglyph/writer/writer.py
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 thothglyph_doc-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-09-03 08:30:24.832210 thothglyph_doc-0.2.4/LICENSE
+-rw-r--r--   0        0        0      899 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.4/README.md
+-rw-r--r--   0        0        0      697 2024-05-07 19:33:59.526964 thothglyph_doc-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-07 19:33:59.526964 thothglyph_doc-0.2.4/thothglyph/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/app/__init__.py
+-rw-r--r--   0        0        0     2500 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/app/converter.py
+-rw-r--r--   0        0        0     3115 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/data/tglyph.svg
+-rw-r--r--   0        0        0     7412 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/data/tglyph_256.png
+-rw-r--r--   0        0        0     1651 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/data/tglyph_64.png
+-rw-r--r--   0        0        0       43 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/error.py
+-rw-r--r--   0        0        0     3432 2024-05-07 19:33:59.526964 thothglyph_doc-0.2.4/thothglyph/ext/blockdiag.py
+-rw-r--r--   0        0        0     1557 2024-05-07 19:33:59.526964 thothglyph_doc-0.2.4/thothglyph/ext/graphviz.py
+-rw-r--r--   0        0        0     2909 2024-05-07 19:33:59.526964 thothglyph_doc-0.2.4/thothglyph/ext/math.py
+-rw-r--r--   0        0        0     3113 2024-05-07 19:33:59.526964 thothglyph_doc-0.2.4/thothglyph/ext/mermaid.py
+-rw-r--r--   0        0        0     3239 2024-05-07 19:33:59.530964 thothglyph_doc-0.2.4/thothglyph/ext/plantuml.py
+-rw-r--r--   0        0        0     1640 2024-05-07 19:33:59.530964 thothglyph_doc-0.2.4/thothglyph/ext/wavedrom.py
+-rw-r--r--   0        0        0      580 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/node/logging.py
+-rw-r--r--   0        0        0    17283 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.4/thothglyph/node/nd.py
+-rw-r--r--   0        0        0      485 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.4/thothglyph/reader/__init__.py
+-rw-r--r--   0        0        0    26011 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/reader/md.py
+-rw-r--r--   0        0        0     7344 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/reader/reader.py
+-rw-r--r--   0        0        0    52453 2024-05-07 19:33:59.530964 thothglyph_doc-0.2.4/thothglyph/reader/tglyph.py
+-rw-r--r--   0        0        0     1557 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/template/common/check_dis.pdf
+-rw-r--r--   0        0        0      627 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/template/common/check_dis.svg
+-rw-r--r--   0        0        0     1597 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/template/common/check_en.pdf
+-rw-r--r--   0        0        0      748 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/template/common/check_en.svg
+-rw-r--r--   0        0        0     1638 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/template/common/check_im.pdf
+-rw-r--r--   0        0        0      735 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/template/common/check_im.svg
+-rw-r--r--   0        0        0    52673 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/template/docx/default/style.docx
+-rw-r--r--   0        0        0     5439 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.4/thothglyph/template/html/default/index.html
+-rw-r--r--   0        0        0     4322 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.4/thothglyph/template/html/preview/index.html
+-rw-r--r--   0        0        0     6793 2024-05-04 04:58:45.492809 thothglyph_doc-0.2.4/thothglyph/template/latex/default/document-ja.tex
+-rw-r--r--   0        0        0     2069 2024-05-07 19:33:59.530964 thothglyph_doc-0.2.4/thothglyph/util/svg.py
+-rw-r--r--   0        0        0      363 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.4/thothglyph/writer/__init__.py
+-rw-r--r--   0        0        0    19089 2024-05-07 19:33:59.530964 thothglyph_doc-0.2.4/thothglyph/writer/docx.py
+-rw-r--r--   0        0        0    17349 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.4/thothglyph/writer/html.py
+-rw-r--r--   0        0        0    18955 2024-05-07 19:33:59.530964 thothglyph_doc-0.2.4/thothglyph/writer/latex.py
+-rw-r--r--   0        0        0     4545 2024-05-07 19:33:59.530964 thothglyph_doc-0.2.4/thothglyph/writer/pdf.py
+-rw-r--r--   0        0        0     5474 2024-05-07 16:56:46.432074 thothglyph_doc-0.2.4/thothglyph/writer/writer.py
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 thothglyph_doc-0.2.4/PKG-INFO
```

### Comparing `thothglyph_doc-0.2.3/LICENSE` & `thothglyph_doc-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/README.md` & `thothglyph_doc-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/pyproject.toml` & `thothglyph_doc-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thothglyph-doc"
-version = "0.2.3"
+version = "0.2.4"
 description = "A Documentation converter and language for Engineers"
 authors = ["nakandev <nakandev.s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "thothglyph" },
 ]
```

### Comparing `thothglyph_doc-0.2.3/thothglyph/app/converter.py` & `thothglyph_doc-0.2.4/thothglyph/app/converter.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/data/tglyph.svg` & `thothglyph_doc-0.2.4/thothglyph/data/tglyph.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/data/tglyph_256.png` & `thothglyph_doc-0.2.4/thothglyph/data/tglyph_256.png`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/data/tglyph_64.png` & `thothglyph_doc-0.2.4/thothglyph/data/tglyph_64.png`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/ext/blockdiag.py` & `thothglyph_doc-0.2.4/thothglyph/ext/blockdiag.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import nwdiag.drawer
 import rackdiag.parser
 import rackdiag.builder
 import rackdiag.drawer
 import packetdiag.parser
 import packetdiag.builder
 import packetdiag.drawer
-from thothglyph.util.svg import svg2pdf
+from thothglyph.util.svg import svg2pdf, svg2png
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 
 def _get_svgstr(text):
     if text.startswith('blockdiag'):
@@ -87,7 +87,18 @@
     fname = os.path.join(self.tmpdirname, node.treeid() + '.pdf')
     svg2pdf(bytestring=svgstr, write_to=fname)
     w = '{}bp'.format(int(w * self.bp_scale))
     self.data += '\\tgincludegraphics[{}]{{{}}}\n\n'.format(w, fname)
 
 def customblock_write_pdf(self, node):
     customblock_write_latex(self, node)
+
+def customblock_write_docx(self, node):
+    text = node.text
+    svgstr, w, h = _get_svgstr(text)
+    w, h = int(w), int(h)
+    fname = os.path.join(self.tmpdirname, node.treeid() + '.png')
+    svg2png(bytestring=svgstr, write_to=fname, scale=0.625)
+    p = self._add_paragraph()
+    if p:
+        r = p.add_run()
+        r.add_picture(fname)
```

### Comparing `thothglyph_doc-0.2.3/thothglyph/ext/graphviz.py` & `thothglyph_doc-0.2.4/thothglyph/ext/graphviz.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import re
 import graphviz
-from thothglyph.util.svg import svg2pdf
+from thothglyph.util.svg import svg2pdf, svg2png
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 
 def customblock_write_html(self, node):
     text = node.text
@@ -32,7 +32,18 @@
     w, _ = int(m.group(1)), int(m.group(2))
     wstr = '{}bp'.format(int(w * self.bp_scale))
     self.data += '\\tgincludegraphics[{}]{{{}}}\n\n'.format(wstr, fname)
 
 
 def customblock_write_pdf(self, node):
     customblock_write_latex(self, node)
+
+def customblock_write_docx(self, node):
+    text = node.text
+    graph = graphviz.Source(text)  # type: ignore
+    svgstr = graph.pipe(format='svg')
+    fname = os.path.join(self.tmpdirname, node.treeid() + '.pdf')
+    svg2png(bytestring=svgstr, write_to=fname, scale=0.625)
+    p = self._add_paragraph()
+    if p:
+        r = p.add_run()
+        r.add_picture(fname)
```

### Comparing `thothglyph_doc-0.2.3/thothglyph/ext/math.py` & `thothglyph_doc-0.2.4/thothglyph/ext/math.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import re
 import subprocess
 
+from thothglyph.util.svg import svg2png
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 
 latextemplate = r'''
 \documentclass[12pt]{article}
@@ -76,7 +77,25 @@
 
 
 def customblock_write_pdf(self, node):
     customblock_write_latex(self, node)
 
 def role_write_pdf(self, node):
     role_write_latex(self, node)
+
+def customblock_write_docx(self, node):
+    text = node.value
+    svgstr = _get_svgstr(self.tmpdirname, text, 'math')
+    fname = os.path.join(self.tmpdirname, node.treeid() + '.png')
+    svg2png(bytestring=svgstr, write_to=fname, scale=0.625)
+    p = self._add_paragraph()
+    if p:
+        r = p.add_run()
+        r.add_picture(fname)
+
+def role_write_docx(self, node):
+    text = node.value
+    svgstr = _get_svgstr(self.tmpdirname, text, 'math')
+    fname = os.path.join(self.tmpdirname, node.treeid() + '.png')
+    svg2png(bytestring=svgstr, write_to=fname, scale=0.625)
+    r = self.p.add_run()
+    r.add_picture(fname)
```

### Comparing `thothglyph_doc-0.2.3/thothglyph/ext/mermaid.py` & `thothglyph_doc-0.2.4/thothglyph/ext/mermaid.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import re
 import subprocess
 
 from thothglyph.error import ThothglyphError
+from thothglyph.util.svg import svg2png
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 
 def customblock_write_html(self, node):
     indata = node.text
@@ -38,16 +39,16 @@
 def customblock_write_latex(self, node):
     indata = node.text
     if isinstance(indata, str):
         indata = indata.encode()
     svgname = os.path.join(self.tmpdirname, node.treeid() + '.svg')
     pdfname = os.path.join(self.tmpdirname, node.treeid() + '.pdf')
     cmds = [
-        ['mmdc', '-o', '{}'.format(svgname)],
-        ['mmdc', '-o', '{}'.format(pdfname), '--pdfFit'],
+        ['mmdc', '-i', '-', '-o', '{}'.format(svgname)],
+        ['mmdc', '-i', '-', '-o', '{}'.format(pdfname), '--pdfFit'],
     ]
     for cmd in cmds:
         p = subprocess.Popen(
             cmd,
             stdin=subprocess.PIPE,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.DEVNULL
@@ -63,7 +64,33 @@
             w = int(float(m.group(1)))
     w = '{}bp'.format(int(w * self.bp_scale))
     self.data += '\\tgincludegraphics[{}]{{{}}}\n\n'.format(w, pdfname)
 
 
 def customblock_write_pdf(self, node):
     customblock_write_latex(self, node)
+
+def customblock_write_docx(self, node):
+    indata = node.text
+    if isinstance(indata, str):
+        indata = indata.encode()
+    svgname = os.path.join(self.tmpdirname, node.treeid() + '.svg')
+    pngname = os.path.join(self.tmpdirname, node.treeid() + '.png')
+    cmds = [
+        ['mmdc', '-i', '-', '-o', '{}'.format(svgname)],
+    ]
+    for cmd in cmds:
+        p = subprocess.Popen(
+            cmd,
+            stdin=subprocess.PIPE,
+            stdout=subprocess.DEVNULL,
+            stderr=subprocess.DEVNULL
+        )
+        p.communicate(input=indata)
+        if p.returncode != 0:
+            msg = '{} command exit with code {}.'.format(cmd[0], p.returncode)
+            raise ThothglyphError(msg)
+    svg2png(url=svgname, write_to=pngname, scale=0.625)
+    p = self._add_paragraph()
+    if p:
+        r = p.add_run()
+        r.add_picture(pngname)
```

### Comparing `thothglyph_doc-0.2.3/thothglyph/ext/plantuml.py` & `thothglyph_doc-0.2.4/thothglyph/ext/plantuml.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import re
 import subprocess
 
-from thothglyph.util.svg import svg2pdf
+from thothglyph.util.svg import svg2pdf, svg2png
 from thothglyph.error import ThothglyphError
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 
 def customblock_write_html(self, node):
@@ -65,7 +65,33 @@
             w = int(float(m.group(1)))
     w = '{}bp'.format(int(w * self.bp_scale))
     self.data += '\\tgincludegraphics[{}]{{{}}}\n\n'.format(w, pdfname)
 
 
 def customblock_write_pdf(self, node):
     customblock_write_latex(self, node)
+
+def customblock_write_docx(self, node):
+    indata = node.text
+    if isinstance(indata, str):
+        indata = indata.encode()
+    umlname = os.path.join(self.tmpdirname, node.treeid() + '.uml')
+    svgname = os.path.join(self.tmpdirname, node.treeid() + '.svg')
+    pngname = os.path.join(self.tmpdirname, node.treeid() + '.png')
+    with open(umlname, 'wb') as f:
+        f.write(indata)
+    cmd = ['plantuml', '-tsvg', umlname]
+    p = subprocess.Popen(
+        cmd,
+        stdin=subprocess.DEVNULL,
+        stdout=subprocess.DEVNULL,
+        stderr=subprocess.DEVNULL
+    )
+    p.communicate()
+    if p.returncode != 0:
+        msg = '{} command exit with code {}.'.format(cmd[0], p.returncode)
+        raise ThothglyphError(msg)
+    svg2png(url=svgname, write_to=pngname, scale=0.625)
+    p = self._add_paragraph()
+    if p:
+        r = p.add_run()
+        r.add_picture(pngname)
```

### Comparing `thothglyph_doc-0.2.3/thothglyph/ext/wavedrom.py` & `thothglyph_doc-0.2.4/thothglyph/ext/wavedrom.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import re
 import wavedrom
 
-from thothglyph.util.svg import svg2pdf
+from thothglyph.util.svg import svg2pdf, svg2png
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 
 def customblock_write_html(self, node):
     text = node.text
@@ -37,7 +37,17 @@
 #     customblock_write_latex(self, node)
 #     text = node.text
 #     svg = wavedrom.render(text)
 #     svg_io = io.StringIO(svg._repr_svg_())
 #     drawing = svg2rlg(svg_io)
 #     fname = os.path.join(self.tmpdirname, node.treeid() + '.pdf')
 #     renderPDF.drawToFile(drawing, fname)
+
+def customblock_write_docx(self, node):
+    text = node.text
+    svg = wavedrom.render(text)  # type: ignore
+    fname = os.path.join(self.tmpdirname, node.treeid() + '.pdf')
+    svg2png(bytestring=svg._repr_svg_(), write_to=fname, scale=0.625)
+    p = self._add_paragraph()
+    if p:
+        r = p.add_run()
+        r.add_picture(fname)
```

### Comparing `thothglyph_doc-0.2.3/thothglyph/node/logging.py` & `thothglyph_doc-0.2.4/thothglyph/node/logging.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/node/nd.py` & `thothglyph_doc-0.2.4/thothglyph/node/nd.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/reader/md.py` & `thothglyph_doc-0.2.4/thothglyph/reader/md.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/reader/reader.py` & `thothglyph_doc-0.2.4/thothglyph/reader/reader.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/reader/tglyph.py` & `thothglyph_doc-0.2.4/thothglyph/reader/tglyph.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
             raise ThothglyphError(msg)
         self._remove_preprocessed_tokens()
         tokens = list() + self.tokens
         tokens = self.p_document(tokens)
         return self.rootnode
 
     def _tokens(self, token: Lexer.Token, offset: int) -> Lexer.Token:
-        if token.no + offset >= len(self.tokens):
+        if self.tokens.index(token) + offset >= len(self.tokens):
             return None
         return self.tokens[self.tokens.index(token) + offset]
 
     def preprocess(self, data: str) -> str:
         self._init_config()
         try:
             self.tokens = self.lexer.lex_preproc(data)
@@ -320,15 +320,15 @@
             lineno = tokens[0].line + 1
             msg = 'Illegal ControlFlow token.'
             msg = f'{self.reader.path}:{lineno}: {msg}'
             raise ThothglyphError(msg)
         return tokens
 
     def p_if_else(self, tokens: List[Lexer.Token], conds: List[bool]) -> List[Lexer.Token]:
-        firstflowtoken = self._tokens(tokens[0], -1)
+        firstflowtoken = self._tokens(tokens[0], -1) or tokens[0]
         lastflowtoken = tokens[0]
         lasttoken = tokens[0]
         while tokens:
             if tokens[0].key == 'TEXT' and all(conds):
                 self.pplines.append(tokens[0].value)
                 lasttoken = tokens.pop(0)
             elif tokens[0].key == 'CONTROL_FLOW':
@@ -758,15 +758,15 @@
             prev = begintoken
             warned = False
             for token in subtokens:
                 if token.line != prev.line:
                     if prev.key != 'CODE_LINE':
                         text += '\n'
                     numspace = re.match(r' *', token.value).end()
-                    if numspace < indent and not warned:
+                    if 0 < numspace < indent and not warned:
                         msg = 'Code indentation is to the left of the block indentation.'
                         lineno = token.line + 1
                         msg = f'{self.reader.path}:{lineno}: {msg}'
                         logger.warn(msg)
                         warned = True
                     text += token.value[indent:]
                 else:
@@ -821,15 +821,15 @@
             text = str()
             warned = False
             for token in subtokens:
                 if token.line != prev.line:
                     if prev.key != 'CUSTOM_LINE':
                         text += '\n'
                     numspace = re.match(r' *', token.value).end()
-                    if numspace < indent and not warned:
+                    if 0 < numspace < indent and not warned:
                         msg = 'Code indentation is to the left of the block indentation.'
                         lineno = token.line + 1
                         msg = f'{self.reader.path}:{lineno}: {msg}'
                         warned = True
                     text += token.value[indent:]
                 else:
                     text += token.value
```

### Comparing `thothglyph_doc-0.2.3/thothglyph/template/common/check_dis.pdf` & `thothglyph_doc-0.2.4/thothglyph/template/common/check_dis.pdf`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/template/common/check_dis.svg` & `thothglyph_doc-0.2.4/thothglyph/template/common/check_dis.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/template/common/check_en.pdf` & `thothglyph_doc-0.2.4/thothglyph/template/common/check_en.pdf`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/template/common/check_en.svg` & `thothglyph_doc-0.2.4/thothglyph/template/common/check_en.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/template/common/check_im.pdf` & `thothglyph_doc-0.2.4/thothglyph/template/common/check_im.pdf`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/template/common/check_im.svg` & `thothglyph_doc-0.2.4/thothglyph/template/common/check_im.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/template/docx/default/style.docx` & `thothglyph_doc-0.2.4/thothglyph/template/docx/default/style.docx`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/template/html/default/index.html` & `thothglyph_doc-0.2.4/thothglyph/template/html/default/index.html`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/template/html/preview/index.html` & `thothglyph_doc-0.2.4/thothglyph/template/html/preview/index.html`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/template/latex/default/document-ja.tex` & `thothglyph_doc-0.2.4/thothglyph/template/latex/default/document-ja.tex`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/util/svg.py` & `thothglyph_doc-0.2.4/thothglyph/util/svg.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,75 @@
 from __future__ import annotations
+import os
 import shutil
 import subprocess
 import cairosvg
 from thothglyph.error import ThothglyphError
 
 
 def svg2pdf(**kwargs) -> None:
+    svg2xxx('pdf', **kwargs)
+
+
+def svg2png(**kwargs) -> None:
+    svg2xxx('png', **kwargs)
+
+
+def svg2xxx(target, **kwargs) -> None:
     inpath = None
     indata = None
     outpath = None
+    scale = 1.0
     if 'url' in kwargs and kwargs['url']:
         inpath = kwargs['url']
     elif 'bytestring' in kwargs and kwargs['bytestring']:
         indata = kwargs['bytestring']
     else:
-        msg = 'svg2pdf(): input not found.'
+        msg = 'svg2{}(): input not found.'.format(target)
         raise ThothglyphError(msg)
 
     if 'write_to' in kwargs and kwargs['write_to']:
         outpath = kwargs['write_to']
     else:
-        msg = 'svg2pdf(): output not found.'
+        msg = 'svg2{}(): output not found.'.format(target)
         raise ThothglyphError(msg)
+    if 'scale' in kwargs:
+        scale = kwargs['scale']
 
     if inpath:
         with open(inpath, 'rb') as f:
             indata = f.read()
     if isinstance(indata, str):
         indata = indata.encode()
 
+    outdir = os.path.dirname(os.path.abspath(outpath))
+    if not os.path.exists(outdir):
+        os.makedirs(outdir, exist_ok=True)
+
     rsvg_convert = shutil.which('rsvg-convert')
     if rsvg_convert:
         rsvg_cmd = [
-            'rsvg-convert', '-f', 'pdf', '-o', '{}.pdf'.format(outpath)
+            'rsvg-convert', '-f', target, '-o', outpath, '-z', str(scale)
         ]
         p = subprocess.Popen(
             rsvg_cmd,
             stdin=subprocess.PIPE,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.DEVNULL
         )
         p.communicate(input=indata)
         if p.returncode != 0:
             msg = '{} command exit with code {}.'.format(rsvg_cmd[0], p.returncode)
             raise ThothglyphError(msg)
     else:
-        cairosvg.svg2pdf(bytestring=indata, write_to='{}.pdf'.format(outpath))
+        if target == 'pdf':
+            cairosvg.svg2pdf(
+                bytestring=indata,
+                write_to=outpath,
+                scale=scale
+            )
+        elif target == 'png':
+            cairosvg.svg2png(
+                bytestring=indata,
+                write_to=outpath,
+                scale=scale
+            )
```

### Comparing `thothglyph_doc-0.2.3/thothglyph/writer/docx.py` & `thothglyph_doc-0.2.4/thothglyph/writer/docx.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from docx.enum.table import WD_TABLE_ALIGNMENT
 from docx.enum.text import WD_BREAK
 from docx.text.paragraph import Paragraph
 # from docx.enum.text import WD_TAB_ALIGNMENT
 # from docx.enum.text import WD_TAB_LEADER
 from thothglyph.error import ThothglyphError
 from thothglyph.writer.writer import Writer
+from thothglyph.util.svg import svg2png
 from thothglyph.node import nd
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 # monkey patch
 if True:
@@ -340,24 +341,25 @@
             else:
                 table.alignment = WD_TABLE_ALIGNMENT.LEFT
         for raw in table.rows:
             for c in raw._tr.tc_lst:
                 tcW = c.tcPr.tcW
                 tcW.type = 'auto'
                 tcW.w = 0
+        self.tables.append(table)
+
+    def leave_tableblock(self, node):
+        table = self.tables[-1]
         if node.headers == 0:
             table.style = self.stylename['table_normal']
         else:
             table.style = self.stylename['table_list']
             for i in range(node.headers):
                 trPr = table.rows[i]._tr.get_or_add_trPr()
                 trPr.get_or_add_tblHeader()
-        self.tables.append(table)
-
-    def leave_tableblock(self, node):
         self.tables.pop()
 
     def visit_tablerow(self, node):
         pass
 
     def leave_tablerow(self, node):
         pass
@@ -404,47 +406,50 @@
         if not self.p:
             self.p = self._add_paragraph()
         if isinstance(node.parent, nd.ListItemNode):
             item = node.parent
             is_first_paragraph = item.children.index(node) == 0
             if is_first_paragraph and self.numIds:
                 self._multilevel_list_numbering(self.p, item.level - 1, self.numIds[-1])
+            elif item.titlebreak:
+                self._multilevel_list_numbering(self.p, item.level, 15)
             else:
                 self._multilevel_list_numbering(self.p, item.level - 1, 15)
             self.is_first_list_item = False
             if isinstance(item.parent, nd.CheckListBlockNode):
-                r_style = self.stylename['strong']
                 assert self.tmpdirname
                 if item.marker == 'x':
                     checkbox = os.path.join(self.tmpdirname, 'check_en.png')
-                    # self.r = self._add_run('[v] ', r_style)
                 elif item.marker == '-':
                     checkbox = os.path.join(self.tmpdirname, 'check_im.png')
-                    # self.r = self._add_run('[-] ', r_style)
                 else:
                     checkbox = os.path.join(self.tmpdirname, 'check_dis.png')
-                    # self.r = self._add_run('[ ] ', r_style)
                 self.r = self._add_run('')
                 self.r.add_picture(checkbox)
                 self.r = self._add_run(' ')
         self.r = self.p.add_run()
 
     def leave_paragraph(self, node):
         self.p = None
         self.r = None
 
     def visit_title(self, node):
         if not self.p:
             self.p = self._add_paragraph()
-        if isinstance(node.parent, nd.DescriptionListBlockNode):
+        if isinstance(node.parent, nd.ListItemNode):
+            item = node.parent
+            self._multilevel_list_numbering(self.p, item.level - 1, 15)
             self.r_style = self.stylename['strong']
 
     def leave_title(self, node):
         self.r_style = None
         self.r = self._add_run(' ')
+        if node.parent.titlebreak:
+            self.p = self._add_paragraph()
+            self.r = self._add_run('')
 
     def visit_decorationrole(self, node):
         stylekey = self.decoration_table[node.role]
         self.r_style = self.stylename[stylekey]
 
     def visit_role(self, node):
         if node.role == '':
@@ -472,16 +477,16 @@
         options = ' '.join(optlist)
 
         image_fullpath = os.path.abspath(node.value)
         imagedir, imagefname = os.path.splitext(image_fullpath)
         fname, ext = os.path.splitext(image_fullpath)
         if ext == '.svg':
             assert self.tmpdirname
-            tmpimage_path = os.path.join(self.tmpdirname, f'{fname}.png')
-            cairosvg.svg2png(
+            tmpimage_path = os.path.join(self.tmpdirname, '{}.png'.format(node.value))
+            svg2png(
                 url=image_fullpath,
                 write_to=tmpimage_path,
                 scale=0.625,
             )
             image_fullpath = tmpimage_path
         if isinstance(node.parent, nd.ParagraphNode):
             if self.r:
```

### Comparing `thothglyph_doc-0.2.3/thothglyph/writer/html.py` & `thothglyph_doc-0.2.4/thothglyph/writer/html.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/thothglyph/writer/latex.py` & `thothglyph_doc-0.2.4/thothglyph/writer/latex.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         'MARKED': '<?tg:U?>',
         'STRIKE': '<?tg:SO?>',
         'VAR': '<?tg:VAR?>',
         'CODE': '',
         'SUP': '',
         'SUB': '',
     }
-    bp_scale: float = 72.0 / 150.0
+    bp_scale: float = 0.625
 
     def __init__(self):
         super().__init__()
         self.tmpdirname: Optional[str] = None
         self.contentphase: str = 'before'  # before, main, after
 
     def parse(self, node) -> None:
```

### Comparing `thothglyph_doc-0.2.3/thothglyph/writer/pdf.py` & `thothglyph_doc-0.2.4/thothglyph/writer/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,14 @@
         pass
 
     def visit_imagerole(self, node: nd.ASTNode) -> None:
         super().visit_imagerole(node)
         fname, ext = os.path.splitext(node.value)
         if ext == '.svg':
             assert self.tmpdirname
-            imgpath = os.path.join(self.tmpdirname, node.value)
+            imgpath = os.path.join(self.tmpdirname, '{}.pdf'.format(node.value))
             svg2pdf(url=node.value, write_to=imgpath)
         else:
             pass
 
     def leave_imagerole(self, node: nd.ASTNode) -> None:
         pass
```

### Comparing `thothglyph_doc-0.2.3/thothglyph/writer/writer.py` & `thothglyph_doc-0.2.4/thothglyph/writer/writer.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.3/PKG-INFO` & `thothglyph_doc-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thothglyph-doc
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Documentation converter and language for Engineers
 License: MIT
 Author: nakandev
 Author-email: nakandev.s@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

