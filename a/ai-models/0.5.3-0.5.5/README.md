# Comparing `tmp/ai-models-0.5.3.tar.gz` & `tmp/ai_models-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-models-0.5.3.tar", last modified: Fri Apr 19 12:46:10 2024, max compression
+gzip compressed data, was "ai_models-0.5.5.tar", last modified: Tue May  7 09:20:16 2024, max compression
```

## Comparing `ai-models-0.5.3.tar` & `ai_models-0.5.5.tar`

### file list

```diff
@@ -1,29 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:46:10.285175 ai-models-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 12:46:02.000000 ai-models-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-19 12:46:10.285175 ai-models-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-19 12:46:02.000000 ai-models-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:46:10.285175 ai-models-0.5.3/ai_models/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:46:10.285175 ai-models-0.5.3/ai_models/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:46:10.285175 ai-models-0.5.3/ai_models/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/outputs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:46:10.285175 ai-models-0.5.3/ai_models/remote/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/remote/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/remote/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/remote/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/stepper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:46:10.285175 ai-models-0.5.3/ai_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 12:46:10.285175 ai-models-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-19 12:46:02.000000 ai-models-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.043257 ai_models-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.035256 ai_models-0.5.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-07 09:20:05.000000 ai_models-0.5.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-07 09:20:05.000000 ai_models-0.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-07 09:20:05.000000 ai_models-0.5.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 09:20:05.000000 ai_models-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-07 09:20:16.043257 ai_models-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-07 09:20:05.000000 ai_models-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-07 09:20:05.000000 ai_models-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:20:16.043257 ai_models-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.035256 ai_models-0.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/src/ai_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 09:20:15.000000 ai_models-0.5.5/src/ai_models/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/src/ai_models/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15486 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/src/ai_models/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/outputs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/src/ai_models/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/remote/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/remote/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/remote/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/src/ai_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-07 09:20:16.000000 ai_models-0.5.5/src/ai_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-07 09:20:16.000000 ai_models-0.5.5/src/ai_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:20:16.000000 ai_models-0.5.5/src/ai_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-07 09:20:16.000000 ai_models-0.5.5/src/ai_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 09:20:16.000000 ai_models-0.5.5/src/ai_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 09:20:16.000000 ai_models-0.5.5/src/ai_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 09:20:05.000000 ai_models-0.5.5/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-07 09:20:05.000000 ai_models-0.5.5/tests/test_code.py
```

### Comparing `ai-models-0.5.3/LICENSE` & `ai_models-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.3/PKG-INFO` & `ai_models-0.5.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: ai-models
-Version: 0.5.3
-Summary: A package to run AI weather models
-Home-page: https://github.com/ecmwf-lab/ai-models
-Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
-Author-email: software.support@ecmwf.int
-License: Apache License Version 2.0
-Keywords: tool
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: provenance
-License-File: LICENSE
-
 # ai-models
 
 The `ai-models` command is used to run AI-based weather forecasting models. These models need to be installed independently.
 
 ## Usage
 
 Although the source code `ai-models` and its plugins are available under open sources licences, some model weights may be available under a different licence. For example some models make their weights available under the CC-BY-NC-SA 4.0 license, which does not allow commercial use. For more informations, please check the license associated with each model on their main home page, that we link from each of the corresponding plugins.
```

### Comparing `ai-models-0.5.3/ai_models/__main__.py` & `ai_models-0.5.5/src/ai_models/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 import argparse
 import logging
 import os
 import shlex
 import sys
 
 from .inputs import available_inputs
-from .model import Timer, available_models, load_model
+from .model import Timer
+from .model import available_models
+from .model import load_model
 from .outputs import available_outputs
 
 LOG = logging.getLogger(__name__)
 
 
 def _main(argv):
     parser = argparse.ArgumentParser()
