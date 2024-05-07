# Comparing `tmp/fsrs-2.0.0.tar.gz` & `tmp/fsrs-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs-2.0.0.tar", last modified: Tue Apr 30 02:42:52 2024, max compression
+gzip compressed data, was "fsrs-2.1.0.tar", last modified: Tue May  7 02:37:18 2024, max compression
```

## Comparing `fsrs-2.0.0.tar` & `fsrs-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:52.385321 fsrs-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-30 02:42:45.000000 fsrs-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-30 02:42:52.385321 fsrs-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-30 02:42:45.000000 fsrs-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-30 02:42:45.000000 fsrs-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 02:42:52.385321 fsrs-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 02:42:45.000000 fsrs-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:52.385321 fsrs-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:52.385321 fsrs-2.0.0/src/fsrs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 02:42:45.000000 fsrs-2.0.0/src/fsrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-30 02:42:45.000000 fsrs-2.0.0/src/fsrs/fsrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-30 02:42:45.000000 fsrs-2.0.0/src/fsrs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:52.385321 fsrs-2.0.0/src/fsrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-30 02:42:52.000000 fsrs-2.0.0/src/fsrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 02:42:52.000000 fsrs-2.0.0/src/fsrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 02:42:52.000000 fsrs-2.0.0/src/fsrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 02:42:52.000000 fsrs-2.0.0/src/fsrs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:52.385321 fsrs-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-30 02:42:45.000000 fsrs-2.0.0/tests/test_fsrs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:37:18.028366 fsrs-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 02:37:13.000000 fsrs-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-07 02:37:18.028366 fsrs-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-07 02:37:13.000000 fsrs-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-07 02:37:13.000000 fsrs-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:37:18.028366 fsrs-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:37:13.000000 fsrs-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:37:18.024366 fsrs-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:37:18.028366 fsrs-2.1.0/src/fsrs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 02:37:13.000000 fsrs-2.1.0/src/fsrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-07 02:37:13.000000 fsrs-2.1.0/src/fsrs/fsrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-05-07 02:37:13.000000 fsrs-2.1.0/src/fsrs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:37:18.028366 fsrs-2.1.0/src/fsrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-07 02:37:18.000000 fsrs-2.1.0/src/fsrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 02:37:18.000000 fsrs-2.1.0/src/fsrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:37:18.000000 fsrs-2.1.0/src/fsrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 02:37:18.000000 fsrs-2.1.0/src/fsrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:37:18.028366 fsrs-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-07 02:37:13.000000 fsrs-2.1.0/tests/test_fsrs.py
```

### Comparing `fsrs-2.0.0/LICENSE` & `fsrs-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fsrs-2.0.0/PKG-INFO` & `fsrs-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 2.0.0
+Version: 2.1.0
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fsrs-2.0.0/README.md` & `fsrs-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fsrs-2.0.0/pyproject.toml` & `fsrs-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fsrs"
-version = "2.0.0"
+version = "2.1.0"
 description = "Free Spaced Repetition Scheduler"
 readme = "README.md"
 authors = [{ name = "Jarrett Ye", email = "jarrett.ye@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `fsrs-2.0.0/src/fsrs/fsrs.py` & `fsrs-2.1.0/src/fsrs/fsrs.py`

 * *Files identical despite different names*

### Comparing `fsrs-2.0.0/src/fsrs/models.py` & `fsrs-2.1.0/src/fsrs/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -47,23 +47,89 @@
     elapsed_days: int
     scheduled_days: int
     reps: int
     lapses: int
     state: State
     last_review: datetime
 
-    def __init__(self) -> None:
-        self.due = datetime.now(UTC)
-        self.stability = 0
-        self.difficulty = 0
-        self.elapsed_days = 0
-        self.scheduled_days = 0
-        self.reps = 0
-        self.lapses = 0
-        self.state = State.New
+    def __init__(
+        self,
+        due=None,
+        stability=0,
+        difficulty=0,
+        elapsed_days=0,
+        scheduled_days=0,
+        reps=0,
+        lapses=0,
+        state=State.New,
+        last_review=None,
+    ) -> None:
+
+        if due is None:
+            self.due = datetime.now(UTC)
+        else:
+            self.due = due
+
+        self.stability = stability
+        self.difficulty = difficulty
+        self.elapsed_days = elapsed_days
+        self.scheduled_days = scheduled_days
+        self.reps = reps
+        self.lapses = lapses
+        self.state = state
+
+        if last_review is not None:
+            self.last_review = last_review
+
+    def to_dict(self):
+
+        return_dict = {
+            "due": self.due.isoformat(),
+            "stability": self.stability,
+            "difficulty": self.difficulty,
+            "elapsed_days": self.elapsed_days,
+            "scheduled_days": self.scheduled_days,
+            "reps": self.reps,
+            "lapses": self.lapses,
+            "state": self.state,
+        }
+
+        if hasattr(self, "last_review"):
+            return_dict["last_review"] = self.last_review.isoformat()
+
+        return return_dict
+
+    @staticmethod
+    def from_dict(source_dict):
+
+        due = datetime.fromisoformat(source_dict["due"])
+        stability = source_dict["stability"]
+        difficulty = source_dict["difficulty"]
+        elapsed_days = source_dict["elapsed_days"]
+        scheduled_days = source_dict["scheduled_days"]
+        reps = source_dict["reps"]
+        lapses = source_dict["lapses"]
+        state = source_dict["state"]
+
+        if "last_review" in source_dict:
+            last_review = datetime.fromisoformat(source_dict["last_review"])
+        else:
+            last_review = None
+
+        return Card(
+            due,
+            stability,
+            difficulty,
+            elapsed_days,
+            scheduled_days,
+            reps,
+            lapses,
+            state,
+            last_review,
+        )
 
     def get_retrievability(self, now: datetime) -> Optional[float]:
         DECAY = -0.5
         FACTOR = 0.9 ** (1 / DECAY) - 1
 
         if self.state == State.Review:
             elapsed_days = max(0, (now - self.last_review).days)
```

### Comparing `fsrs-2.0.0/src/fsrs.egg-info/PKG-INFO` & `fsrs-2.1.0/src/fsrs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 2.0.0
+Version: 2.1.0
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

