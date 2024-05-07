# Comparing `tmp/snakemake_executor_plugin_googlebatch-0.3.3.tar.gz` & `tmp/snakemake_executor_plugin_googlebatch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_executor_plugin_googlebatch-0.3.3.tar", max compression
+gzip compressed data, was "snakemake_executor_plugin_googlebatch-0.4.0.tar", max compression
```

## Comparing `snakemake_executor_plugin_googlebatch-0.3.3.tar` & `snakemake_executor_plugin_googlebatch-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1128 2024-04-06 03:27:06.200806 snakemake_executor_plugin_googlebatch-0.3.3/LICENSE
--rw-r--r--   0        0        0     1167 2024-04-06 03:27:06.200806 snakemake_executor_plugin_googlebatch-0.3.3/NOTICE
--rw-r--r--   0        0        0     1326 2024-04-06 03:27:06.200806 snakemake_executor_plugin_googlebatch-0.3.3/README.md
--rw-r--r--   0        0        0     1181 2024-04-06 03:27:06.200806 snakemake_executor_plugin_googlebatch-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     6275 2024-04-06 03:27:06.200806 snakemake_executor_plugin_googlebatch-0.3.3/snakemake_executor_plugin_googlebatch/__init__.py
--rw-r--r--   0        0        0     5638 2024-04-06 03:27:06.200806 snakemake_executor_plugin_googlebatch-0.3.3/snakemake_executor_plugin_googlebatch/command.py
--rw-r--r--   0        0        0    17517 2024-04-06 03:27:06.200806 snakemake_executor_plugin_googlebatch-0.3.3/snakemake_executor_plugin_googlebatch/executor.py
--rw-r--r--   0        0        0     5588 2024-04-06 03:27:06.200806 snakemake_executor_plugin_googlebatch-0.3.3/snakemake_executor_plugin_googlebatch/snippet.py
--rw-r--r--   0        0        0      171 2024-04-06 03:27:06.200806 snakemake_executor_plugin_googlebatch-0.3.3/snakemake_executor_plugin_googlebatch/snippets/intel-mpi/include/paths.sh
--rw-r--r--   0        0        0      265 2024-04-06 03:27:06.200806 snakemake_executor_plugin_googlebatch-0.3.3/snakemake_executor_plugin_googlebatch/snippets/intel-mpi/run.sh
--rw-r--r--   0        0        0      447 2024-04-06 03:27:06.200806 snakemake_executor_plugin_googlebatch-0.3.3/snakemake_executor_plugin_googlebatch/snippets/intel-mpi/setup.sh
--rw-r--r--   0        0        0     1530 2024-04-06 03:27:06.200806 snakemake_executor_plugin_googlebatch-0.3.3/snakemake_executor_plugin_googlebatch/utils.py
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 snakemake_executor_plugin_googlebatch-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1128 2024-05-07 11:58:09.528417 snakemake_executor_plugin_googlebatch-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1167 2024-05-07 11:58:09.528417 snakemake_executor_plugin_googlebatch-0.4.0/NOTICE
+-rw-r--r--   0        0        0     1326 2024-05-07 11:58:09.528417 snakemake_executor_plugin_googlebatch-0.4.0/README.md
+-rw-r--r--   0        0        0     1181 2024-05-07 11:58:09.532418 snakemake_executor_plugin_googlebatch-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7003 2024-05-07 11:58:09.532418 snakemake_executor_plugin_googlebatch-0.4.0/snakemake_executor_plugin_googlebatch/__init__.py
+-rw-r--r--   0        0        0     5562 2024-05-07 11:58:09.532418 snakemake_executor_plugin_googlebatch-0.4.0/snakemake_executor_plugin_googlebatch/command.py
+-rw-r--r--   0        0        0    19389 2024-05-07 11:58:09.532418 snakemake_executor_plugin_googlebatch-0.4.0/snakemake_executor_plugin_googlebatch/executor.py
+-rw-r--r--   0        0        0     5492 2024-05-07 11:58:09.532418 snakemake_executor_plugin_googlebatch-0.4.0/snakemake_executor_plugin_googlebatch/snippet.py
+-rw-r--r--   0        0        0      171 2024-05-07 11:58:09.532418 snakemake_executor_plugin_googlebatch-0.4.0/snakemake_executor_plugin_googlebatch/snippets/intel-mpi/include/paths.sh
+-rw-r--r--   0        0        0      265 2024-05-07 11:58:09.532418 snakemake_executor_plugin_googlebatch-0.4.0/snakemake_executor_plugin_googlebatch/snippets/intel-mpi/run.sh
+-rw-r--r--   0        0        0      447 2024-05-07 11:58:09.532418 snakemake_executor_plugin_googlebatch-0.4.0/snakemake_executor_plugin_googlebatch/snippets/intel-mpi/setup.sh
+-rw-r--r--   0        0        0     1530 2024-05-07 11:58:09.532418 snakemake_executor_plugin_googlebatch-0.4.0/snakemake_executor_plugin_googlebatch/utils.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 snakemake_executor_plugin_googlebatch-0.4.0/PKG-INFO
```

### Comparing `snakemake_executor_plugin_googlebatch-0.3.3/LICENSE` & `snakemake_executor_plugin_googlebatch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_googlebatch-0.3.3/NOTICE` & `snakemake_executor_plugin_googlebatch-0.4.0/NOTICE`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_googlebatch-0.3.3/README.md` & `snakemake_executor_plugin_googlebatch-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_googlebatch-0.3.3/pyproject.toml` & `snakemake_executor_plugin_googlebatch-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-executor-plugin-googlebatch"
-version = "0.3.3"
+version = "0.4.0"
 description = ""
 authors = [
     "Vanessa Sochat <sochat1@llnl.gov>",
     "Johannes Koester <johannes.koester@uni-due.de>"
 ]
 readme = "README.md"
 license = "MIT"
```

