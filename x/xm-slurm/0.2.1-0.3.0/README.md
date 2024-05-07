# Comparing `tmp/xm_slurm-0.2.1-py3-none-any.whl.zip` & `tmp/xm_slurm-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,38 +1,40 @@
-Zip file size: 49214 bytes, number of entries: 36
--rw-r--r--  2.0 unx      903 b- defN 16-Jan-01 00:00 xm_slurm-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 xm_slurm-0.2.1.dist-info/WHEEL
+Zip file size: 51819 bytes, number of entries: 38
+-rw-r--r--  2.0 unx      903 b- defN 16-Jan-01 00:00 xm_slurm-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 xm_slurm-0.3.0.dist-info/WHEEL
 -rw-r--r--  2.0 unx     1019 b- defN 16-Jan-01 00:00 xm_slurm/__init__.py
--rw-r--r--  2.0 unx     9105 b- defN 16-Jan-01 00:00 xm_slurm/api.py
+-rw-r--r--  2.0 unx     9533 b- defN 16-Jan-01 00:00 xm_slurm/api.py
 -rw-r--r--  2.0 unx     4379 b- defN 16-Jan-01 00:00 xm_slurm/batching.py
--rw-r--r--  2.0 unx     3394 b- defN 16-Jan-01 00:00 xm_slurm/config.py
+-rw-r--r--  2.0 unx     4955 b- defN 16-Jan-01 00:00 xm_slurm/config.py
 -rw-r--r--  2.0 unx       54 b- defN 16-Jan-01 00:00 xm_slurm/console.py
+-rw-r--r--  2.0 unx     1600 b- defN 16-Jan-01 00:00 xm_slurm/contrib/clusters/__init__.py
+-rw-r--r--  2.0 unx     5201 b- defN 16-Jan-01 00:00 xm_slurm/contrib/clusters/drac.py
 -rw-r--r--  2.0 unx     5762 b- defN 16-Jan-01 00:00 xm_slurm/executables.py
--rw-r--r--  2.0 unx    18847 b- defN 16-Jan-01 00:00 xm_slurm/execution.py
+-rw-r--r--  2.0 unx    17998 b- defN 16-Jan-01 00:00 xm_slurm/execution.py
 -rw-r--r--  2.0 unx     4723 b- defN 16-Jan-01 00:00 xm_slurm/executors.py
--rw-r--r--  2.0 unx    25033 b- defN 16-Jan-01 00:00 xm_slurm/experiment.py
+-rw-r--r--  2.0 unx    25578 b- defN 16-Jan-01 00:00 xm_slurm/experiment.py
 -rw-r--r--  2.0 unx      482 b- defN 16-Jan-01 00:00 xm_slurm/job_blocks.py
 -rw-r--r--  2.0 unx    11216 b- defN 16-Jan-01 00:00 xm_slurm/packageables.py
 -rw-r--r--  2.0 unx      233 b- defN 16-Jan-01 00:00 xm_slurm/packaging/__init__.py
 -rw-r--r--  2.0 unx     2474 b- defN 16-Jan-01 00:00 xm_slurm/packaging/docker/__init__.py
 -rw-r--r--  2.0 unx     3830 b- defN 16-Jan-01 00:00 xm_slurm/packaging/docker/abc.py
 -rw-r--r--  2.0 unx    21300 b- defN 16-Jan-01 00:00 xm_slurm/packaging/docker/cloud.py
 -rw-r--r--  2.0 unx     8008 b- defN 16-Jan-01 00:00 xm_slurm/packaging/docker/local.py
 -rw-r--r--  2.0 unx     1148 b- defN 16-Jan-01 00:00 xm_slurm/packaging/registry.py
 -rw-r--r--  2.0 unx     2033 b- defN 16-Jan-01 00:00 xm_slurm/packaging/router.py
 -rw-r--r--  2.0 unx     6219 b- defN 16-Jan-01 00:00 xm_slurm/packaging/utils.py
--rw-r--r--  2.0 unx     4342 b- defN 16-Jan-01 00:00 xm_slurm/resources.py
+-rw-r--r--  2.0 unx     4835 b- defN 16-Jan-01 00:00 xm_slurm/resources.py
 -rw-r--r--  2.0 unx     6653 b- defN 16-Jan-01 00:00 xm_slurm/status.py
 -rw-r--r--  2.0 unx     1313 b- defN 16-Jan-01 00:00 xm_slurm/templates/docker/docker-bake.hcl.j2
 -rw-r--r--  2.0 unx      716 b- defN 16-Jan-01 00:00 xm_slurm/templates/docker/mamba.Dockerfile
 -rw-r--r--  2.0 unx      748 b- defN 16-Jan-01 00:00 xm_slurm/templates/docker/pdm.Dockerfile
 -rw-r--r--  2.0 unx      738 b- defN 16-Jan-01 00:00 xm_slurm/templates/docker/python.Dockerfile
 -rw-r--r--  2.0 unx     1071 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/fragments/monitor.bash.j2
 -rw-r--r--  2.0 unx      814 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/fragments/proxy.bash.j2
 -rw-r--r--  2.0 unx      599 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/job-array.bash.j2
 -rw-r--r--  2.0 unx     1120 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/job-group.bash.j2
 -rw-r--r--  2.0 unx     1852 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/job.bash.j2
--rw-r--r--  2.0 unx     2884 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/runtimes/apptainer.bash.j2
--rw-r--r--  2.0 unx     1317 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/runtimes/podman.bash.j2
+-rw-r--r--  2.0 unx     3241 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/runtimes/apptainer.bash.j2
+-rw-r--r--  2.0 unx     1469 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/runtimes/podman.bash.j2
 -rw-r--r--  2.0 unx     1930 b- defN 16-Jan-01 00:00 xm_slurm/utils.py
-?rw-------  2.0 unx     3103 b- defN 16-Jan-01 00:00 xm_slurm-0.2.1.dist-info/RECORD
-36 files, 159452 bytes uncompressed, 44230 bytes compressed:  72.3%
+?rw-------  2.0 unx     3287 b- defN 16-Jan-01 00:00 xm_slurm-0.3.0.dist-info/RECORD
+38 files, 169124 bytes uncompressed, 46543 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: xm_slurm-0.2.1.dist-info/METADATA
+Filename: xm_slurm-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: xm_slurm-0.2.1.dist-info/WHEEL
+Filename: xm_slurm-0.3.0.dist-info/WHEEL
 Comment: 
 
 Filename: xm_slurm/__init__.py
 Comment: 
 
 Filename: xm_slurm/api.py
 Comment: 
@@ -15,14 +15,20 @@
 
 Filename: xm_slurm/config.py
 Comment: 
 
 Filename: xm_slurm/console.py
 Comment: 
 
+Filename: xm_slurm/contrib/clusters/__init__.py
+Comment: 
+
+Filename: xm_slurm/contrib/clusters/drac.py
+Comment: 
+
 Filename: xm_slurm/executables.py
 Comment: 
 
 Filename: xm_slurm/execution.py
 Comment: 
 
 Filename: xm_slurm/executors.py