@@ -42,44 +44,49 @@
         action="count",
         default=0,
         help="Increase verbosity",
     )
 
     parser.add_argument(
         "--retrieve-requests",
-        help=(
-            "Print mars requests to stdout."
-            "Use --requests-extra to extend or overide the requests. "
-        ),
+        help=("Print mars requests to stdout." "Use --requests-extra to extend or overide the requests. "),
         action="store_true",
     )
 
     parser.add_argument(
         "--archive-requests",
-        help=(
-            "Save mars archive requests to FILE."
-            "Use --requests-extra to extend or overide the requests. "
-        ),
+        help=("Save mars archive requests to FILE." "Use --requests-extra to extend or overide the requests. "),
         metavar="FILE",
     )
 
     parser.add_argument(
         "--requests-extra",
-        help=(
-            "Extends the retrieve or archive requests with a list of key1=value1,key2=value."
-        ),
+        help=("Extends the retrieve or archive requests with a list of key1=value1,key2=value."),
     )
 
     parser.add_argument(
         "--json",
         action="store_true",
         help=("Dump the requests in JSON format."),
     )
 
     parser.add_argument(
+        "--retrieve-fields-type",
+        help="Type of field to retrieve. To use with --retrieve-requests.",
+        choices=["constants", "prognostics", "all"],
+        default="all",
+    )
+
+    parser.add_argument(
+        "--retrieve-only-one-date",
+        help="Only retrieve the last date/time. To use with --retrieve-requests.",
+        action="store_true",
+    )
+
+    parser.add_argument(
         "--dump-provenance",
         metavar="FILE",
         help=("Dump information for tracking provenance."),
     )
 
     parser.add_argument(
         "--input",
@@ -185,14 +192,19 @@
 
     parser.add_argument(
         "--hindcast-reference-year",
         help="For encoding hincast-like outputs",
     )
 
     parser.add_argument(
+        "--hindcast-reference-date",
+        help="For encoding hincast-like outputs",
+    )
+
+    parser.add_argument(
         "--staging-dates",
         help="For encoding hincast-like outputs",
     )
 
     parser.add_argument(
         "--only-gpu",
         help="Fail if GPU is not available",
@@ -271,17 +283,15 @@
         args.metadata["expver"] = args.expver
 
     if args.class_ is not None:
         args.metadata["class"] = args.class_
 
     if args.requests_extra:
         if not args.retrieve_requests and not args.archive_requests:
-            parser.error(
-                "You need to specify --retrieve-requests or --archive-requests"
-            )
+            parser.error("You need to specify --retrieve-requests or --archive-requests")
 
     run(vars(args), unknownargs)
 
 
 def run(cfg: dict, model_args: list):
     if cfg["remote_execution"]:
         from .remote import RemoteModel
@@ -291,17 +301,15 @@
         model = load_model(cfg["model"], **cfg, model_args=model_args)
 
     if cfg["fields"]:
         model.print_fields()
         sys.exit(0)
 
     # This logic is a bit convoluted, but it is for backwards compatibility.
-    if cfg["retrieve_requests"] or (
-        cfg["requests_extra"] and not cfg["archive_requests"]
-    ):
+    if cfg["retrieve_requests"] or (cfg["requests_extra"] and not cfg["archive_requests"]):
         model.print_requests()
         sys.exit(0)
 
     if cfg["assets_list"]:
         model.print_assets_list()
         sys.exit(0)
```

### Comparing `ai-models-0.5.3/ai_models/checkpoint.py` & `ai_models-0.5.5/src/ai_models/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,15 @@
 
 def peek(path):
     with zipfile.ZipFile(path, "r") as f:
         data_pkl = None
         for b in f.namelist():
             if os.path.basename(b) == "data.pkl":
                 if data_pkl is not None:
-                    raise Exception(
-                        f"Found two data.pkl files in {path}: {data_pkl} and {b}"
-                    )
+                    raise Exception(f"Found two data.pkl files in {path}: {data_pkl} and {b}")
                 data_pkl = b
 
     LOG.info(f"Found data.pkl at {data_pkl}")
 
     with zipfile.ZipFile(path, "r") as f:
         unpickler = UnpicklerWrapper(f.open(data_pkl, "r"))
         x = tidy(unpickler.load())
```

### Comparing `ai-models-0.5.3/ai_models/inputs/__init__.py` & `ai_models-0.5.5/src/ai_models/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.3/ai_models/model.py` & `ai_models-0.5.5/src/ai_models/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,17 +50,15 @@
 
     def add(self, field):
         self.expect += 1
         for k, v in field.items():
             self.request[k].add(str(v))
             if k in self.UNIQUE:
                 if len(self.request[k]) > 1:
-                    raise ValueError(
-                        f"Field {field} has different values for {k}: {self.request[k]}"
-                    )
+                    raise ValueError(f"Field {field} has different values for {k}: {self.request[k]}")
 
 
 class Model:
     lagged = False
     assets_extra_dir = None
     retrieve = {}  # Extra parameters for retrieve
     version = 1  # To be overriden in subclasses
@@ -121,15 +119,15 @@
         self.collect_archive_requests(
             self.output.write(*args, **kwargs, **self.grib_extra_metadata),
         )
 
     def collect_archive_requests(self, written):
         if self.archive_requests:
             handle, path = written
-            if self.hindcast_reference_year:
+            if self.hindcast_reference_year or self.hindcast_reference_date:
                 # The clone is necessary because the handle
                 # does not return always return recently set keys
                 handle = handle.clone()
 
             self.archiving[path].add(handle.as_mars())
 
     def finalise(self):
@@ -329,15 +327,15 @@
         if self.json:
             print(json.dumps(requests, indent=4))
             return
 
         for r in requests:
             self._print_request("retrieve", r)
 
-    def _requests(self):
+    def _requests_unfiltered(self):
         result = []
 
         first = dict(
             target="input.grib",
             grid=self.grid,
             area=self.area,
         )
@@ -371,14 +369,63 @@
             r.pop("levelist", None)
 
             self.patch_retrieve_request(r)
             result.append(dict(**r))
 
         return result
 
+    def _requests(self):
+
+        def filter_constant(request):
+            # We check for 'sfc' because param 'z' can be ambiguous
+            if request.get("levtype") == "sfc":
+                param = set(self.constant_fields) & set(request.get("param", []))
+                if param:
+                    request["param"] = list(param)
+                    return True
+
+            return False
+
+        def filter_prognostic(request):
+            # TODO: We assume here that prognostic fields are
+            # the ones that are not constant. This may not always be true
+            if request.get("levtype") == "sfc":
+                param = set(request.get("param", [])) - set(self.constant_fields)
+                if param:
+                    request["param"] = list(param)
+                    return True
+                return False
+
+            return True
+
+        def filter_last_date(request):
+            date, time = max(self.datetimes())
+            return request["date"] == date and request["time"] == time
+
+        def noop(request):
+            return request
+
+        filter_type = {
+            "constants": filter_constant,
+            "prognostics": filter_prognostic,
+            "all": noop,
+        }[self.retrieve_fields_type]
+
+        filter_dates = {
+            True: filter_last_date,
+            False: noop,
+        }[self.retrieve_only_one_date]
+
+        result = []
+        for r in self._requests_unfiltered():
+            if filter_type(r) and filter_dates(r):
+                result.append(r)
+
+        return result
+
     def patch_retrieve_request(self, request):
         # Overriden in subclasses if needed
         pass
 
     def peek_into_checkpoint(self, path):
         return peek(path)
 
@@ -409,14 +456,18 @@
     def gridpoints(self):
         return len(self.all_fields[0].grid_points()[0])
 
     @cached_property
     def start_datetime(self):
         return self.all_fields.order_by(valid_datetime="ascending")[-1].datetime()
 
+    @property
+    def constant_fields(self):
+        raise NotImplementedError("constant_fields")
+
     def write_input_fields(
         self,
         fields,
         accumulations=None,
         accumulations_template=None,
         accumulations_shape=None,
         ignore=None,
```

### Comparing `ai-models-0.5.3/ai_models/outputs/__init__.py` & `ai_models-0.5.5/src/ai_models/outputs/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -50,21 +50,17 @@
 
         try:
             handle, path = self.output.write(data, *args, **kwargs)
 
         except Exception:
             if data is not None:
                 if np.isnan(data).any():
-                    raise ValueError(
-                        f"NaN values found in field. args={args} kwargs={kwargs}"
-                    )
+                    raise ValueError(f"NaN values found in field. args={args} kwargs={kwargs}")
                 if np.isinf(data).any():
-                    raise ValueError(
-                        f"Infinite values found in field. args={args} kwargs={kwargs}"
-                    )
+                    raise ValueError(f"Infinite values found in field. args={args} kwargs={kwargs}")
                 raise
 
         if check:
             # Check that the GRIB keys are as expected
             for key, value in itertools.chain(self.grib_keys.items(), kwargs.items()):
                 if key in ("template",):
                     continue
@@ -78,48 +74,54 @@
 
                 assert str(handle.get(key)) == str(value), (key, handle.get(key), value)
 
         return handle, path
 
 
 class HindcastReLabel:
-    def __init__(self, owner, output, hindcast_reference_year, **kwargs):
+    def __init__(self, owner, output, hindcast_reference_year, hind_cast_reference_date, **kwargs):
         self.owner = owner
         self.output = output
-        self.hindcast_reference_year = int(hindcast_reference_year)
+        self.hindcast_reference_year = int(hindcast_reference_year) if hindcast_reference_year else None
+        self.hind_cast_reference_date = int(hind_cast_reference_date) if hind_cast_reference_date else None
+        assert self.hindcast_reference_year is not None or self.hind_cast_reference_date is not None
 
     def write(self, *args, **kwargs):
         if "hdate" in kwargs:
-            warnings.warn(
-                f"Ignoring hdate='{kwargs['hdate']}' in HindcastReLabel", stacklevel=3
-            )
+            warnings.warn(f"Ignoring hdate='{kwargs['hdate']}' in HindcastReLabel", stacklevel=3)
             kwargs.pop("hdate")
 
         if "date" in kwargs:
-            warnings.warn(
-                f"Ignoring date='{kwargs['date']}' in HindcastReLabel", stacklevel=3
-            )
+            warnings.warn(f"Ignoring date='{kwargs['date']}' in HindcastReLabel", stacklevel=3)
             kwargs.pop("date")
 
         date = kwargs["template"]["date"]
         hdate = kwargs["template"]["hdate"]
 
         if hdate is not None:
             # Input was a hindcast
-            referenceDate = self.hindcast_reference_year * 10000 + date % 10000
+            referenceDate = (
+                self.hind_cast_reference_date
+                if self.hind_cast_reference_date is not None
+                else self.hindcast_reference_year * 10000 + date % 10000
+            )
             assert date == referenceDate, (
                 date,
                 referenceDate,
                 hdate,
                 kwargs["template"],
             )
             kwargs["referenceDate"] = referenceDate
             kwargs["hdate"] = hdate
         else:
-            referenceDate = self.hindcast_reference_year * 10000 + date % 10000
+            referenceDate = (
+                self.hind_cast_reference_date
+                if self.hind_cast_reference_date is not None
+                else self.hindcast_reference_year * 10000 + date % 10000
+            )
             kwargs["referenceDate"] = referenceDate
             kwargs["hdate"] = date
 
         kwargs.setdefault("check", True)
 
         return self.output.write(*args, **kwargs)
 
@@ -130,15 +132,15 @@
 
     def write(self, *args, **kwargs):
         pass
 
 
 def get_output(name, owner, *args, **kwargs):
     result = available_outputs()[name].load()(owner, *args, **kwargs)
-    if kwargs.get("hindcast_reference_year") is not None:
+    if kwargs.get("hindcast_reference_year") is not None or kwargs.get("hindcast_reference_date") is not None:
         result = HindcastReLabel(owner, result, **kwargs)
     return result
 
 
 def available_outputs():
     result = {}
     for e in entrypoints.get_group_all("ai_models.output"):
```

### Comparing `ai-models-0.5.3/ai_models/remote/api.py` & `ai_models-0.5.5/src/ai_models/remote/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import logging
 import os
 import sys
 import time
 from urllib.parse import urljoin
 
 import requests
-from multiurl import download, robust
+from multiurl import download
+from multiurl import robust
 from tqdm import tqdm
 
-from .config import API_URL, CONFIG_PATH, load_config
+from .config import API_URL
+from .config import CONFIG_PATH
+from .config import load_config
 
 LOG = logging.getLogger(__name__)
 
 
 class BearerAuth(requests.auth.AuthBase):
     def __init__(self, token):
         self.token = token
@@ -28,17 +31,15 @@
         input_file: str = None,
         output_file: str = "output.grib",
         url: str = None,
         token: str = None,
     ):
         config = load_config()
 
-        self.url = (
-            url or os.getenv("AI_MODELS_REMOTE_URL") or config.get("url") or API_URL
-        )
+        self.url = url or os.getenv("AI_MODELS_REMOTE_URL") or config.get("url") or API_URL
         if not self.url.endswith("/"):
             self.url += "/"
 
         self.token = token or os.getenv("AI_MODELS_REMOTE_TOKEN") or config.get("token")
 
         if not self.token:
             LOG.error(
@@ -122,21 +123,17 @@
 
         download(urljoin(self.url, data["href"]), target=self.output_file)
 
         LOG.debug("Result written to %s", self.output_file)
 
     def metadata(self, model, model_version, param) -> dict:
         if isinstance(param, str):
-            return self._request(
-                requests.get, f"metadata/{model}/{model_version}/{param}"
-            )
+            return self._request(requests.get, f"metadata/{model}/{model_version}/{param}")
         elif isinstance(param, (list, dict)):
-            return self._request(
-                requests.post, f"metadata/{model}/{model_version}", json=param
-            )
+            return self._request(requests.post, f"metadata/{model}/{model_version}", json=param)
         else:
             raise ValueError("param must be a string, list, or dict with 'param' key.")
 
     def models(self):
         results = self._request(requests.get, "models")
 
         if not isinstance(results, list):
```

### Comparing `ai-models-0.5.3/ai_models/remote/config.py` & `ai_models-0.5.5/src/ai_models/remote/config.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.3/ai_models/remote/model.py` & `ai_models-0.5.5/src/ai_models/remote/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,15 @@
         self.model = self.cfg["model"]
         self.model_version = self.cfg.get("model_version", "latest")
         self._param = {}
         self.api = RemoteAPI()
 
         if self.model not in self.api.models():
             LOG.error(f"Model '{self.model}' not available on remote server.")
-            LOG.error(
-                "Rerun the command with --models --remote to list available remote models."
-            )
+            LOG.error("Rerun the command with --models --remote to list available remote models.")
             sys.exit(1)
 
         self.load_parameters()
 
         super().__init__(**self.cfg)
 
     def __getattr__(self, name):
```

### Comparing `ai-models-0.5.3/ai_models/stepper.py` & `ai_models-0.5.5/src/ai_models/stepper.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.3/setup.py` & `ai_models-0.5.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,74 @@
 #!/usr/bin/env python
-# (C) Copyright 2023 ECMWF.
+# (C) Copyright 2024 ECMWF.
 #
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
-#
-
-
-import io
-import os
 
-import setuptools
+# https://packaging.python.org/en/latest/guides/writing-pyproject-toml/
 
+[build-system]
+requires = ["setuptools>=60", "setuptools-scm>=8.0"]
 
-def read(fname):
-    file_path = os.path.join(os.path.dirname(__file__), fname)
-    return io.open(file_path, encoding="utf-8").read()
-
-
-version = None
-for line in read("ai_models/__init__.py").split("\n"):
-    if line.startswith("__version__"):
-        version = line.split("=")[-1].strip()[1:-1]
-
-
-assert version
-
-
-setuptools.setup(
-    name="ai-models",
-    version=version,
-    description="A package to run AI weather models",
-    long_description=read("README.md"),
-    long_description_content_type="text/markdown",
-    author="European Centre for Medium-Range Weather Forecasts (ECMWF)",
-    author_email="software.support@ecmwf.int",
-    license="Apache License Version 2.0",
-    url="https://github.com/ecmwf-lab/ai-models",
-    packages=setuptools.find_packages(),
-    include_package_data=True,
-    install_requires=[
-        "entrypoints",
-        "requests",
-        "climetlab>=0.20.11",
-        "multiurl",
-        "ecmwflibs>=0.6.1",
-        "gputil",
-        "earthkit-meteo",
-        "pyyaml",
-        "tqdm",
-    ],
-    extras_require={
-        "provenance": [
-            "nvsmi",
-            "GitPython",
-        ]
-    },
-    zip_safe=True,
-    keywords="tool",
-    entry_points={
-        "console_scripts": ["ai-models=ai_models.__main__:main"],
-        "ai_models.input": [
-            "file=ai_models.inputs:FileInput",
-            "mars=ai_models.inputs:MarsInput",
-            "cds=ai_models.inputs:CdsInput",
-            "opendata=ai_models.inputs:OpenDataInput",
-        ],
-        "ai_models.output": [
-            "file=ai_models.outputs:FileOutput",
-            "none=ai_models.outputs:NoneOutput",
-        ],
-    },
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Programming Language :: Python :: Implementation :: PyPy",
-        "Operating System :: OS Independent",
-    ],
-)
+[project]
+description = "A package to run AI weather models."
+name = "ai-models"
+
+dynamic = ["version"]
+license = { file = "LICENSE" }
+requires-python = ">=3.9"
+
+authors = [
+    { name = "European Centre for Medium-Range Weather Forecasts (ECMWF)", email = "software.support@ecmwf.int" },
+]
+
+keywords = ["tools", "ai"]
+
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
+    "Operating System :: OS Independent",
+]
+
+dependencies = [
+    "entrypoints",
+    "requests",
+    "climetlab>=0.20.11",
+    "multiurl",
+    "ecmwflibs>=0.6.1",
+    "gputil",
+    "earthkit-meteo",
+    "pyyaml",
+    "tqdm",
+]
+
+
+[project.urls]
+Homepage = "https://github.com/ecmwf/ai-models/"
+Repository = "https://github.com/ecmwf/ai-models/"
+Issues = "https://github.com/ecmwf/ai-models/issues"
+
+[project.scripts]
+ai-models = "ai_models.__main__:main"
+
+[tool.setuptools_scm]
+version_file = "src/ai_models/_version.py"
+
+[project.entry-points."ai_models.input"]
+file = "ai_models.inputs:FileInput"
+mars = "ai_models.inputs:MarsInput"
+cds = "ai_models.inputs:CdsInput"
+opendata = "ai_models.inputs:OpenDataInput"
+
+[project.entry-points."ai_models.output"]
+file = "ai_models.outputs:FileOutput"
+none = "ai_models.outputs:NoneOutput"
```

