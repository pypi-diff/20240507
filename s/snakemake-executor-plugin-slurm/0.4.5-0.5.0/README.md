# Comparing `tmp/snakemake_executor_plugin_slurm-0.4.5.tar.gz` & `tmp/snakemake_executor_plugin_slurm-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_executor_plugin_slurm-0.4.5.tar", max compression
+gzip compressed data, was "snakemake_executor_plugin_slurm-0.5.0.tar", max compression
```

## Comparing `snakemake_executor_plugin_slurm-0.4.5.tar` & `snakemake_executor_plugin_slurm-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2024-04-17 12:12:52.719136 snakemake_executor_plugin_slurm-0.4.5/LICENSE
--rw-r--r--   0        0        0      319 2024-04-17 12:12:52.719136 snakemake_executor_plugin_slurm-0.4.5/README.md
--rw-r--r--   0        0        0     1151 2024-04-17 12:12:52.719136 snakemake_executor_plugin_slurm-0.4.5/pyproject.toml
--rw-r--r--   0        0        0    20094 2024-04-17 12:12:52.719136 snakemake_executor_plugin_slurm-0.4.5/snakemake_executor_plugin_slurm/__init__.py
--rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 snakemake_executor_plugin_slurm-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-07 18:57:25.612998 snakemake_executor_plugin_slurm-0.5.0/LICENSE
+-rw-r--r--   0        0        0      319 2024-05-07 18:57:25.612998 snakemake_executor_plugin_slurm-0.5.0/README.md
+-rw-r--r--   0        0        0     1151 2024-05-07 18:57:25.612998 snakemake_executor_plugin_slurm-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    20257 2024-05-07 18:57:25.612998 snakemake_executor_plugin_slurm-0.5.0/snakemake_executor_plugin_slurm/__init__.py
+-rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 snakemake_executor_plugin_slurm-0.5.0/PKG-INFO
```

### Comparing `snakemake_executor_plugin_slurm-0.4.5/LICENSE` & `snakemake_executor_plugin_slurm-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_slurm-0.4.5/pyproject.toml` & `snakemake_executor_plugin_slurm-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-executor-plugin-slurm"
-version = "0.4.5"
+version = "0.5.0"
 description = "A Snakemake executor plugin for submitting jobs to a SLURM cluster."
 authors = [
     "Christian Meesters <meesters@uni-mainz.de>",
     "David Lähnemann <david.laehnemann@dkfz-heidelberg.de>",
     "Johannes Koester <johannes.koester@uni-due.de>",
 ]
 readme = "README.md"
```

### Comparing `snakemake_executor_plugin_slurm-0.4.5/snakemake_executor_plugin_slurm/__init__.py` & `snakemake_executor_plugin_slurm-0.5.0/snakemake_executor_plugin_slurm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,17 +85,21 @@
             "happy. Otherwise we get silent fails without logfiles being created."
         )
         os.makedirs(logdir, exist_ok=True)
 
         # generic part of a submission string:
         # we use a run_uuid as the job-name, to allow `--name`-based
         # filtering in the job status checks (`sacct --name` and `squeue --name`)
+        if wildcard_str == "":
+            comment_str = f"rule_{job.name}"
+        else:
+            comment_str = f"rule_{job.name}_wildcards_{wildcard_str}"
         call = (
             f"sbatch --job-name {self.run_uuid} --output {slurm_logfile} --export=ALL "
-            f"--comment {job.name}"
+            f"--comment {comment_str}"
         )
 
         call += self.get_account_arg(job)
         call += self.get_partition_arg(job)
 
         if job.resources.get("runtime"):
             call += f" -t {job.resources.runtime}"
```

### Comparing `snakemake_executor_plugin_slurm-0.4.5/PKG-INFO` & `snakemake_executor_plugin_slurm-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-executor-plugin-slurm
-Version: 0.4.5
+Version: 0.5.0
 Summary: A Snakemake executor plugin for submitting jobs to a SLURM cluster.
 Home-page: https://github.com/snakemake/snakemake-executor-plugin-slurm
 License: MIT
 Keywords: snakemake,plugin,executor,cluster,slurm
 Author: Christian Meesters
 Author-email: meesters@uni-mainz.de
 Requires-Python: >=3.11,<4.0
```