@@ -99,11 +105,11 @@
 
 Filename: xm_slurm/templates/slurm/runtimes/podman.bash.j2
 Comment: 
 
 Filename: xm_slurm/utils.py
 Comment: 
 
-Filename: xm_slurm-0.2.1.dist-info/RECORD
+Filename: xm_slurm-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xm_slurm/api.py

```diff
@@ -1,9 +1,10 @@
 import dataclasses
 import functools
+import importlib.util
 import logging
 import os
 import time
 import typing
 from typing import Any
 
 logger = logging.getLogger(__name__)
@@ -97,27 +98,32 @@
     def insert_experiment_artifact(self, experiment_id: int, artifact: ArtifactModel) -> None:
         del experiment_id, artifact
         logger.debug("`insert_experiment_artifact` is not implemented without a storage backend.")
 
 
 class XManagerWebAPI(XManagerAPI):
     def __init__(self, base_url: str, token: str):
-        from xm_slurm_api_client import AuthenticatedClient
-        from xm_slurm_api_client import models as _models
+        if importlib.util.find_spec("xm_slurm_api_client") is None:
+            raise ImportError("xm_slurm_api_client not found.")
+
+        from xm_slurm_api_client import AuthenticatedClient  # type: ignore
+        from xm_slurm_api_client import models as _models  # type: ignore
 
         self.models = _models
         self.client = AuthenticatedClient(
             base_url,
             token=token,
             raise_on_unexpected_status=True,
             verify_ssl=False,
         )
 
     def get_experiment(self, xid: int) -> ExperimentModel:
-        from xm_slurm_api_client.api.experiment import get_experiment as _get_experiment
+        from xm_slurm_api_client.api.experiment import (  # type: ignore
+            get_experiment as _get_experiment,
+        )
 
         experiment: Any = _get_experiment.sync(xid, client=self.client)  # type: ignore
         wus = []
         for wu in experiment.work_units:
             jobs = []
             for job in wu.jobs:
                 jobs.append(SlurmJobModel(**job.dict()))
@@ -144,107 +150,112 @@
             note=experiment.note,
             tags=experiment.tags,
             work_units=wus,
             artifacts=artifacts,
         )
 
     def delete_experiment(self, experiment_id: int) -> None:
-        from xm_slurm_api_client.api.experiment import delete_experiment as _delete_experiment
+        from xm_slurm_api_client.api.experiment import (  # type: ignore
+            delete_experiment as _delete_experiment,
+        )
 
         _delete_experiment.sync(experiment_id, client=self.client)
 
     def insert_experiment(self, experiment: ExperimentPatchModel) -> int:
-        from xm_slurm_api_client.api.experiment import insert_experiment as _insert_experiment
+        from xm_slurm_api_client.api.experiment import (  # type: ignore
+            insert_experiment as _insert_experiment,
+        )
 
         assert experiment.title is not None, "Title must be set in the experiment model."
         assert (
             experiment.description is None and experiment.note is None and experiment.tags is None
         ), "Only title should be set in the experiment model."
         experiment_response = _insert_experiment.sync(
             client=self.client,
             body=self.models.Experiment(title=experiment.title),
         )
         return typing.cast(int, experiment_response["xid"])  # type: ignore
 
     def update_experiment(self, experiment_id: int, experiment_patch: ExperimentPatchModel) -> None:
-        from xm_slurm_api_client.api.experiment import update_experiment as _update_experiment
+        from xm_slurm_api_client.api.experiment import (  # type: ignore
+            update_experiment as _update_experiment,
+        )
 
         m = self.models.ExperimentPatch(**dataclasses.asdict(experiment_patch))
 
         _update_experiment.sync(
             experiment_id,
             client=self.client,
             body=self.models.ExperimentPatch(**dataclasses.asdict(experiment_patch)),
         )
 
     def insert_job(self, experiment_id: int, work_unit_id: int, job: SlurmJobModel) -> None:
-        from xm_slurm_api_client.api.job import insert_job as _insert_job
+        from xm_slurm_api_client.api.job import insert_job as _insert_job  # type: ignore
 
         _insert_job.sync(
             experiment_id,
             work_unit_id,
             client=self.client,
             body=self.models.SlurmJob(**dataclasses.asdict(job)),
         )
 
     def insert_work_unit(self, experiment_id: int, work_unit: WorkUnitPatchModel) -> None:
-        from xm_slurm_api_client.api.work_unit import insert_work_unit as _insert_work_unit
+        from xm_slurm_api_client.api.work_unit import (  # type: ignore
+            insert_work_unit as _insert_work_unit,
+        )
 
         _insert_work_unit.sync(
             experiment_id,
             client=self.client,
             body=self.models.WorkUnit(**dataclasses.asdict(work_unit)),
         )
 
     def delete_work_unit_artifact(self, experiment_id: int, work_unit_id: int, name: str) -> None:
-        from xm_slurm_api_client.api.artifact import (
+        from xm_slurm_api_client.api.artifact import (  # type: ignore
             delete_work_unit_artifact as _delete_work_unit_artifact,
         )
 
         _delete_work_unit_artifact.sync(experiment_id, work_unit_id, name, client=self.client)
 
     def insert_work_unit_artifact(
         self, experiment_id: int, work_unit_id: int, artifact: ArtifactModel
     ) -> None:
-        from xm_slurm_api_client.api.artifact import (
+        from xm_slurm_api_client.api.artifact import (  # type: ignore
             insert_work_unit_artifact as _insert_work_unit_artifact,
         )
 
         _insert_work_unit_artifact.sync(
             experiment_id,
             work_unit_id,
             client=self.client,
             body=self.models.Artifact(**dataclasses.asdict(artifact)),
         )
 
     def delete_experiment_artifact(self, experiment_id: int, name: str) -> None: ...
 
     def insert_experiment_artifact(self, experiment_id: int, artifact: ArtifactModel) -> None:
-        from xm_slurm_api_client.api.artifact import (
+        from xm_slurm_api_client.api.artifact import (  # type: ignore
             insert_experiment_artifact as _insert_experiment_artifact,
         )
 
         _insert_experiment_artifact.sync(
             experiment_id,
             client=self.client,
             body=self.models.Artifact(**dataclasses.asdict(artifact)),
         )
 
 
 @functools.cache
 def client() -> XManagerAPI:
-    try:
-        import xm_slurm_api_client  # noqa: F401
-    except ImportError:
-        logger.debug("xm_slurm_api_client not found... skipping logging to the API.")
-    else:
+    if importlib.util.find_spec("xm_slurm_api_client") is not None:
         if (base_url := os.environ.get("XM_SLURM_API_BASE_URL")) is not None and (
             token := os.environ.get("XM_SLURM_API_TOKEN")
         ) is not None:
             return XManagerWebAPI(base_url=base_url, token=token)
         else:
             logger.warn(
                 "XM_SLURM_API_BASE_URL and XM_SLURM_API_TOKEN not set. "
                 "Disabling XManager API client."
             )
 
+    logger.debug("xm_slurm_api_client not found... skipping logging to the API.")
     return XManagerAPI()
```

