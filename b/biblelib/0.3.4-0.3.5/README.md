# Comparing `tmp/biblelib-0.3.4.tar.gz` & `tmp/biblelib-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biblelib-0.3.4.tar", max compression
+gzip compressed data, was "biblelib-0.3.5.tar", max compression
```

## Comparing `biblelib-0.3.4.tar` & `biblelib-0.3.5.tar`

### file list

```diff
@@ -1,39 +1,42 @@
--rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.3.4/LICENSE.md
--rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.3.4/LICENSE.md~
--rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.3.4/README.md
--rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.3.4/biblelib/__init__.py
--rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.3.4/biblelib/book/ReadMe.md
--rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.3.4/biblelib/book/__init__.py
--rw-r--r--   0        0        0    15533 2024-03-24 20:04:43.564328 biblelib-0.3.4/biblelib/book/book.py
--rw-r--r--   0        0        0     5178 2024-04-18 23:10:23.491912 biblelib-0.3.4/biblelib/book/books.tsv
--rw-r--r--   0        0        0     2114 2024-03-11 18:59:03.207673 biblelib-0.3.4/biblelib/sources.py
--rw-r--r--   0        0        0      807 2024-02-02 00:29:34.781053 biblelib-0.3.4/biblelib/unit/__init__.py
--rw-r--r--   0        0        0     5936 2024-04-23 02:01:59.233109 biblelib-0.3.4/biblelib/unit/book.py
--rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.3.4/biblelib/unit/bookchapters.tsv
--rw-r--r--   0        0        0     7217 2024-04-23 02:09:13.463233 biblelib-0.3.4/biblelib/unit/chapter.py
--rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.3.4/biblelib/unit/chapters.tsv
--rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.3.4/biblelib/unit/chapterverses.tsv
--rw-r--r--   0        0        0     7558 2023-09-08 17:09:37.206917 biblelib-0.3.4/biblelib/unit/pericope.py
--rw-r--r--   0        0        0    29962 2023-09-01 16:52:21.204686 biblelib-0.3.4/biblelib/unit/tempchapter.py
--rw-r--r--   0        0        0     3564 2024-02-02 00:50:46.449409 biblelib-0.3.4/biblelib/unit/unit.py
--rw-r--r--   0        0        0     6339 2024-04-23 02:09:29.760805 biblelib-0.3.4/biblelib/unit/unitrange.py
--rw-r--r--   0        0        0     1534 2023-11-15 21:26:03.558678 biblelib-0.3.4/biblelib/unit/verse.py
--rw-r--r--   0        0        0     5010 2024-03-11 18:59:15.691582 biblelib-0.3.4/biblelib/versification/Enumerator.py
--rw-r--r--   0        0        0     2108 2024-03-19 16:38:12.467449 biblelib-0.3.4/biblelib/versification/Mapper.py
--rw-r--r--   0        0        0     2992 2024-02-21 01:50:54.075772 biblelib-0.3.4/biblelib/versification/ReadMe.md
--rw-r--r--   0        0        0     1871 2024-03-15 00:46:57.917308 biblelib-0.3.4/biblelib/versification/VrefReader.py
--rw-r--r--   0        0        0      355 2024-03-11 19:15:48.838121 biblelib-0.3.4/biblelib/versification/__init__.py
--rw-r--r--   0        0        0    73057 2024-02-21 01:58:50.596799 biblelib-0.3.4/biblelib/versification/eng-nt-vref.txt
--rw-r--r--   0        0        0   217072 2024-02-21 01:58:57.893444 biblelib-0.3.4/biblelib/versification/eng-ot-vref.txt
--rw-r--r--   0        0        0   290129 2024-02-21 01:59:00.692427 biblelib-0.3.4/biblelib/versification/eng-protestant-vref.txt
--rw-r--r--   0        0        0    73037 2024-02-21 01:59:10.108486 biblelib-0.3.4/biblelib/versification/org-nt-vref.txt
--rw-r--r--   0        0        0   217742 2024-02-21 01:59:11.043178 biblelib-0.3.4/biblelib/versification/org-ot-vref.txt
--rw-r--r--   0        0        0   290779 2024-02-21 01:59:12.401051 biblelib-0.3.4/biblelib/versification/org-protestant-vref.txt
--rw-r--r--   0        0        0    73017 2024-02-21 02:01:54.453211 biblelib-0.3.4/biblelib/versification/rso-nt-vref.txt
--rw-r--r--   0        0        0   219552 2024-02-21 02:03:39.027636 biblelib-0.3.4/biblelib/versification/rso-ot-vref.txt
--rw-r--r--   0        0        0   292569 2024-02-21 02:01:57.600383 biblelib-0.3.4/biblelib/versification/rso-protestant-vref.txt
--rw-r--r--   0        0        0      993 2024-04-23 02:10:18.899048 biblelib-0.3.4/biblelib/word/__init__.py
--rw-r--r--   0        0        0    25849 2024-04-23 02:10:27.855441 biblelib-0.3.4/biblelib/word/bcvwpid.py
--rw-r--r--   0        0        0     4432 2022-11-17 00:30:21.039343 biblelib-0.3.4/biblelib/word/mappings.py
--rw-r--r--   0        0        0     1324 2024-04-23 02:14:02.953441 biblelib-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 biblelib-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.3.5/LICENSE.md
+-rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.3.5/LICENSE.md~
+-rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.3.5/README.md
+-rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.3.5/biblelib/__init__.py
+-rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.3.5/biblelib/book/ReadMe.md
+-rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.3.5/biblelib/book/__init__.py
+-rw-r--r--   0        0        0    15533 2024-03-24 20:04:43.564328 biblelib-0.3.5/biblelib/book/book.py
+-rw-r--r--   0        0        0     5178 2024-04-18 23:10:23.491912 biblelib-0.3.5/biblelib/book/books.tsv
+-rw-r--r--   0        0        0     2114 2024-03-11 18:59:03.207673 biblelib-0.3.5/biblelib/sources.py
+-rw-r--r--   0        0        0      807 2024-02-02 00:29:34.781053 biblelib-0.3.5/biblelib/unit/__init__.py
+-rw-r--r--   0        0        0     5936 2024-04-23 02:01:59.233109 biblelib-0.3.5/biblelib/unit/book.py
+-rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.3.5/biblelib/unit/bookchapters.tsv
+-rw-r--r--   0        0        0     7217 2024-04-23 02:09:13.463233 biblelib-0.3.5/biblelib/unit/chapter.py
+-rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.3.5/biblelib/unit/chapters.tsv
+-rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.3.5/biblelib/unit/chapterverses.tsv
+-rw-r--r--   0        0        0     7558 2023-09-08 17:09:37.206917 biblelib-0.3.5/biblelib/unit/pericope.py
+-rw-r--r--   0        0        0    29962 2023-09-01 16:52:21.204686 biblelib-0.3.5/biblelib/unit/tempchapter.py
+-rw-r--r--   0        0        0     3564 2024-02-02 00:50:46.449409 biblelib-0.3.5/biblelib/unit/unit.py
+-rw-r--r--   0        0        0     6339 2024-04-23 02:09:29.760805 biblelib-0.3.5/biblelib/unit/unitrange.py
+-rw-r--r--   0        0        0     1534 2023-11-15 21:26:03.558678 biblelib-0.3.5/biblelib/unit/verse.py
+-rw-r--r--   0        0        0     5010 2024-03-11 18:59:15.691582 biblelib-0.3.5/biblelib/versification/Enumerator.py
+-rw-r--r--   0        0        0     2108 2024-03-19 16:38:12.467449 biblelib-0.3.5/biblelib/versification/Mapper.py
+-rw-r--r--   0        0        0     2992 2024-02-21 01:50:54.075772 biblelib-0.3.5/biblelib/versification/ReadMe.md
+-rw-r--r--   0        0        0     1871 2024-03-15 00:46:57.917308 biblelib-0.3.5/biblelib/versification/VrefReader.py
+-rw-r--r--   0        0        0      355 2024-03-11 19:15:48.838121 biblelib-0.3.5/biblelib/versification/__init__.py
+-rw-r--r--   0        0        0    73057 2024-02-21 01:58:50.596799 biblelib-0.3.5/biblelib/versification/eng-nt-vref.txt
+-rw-r--r--   0        0        0   217072 2024-02-21 01:58:57.893444 biblelib-0.3.5/biblelib/versification/eng-ot-vref.txt
+-rw-r--r--   0        0        0   290129 2024-02-21 01:59:00.692427 biblelib-0.3.5/biblelib/versification/eng-protestant-vref.txt
+-rw-r--r--   0        0        0    73037 2024-02-21 01:59:10.108486 biblelib-0.3.5/biblelib/versification/org-nt-vref.txt
+-rw-r--r--   0        0        0   217742 2024-02-21 01:59:11.043178 biblelib-0.3.5/biblelib/versification/org-ot-vref.txt
+-rw-r--r--   0        0        0   290779 2024-02-21 01:59:12.401051 biblelib-0.3.5/biblelib/versification/org-protestant-vref.txt
+-rw-r--r--   0        0        0    73017 2024-02-21 02:01:54.453211 biblelib-0.3.5/biblelib/versification/rso-nt-vref.txt
+-rw-r--r--   0        0        0   219552 2024-02-21 02:03:39.027636 biblelib-0.3.5/biblelib/versification/rso-ot-vref.txt
+-rw-r--r--   0        0        0   292569 2024-02-21 02:01:57.600383 biblelib-0.3.5/biblelib/versification/rso-protestant-vref.txt
+-rw-r--r--   0        0        0      910 2024-05-06 23:25:56.736634 biblelib-0.3.5/biblelib/word/__init__.py
+-rw-r--r--   0        0        0    25126 2024-05-07 00:20:10.294458 biblelib-0.3.5/biblelib/word/bcvwpid.py
+-rw-r--r--   0        0        0      356 2024-05-06 23:17:32.231962 biblelib-0.3.5/biblelib/word/mappings/__init__.py
+-rw-r--r--   0        0        0     5513 2024-05-06 22:42:51.746991 biblelib-0.3.5/biblelib/word/mappings/gnt.py
+-rw-r--r--   0        0        0     1189 2024-05-07 00:20:11.048356 biblelib-0.3.5/biblelib/word/mappings/marble.py
+-rw-r--r--   0        0        0     3671 2024-05-06 21:44:17.650867 biblelib-0.3.5/biblelib/word/mappings/wlcm.py
+-rw-r--r--   0        0        0     1324 2024-05-07 00:36:40.536806 biblelib-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 biblelib-0.3.5/PKG-INFO
```

### Comparing `biblelib-0.3.4/LICENSE.md` & `biblelib-0.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/LICENSE.md~` & `biblelib-0.3.5/LICENSE.md~`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/README.md` & `biblelib-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/book/ReadMe.md` & `biblelib-0.3.5/biblelib/book/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/book/book.py` & `biblelib-0.3.5/biblelib/book/book.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/book/books.tsv` & `biblelib-0.3.5/biblelib/book/books.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/sources.py` & `biblelib-0.3.5/biblelib/sources.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/unit/__init__.py` & `biblelib-0.3.5/biblelib/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/unit/book.py` & `biblelib-0.3.5/biblelib/unit/book.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/unit/bookchapters.tsv` & `biblelib-0.3.5/biblelib/unit/bookchapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/unit/chapter.py` & `biblelib-0.3.5/biblelib/unit/chapter.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/unit/chapters.tsv` & `biblelib-0.3.5/biblelib/unit/chapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/unit/chapterverses.tsv` & `biblelib-0.3.5/biblelib/unit/chapterverses.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/unit/pericope.py` & `biblelib-0.3.5/biblelib/unit/pericope.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/unit/tempchapter.py` & `biblelib-0.3.5/biblelib/unit/tempchapter.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/unit/unit.py` & `biblelib-0.3.5/biblelib/unit/unit.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/unit/unitrange.py` & `biblelib-0.3.5/biblelib/unit/unitrange.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/unit/verse.py` & `biblelib-0.3.5/biblelib/unit/verse.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/versification/Enumerator.py` & `biblelib-0.3.5/biblelib/versification/Enumerator.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/versification/Mapper.py` & `biblelib-0.3.5/biblelib/versification/Mapper.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/versification/ReadMe.md` & `biblelib-0.3.5/biblelib/versification/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/versification/VrefReader.py` & `biblelib-0.3.5/biblelib/versification/VrefReader.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/versification/eng-nt-vref.txt` & `biblelib-0.3.5/biblelib/versification/eng-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/versification/eng-ot-vref.txt` & `biblelib-0.3.5/biblelib/versification/eng-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/versification/eng-protestant-vref.txt` & `biblelib-0.3.5/biblelib/versification/eng-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/versification/org-nt-vref.txt` & `biblelib-0.3.5/biblelib/versification/org-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/versification/org-ot-vref.txt` & `biblelib-0.3.5/biblelib/versification/org-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/versification/org-protestant-vref.txt` & `biblelib-0.3.5/biblelib/versification/org-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/versification/rso-nt-vref.txt` & `biblelib-0.3.5/biblelib/versification/rso-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/versification/rso-ot-vref.txt` & `biblelib-0.3.5/biblelib/versification/rso-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/versification/rso-protestant-vref.txt` & `biblelib-0.3.5/biblelib/versification/rso-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.4/biblelib/word/__init__.py` & `biblelib-0.3.5/biblelib/word/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 * [Clear-Bible/macula-greek](https://github.com/Clear-Bible/macula-greek):
   Syntax trees, morphology, and linguistic annotations for the Greek
   New Testament
 
 """
 
-from .mappings import Mapping, Mappings
 from .bcvwpid import (
     BID,
     BCID,
     BCVID,
     BCVIDRange,
     BCVWPID,
     fromlogos,
@@ -40,11 +39,8 @@
     "fromname",
     "fromosis",
     "fromusfm",
     "fromubs",
     "reftypes",
     "simplify",
     "to_bcv",
-    # words
-    "Mapping",
-    "Mappings",
 ]
```