### Comparing `snakemake_executor_plugin_googlebatch-0.3.3/snakemake_executor_plugin_googlebatch/__init__.py` & `snakemake_executor_plugin_googlebatch-0.4.0/snakemake_executor_plugin_googlebatch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,41 @@
         metadata={
             "help": "The name of the Google Project region (e.g., us-central1)",
             "env_var": True,
             "required": True,
         },
     )
 
+    container: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": "A custom container for use with Google Batch COS",
+            "env_var": False,
+            "required": False,
+        },
+    )
+
+    docker_password: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": "A docker registry password for COS if credentials are required",
+            "env_var": True,
+            "required": False,
+        },
+    )
+
+    docker_username: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": "A docker registry username for COS if credentials are required",
+            "env_var": True,
+            "required": False,
+        },
+    )
+
     # mpitune configurations are validated on c2 and c2d instances only.
     machine_type: Optional[str] = field(
         default="c2-standard-4",
         metadata={
             "help": "Google Cloud machine type or VM (mpitune on c2 and c2d family)",
             "env_var": False,
             "required": False,
```

### Comparing `snakemake_executor_plugin_googlebatch-0.3.3/snakemake_executor_plugin_googlebatch/executor.py` & `snakemake_executor_plugin_googlebatch-0.4.0/snakemake_executor_plugin_googlebatch/executor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import uuid
 
-from typing import List, Generator
+from typing import List
 from snakemake_interface_common.exceptions import WorkflowError
 from snakemake_interface_executor_plugins.executors.base import SubmittedJobInfo
 from snakemake_interface_executor_plugins.executors.remote import RemoteExecutor
 from snakemake_interface_executor_plugins.jobs import (
     JobExecutorInterface,
 )
 import snakemake_executor_plugin_googlebatch.utils as utils
@@ -91,29 +91,63 @@
     def generate_jobid(self, job):
         """
         Generate a random jobid
         """
         uid = str(uuid.uuid4())
         return job.name.replace("_", "-") + "-" + uid[0:6]
 
-    def validate(self, job):
+    def get_container(self, job, entrypoint=None, commands=None):
         """
-        Ensure the choices of arguments make sense.
+        Get a container, if batch-cos is defined.
         """
-        container = self.get_container(job)
         family = self.get_param(job, "image_family")
+        if "batch-cos" not in family:
+            return
+
+        # Default entrypoint assumes the setup wrote our command here
+        if entrypoint is None:
+            entrypoint = "/bin/bash"
+        if commands is None:
+            commands = ["/tmp/workdir/entrypoint.sh"]
+
+        # We use the default snakemake image or the container, but also
+        # honor a googlebatch_container in case it is distinct
+        image = self.workflow.remote_execution_settings.container_image
+        image = self.get_param(job, "container") or image
+        container = batch_v1.Runnable.Container()
+        container.image_uri = image
+
+        # This is written by writer.setup() for COS
+        container.entrypoint = entrypoint
+        container.commands = commands
+
+        # This will ensure the Snakefile is in the PWD of the COS container
+        container.volumes = ["/tmp/workdir:/tmp/workdir"]
+        container.options = (
+            "--network host --workdir /tmp/workdir -e PYTHONUNBUFFERED=1"
+        )
+
+        username = self.get_param(job, "docker_username")
+        password = self.get_param(job, "docker_password")
 
-        # We can't take a custom container if batch-cos is not set
-        # We only give a warning here in case it's a one-off setting
-        # https://cloud.google.com/batch/docs/vm-os-environment-overview
-        if "batch-cos" not in family and container:
-            self.logger.warning(
-                f"Job {job} has container without image_family batch-cos*."
+        # Both are required
+        if (username and not password) or (password and not username):
+            raise WorkflowError(
+                "docker username and password are required if one is provided"
             )
 
+        if username and password:
+            container.username = username
+            container.password = password
+
+        # Not sure if we want to add this
+        # https://github.com/googleapis/googleapis/blob/master/google/cloud/batch/v1/task.proto#L230-L234
+        # enable_image_streaming true
+        return container
+
     def is_preemptible(self, job):
         """
         Determine if a job is preemptible.
 
         The logic for determining if the set is valid should belong upstream.
         """
         is_p = self.workflow.remote_execution_settings.preemptible_rules.is_preemptible
@@ -124,26 +158,28 @@
         return preemptible
 
     def get_command_writer(self, job):
         """
         Get a command writer for a job.
         """
         family = self.get_param(job, "image_family")
-        container = self.workflow.remote_execution_settings.container_image
         command = self.format_job_exec(job)
         snakefile = self.read_snakefile()
 
         # Any custom snippets
         snippets = self.get_param(job, "snippets")
 
+        snakefile_path = "./Snakefile"
+        if "batch-cos" in family:
+            snakefile_path = "/tmp/workdir/Snakefile"
         return cmdutil.get_writer(family)(
             command=command,
-            container=container,
             snakefile=snakefile,
             snippets=snippets,
+            snakefile_path=snakefile_path,
             settings=self.workflow.executor_settings,
             resources=job.resources,
         )
 
     def run_job(self, job: JobExecutorInterface):
         """
         Run the Google Batch job.
@@ -163,28 +199,39 @@
         writer = self.get_command_writer(job)
 
         # Setup command
         setup_command = writer.setup()
         self.logger.info("\n🌟️ Setup Command:")
         print(setup_command)
 
-        pre_commands = []
-
-        # Run command
-        run_command = writer.run(pre_commands)
-        self.logger.info("\n🐍️ Snakemake Command:")
-        print(run_command)
-
         # Add environment variables to the task
         envars = self.workflow.spawned_job_args_factory.envvars()
 
         # A single runnable to execute snakemake
         runnable = batch_v1.Runnable()
-        runnable.script = batch_v1.Runnable.Script()
-        runnable.script.text = run_command
+
+        # If we have a container, add it - the script isn't used
+        container = self.get_container(job)
+        if container is not None:
+            runnable.container = container
+            snakefile_text = writer.write_snakefile()
+        else:
+            # Run command (not used for COS)
+            run_command = writer.run()
+            self.logger.info("\n🐍️ Snakemake Command:")
+            print(run_command)
+
+            runnable.script = batch_v1.Runnable.Script()
+            runnable.script.text = run_command
+            snakefile_text = writer.write_snakefile()
+
+        # Runnable to write Snakefile on the host
+        snakefile_step = batch_v1.Runnable()
+        snakefile_step.script = batch_v1.Runnable.Script()
+        snakefile_step.script.text = snakefile_text
 
         # Note that secret variables seem to require some
         # extra secret API enabled
         runnable.environment.variables = envars
 
         # Snakemake setup must finish before snakemake is run
         setup = batch_v1.Runnable()
@@ -194,15 +241,15 @@
         # Placement policy
         # https://cloud.google.com/python/docs/reference/batch/latest/google.cloud.batch_v1.types.AllocationPolicy.PlacementPolicy
 
         # This will ensure all nodes finish first
         barrier = batch_v1.Runnable()
         barrier.barrier = batch_v1.Runnable.Barrier()
         barrier.barrier.name = "wait-for-setup"
-        task.runnables = [setup, barrier, runnable]
+        task.runnables = [setup, snakefile_step, barrier, runnable]
 
         # Are we adding storage?
         self.add_storage(job, task)
 
         # We can specify what resources are requested by each task.
         task.compute_resource = self.get_task_resources(job)
 
@@ -239,14 +286,15 @@
         create_request = batch_v1.CreateJobRequest()
         create_request.job = batchjob
         create_request.job_id = self.generate_jobid(job)
 
         # The job's parent is the region in which the job will run
         create_request.parent = self.project_parent(job)
         createdjob = self.batch.create_job(create_request)
+        print(createdjob)
 
         # Save aux metadata
         # Last seen will hold the timestamp of last recorded status
         aux = {"batch_job": createdjob, "logfile": logfile, "last_seen": None}
 
         # Record job info - the name is what we use to get a status later
         self.report_job_submission(
@@ -396,17 +444,15 @@
     def get_snakefile(self):
         """
         Use a Snakefile in the present working directory since we write it.
         """
         assert os.path.exists(self.workflow.main_snakefile)
         return os.path.relpath(self.workflow.main_snakefile, os.getcwd())
 
-    async def check_active_jobs(
-        self, active_jobs: List[SubmittedJobInfo]
-    ) -> Generator[SubmittedJobInfo, None, None]:
+    async def check_active_jobs(self, active_jobs: List[SubmittedJobInfo]):
         """
         Check the status of active jobs.
         """
         # Loop through active jobs and act on status
         for j in active_jobs:
             jobid = j.external_jobid
             request = batch_v1.GetJobRequest(name=jobid)
@@ -416,14 +462,15 @@
             last_seen = j.aux["last_seen"]
 
             try:
                 response = self.batch.get_job(request=request)
             except DeadlineExceeded:
                 msg = f"Google Batch job '{j.external_jobid}' exceeded deadline. "
                 self.report_job_error(j, msg=msg, aux_logs=aux_logs)
+                yield j
 
             self.logger.info(f"Job {jobid} has state {response.status.state.name}")
             for event in response.status.status_events:
                 if not last_seen or event.event_time.nanosecond > last_seen:
                     self.logger.info(f"{event.type_}: {event.description}")
                     last_seen = event.event_time.nanosecond
```

### Comparing `snakemake_executor_plugin_googlebatch-0.3.3/snakemake_executor_plugin_googlebatch/snippet.py` & `snakemake_executor_plugin_googlebatch-0.4.0/snakemake_executor_plugin_googlebatch/snippet.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,39 +33,37 @@
         self.has_run_command_snippet = False
         self.snippets = []
         self.settings = settings
         self.resources = resources
         self.load(spec)
         self.parse()
 
-    def render_setup(self, command, container):
+    def render_setup(self, command):
         """
         Render snippets into a chunk for the setup.
         """
         render = ""
         for snippet in self.snippets:
             render += snippet.render_setup(
                 settings=self.settings,
                 resources=self.resources,
                 command=command,
-                container=container,
             )
         return render
 
-    def render_run(self, command, container):
+    def render_run(self, command):
         """
         Render snippets into a chunk for the run.
         """
         render = ""
         for snippet in self.snippets:
             render += snippet.render_run(
                 settings=self.settings,
                 resources=self.resources,
                 command=command,
-                container=container,
             )
         return render
 
     def load(self, spec):
         """
         Load a spec for one or more snippets.
         """
```

### Comparing `snakemake_executor_plugin_googlebatch-0.3.3/snakemake_executor_plugin_googlebatch/utils.py` & `snakemake_executor_plugin_googlebatch-0.4.0/snakemake_executor_plugin_googlebatch/utils.py`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_googlebatch-0.3.3/PKG-INFO` & `snakemake_executor_plugin_googlebatch-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-executor-plugin-googlebatch
-Version: 0.3.3
+Version: 0.4.0
 Summary: 
 Home-page: https://github.com/snakemake/snakemake-executor-plugin-googlebatch
 License: MIT
 Keywords: snakemake,plugin,executor,cloud,google-batch
 Author: Vanessa Sochat
 Author-email: sochat1@llnl.gov
 Requires-Python: >=3.11,<4.0
```