## xm_slurm/config.py

```diff
@@ -1,15 +1,16 @@
 import dataclasses
 import enum
 import functools
-import json
+import getpass
+import os
 import pathlib
-from typing import Literal, Mapping
+from typing import Literal, Mapping, NamedTuple
 
-import toml
+import asyncssh
 
 
 class ContainerRuntime(enum.Enum):
     """The container engine to use."""
 
     SINGULARITY = enum.auto()
     APPTAINER = enum.auto()
@@ -36,24 +37,25 @@
             return "docker"
         elif self is self.PODMAN:
             return "podman"
         else:
             raise NotImplementedError
 
 
-class JSONEncoder(json.JSONEncoder):
-    def default(self, obj):
-        if type(obj) is ContainerRuntime:
-            return {"__type__": "ContainerRuntime", "value": str(obj)}
-        return json.JSONEncoder.default(self, obj)
+class PublicKey(NamedTuple):
+    algorithm: str
+    key: str
 
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
 class SlurmClusterConfig:
+    name: str
+
     host: str
+    host_public_key: PublicKey | None = None
     user: str | None = None
     port: int | None = None
 
     # Job submission directory
     cwd: str | None = None
 
     # Additional scripting
@@ -69,25 +71,83 @@
     proxy: Literal["submission-host"] | str | None = None
 
     runtime: ContainerRuntime
 
     # Environment variables
     environment: Mapping[str, str] = dataclasses.field(default_factory=dict)
 
-    def to_json(self) -> str:
-        return json.dumps(dataclasses.asdict(self), cls=JSONEncoder)
+    # Mounts
+    mounts: Mapping[os.PathLike[str] | str, os.PathLike[str] | str] = dataclasses.field(
+        default_factory=dict
+    )
+
+    # Resource mapping
+    resources: Mapping[str, "xm_slurm.ResourceType"] = dataclasses.field(default_factory=dict)  # type: ignore # noqa: F821
+
+    def __post_init__(self) -> None:
+        for src, dst in self.mounts.items():
+            if not isinstance(src, (str, os.PathLike)):
+                raise TypeError(
+                    f"Mount source must be a string or path-like object, not {type(src)}"
+                )
+            if not isinstance(dst, (str, os.PathLike)):
+                raise TypeError(
+                    f"Mount destination must be a string or path-like object, not {type(dst)}"
+                )
+
+            if not pathlib.Path(src).is_absolute():
+                raise ValueError(f"Mount source must be an absolute path: {src}")
+            if not pathlib.Path(dst).is_absolute():
+                raise ValueError(f"Mount destination must be an absolute path: {dst}")
+
+    @functools.cached_property
+    def ssh_known_hosts(self) -> asyncssh.SSHKnownHosts | None:
+        if self.host_public_key is None:
+            return None
 
-    @classmethod
-    def from_json(cls, json_str: str) -> "SlurmClusterConfig":
-        def object_hook(tree):
-            if "__type__" in tree and tree["__type__"] == "ContainerRuntime":
-                return ContainerRuntime.from_string(tree["value"])
-            return tree
+        return asyncssh.import_known_hosts(
+            f"[{self.host}]:{self.port} {self.host_public_key.algorithm} {self.host_public_key.key}"
+        )
+
+    @functools.cached_property
+    def ssh_config(self) -> asyncssh.config.SSHConfig:
+        ssh_config_paths = []
+        if (ssh_config := pathlib.Path.home() / ".ssh" / "config").exists():
+            ssh_config_paths.append(ssh_config)
+        if (xm_ssh_config := os.environ.get("XM_SLURM_SSH_CONFIG")) and (
+            xm_ssh_config := pathlib.Path(xm_ssh_config).expanduser()
+        ).exists():
+            ssh_config_paths.append(xm_ssh_config)
+
+        config = asyncssh.config.SSHClientConfig.load(
+            None,
+            ssh_config_paths,
+            True,
+            getpass.getuser(),
+            self.user or (),
+            self.host or (),
+            self.port or (),
+        )
 
-        return cls(**json.loads(json_str, object_hook=object_hook))
+        if config.get("Hostname") is None:
+            raise RuntimeError(
+                f"Failed to parse hostname from host `{self.host}` using SSH configs: {', '.join(map(str, ssh_config_paths))}"
+            )
+        if config.get("User") is None:
+            raise RuntimeError(
+                f"Failed to parse user from SSH configs: {', '.join(map(str, ssh_config_paths))}"
+            )
+
+        return config
+
+    @functools.cached_property
+    def ssh_connection_options(self) -> asyncssh.SSHClientConnectionOptions:
+        options = asyncssh.SSHClientConnectionOptions(config=None)
+        options.prepare(last_config=self.ssh_config, known_hosts=self.ssh_known_hosts)
+        return options
 
     def __hash__(self):
         return hash((
             self.host,
             self.user,
             self.port,
             self.cwd,
@@ -96,29 +156,7 @@
             self.account,
             self.partition,
             self.qos,
             self.proxy,
             self.runtime,
             frozenset(self.environment.items()),
         ))
-
-
-@functools.cache
-def clusters(pyproject_path: pathlib.Path) -> list[SlurmClusterConfig]:
-    if not pyproject_path.exists():
-        raise RuntimeError(f"{pyproject_path} does not exist")
-
-    with pyproject_path.open("r") as fp:
-        config = functools.reduce(
-            lambda d, key: d.get(key, {}),
-            ["tool", "xmanager", "slurm"],
-            toml.load(fp),
-        )
-        if not config:
-            return []
-
-        clusters = []
-        for cluster in config.pop("clusters", []):
-            cluster["runtime"] = ContainerRuntime.from_string(cluster["runtime"])
-            clusters.append(SlurmClusterConfig(**config, **cluster))
-
-        return clusters
```

## xm_slurm/execution.py

