# Comparing `tmp/md2tgmd-0.1.2.tar.gz` & `tmp/md2tgmd-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2tgmd-0.1.2.tar", last modified: Thu Mar 21 06:45:43 2024, max compression
+gzip compressed data, was "md2tgmd-0.1.4.tar", last modified: Tue May  7 07:30:50 2024, max compression
```

## Comparing `md2tgmd-0.1.2.tar` & `md2tgmd-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 06:45:43.720437 md2tgmd-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-03-21 06:45:35.000000 md2tgmd-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-21 06:45:43.720437 md2tgmd-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-03-21 06:45:35.000000 md2tgmd-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 06:45:43.720437 md2tgmd-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-21 06:45:35.000000 md2tgmd-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 06:45:43.716437 md2tgmd-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 06:45:43.716437 md2tgmd-0.1.2/src/md2tgmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-21 06:45:43.000000 md2tgmd-0.1.2/src/md2tgmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-21 06:45:43.000000 md2tgmd-0.1.2/src/md2tgmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 06:45:43.000000 md2tgmd-0.1.2/src/md2tgmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 06:45:43.000000 md2tgmd-0.1.2/src/md2tgmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-03-21 06:45:35.000000 md2tgmd-0.1.2/src/md2tgmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:30:50.308371 md2tgmd-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-07 07:30:41.000000 md2tgmd-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-07 07:30:50.308371 md2tgmd-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-07 07:30:41.000000 md2tgmd-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:30:50.308371 md2tgmd-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 07:30:41.000000 md2tgmd-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:30:50.308371 md2tgmd-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:30:50.308371 md2tgmd-0.1.4/src/md2tgmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-07 07:30:50.000000 md2tgmd-0.1.4/src/md2tgmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 07:30:50.000000 md2tgmd-0.1.4/src/md2tgmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:30:50.000000 md2tgmd-0.1.4/src/md2tgmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 07:30:50.000000 md2tgmd-0.1.4/src/md2tgmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-07 07:30:41.000000 md2tgmd-0.1.4/src/md2tgmd.py
```

### Comparing `md2tgmd-0.1.2/LICENSE` & `md2tgmd-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `md2tgmd-0.1.2/PKG-INFO` & `md2tgmd-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2tgmd
-Version: 0.1.2
+Version: 0.1.4
 Summary: md2tgmd is a Markdown to Telegram-specific-markdown converter.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # md2tgmd
 
 md2tgmd is a Markdown to [Telegram-specific-markdown](https://core.telegram.org/bots/api#formatting-options) converter.
```

### Comparing `md2tgmd-0.1.2/README.md` & `md2tgmd-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `md2tgmd-0.1.2/src/md2tgmd.egg-info/PKG-INFO` & `md2tgmd-0.1.4/src/md2tgmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2tgmd
-Version: 0.1.2
+Version: 0.1.4
 Summary: md2tgmd is a Markdown to Telegram-specific-markdown converter.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # md2tgmd
 
 md2tgmd is a Markdown to [Telegram-specific-markdown](https://core.telegram.org/bots/api#formatting-options) converter.
```

### Comparing `md2tgmd-0.1.2/src/md2tgmd.py` & `md2tgmd-0.1.4/src/md2tgmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,17 +33,23 @@
 
 def escapeminus(text):
     return '\\' + text
 
 def escapebackquote(text):
     return r'\`\`'
 
+def escapebackquoteincode(text):
+    return r'@->@'
+
 def escapeplus(text):
     return '\\' + text
 
+def escape_all_backquote(text):
+    return '\\' + text
+
 def escape(text, flag=0):
     # In all other places characters
     # _ * [ ] ( ) ~ ` > # + - = | { } . !
     # must be escaped with the preceding character '\'.
     text = re.sub(r"\\\[", '@->@', text)
     text = re.sub(r"\\\]", '@<-@', text)
     text = re.sub(r"\\\(", '@-->@', text)
@@ -73,14 +79,19 @@
     text = replace_all(text, r"(^#+\s.+?$)|```[\D\d\s]+?```", escapeshape)
     text = re.sub(r"#", '\#', text)
     text = replace_all(text, r"(\+)|\n[\s]*-\s|```[\D\d\s]+?```|`[\D\d\s]*?`", escapeplus)
     text = re.sub(r"\n{1,2}(\s*)-\s", '\n\n\\1• ', text)
     text = re.sub(r"\n{1,2}(\s*\d{1,2}\.\s)", '\n\n\\1', text)
     text = replace_all(text, r"(-)|\n[\s]*-\s|```[\D\d\s]+?```|`[\D\d\s]*?`", escapeminus)
     text = re.sub(r"```([\D\d\s]+?)```", '@@@\\1@@@', text)
+    # 把 code block 里面的`替换掉
+    text = replace_all(text, r"\@\@\@[\s\d\D]+?\@\@\@|(`)", escapebackquoteincode)
+    text = re.sub(r"`", '\`', text)
+    text = re.sub(r"\@\-\>\@", '`', text)
+
     text = replace_all(text, r"(``)", escapebackquote)
     text = re.sub(r"\@{3}([\D\d\s]+?)\@{3}", '```\\1```', text)
     text = re.sub(r"=", '\=', text)
     text = re.sub(r"\|", '\|', text)
     text = re.sub(r"{", '\{', text)
     text = re.sub(r"}", '\}', text)
     text = re.sub(r"\.", '\.', text)
@@ -131,14 +142,17 @@
 \subsubsection{1.1}
 
 And simple text `with-ten`  `with+ten` + some - **symbols**. # `with-ten`里面的`-`不会被转义
 
 
 ```
 print("Hello, World!") -
+app.listen(PORT, () => {
+    console.log(`Server is running on http://localhost:${PORT}`);
+});
 ```
 
 Cxy = abs (Pxy)**2/ (Pxx*Pyy)
 
 `a`a-b-c`n`
 \[ E[X^4] = \int_{-\infty}^{\infty} x^4 f(x) dx \]
```