### Comparing `biblelib-0.3.4/biblelib/word/bcvwpid.py` & `biblelib-0.3.5/biblelib/word/bcvwpid.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 """
 
 from dataclasses import dataclass, field
 import re
 from typing import Any, Union, get_args
 
 from biblelib.book import Books
+from .mappings import Mapper
 
 BOOKS = Books()
 
 
 @dataclass(order=True)
 class _Base:
     """Base class for units."""
@@ -670,52 +671,39 @@
             return BCID(f"{usfmbook}{pad3(rest)}")
         else:
             # book, chapter, verse
             chapter, verse = rest.split(":", 1)
             return BCVID(f"{usfmbook}{pad3(chapter)}{pad3(verse)}")
 
 
-def fromubs(ref: str, strict: bool = False) -> BCVWPID:
-    """Return a BCVWP instance for a single UBS reference.
+def fromubs(ref: str) -> list[BCVID | BCVWPID]:
+    """Return a list of BCV(WP) instances for a single UBS reference.
 
-    UBS references are 14 characters with an extra leading digit, a
-    segment code that is empty except for DC and LXX books, and the
-    word numbers are doubled.
-
-    Odd word numbers are rounded down, assuming they represent (wn *
-    2) + 1 for a variant. With strict=True (default is False), odd
-    word numbers raise an error.
-
-    """
-
-    def evenp(digits: int | str) -> bool:
-        """Return True if digits is an even-numbered integer, else False."""
-        return (int(digits) % 2) == 0
-
-    # some UBS DGNT references have this as a suffix: fragile
-    if re.search(r"\({N:00\d}\)$", ref) or re.search(r"{N:00\d}$", ref):
-        ref = ref[:14]
-    assert len(ref) == 14, f"Not a UBS reference: {ref}"
-    # drop leading digit
-    assert ref[0] == "0", f"Leading digit should be 0: {ref}"
-    book = ref[1:3]
-    chapter = ref[3:6]
-    verse = ref[6:9]
-    # next two digits are the segment: per
-    # https://docs.google.com/document/d/1hAGSokibAXkxL28fKXQQzYV_BkMnzs7ILX7W07q3JN0/
-    # "relevant for DC books and LXX only, otherwise 00"
-    assert ref[9:11] == "00", f"Segment code should be 00: {ref}"
-    # MARBLE data only uses even numbers for word positions, so divide by 2
-    word = ref[11:14]
-    if not evenp(word) and strict:
-        raise ValueError(f"Word code should be an even number: {ref}")
-    # this drops any fractional part after dividing by 2
-    wnstr = pad3(str(int(int(word) / 2)))
-    # this adds a Part identifier: that does not seem correct
-    return BCVWPID(ID=f"{book}{chapter}{verse}{wnstr}")
+    Hebrew Bible references sometimes map to two Macula tokens because
+    of segmentation differences. Word/part-level references return
+    BCVWPID instances based on mapping files. Those without a non-zero
+    word index are calculated and return BCVIDs.
+
+    This does not yet handle range references.
+
+    """
+    mpr = Mapper()
+    macularefs = mpr.to_macula(ref)
+    reflist: list[BCVID | BCVWPID] = []
+    if macularefs:
+        reflist = [BCVWPID(r) for r in macularefs]
+    elif ref.endswith("0000"):
+        # verse-level reference
+        # drop leading digit
+        assert ref[0] == "0", f"Leading digit should be 0: {ref}"
+        book = ref[1:3]
+        chapter = ref[3:6]
+        verse = ref[6:9]
+        reflist = [BCVID(ID=f"{book}{chapter}{verse}")]
+    return reflist
 
 
 def to_bcv(token: str | BCVWPID | BCVID) -> str:
     """Return the BCV string for a reference instance or identifier.
 
     This handles several input types for generality.
     """
```

### Comparing `biblelib-0.3.4/pyproject.toml` & `biblelib-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biblelib"
-version = "0.3.4"
+version = "0.3.5"
 description = "Utilities for working with metadata for Bible books, references, pericopes, and other units."
 authors = ["Sean Boisen <sean.boisen@gmail.com>"]
 repository = "https://github.com/Clear-Bible/Biblelib/"
 # documentation = "https://sboisen.github.io/Biblelib/"
 readme = "README.md"
 # apparently text files are also shipped?
 # include = [
```

### Comparing `biblelib-0.3.4/PKG-INFO` & `biblelib-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblelib
-Version: 0.3.4
+Version: 0.3.5
 Summary: Utilities for working with metadata for Bible books, references, pericopes, and other units.
 Home-page: https://github.com/Clear-Bible/Biblelib/
 Author: Sean Boisen
 Author-email: sean.boisen@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