```diff
@@ -1,29 +1,27 @@
 import asyncio
 import collections.abc
 import dataclasses
-import datetime as dt
 import functools
+import hashlib
 import logging
 import operator
 import re
 import shlex
 import typing
 from typing import Any, Mapping, Sequence
 
 import asyncssh
 import backoff
-import humanize
 import jinja2 as j2
 from asyncssh.auth import KbdIntPrompts, KbdIntResponse
 from asyncssh.misc import MaybeAwait
-from rich.table import Table
 from xmanager import xm
 
-from xm_slurm import batching, config, status, utils
+from xm_slurm import batching, config, executors, status
 from xm_slurm.console import console
 
 SlurmClusterConfig = config.SlurmClusterConfig
 ContainerRuntime = config.ContainerRuntime
 
 """
 === Runtime Configurations ===
@@ -65,38 +63,38 @@
     def kbdint_challenge_received(
         self, name: str, instructions: str, lang: str, prompts: KbdIntPrompts
     ) -> MaybeAwait[KbdIntResponse | None]:
         del name, instructions, lang, prompts
         return []
 
 
-def _group_by_cluster(
-    clusters: Sequence[SlurmClusterConfig], job_ids: Sequence[str]
-) -> dict[SlurmClusterConfig, list[str]]:
+def _group_by_ssh_options(
+    ssh_options: Sequence[asyncssh.SSHClientConnectionOptions], job_ids: Sequence[str]
+) -> dict[asyncssh.SSHClientConnectionOptions, list[str]]:
     jobs_by_cluster = collections.defaultdict(list)
-    for cluster, job_id in zip(clusters, job_ids):
-        jobs_by_cluster[cluster].append(job_id)
+    for options, job_id in zip(ssh_options, job_ids):
+        jobs_by_cluster[options].append(job_id)
     return jobs_by_cluster
 
 
 class _BatchedSlurmHandle:
     @functools.partial(
         batching.batch,
         max_batch_size=_BATCHED_BATCH_SIZE,
         batch_timeout=_BATCHED_TIMEOUT,
     )
     @staticmethod
     async def _batched_get_state(
-        clusters: Sequence[SlurmClusterConfig], job_ids: Sequence[str]
+        ssh_options: Sequence[asyncssh.SSHClientConnectionOptions], job_ids: Sequence[str]
     ) -> Sequence[status.SlurmJobState]:
         async def _get_state(
-            cluster: SlurmClusterConfig, job_ids: Sequence[str]
+            options: asyncssh.SSHClientConnectionOptions, job_ids: Sequence[str]
         ) -> Sequence[status.SlurmJobState]:
             result = await get_client().run(
-                cluster,
+                options,
                 [
                     "sacct",
                     "--jobs",
                     ",".join(job_ids),
                     "--format",
                     "JobID,State",
                     "--allocations",
@@ -121,51 +119,55 @@
                 # and it's an array job, then it's pending.
                 elif re.match(r"^\d+_\d+$", job_id) is not None:
                     job_states.append(status.SlurmJobState.PENDING)
                 else:
                     raise SlurmExecutionError(f"Failed to find job state info for {job_id}")
             return job_states
 
-        jobs_by_cluster = _group_by_cluster(clusters, job_ids)
+        jobs_by_cluster = _group_by_ssh_options(ssh_options, job_ids)
 
         job_states_per_cluster = await asyncio.gather(*[
-            _get_state(cluster, job_ids) for cluster, job_ids in jobs_by_cluster.items()
+            _get_state(options, job_ids) for options, job_ids in jobs_by_cluster.items()
         ])
-        job_states_by_cluster: dict[SlurmClusterConfig, dict[str, status.SlurmJobState]] = {}
-        for cluster, job_states in zip(clusters, job_states_per_cluster):
-            job_states_by_cluster[cluster] = dict(zip(jobs_by_cluster[cluster], job_states))
+        job_states_by_cluster: dict[
+            asyncssh.SSHClientConnectionOptions, dict[str, status.SlurmJobState]
+        ] = {}
+        for options, job_states in zip(ssh_options, job_states_per_cluster):
+            job_states_by_cluster[options] = dict(zip(jobs_by_cluster[options], job_states))
 
         job_states = []
-        for cluster, job_id in zip(clusters, job_ids):
-            job_states.append(job_states_by_cluster[cluster][job_id])
+        for options, job_id in zip(ssh_options, job_ids):
+            job_states.append(job_states_by_cluster[options][job_id])
         return job_states
 
     @functools.partial(
         batching.batch,
         max_batch_size=_BATCHED_BATCH_SIZE,
         batch_timeout=_BATCHED_TIMEOUT,
     )
     @staticmethod
     async def _batched_cancel(
-        clusters: Sequence[SlurmClusterConfig], job_ids: Sequence[str]
+        ssh_options: Sequence[asyncssh.SSHClientConnectionOptions], job_ids: Sequence[str]
     ) -> Sequence[None]:
-        async def _cancel(cluster: SlurmClusterConfig, job_ids: Sequence[str]) -> None:
-            await get_client().run(cluster, ["scancel", " ".join(job_ids)], check=True)
+        async def _cancel(
+            options: asyncssh.SSHClientConnectionOptions, job_ids: Sequence[str]
+        ) -> None:
+            await get_client().run(options, ["scancel", " ".join(job_ids)], check=True)
 
-        jobs_by_cluster = _group_by_cluster(clusters, job_ids)
+        jobs_by_cluster = _group_by_ssh_options(ssh_options, job_ids)
         return await asyncio.gather(*[
-            _cancel(cluster, job_ids) for cluster, job_ids in jobs_by_cluster.items()
+            _cancel(options, job_ids) for options, job_ids in jobs_by_cluster.items()
         ])
 
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
 class SlurmHandle(_BatchedSlurmHandle):
     """A handle for referring to the launched container."""
 
-    cluster: SlurmClusterConfig
+    ssh_connection_options: asyncssh.SSHClientConnectionOptions
     job_id: str
 
     def __post_init__(self):
         if re.match(r"^\d+(_\d+|\+\d+)?$", self.job_id) is None:
             raise ValueError(f"Invalid job ID: {self.job_id}")
 
     @backoff.on_predicate(
@@ -174,18 +176,18 @@
         jitter=None,
         interval=_POLL_INTERVAL,
     )
     async def wait(self) -> status.SlurmJobState:
         return await self.get_state()
 
     async def stop(self) -> None:
-        await self._batched_cancel(self.cluster, self.job_id)
+        await self._batched_cancel(self.ssh_connection_options, self.job_id)
 
     async def get_state(self) -> status.SlurmJobState:
-        return await self._batched_get_state(self.cluster, self.job_id)
+        return await self._batched_get_state(self.ssh_connection_options, self.job_id)
 
 
 @functools.cache
 def get_client() -> "Client":
     return Client()
 
 
@@ -211,60 +213,54 @@
     template_env.globals.update(runtime_template.module.__dict__)
 
     return template_env
 
 
 class Client:
     def __init__(self):
-        self._connections: dict[SlurmClusterConfig, asyncssh.SSHClientConnection] = {}
+        self._connections: dict[
+            asyncssh.SSHClientConnectionOptions, asyncssh.SSHClientConnection
+        ] = {}
         self._connection_lock = asyncio.Lock()
 
-        self._clusters = config.clusters(utils.find_project_root() / "pyproject.toml")
-
     @backoff.on_exception(backoff.expo, asyncssh.Error, max_tries=5, max_time=60.0)
     async def _setup_remote_connection(self, conn: asyncssh.SSHClientConnection) -> None:
         # Make sure the xm-slurm state directory exists
         await conn.run("mkdir -p ~/.local/state/xm-slurm", check=True)
 
-    async def connection(self, cluster: SlurmClusterConfig) -> asyncssh.SSHClientConnection:
-        if cluster not in self._connections:
+    async def connection(
+        self,
+        options: asyncssh.SSHClientConnectionOptions,
+    ) -> asyncssh.SSHClientConnection:
+        if options not in self._connections:
             async with self._connection_lock:
                 try:
-                    conn, _ = await asyncssh.create_connection(
-                        NoKBAuthSSHClient,
-                        host=cluster.host,
-                        port=cluster.port or (),
-                        username=cluster.user,
-                    )
+                    conn, _ = await asyncssh.create_connection(NoKBAuthSSHClient, options=options)
                     await self._setup_remote_connection(conn)
-                    self._connections[cluster] = conn
+                    self._connections[options] = conn
                 except asyncssh.misc.PermissionDenied as ex:
-                    raise RuntimeError(f"Permission denied connecting to {cluster.host}") from ex
-        return self._connections[cluster]
+                    raise RuntimeError(f"Permission denied connecting to {options.host}") from ex
+        return self._connections[options]
 
     @backoff.on_exception(backoff.expo, asyncssh.Error, max_tries=5, max_time=60.0)
     async def run(
         self,
-        cluster: SlurmClusterConfig,
+        options: asyncssh.SSHClientConnectionOptions,
         command: xm.SequentialArgs | str | Sequence[str],
         *,
         check: bool = False,
         timeout: float | None = None,
     ) -> asyncssh.SSHCompletedProcess:
-        client = await self.connection(cluster)
+        client = await self.connection(options)
         if isinstance(command, xm.SequentialArgs):
             command = command.to_list()
         if not isinstance(command, str) and isinstance(command, collections.abc.Sequence):
             command = shlex.join(command)
         assert isinstance(command, str)
-        if cluster.cwd:
-            logging.debug("Running command on %s: %s from %s", cluster.host, command, cluster.cwd)
-            command = f"cd {cluster.cwd} && {command}"
-        else:
-            logging.debug("Running command on %s: %s", cluster.host, command)
+        logging.debug("Running command on %s: %s", options.host, command)
 
         return await client.run(command, check=check, timeout=timeout)
 
     async def template(
         self,
         *,
         job: xm.Job | xm.JobGroup,
@@ -335,154 +331,97 @@
                     env_vars=env_vars,
                     experiment_id=experiment_id,
                     identity=identity,
                 )
             case _:
                 raise ValueError(f"Unsupported job type: {type(job)}")
 
-    async def _select_cluster(
-        self,
-        *,
-        job: xm.Job | xm.JobGroup,
-        args: Mapping[str, Any] | Sequence[Mapping[str, Any]] | None,
-        experiment_id: int,
-        identity: str | None,
-    ) -> tuple[SlurmClusterConfig, dt.datetime | BaseException]:
-        assert len(self._clusters) > 0, "Need at least one cluster"
-
-        async def _cluster_eta(cluster: SlurmClusterConfig) -> dt.datetime:
-            template = await self.template(
-                job=job,
-                cluster=cluster,
-                args=args,
-                experiment_id=experiment_id,
-                identity=identity,
-            )
-            command = f"sbatch --test-only <<'SBATCH_EOF'\n{template}\nSBATCH_EOF"
-            result = await self.run(cluster, command)
-            if result.returncode != 0:
-                raise SlurmExecutionError(
-                    f"Failed to test job on host {cluster.host}.\n{result.stderr}"
-                )
-            assert result.stderr is not None and isinstance(result.stderr, str)
-            if match := re.search(r"(\d{4}-\d{2}-\d{2}T\d{2}:\d{1,2}:\d{1,2})", result.stderr):
-                return dt.datetime.strptime(match.group(1), "%Y-%m-%dT%H:%M:%S")
-            raise SlurmExecutionError(
-                f"Failed to parse job ETA on cluster {cluster.host}\n{result.stderr}"
-            )
-
-        now = dt.datetime.now()
-        etas = await asyncio.gather(
-            *[_cluster_eta(cluster) for cluster in self._clusters],
-            return_exceptions=True,
-        )
-        sorted_cluster_etas: list[tuple[SlurmClusterConfig, dt.datetime | BaseException]] = list(
-            sorted(
-                zip(self._clusters, etas),
-                key=lambda x: dt.datetime.max if isinstance(x[1], Exception) else x[1],  # type: ignore
-            )
-        )
-
-        table = Table(title="Cluster ETAs")
-        table.add_column("Cluster", justify="right", style="cyan", no_wrap=True)
-        table.add_column("Account", justify="center", style="cyan", no_wrap=True)
-        table.add_column("Partition", justify="center", style="cyan", no_wrap=True)
-        table.add_column("QoS", justify="center", style="cyan", no_wrap=True)
-        table.add_column("Scheduled Time", style="bold magenta")
-        for cluster, eta_or_exception in sorted_cluster_etas:
-            if isinstance(eta_or_exception, SlurmExecutionError):
-                logging.warning(str(eta_or_exception))
-                continue
-            elif isinstance(eta_or_exception, Exception):
-                raise eta_or_exception
-
-            table.add_row(
-                cluster.host,
-                cluster.account,
-                cluster.partition,
-                cluster.qos,
-                humanize.naturaltime(eta_or_exception, when=now),
-            )
-        console.print(table)
-
-        return sorted_cluster_etas[0]
-
     @typing.overload
     async def launch(
         self,
         *,
+        cluster: SlurmClusterConfig,
         job: xm.Job | xm.JobGroup,
         args: Mapping[str, Any] | None,
         experiment_id: int,
         identity: str | None = ...,
     ) -> SlurmHandle: ...
 
     @typing.overload
     async def launch(
         self,
         *,
+        cluster: SlurmClusterConfig,
         job: xm.Job | xm.JobGroup,
         args: Sequence[Mapping[str, Any]],
         experiment_id: int,
         identity: str | None = ...,
     ) -> Sequence[SlurmHandle]: ...
 
     async def launch(
         self,
         *,
+        cluster: SlurmClusterConfig,
         job: xm.Job | xm.JobGroup,
         args: Mapping[str, Any] | Sequence[Mapping[str, Any]] | None,
         experiment_id: int,
         identity: str | None = None,
     ) -> SlurmHandle | Sequence[SlurmHandle]:
-        # Select cluster to run on
-        cluster, eta_or_exception = await self._select_cluster(
-            job=job,
-            args=args,
-            experiment_id=experiment_id,
-            identity=identity,
-        )
-
         # Construct template
         template = await self.template(
             job=job,
             cluster=cluster,
             args=args,
             experiment_id=experiment_id,
             identity=identity,
         )
         logging.debug("Slurm submission script:\n%s", template)
 
+        # Hash submission script
+        template_hash = hashlib.blake2s(template.encode()).hexdigest()[:8]
+
+        conn = await self.connection(cluster.ssh_connection_options)
+        async with conn.start_sftp_client() as sftp:
+            # Write the submission script to the cluster
+            # TODO(jfarebro): SHOULD FIND A WAY TO GET THE HOME DIRECTORY
+            # INSTEAD OF ASSUMING SFTP PUTS US IN THE HOME DIRECTORY
+            await sftp.makedirs(f".local/state/xm-slurm/{experiment_id}", exist_ok=True)
+            async with sftp.open(
+                f".local/state/xm-slurm/{experiment_id}/submission-script-{template_hash}.sh", "w"
+            ) as fp:
+                await fp.write(template)
+
         # Construct and run command on the cluster
-        command = f"sbatch --chdir $HOME/.local/state/xm-slurm/{experiment_id} --parsable <<'SBATCH_EOF'\n{template}\nSBATCH_EOF"
-        result = await self.run(cluster, command)
+        command = f"sbatch --chdir .local/state/xm-slurm/{experiment_id} --parsable submission-script-{template_hash}.sh"
+        result = await self.run(cluster.ssh_connection_options, command)
         if result.returncode != 0:
             raise RuntimeError(f"Failed to schedule job on {cluster.host}: {result.stderr}")
 
         assert isinstance(result.stdout, str)
         slurm_job_id, *_ = result.stdout.split(",")
         slurm_job_id = slurm_job_id.strip()
 
-        # If eta_or_exception is an exception, we have already logged the warning
-        # se we don't need to do it again here.
-        # TODO: Move this into the resource selector.
-        if isinstance(eta_or_exception, dt.datetime):
-            console.print(
-                f"[magenta]:rocket: Job [cyan]{slurm_job_id}[/cyan] will be launched on "
-                f"[cyan]{cluster.host}[/cyan] "
-                f"{humanize.naturaltime(max(eta_or_exception, dt.datetime.now()), when=dt.datetime.now())}."
-            )
+        console.log(
+            f"[magenta]:rocket: Job [cyan]{slurm_job_id}[/cyan] will be launched on "
+            f"[cyan]{cluster.name}[/cyan] "
+        )
 
         if isinstance(job, xm.Job) and isinstance(args, collections.abc.Sequence):
             return [
-                SlurmHandle(cluster=cluster, job_id=f"{slurm_job_id}_{array_index}")
+                SlurmHandle(
+                    ssh_connection_options=cluster.ssh_connection_options,
+                    job_id=f"{slurm_job_id}_{array_index}",
+                )
                 for array_index in range(len(args))
             ]
 
-        return SlurmHandle(cluster=cluster, job_id=slurm_job_id)
+        return SlurmHandle(
+            ssh_connection_options=cluster.ssh_connection_options,
+            job_id=slurm_job_id,
+        )
 
 
 @typing.overload
 async def launch(
     *,
     job: xm.Job | xm.JobGroup,
     args: Mapping[str, Any],
@@ -504,13 +443,49 @@
 async def launch(
     *,
     job: xm.Job | xm.JobGroup,
     args: Mapping[str, Any] | Sequence[Mapping[str, Any]],
     experiment_id: int,
     identity: str | None = None,
 ) -> SlurmHandle | Sequence[SlurmHandle]:
-    return await get_client().launch(
-        job=job,
-        args=args,
-        experiment_id=experiment_id,
-        identity=identity,
-    )
+    match job:
+        case xm.Job():
+            if not isinstance(job.executor, executors.Slurm):
+                raise ValueError("Job must have a Slurm executor")
+            job_requirements = job.executor.requirements
+            cluster = job_requirements.cluster
+            if cluster is None:
+                raise ValueError("Job must have a cluster requirement")
+
+            return await get_client().launch(
+                cluster=cluster,
+                job=job,
+                args=args,
+                experiment_id=experiment_id,
+                identity=identity,
+            )
+        case xm.JobGroup() as job_group:
+            job_group_executors = set()
+            job_group_clusters = set()
+            for job_item in job_group.jobs.values():
+                if not isinstance(job_item, xm.Job):
+                    raise ValueError("Job group must contain only jobs")
+                if not isinstance(job_item.executor, executors.Slurm):
+                    raise ValueError("Job must have a Slurm executor")
+                if job_item.executor.requirements.cluster is None:
+                    raise ValueError("Job must have a cluster requirement")
+                job_group_clusters.add(job_item.executor.requirements.cluster)
+                job_group_executors.add(id(job_item.executor))
+            if len(job_group_executors) != 1:
+                raise ValueError("Job group must have the same executor for all jobs")
+            if len(job_group_clusters) != 1:
+                raise ValueError("Job group must have the same cluster for all jobs")
+
+            return await get_client().launch(
+                cluster=job_group_clusters.pop(),
+                job=job,
+                args=args,
+                experiment_id=experiment_id,
+                identity=identity,
+            )
+        case _:
+            raise ValueError("Unsupported job type")
```

