# Comparing `tmp/parallel_corpus-0.1.0.tar.gz` & `tmp/parallel_corpus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallel_corpus-0.1.0.tar", last modified: Mon May  6 10:03:25 2024, max compression
+gzip compressed data, was "parallel_corpus-0.1.1.tar", last modified: Tue May  7 06:56:15 2024, max compression
```

## Comparing `parallel_corpus-0.1.0.tar` & `parallel_corpus-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1069 2024-04-23 07:08:38.366466 parallel_corpus-0.1.0/LICENSE
--rw-r--r--   0        0        0     3017 2024-05-06 10:03:10.375496 parallel_corpus-0.1.0/README.md
--rw-r--r--   0        0        0     1382 2024-05-06 10:03:25.582164 parallel_corpus-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 09:16:10.481984 parallel_corpus-0.1.0/src/parallel_corpus/__init__.py
--rw-r--r--   0        0        0    13186 2024-05-06 09:34:47.228722 parallel_corpus-0.1.0/src/parallel_corpus/graph.py
--rw-r--r--   0        0        0      468 2024-05-06 09:16:10.485318 parallel_corpus-0.1.0/src/parallel_corpus/shared/__init__.py
--rw-r--r--   0        0        0      701 2024-05-06 09:16:10.485318 parallel_corpus-0.1.0/src/parallel_corpus/shared/dicts.py
--rw-r--r--   0        0        0     4351 2024-05-06 09:16:10.485318 parallel_corpus-0.1.0/src/parallel_corpus/shared/diffs.py
--rw-r--r--   0        0        0      306 2024-05-06 09:16:10.485318 parallel_corpus-0.1.0/src/parallel_corpus/shared/functional.py
--rw-r--r--   0        0        0      565 2024-05-06 09:16:10.485318 parallel_corpus-0.1.0/src/parallel_corpus/shared/ids.py
--rw-r--r--   0        0        0     1500 2024-05-06 09:16:10.485318 parallel_corpus-0.1.0/src/parallel_corpus/shared/lists.py
--rw-r--r--   0        0        0     1414 2024-05-06 09:16:10.485318 parallel_corpus-0.1.0/src/parallel_corpus/shared/ranges.py
--rw-r--r--   0        0        0      170 2024-05-06 09:16:10.485318 parallel_corpus-0.1.0/src/parallel_corpus/shared/str_map.py
--rw-r--r--   0        0        0     3349 2024-05-06 09:16:10.485318 parallel_corpus-0.1.0/src/parallel_corpus/shared/union_find.py
--rw-r--r--   0        0        0      911 2024-05-06 09:16:10.485318 parallel_corpus-0.1.0/src/parallel_corpus/shared/unique_check.py
--rw-r--r--   0        0        0      649 2024-05-06 09:16:10.488651 parallel_corpus-0.1.0/src/parallel_corpus/source_target.py
--rw-r--r--   0        0        0     2056 2024-05-06 09:16:10.488651 parallel_corpus-0.1.0/src/parallel_corpus/token.py
--rw-r--r--   0        0        0        0 2024-04-23 07:45:06.624570 parallel_corpus-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2527 2024-05-06 09:16:10.488651 parallel_corpus-0.1.0/tests/__snapshots__/test_graph.ambr
--rw-r--r--   0        0        0      514 2024-05-06 09:16:10.488651 parallel_corpus-0.1.0/tests/__snapshots__/test_token.ambr
--rw-r--r--   0        0        0    11084 2024-05-06 09:16:10.488651 parallel_corpus-0.1.0/tests/requirements-testing.lock
--rw-r--r--   0        0        0     7921 2024-05-06 09:16:10.488651 parallel_corpus-0.1.0/tests/test_graph.py
--rw-r--r--   0        0        0      965 2024-05-06 09:16:10.488651 parallel_corpus-0.1.0/tests/test_shared/__snapshots__/test_ranges.ambr
--rw-r--r--   0        0        0      470 2024-05-06 09:16:10.488651 parallel_corpus-0.1.0/tests/test_shared/test_diffs.py
--rw-r--r--   0        0        0      393 2024-05-06 09:16:10.491984 parallel_corpus-0.1.0/tests/test_shared/test_functional.py
--rw-r--r--   0        0        0      225 2024-05-06 09:16:10.491984 parallel_corpus-0.1.0/tests/test_shared/test_ids.py
--rw-r--r--   0        0        0      377 2024-05-06 09:16:10.491984 parallel_corpus-0.1.0/tests/test_shared/test_lists.py
--rw-r--r--   0        0        0      484 2024-05-06 09:16:10.491984 parallel_corpus-0.1.0/tests/test_shared/test_ranges.py
--rw-r--r--   0        0        0     1143 2024-05-06 09:16:10.491984 parallel_corpus-0.1.0/tests/test_shared/test_union_find.py
--rw-r--r--   0        0        0      867 2024-05-06 09:16:10.491984 parallel_corpus-0.1.0/tests/test_token.py
--rw-r--r--   0        0        0     4137 1970-01-01 00:00:00.000000 parallel_corpus-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-07 06:56:01.413518 parallel_corpus-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3001 2024-05-07 06:56:01.413518 parallel_corpus-0.1.1/README.md
+-rw-r--r--   0        0        0     1382 2024-05-07 06:56:15.877604 parallel_corpus-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 06:56:01.413518 parallel_corpus-0.1.1/src/parallel_corpus/__init__.py
+-rw-r--r--   0        0        0    13388 2024-05-07 06:56:01.413518 parallel_corpus-0.1.1/src/parallel_corpus/graph.py
+-rw-r--r--   0        0        0      468 2024-05-07 06:56:01.413518 parallel_corpus-0.1.1/src/parallel_corpus/shared/__init__.py
+-rw-r--r--   0        0        0      701 2024-05-07 06:56:01.413518 parallel_corpus-0.1.1/src/parallel_corpus/shared/dicts.py
+-rw-r--r--   0        0        0     4351 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/diffs.py
+-rw-r--r--   0        0        0      306 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/functional.py
+-rw-r--r--   0        0        0      565 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/ids.py
+-rw-r--r--   0        0        0     1500 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/lists.py
+-rw-r--r--   0        0        0     1414 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/ranges.py
+-rw-r--r--   0        0        0      170 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/str_map.py
+-rw-r--r--   0        0        0     3349 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/union_find.py
+-rw-r--r--   0        0        0      911 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/unique_check.py
+-rw-r--r--   0        0        0      649 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/source_target.py
+-rw-r--r--   0        0        0     2056 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/token.py
+-rw-r--r--   0        0        0        0 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2527 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/__snapshots__/test_graph.ambr
+-rw-r--r--   0        0        0      514 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/__snapshots__/test_token.ambr
+-rw-r--r--   0        0        0    21049 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/requirements-testing.lock
+-rw-r--r--   0        0        0     7921 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_graph.py
+-rw-r--r--   0        0        0      965 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/__snapshots__/test_ranges.ambr
+-rw-r--r--   0        0        0      470 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/test_diffs.py
+-rw-r--r--   0        0        0      393 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/test_functional.py
+-rw-r--r--   0        0        0      225 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/test_ids.py
+-rw-r--r--   0        0        0      377 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/test_lists.py
+-rw-r--r--   0        0        0      484 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/test_ranges.py
+-rw-r--r--   0        0        0     1143 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/test_union_find.py
+-rw-r--r--   0        0        0      867 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_token.py
+-rw-r--r--   0        0        0     4121 1970-01-01 00:00:00.000000 parallel_corpus-0.1.1/PKG-INFO
```

### Comparing `parallel_corpus-0.1.0/LICENSE` & `parallel_corpus-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/README.md` & `parallel_corpus-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/parallel-corpus)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/parallel-corpus)](https://pypi.org/project/parallel-corpus/)
 
 [![Maturity badge - level 2](https://img.shields.io/badge/Maturity-Level%202%20--%20First%20Release-yellowgreen.svg)](https://github.com/spraakbanken/getting-started/blob/main/scorecard.md)
 [![Stage](https://img.shields.io/pypi/status/parallel-corpus)](https://pypi.org/project/parallel-corpus/)
 
 [![Codecov](https://codecov.io/gh/spraakbanken/parallel-corpus-py/coverage.svg)](https://codecov.io/gh/spraakbanken/parallel-corpus-py)
-[![CI(release)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/release-kb-bert.yml/badge.svg)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/release-kb-bert.yml)
+[![CI(release)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/release.yml/badge.svg)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/release.yml)
 [![CI(check)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/check.yml/badge.svg)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/check.yml)
 [![CI(test)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/test.yml/badge.svg)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/test.yml)
 [![CI(scheduled)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/scheduled.yml/badge.svg)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/scheduled.yml)
 
 Parallel corpus as a graph.
 
 Ported from [Graph in spraakbanken/swell-editor](https://github.com/spraakbanken/swell-editor).
@@ -31,15 +31,15 @@
 pdm add parallel-corpus
 ```
 
 To add `parallel-corpus` manually to `pyproject.toml`:
 
 ```toml
 [project]
-dependencies = ["parallel-corpus>=0.1.0"]
+dependencies = ["parallel-corpus>=0.1.1"]
 ```
 
 ## Usage
 
 ```python
 first = "Jonathan saknades ."
```

### Comparing `parallel_corpus-0.1.0/pyproject.toml` & `parallel_corpus-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "parallel-corpus"
-version = "0.1.0"
+version = "0.1.1"
 description = "Parallel corpus as a graph."
 authors = [
     { name = "Språkbanken Text", email = "sb-info@svenska.gu.se" },
     { name = "Kristoffer Andersson", email = "kristoffer.andersson@gu.se" },
 ]
 dependencies = [
     "diff-match-patch>=20230430",
```

### Comparing `parallel_corpus-0.1.0/src/parallel_corpus/graph.py` & `parallel_corpus-0.1.1/src/parallel_corpus/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,22 @@
     return parallel_corpus.shared.str_map.str_map(
         token.text,
         lambda char, _i: CharIdPair(char=char, id=None if char == " " else token.id),
     )
 
 
 def edge_map(g: Graph) -> Dict[str, Edge]:
+    """Map from token ids to edges
+
+    Args:
+        g (Graph): the Graph to build the edge map from.
+
+    Returns:
+        Dict[str, Edge]: a map from token ids to edges
+    """
     edges = {}
     for e in g.edges.values():
         for i in e.ids:
             edges[i] = e
     return edges
 
 
@@ -250,15 +258,15 @@
 
     Indexes are character offsets (use CodeMirror's doc.posFromIndex and doc.indexFromPos to convert)
     """  # noqa: E501
 
     tokens = get_side_texts(g, side)
     token_at = token.token_at(tokens, from_)
     from_token, from_ix = token_at["token"], token_at["offset"]
-    pre = (tokens[from_token] or "")[:from_ix]
+    pre = (tokens[from_token] if from_token < len(tokens) else "")[:from_ix]
     if to == len(get_side_text(g, side)):
         return unaligned_modify_tokens(g, from_token, len(g.get_side(side)), pre + text, side)
     to_token_at = token.token_at(tokens, to)
     to_token, to_ix = to_token_at["token"], to_token_at["offset"]
     post = (tokens[to_token] or "")[to_ix:]
     return unaligned_modify_tokens(g, from_token, to_token + 1, pre + text + post, side)
 
@@ -270,15 +278,15 @@
 def get_side_texts(g: Graph, side: Side) -> List[str]:
     return token.texts(g.get_side(side))
 
 
 def unaligned_modify_tokens(  # noqa: C901
     g: Graph, from_: int, to: int, text: str, side: Side = Side.target
 ) -> Graph:
-    """# /** Replace the text at some position, merging the spans it touches upon.
+    """Replace the text at some position, merging the spans it touches upon.
 
     #   const show = (g: Graph) => g.target.map(t => t.text)
     #   const ids = (g: Graph) => g.target.map(t => t.id).join(' ')
     #   const g = init('test graph hello')
     #   show(g) // => ['test ', 'graph ', 'hello ']
     #   show(unaligned_modify_tokens(g, 0, 0, 'this '))     // => ['this ', 'test ', 'graph ', 'hello ']
     #   show(unaligned_modify_tokens(g, 0, 1, 'this '))     // => ['this ', 'graph ', 'hello ']
@@ -297,15 +305,15 @@
     #   ids(unaligned_modify_tokens(g, 0, 1, 'this '))     // => 't3 t1 t2'
     #   ids(unaligned_modify_tokens(g, 0, 1, 'this'))      // => 't3 t2'
     #   const showS = (g: Graph) => g.source.map(t => t.text)
     #   const idsS = (g: Graph) => g.source.map(t => t.id).join(' ')
     #   showS(unaligned_modify_tokens(g, 0, 0, 'this ', 'source')) // => ['this ', 'test ', 'graph ', 'hello ']
     #   idsS(unaligned_modify_tokens(g, 0, 0, 'this ', 'source'))  // => 's3 s0 s1 s2'
 
-    # Indexes are token offsets
+    Indexes are token offsets
     """  # noqa: E501
 
     if (
         from_ < 0
         or to < 0
         or from_ > len(g.get_side(side))
         or to > len(g.get_side(side))
```

### Comparing `parallel_corpus-0.1.0/src/parallel_corpus/shared/dicts.py` & `parallel_corpus-0.1.1/src/parallel_corpus/shared/dicts.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/src/parallel_corpus/shared/diffs.py` & `parallel_corpus-0.1.1/src/parallel_corpus/shared/diffs.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/src/parallel_corpus/shared/ids.py` & `parallel_corpus-0.1.1/src/parallel_corpus/shared/ids.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/src/parallel_corpus/shared/lists.py` & `parallel_corpus-0.1.1/src/parallel_corpus/shared/lists.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/src/parallel_corpus/shared/ranges.py` & `parallel_corpus-0.1.1/src/parallel_corpus/shared/ranges.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/src/parallel_corpus/shared/union_find.py` & `parallel_corpus-0.1.1/src/parallel_corpus/shared/union_find.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/src/parallel_corpus/shared/unique_check.py` & `parallel_corpus-0.1.1/src/parallel_corpus/shared/unique_check.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/src/parallel_corpus/source_target.py` & `parallel_corpus-0.1.1/src/parallel_corpus/source_target.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/src/parallel_corpus/token.py` & `parallel_corpus-0.1.1/src/parallel_corpus/token.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/tests/__snapshots__/test_graph.ambr` & `parallel_corpus-0.1.1/tests/__snapshots__/test_graph.ambr`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/tests/__snapshots__/test_token.ambr` & `parallel_corpus-0.1.1/tests/__snapshots__/test_token.ambr`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/tests/test_graph.py` & `parallel_corpus-0.1.1/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/tests/test_shared/__snapshots__/test_ranges.ambr` & `parallel_corpus-0.1.1/tests/test_shared/__snapshots__/test_ranges.ambr`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/tests/test_shared/test_union_find.py` & `parallel_corpus-0.1.1/tests/test_shared/test_union_find.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/tests/test_token.py` & `parallel_corpus-0.1.1/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.0/PKG-INFO` & `parallel_corpus-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallel-corpus
-Version: 0.1.0
+Version: 0.1.1
 Summary: Parallel corpus as a graph.
 Author-Email: =?utf-8?q?Spr=C3=A5kbanken_Text?= <sb-info@svenska.gu.se>, Kristoffer Andersson <kristoffer.andersson@gu.se>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
@@ -31,15 +31,15 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/parallel-corpus)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/parallel-corpus)](https://pypi.org/project/parallel-corpus/)
 
 [![Maturity badge - level 2](https://img.shields.io/badge/Maturity-Level%202%20--%20First%20Release-yellowgreen.svg)](https://github.com/spraakbanken/getting-started/blob/main/scorecard.md)
 [![Stage](https://img.shields.io/pypi/status/parallel-corpus)](https://pypi.org/project/parallel-corpus/)
 
 [![Codecov](https://codecov.io/gh/spraakbanken/parallel-corpus-py/coverage.svg)](https://codecov.io/gh/spraakbanken/parallel-corpus-py)
-[![CI(release)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/release-kb-bert.yml/badge.svg)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/release-kb-bert.yml)
+[![CI(release)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/release.yml/badge.svg)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/release.yml)
 [![CI(check)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/check.yml/badge.svg)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/check.yml)
 [![CI(test)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/test.yml/badge.svg)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/test.yml)
 [![CI(scheduled)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/scheduled.yml/badge.svg)](https://github.com/spraakbanken/parallel-corpus-py/actions/workflows/scheduled.yml)
 
 Parallel corpus as a graph.
 
 Ported from [Graph in spraakbanken/swell-editor](https://github.com/spraakbanken/swell-editor).
@@ -58,15 +58,15 @@
 pdm add parallel-corpus
 ```
 
 To add `parallel-corpus` manually to `pyproject.toml`:
 
 ```toml
 [project]
-dependencies = ["parallel-corpus>=0.1.0"]
+dependencies = ["parallel-corpus>=0.1.1"]
 ```
 
 ## Usage
 
 ```python
 first = "Jonathan saknades ."
```

