# Comparing `tmp/md2tgmd-0.1.5.tar.gz` & `tmp/md2tgmd-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2tgmd-0.1.5.tar", last modified: Tue May  7 08:39:09 2024, max compression
+gzip compressed data, was "md2tgmd-0.1.6.tar", last modified: Tue May  7 08:48:46 2024, max compression
```

## Comparing `md2tgmd-0.1.5.tar` & `md2tgmd-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:39:09.497786 md2tgmd-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-07 08:39:00.000000 md2tgmd-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-07 08:39:09.497786 md2tgmd-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-07 08:39:00.000000 md2tgmd-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:39:09.497786 md2tgmd-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 08:39:00.000000 md2tgmd-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:39:09.493786 md2tgmd-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:39:09.497786 md2tgmd-0.1.5/src/md2tgmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-07 08:39:09.000000 md2tgmd-0.1.5/src/md2tgmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 08:39:09.000000 md2tgmd-0.1.5/src/md2tgmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:39:09.000000 md2tgmd-0.1.5/src/md2tgmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 08:39:09.000000 md2tgmd-0.1.5/src/md2tgmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-07 08:39:00.000000 md2tgmd-0.1.5/src/md2tgmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:46.010561 md2tgmd-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-07 08:48:37.000000 md2tgmd-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-07 08:48:46.010561 md2tgmd-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-07 08:48:37.000000 md2tgmd-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:48:46.010561 md2tgmd-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 08:48:37.000000 md2tgmd-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:46.006561 md2tgmd-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:46.010561 md2tgmd-0.1.6/src/md2tgmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-07 08:48:45.000000 md2tgmd-0.1.6/src/md2tgmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 08:48:45.000000 md2tgmd-0.1.6/src/md2tgmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:48:45.000000 md2tgmd-0.1.6/src/md2tgmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 08:48:45.000000 md2tgmd-0.1.6/src/md2tgmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-07 08:48:37.000000 md2tgmd-0.1.6/src/md2tgmd.py
```

### Comparing `md2tgmd-0.1.5/LICENSE` & `md2tgmd-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `md2tgmd-0.1.5/PKG-INFO` & `md2tgmd-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2tgmd
-Version: 0.1.5
+Version: 0.1.6
 Summary: md2tgmd is a Markdown to Telegram-specific-markdown converter.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # md2tgmd
 
 md2tgmd is a Markdown to [Telegram-specific-markdown](https://core.telegram.org/bots/api#formatting-options) converter.
```

### Comparing `md2tgmd-0.1.5/README.md` & `md2tgmd-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `md2tgmd-0.1.5/src/md2tgmd.egg-info/PKG-INFO` & `md2tgmd-0.1.6/src/md2tgmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2tgmd
-Version: 0.1.5
+Version: 0.1.6
 Summary: md2tgmd is a Markdown to Telegram-specific-markdown converter.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # md2tgmd
 
 md2tgmd is a Markdown to [Telegram-specific-markdown](https://core.telegram.org/bots/api#formatting-options) converter.
```

### Comparing `md2tgmd-0.1.5/src/md2tgmd.py` & `md2tgmd-0.1.6/src/md2tgmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     返回:
     list: 满足条件的行的索引列表。
     """
     lines = s.split('\n')  # 按行拆分字符串
 
     for index, line in enumerate(lines):
-        if line.count(char) >= min_count or re.sub(r"```", '', line).count(char) % 2 != 0:
+        if line.count(char) >= min_count or re.sub(r"```", '', line).count(char) % 2 != 0 or (not line.strip().startswith("```") and line.count(char) % 2 != 0):
             # lines[index] = re.sub(r"`", '\`', line)
             lines[index] = replace_all(lines[index], r"\\`|(`)", escape_all_backquote)
 
     return "\n".join(lines)
 
 def escape(text, flag=0):
     # In all other places characters
@@ -186,14 +186,16 @@
 
 `-a----++++`++a-b-c`-n-`
 `[^``]*`a``b-c``d``
 # pattern = r"`[^`]*`-([^`-]*)"``
 w`-a----`ccccc`-n-`bbbb``a
 
 1. 打开 VSCode 的终端：选择菜单中的 `视图` > `终端`，或者使用快捷键 `Ctrl+``（反引号）。
+
+python line.strip().startwith("```")怎么写？
 '''
 
 if __name__ == '__main__':
     import os
     os.system('clear')
     text = escape(text)
     print(text)
```