## xm_slurm/experiment.py

```diff
@@ -9,15 +9,15 @@
 import typing
 from concurrent import futures
 from typing import Any, Awaitable, Callable, Mapping, MutableSet, Sequence
 
 from xmanager import xm
 from xmanager.xm import async_packager, id_predictor
 
-from xm_slurm import api, execution
+from xm_slurm import api, execution, executors
 from xm_slurm.console import console
 from xm_slurm.packaging import router
 from xm_slurm.status import SlurmWorkUnitStatus
 from xm_slurm.utils import UserSet
 
 _current_job_array_queue = contextvars.ContextVar[
     asyncio.Queue[tuple[xm.JobGroup, asyncio.Future]] | None
@@ -224,15 +224,20 @@
         self._execution_handles.append(handle)
         api.client().insert_job(
             self.experiment_id,
             self.work_unit_id,
             api.SlurmJobModel(
                 name=self.experiment_unit_name,
                 slurm_job_id=handle.job_id,  # type: ignore
-                slurm_cluster=handle.cluster.to_json(),
+                slurm_cluster=json.dumps({
+                    "host": handle.ssh_connection_options.host,
+                    "username": handle.ssh_connection_options.username,
+                    "port": handle.ssh_connection_options.port,
+                    "config": handle.ssh_connection_options.config.get_options(False),
+                }),
             ),
         )
 
     async def _launch_job_group(
         self,
         job: xm.JobGroup,
         args_view: Mapping[str, Any],
@@ -569,14 +574,16 @@
             resolved_args.append(
                 set(xm.SequentialArgs.from_collection(job_view.args).to_dict().items())
             )
             resolved_env_vars.append(set(job_view.env_vars.items()))
             resolved_futures.append(future)
         assert executable is not None, "No executable found?"
         assert executor is not None, "No executor found?"
+        assert isinstance(executor, executors.Slurm), "Only Slurm executors are supported."
+        assert executor.requirements.cluster is not None, "Cluster must be set on executor."
 
         common_args: set = functools.reduce(lambda a, b: a & b, resolved_args, set())
         common_env_vars: set = functools.reduce(lambda a, b: a & b, resolved_env_vars, set())
 
         sweep_args = [
             {
                 "args": dict(a.difference(common_args)),
@@ -586,14 +593,15 @@
         ]
 
         # No support for sweep_env_vars right now.
         # We schedule the job array and then we'll resolve all the work units with
         # the handles Slurm gives back to us.
         try:
             handles = await execution.get_client().launch(
+                cluster=executor.requirements.cluster,
                 job=xm.Job(
                     executable=executable,
                     executor=executor,
                     name=name,
                     args=dict(common_args),
                     env_vars=dict(common_env_vars),
                 ),
```

## xm_slurm/resources.py

```diff
@@ -1,81 +1,95 @@
 import enum
 import itertools
 import math
 from typing import Mapping
 
 import immutabledict
 
+from xm_slurm import config
+
 
 class ResourceType(enum.IntEnum):
     CPU = 1
 
     MEMORY = 2
     RAM = 2
 
     EPHEMERAL_STORAGE = 3
     DISK = 3
 
     GPU = 1000
     RTX8000 = 1001
     P4 = 1010
+
     P100 = 1011
+    P100_16GIB = 1012
+
     V100 = 1020
+    V100_32GIB = 1021
+
     A100 = 1030
     A100_80GIB = 1031
-    A6000 = 1032
+    A5000 = 1032
+    A6000 = 1033
+
     H100 = 1040
 
 
 AcceleratorType = set([
     ResourceType.P4,
     ResourceType.P100,
     ResourceType.V100,
     ResourceType.A100,
     ResourceType.A100_80GIB,
     ResourceType.A6000,
     ResourceType.H100,
-    ResourceType.GPU
+    ResourceType.GPU,
 ])
 
 
 ResourceQuantity = int | float
 
 
 class JobRequirements:
     replicas: int
     location: str | None
     accelerator: ResourceType | None
+    cluster: config.SlurmClusterConfig | None = None
 
     def __init__(
         self,
         *,
         resources: Mapping[ResourceType | str, ResourceQuantity] = immutabledict.immutabledict(),
         replicas: int = 1,
         location: str | None = None,
+        cluster: config.SlurmClusterConfig | None = None,
         **kw_resources: ResourceQuantity,
     ):
         self.replicas = replicas or 1
         self.location = location
         self.accelerator = None
+        self.cluster = cluster
 
         self.task_requirements: dict[ResourceType | str, ResourceQuantity] = {}
         for resource_name, value in itertools.chain(resources.items(), kw_resources.items()):
             match resource_name:
                 case str() if resource_name.upper() in ResourceType.__members__:
                     resource = ResourceType[resource_name.upper()]
                 case ResourceType():
                     resource = resource_name
                 case str():
                     resource = resource_name
 
-            if resource in AcceleratorType or (isinstance(resource, str) and resource.startswith("gpu")):
+            if resource in AcceleratorType or (
+                isinstance(resource, str) and resource.startswith("gpu")
+            ):
                 if self.accelerator is not None:
                     raise ValueError("Accelerator already set.")
-                self.accelerator = resource
+                self.accelerator = resource  # type: ignore
 
             if resource in self.task_requirements:
                 raise ValueError(f"{resource} has been specified twice.")
             self.task_requirements[resource] = value
 
     def to_directives(self) -> list[str]:
         directives = []
@@ -104,25 +118,33 @@
 
         directives.append(f"--ntasks={self.replicas}")
         if self.location:
             directives.append(f"--nodelist={self.location}")
 
         return directives
 
-    def replace(self, **kw_resources: ResourceQuantity) -> "JobRequirements":
+    def replace(
+        self,
+        cluster: config.SlurmClusterConfig | None,
+        **kw_resources: ResourceQuantity,
+    ) -> "JobRequirements":
         return JobRequirements(
             resources=self.task_requirements | kw_resources,  # type: ignore
             replicas=self.replicas,
+            cluster=cluster or self.cluster,
         )
 
     def __repr__(self) -> str:
         args = []
 
         for resource, value in self.task_requirements.items():
             if isinstance(resource, ResourceType):
                 resource = resource.name
             args.append(f"{resource.lower()}={value!r}")
 
         if self.replicas != 1:
             args.append(f"replicas={self.replicas}")
 
+        if self.cluster is not None:
+            args.append(f"cluster={self.cluster!r}")
+
         return f'xm_slurm.JobRequirements({", ".join(args)})'
```

## xm_slurm/templates/slurm/runtimes/apptainer.bash.j2

```diff
@@ -56,23 +56,34 @@
 time ${CONTAINER_RUNTIME} build \
   --force \
   --sandbox \
   --fix-perms \
   "$SLURM_TMPDIR"/container \
   docker://{{ job.executable.image }}
 
+{% if (cluster.runtime | string) == "singularity" and cluster.mounts %}
+{% for source, dest in cluster.mounts.items() %}
+mkdir -p "$SLURM_TMPDIR"/container/{{ dest | trim('/') }}
+{% endfor %}
+{% endif %}
+
 exec ${CONTAINER_RUNTIME} run \
 {% if job.executor.requirements.accelerator %}
   --nv \
 {% endif %}
   --no-init \
   --no-umask \
   --no-home \
   --cleanenv \
   --containall \
+{% if cluster.mounts %}
+{% for source, dest in cluster.mounts.items() %}
+  --mount type=bind,src={{ source }},dst={{ dest }} \
+{% endfor %}
+{% endif %}
   --workdir "$SLURM_TMPDIR"/container-workdir \
 {% if (cluster.runtime | string) == "apptainer" %}
   --overlay "$SLURM_TMPDIR"/container-overlay \
 {% else %}
   --writable \
 {% endif %}
 {% if job.executable.workdir %}
```

## xm_slurm/templates/slurm/runtimes/podman.bash.j2

```diff
@@ -30,14 +30,19 @@
   --env PODMANENV* \
   --pull never \
   --restart no \
   --rm \
 {% if job.executor.requirements.accelerator %}
   --device nvidia.com/gpu=all \
 {% endif %}
+{% if cluster.mounts %}
+{% for source, dest in cluster.mounts.items() %}
+  --mount type=bind,src={{ source }},dst={{ dest }} \
+{% endfor %}
+{% endif %}
 {% if job.executable.workdir %}
   --workdir {{ job.executable.workdir }} \
 {% endif %}
   {{ job.executable.image }} \
 {% for arg in job.executable.args.to_list() %}
   {{ arg }} \
 {% endfor %}
```

## Comparing `xm_slurm-0.2.1.dist-info/METADATA` & `xm_slurm-0.3.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xm-slurm
-Version: 0.2.1
+Version: 0.3.0
 Summary: Slurm backend for XManager.
 Author-Email: Jesse Farebrother <jfarebro@cs.mcgill.ca>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: xmanager>=0.4.0
 Requires-Dist: asyncssh>=2.13.2
 Requires-Dist: humanize>=4.8.0
```

## Comparing `xm_slurm-0.2.1.dist-info/RECORD` & `xm_slurm-0.3.0.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-xm_slurm-0.2.1.dist-info/METADATA,sha256=HQOrO0uhBPim-mvuhOP0THwUzAagAfiyUdoRRMrAl1k,903
-xm_slurm-0.2.1.dist-info/WHEEL,sha256=7sv5iXvIiTVJSnAxCz2tGBm9DHsb2vPSzeYeT7pvGUY,90
+xm_slurm-0.3.0.dist-info/METADATA,sha256=N6daEj9YzfCuf5CnwKSWvSqs4gTArt5NLrs5iGMhEKU,903
+xm_slurm-0.3.0.dist-info/WHEEL,sha256=vnE8JVcI2Wz7GRKorsPArnBdnW2SWKWGow5gu5tHlRU,90
 xm_slurm/__init__.py,sha256=J5FkaAXbcT7yWmcNgBq3mDLOmnNZW7c4WekSt7JVoFc,1019
-xm_slurm/api.py,sha256=5C9bgqSosqNHXwUb-7HoBqnyo6qW53BZiV70w8UD2BQ,9105
+xm_slurm/api.py,sha256=LhAnNfP_M62FEbTSa-NgToxi0OA8kCrUx2czbxfpOjw,9533
 xm_slurm/batching.py,sha256=mGVvccehsC4dfjtg7QqrtxuoxYI_Fs8o1GLJIGVyvyo,4379
-xm_slurm/config.py,sha256=Vdn83DVIZDfppegpg2yObdffDwCJd_AUMxO9D6UiGgI,3394
+xm_slurm/config.py,sha256=St2bdp2m2pajGxivmsRkmZrKd-inBKF7Hn6oezTT9zM,4955
 xm_slurm/console.py,sha256=UpMqeJ0C8i0pkue1AHnnyyX0bFJ9zZeJ7HBR6yhuA8A,54
+xm_slurm/contrib/clusters/__init__.py,sha256=BM9W2iJE3616uwAUdj1uqcXF70zunXlxWHEXgLdH2xs,1600
+xm_slurm/contrib/clusters/drac.py,sha256=Tl4Cv0DOHssJcnTU5c60w0Ye3dwlDZE4AkPtmew6-lQ,5201
 xm_slurm/executables.py,sha256=4SVn6obIvOKh54RXYccixUx993Xma0rLGanD3TfXNS4,5762
-xm_slurm/execution.py,sha256=Si4VUcPRAsrEzc22aeqbgZobXu3QjlhQNFYZ2Y6TKvw,18847
+xm_slurm/execution.py,sha256=EDckbWYtBoMAc0yWU-BitFWGPOkA-AxoQRFv7XdUNcA,17998
 xm_slurm/executors.py,sha256=vilogTjlxHLfZDms4aYOZWUW8w-2IdxU7xh-9vcW1Y0,4723
-xm_slurm/experiment.py,sha256=bWdzYOglKdvNVMwlE7H3-eQRsP0KTUdef3mKC8jaM5M,25033
+xm_slurm/experiment.py,sha256=y5K-kZgavRk022IGXw5bg7beX4cnU1JtUOeP9824sRA,25578
 xm_slurm/job_blocks.py,sha256=1H1eZ5gbEGEoDYcoSh8S_gvp04MLXP7G128crDJlMYo,482
 xm_slurm/packageables.py,sha256=nzmkREacDPJXmo6D1mk4bKjUrLTjHj3rue-PoO_EATk,11216
 xm_slurm/packaging/__init__.py,sha256=dh307yLpUT9KN7rJ1e9fYC6hegGKfZcGboUq9nGpDVQ,233
 xm_slurm/packaging/docker/__init__.py,sha256=SQxaDtomYc4NwZ5lSoCiMoy2S2lRmc0sgwVMbENIatU,2474
 xm_slurm/packaging/docker/abc.py,sha256=f8XvUA_FusIpXI45PR5isA2msxM003ycW5mWbAyiKfk,3830
 xm_slurm/packaging/docker/cloud.py,sha256=8V3Hg_v_TLe6WoJkk3l6S-m7OgK2TNxwfK2glLSFN3o,21300
 xm_slurm/packaging/docker/local.py,sha256=-_elHmU-v0R3XucNMpYF98HCQcMV0x_RTvkt1jLnes4,8008
 xm_slurm/packaging/registry.py,sha256=GrdmQg9MgSo38OiqOzMKWSkQyBuyryOfc3zcdgZ4CUE,1148
 xm_slurm/packaging/router.py,sha256=6qjtsy4BoYgSaQzC_pQSHVHeWcphG_xWVsWgW6ALC7U,2033
 xm_slurm/packaging/utils.py,sha256=dCWAuUXT5COXGe1BQEW8luo5patxTeLSAGOWPR63iY8,6219
-xm_slurm/resources.py,sha256=jseYCxqKIk2TuZayhR3P1ZhTU3cpfaFyPSjsw7LMViY,4342
+xm_slurm/resources.py,sha256=FqAULBhchu6z66On3SRDOJvXfs0sLGfBvcMGUUB3jxU,4835
 xm_slurm/status.py,sha256=4BUBm-qwVWH_RJGzRxO8Eom5d92_cp8jydQVwqH8v6U,6653
 xm_slurm/templates/docker/docker-bake.hcl.j2,sha256=Ur9t9Yk_LfLPLvJvur47ZKFZmY07H-pJ76edQzAgYfU,1313
 xm_slurm/templates/docker/mamba.Dockerfile,sha256=vsOYkm-T33C2RanwbdjJIUjhPJ_H1NDBeEACguQJZ8c,716
 xm_slurm/templates/docker/pdm.Dockerfile,sha256=Yg5-lOXkNVJr0OER_yOnRvn9NlFLnt3RfdYfq4f0ilg,748
 xm_slurm/templates/docker/python.Dockerfile,sha256=O6lHesmsLz7cX-efVQpsafEVYmbHPyV73xA9WbBKGKg,738
 xm_slurm/templates/slurm/fragments/monitor.bash.j2,sha256=CxtbxOJzd0Un-ApDO6T8JHuKlSv6uwwBFMJPeGjCKnk,1071
 xm_slurm/templates/slurm/fragments/proxy.bash.j2,sha256=VJLglZo-Nvx9R-qe3rHTxr07CylTQ6Z9NwBzvIpAZrA,814
 xm_slurm/templates/slurm/job-array.bash.j2,sha256=d4twfV1PATGQwTIleFBUIGmMAIHH-F7RjBsdfaAIQko,599
 xm_slurm/templates/slurm/job-group.bash.j2,sha256=UkjfBE7jg9mepcUWaHZEAjkiXsIM1j_sLxLzxkteD-Y,1120
 xm_slurm/templates/slurm/job.bash.j2,sha256=EUeq3P2xqTIqlHi2SVhFBT7NL4lUj8okYUa3GnlaIIc,1852
-xm_slurm/templates/slurm/runtimes/apptainer.bash.j2,sha256=HYs9FIjRYehGjJwhZKFgT_aMvL9xMetjXdhaB5TT-jw,2884
-xm_slurm/templates/slurm/runtimes/podman.bash.j2,sha256=J_iGoAaW30bbjhSaN0t9wOwbzT0Oc_KRHjuxxOr-lWE,1317
+xm_slurm/templates/slurm/runtimes/apptainer.bash.j2,sha256=Z8Mc4wbmOJW_n9V0hcKsPNEnveZFqsASg8Z3dICaETk,3241
+xm_slurm/templates/slurm/runtimes/podman.bash.j2,sha256=xKXYFvQvazMx0PgvmlRXR6eecoiBUl8y52dIzQtWkBE,1469
 xm_slurm/utils.py,sha256=PNd0vTn33UKm5LpC41TdO9QIFe21V5A0RbYEhQIMjrA,1930
-xm_slurm-0.2.1.dist-info/RECORD,,
+xm_slurm-0.3.0.dist-info/RECORD,,
```

