# Comparing `tmp/streamflow-0.2.0.dev8.tar.gz` & `tmp/streamflow-0.2.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamflow-0.2.0.dev8.tar", last modified: Mon Aug 28 13:06:15 2023, max compression
+gzip compressed data, was "streamflow-0.2.0.dev9.tar", last modified: Sun Sep 10 08:16:23 2023, max compression
```

## Comparing `streamflow-0.2.0.dev8.tar` & `streamflow-0.2.0.dev9.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.421953 streamflow-0.2.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (999)     7652 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      212 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)    11568 2023-08-28 13:06:15.421953 streamflow-0.2.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    10253 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       13 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/bandit-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.397952 streamflow-0.2.0.dev8/docs/
--rw-r--r--   0 runner    (1001) docker     (999)       63 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)       72 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/lint-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)     3484 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       43 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/report-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)      286 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 13:06:15.421953 streamflow-0.2.0.dev8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.401952 streamflow-0.2.0.dev8/streamflow/
--rw-r--r--   0 runner    (1001) docker     (999)       62 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      117 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.401952 streamflow-0.2.0.dev8/streamflow/config/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4926 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/config/config.py
--rw-r--r--   0 runner    (1001) docker     (999)     3730 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/config/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.393952 streamflow-0.2.0.dev8/streamflow/config/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.401952 streamflow-0.2.0.dev8/streamflow/config/schemas/v1.0/
--rw-r--r--   0 runner    (1001) docker     (999)    11727 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/config/schemas/v1.0/config_schema.json
--rw-r--r--   0 runner    (1001) docker     (999)     1535 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/config/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.405952 streamflow-0.2.0.dev8/streamflow/core/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4460 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/core/asyncache.py
--rw-r--r--   0 runner    (1001) docker     (999)     2620 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/core/config.py
--rw-r--r--   0 runner    (1001) docker     (999)     1640 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/core/context.py
--rw-r--r--   0 runner    (1001) docker     (999)     3358 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/core/data.py
--rw-r--r--   0 runner    (1001) docker     (999)     9361 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/core/deployment.py
--rw-r--r--   0 runner    (1001) docker     (999)      674 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/core/exception.py
--rw-r--r--   0 runner    (1001) docker     (999)     7263 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/core/persistence.py
--rw-r--r--   0 runner    (1001) docker     (999)     1017 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/core/provenance.py
--rw-r--r--   0 runner    (1001) docker     (999)     1730 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/core/recovery.py
--rw-r--r--   0 runner    (1001) docker     (999)     7727 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/core/scheduling.py
--rw-r--r--   0 runner    (1001) docker     (999)     7368 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (999)    24159 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.405952 streamflow-0.2.0.dev8/streamflow/cwl/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.405952 streamflow-0.2.0.dev8/streamflow/cwl/antlr/
--rw-r--r--   0 runner    (1001) docker     (999)    52296 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/antlr/ECMAScriptLexer.py
--rw-r--r--   0 runner    (1001) docker     (999)    33065 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/antlr/ECMAScriptListener.py
--rw-r--r--   0 runner    (1001) docker     (999)   228650 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/antlr/ECMAScriptParser.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/antlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3683 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/combinator.py
--rw-r--r--   0 runner    (1001) docker     (999)    53059 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/command.py
--rw-r--r--   0 runner    (1001) docker     (999)     4591 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/expression.py
--rw-r--r--   0 runner    (1001) docker     (999)     2933 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/hardware.py
--rw-r--r--   0 runner    (1001) docker     (999)     3388 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/main.py
--rw-r--r--   0 runner    (1001) docker     (999)    49556 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.405952 streamflow-0.2.0.dev8/streamflow/cwl/requirement/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/requirement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.409952 streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/
--rw-r--r--   0 runner    (1001) docker     (999)      475 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    15297 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/docker.py
--rw-r--r--   0 runner    (1001) docker     (999)     3481 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/kubernetes.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.409952 streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/schemas/
--rw-r--r--   0 runner    (1001) docker     (999)    13791 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/schemas/docker.json
--rw-r--r--   0 runner    (1001) docker     (999)      928 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2
--rw-r--r--   0 runner    (1001) docker     (999)     2752 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/schemas/kubernetes.json
--rw-r--r--   0 runner    (1001) docker     (999)     9310 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/schemas/singularity.json
--rw-r--r--   0 runner    (1001) docker     (999)     9715 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/singularity.py
--rw-r--r--   0 runner    (1001) docker     (999)      902 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/translator.py
--rw-r--r--   0 runner    (1001) docker     (999)     4146 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/runner.py
--rw-r--r--   0 runner    (1001) docker     (999)    23143 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/step.py
--rw-r--r--   0 runner    (1001) docker     (999)     3031 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/token.py
--rw-r--r--   0 runner    (1001) docker     (999)    12751 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/transformer.py
--rw-r--r--   0 runner    (1001) docker     (999)   113838 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/translator.py
--rw-r--r--   0 runner    (1001) docker     (999)    40610 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/cwl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.409952 streamflow-0.2.0.dev8/streamflow/data/
--rw-r--r--   0 runner    (1001) docker     (999)      111 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    16179 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/data/manager.py
--rw-r--r--   0 runner    (1001) docker     (999)    15071 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/data/remotepath.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.409952 streamflow-0.2.0.dev8/streamflow/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (999)      210 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/data/schemas/data_manager.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.409952 streamflow-0.2.0.dev8/streamflow/deployment/
--rw-r--r--   0 runner    (1001) docker     (999)      135 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    36140 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/aiotarstream.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.413952 streamflow-0.2.0.dev8/streamflow/deployment/connector/
--rw-r--r--   0 runner    (1001) docker     (999)      950 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    13563 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/base.py
--rw-r--r--   0 runner    (1001) docker     (999)    52606 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/container.py
--rw-r--r--   0 runner    (1001) docker     (999)    43726 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (999)     3786 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (999)    15378 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/occam.py
--rw-r--r--   0 runner    (1001) docker     (999)    43741 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.413952 streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/
--rw-r--r--   0 runner    (1001) docker     (999)     4466 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/docker-compose.json
--rw-r--r--   0 runner    (1001) docker     (999)    14609 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/docker.json
--rw-r--r--   0 runner    (1001) docker     (999)     5498 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/flux.json
--rw-r--r--   0 runner    (1001) docker     (999)     6556 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/helm3.json
--rw-r--r--   0 runner    (1001) docker     (999)     3226 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/kubernetes.json
--rw-r--r--   0 runner    (1001) docker     (999)      388 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/local.json
--rw-r--r--   0 runner    (1001) docker     (999)     1103 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/occam.json
--rw-r--r--   0 runner    (1001) docker     (999)     3655 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/pbs.json
--rw-r--r--   0 runner    (1001) docker     (999)     3589 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/queue_manager.json
--rw-r--r--   0 runner    (1001) docker     (999)    10114 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/singularity.json
--rw-r--r--   0 runner    (1001) docker     (999)    21190 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/slurm.json
--rw-r--r--   0 runner    (1001) docker     (999)     5017 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/ssh.json
--rw-r--r--   0 runner    (1001) docker     (999)    25573 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/connector/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.417952 streamflow-0.2.0.dev8/streamflow/deployment/filter/
--rw-r--r--   0 runner    (1001) docker     (999)      130 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.417952 streamflow-0.2.0.dev8/streamflow/deployment/filter/schemas/
--rw-r--r--   0 runner    (1001) docker     (999)      218 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/filter/schemas/shuffle.json
--rw-r--r--   0 runner    (1001) docker     (999)      572 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/filter/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (999)     5765 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/future.py
--rw-r--r--   0 runner    (1001) docker     (999)     9772 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.417952 streamflow-0.2.0.dev8/streamflow/deployment/schemas/
--rw-r--r--   0 runner    (1001) docker     (999)      223 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/schemas/deployment_manager.json
--rw-r--r--   0 runner    (1001) docker     (999)     2291 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/stream.py
--rw-r--r--   0 runner    (1001) docker     (999)      937 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/template.py
--rw-r--r--   0 runner    (1001) docker     (999)     2944 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/utils.py
--rw-r--r--   0 runner    (1001) docker     (999)     3308 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/deployment/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.417952 streamflow-0.2.0.dev8/streamflow/ext/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3806 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/ext/plugin.py
--rw-r--r--   0 runner    (1001) docker     (999)    15356 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/ext/utils.py
--rw-r--r--   0 runner    (1001) docker     (999)     3692 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (999)    10162 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/main.py
--rw-r--r--   0 runner    (1001) docker     (999)     7243 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.417952 streamflow-0.2.0.dev8/streamflow/persistence/
--rw-r--r--   0 runner    (1001) docker     (999)      131 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      691 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/persistence/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     2652 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/persistence/loading_context.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.417952 streamflow-0.2.0.dev8/streamflow/persistence/schemas/
--rw-r--r--   0 runner    (1001) docker     (999)      622 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/persistence/schemas/sqlite.json
--rw-r--r--   0 runner    (1001) docker     (999)     2036 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/persistence/schemas/sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (999)    20158 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/persistence/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.417952 streamflow-0.2.0.dev8/streamflow/provenance/
--rw-r--r--   0 runner    (1001) docker     (999)      142 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    64158 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/provenance/run_crate.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.417952 streamflow-0.2.0.dev8/streamflow/recovery/
--rw-r--r--   0 runner    (1001) docker     (999)      432 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/recovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2167 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/recovery/checkpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (999)    11361 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/recovery/failure_manager.py
--rw-r--r--   0 runner    (1001) docker     (999)      516 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/recovery/recovery.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.417952 streamflow-0.2.0.dev8/streamflow/recovery/schemas/
--rw-r--r--   0 runner    (1001) docker     (999)      418 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/recovery/schemas/default_checkpoint_manager.json
--rw-r--r--   0 runner    (1001) docker     (999)      567 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/recovery/schemas/default_failure_manager.json
--rw-r--r--   0 runner    (1001) docker     (999)      226 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/recovery/schemas/dummy_checkpoint_manager.json
--rw-r--r--   0 runner    (1001) docker     (999)      223 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/recovery/schemas/dummy_failure_manager.json
--rw-r--r--   0 runner    (1001) docker     (999)     2286 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/report.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.417952 streamflow-0.2.0.dev8/streamflow/scheduling/
--rw-r--r--   0 runner    (1001) docker     (999)      112 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/scheduling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.417952 streamflow-0.2.0.dev8/streamflow/scheduling/policy/
--rw-r--r--   0 runner    (1001) docker     (999)      130 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/scheduling/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3178 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/scheduling/policy/data_locality.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.421953 streamflow-0.2.0.dev8/streamflow/scheduling/policy/schemas/
--rw-r--r--   0 runner    (1001) docker     (999)      217 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/scheduling/policy/schemas/data_locality.json
--rw-r--r--   0 runner    (1001) docker     (999)    16466 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/scheduling/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.421953 streamflow-0.2.0.dev8/streamflow/scheduling/schemas/
--rw-r--r--   0 runner    (1001) docker     (999)      373 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/scheduling/schemas/scheduler.json
--rw-r--r--   0 runner    (1001) docker     (999)       23 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.421953 streamflow-0.2.0.dev8/streamflow/workflow/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     8428 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/workflow/combinator.py
--rw-r--r--   0 runner    (1001) docker     (999)     6399 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (999)      815 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/workflow/port.py
--rw-r--r--   0 runner    (1001) docker     (999)    66334 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/workflow/step.py
--rw-r--r--   0 runner    (1001) docker     (999)     4849 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/workflow/token.py
--rw-r--r--   0 runner    (1001) docker     (999)     1591 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/workflow/transformer.py
--rw-r--r--   0 runner    (1001) docker     (999)     1751 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/streamflow/workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.401952 streamflow-0.2.0.dev8/streamflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)    11568 2023-08-28 13:06:15.000000 streamflow-0.2.0.dev8/streamflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     5139 2023-08-28 13:06:15.000000 streamflow-0.2.0.dev8/streamflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 13:06:15.000000 streamflow-0.2.0.dev8/streamflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       90 2023-08-28 13:06:15.000000 streamflow-0.2.0.dev8/streamflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      629 2023-08-28 13:06:15.000000 streamflow-0.2.0.dev8/streamflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-28 13:06:15.000000 streamflow-0.2.0.dev8/streamflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 13:06:14.000000 streamflow-0.2.0.dev8/streamflow.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)      103 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 13:06:15.421953 streamflow-0.2.0.dev8/tests/
--rw-r--r--   0 runner    (1001) docker     (999)     8288 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/tests/test_cwl_loop.py
--rw-r--r--   0 runner    (1001) docker     (999)    24693 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/tests/test_cwl_persistence.py
--rw-r--r--   0 runner    (1001) docker     (999)    21328 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/tests/test_cwl_provenance.py
--rw-r--r--   0 runner    (1001) docker     (999)    10588 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/tests/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (999)    17890 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/tests/test_provenance.py
--rw-r--r--   0 runner    (1001) docker     (999)     7568 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/tests/test_remotepath.py
--rw-r--r--   0 runner    (1001) docker     (999)    16712 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (999)     7508 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (999)     7532 2023-08-28 13:06:00.000000 streamflow-0.2.0.dev8/tests/test_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.608965 streamflow-0.2.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12898 2023-09-10 08:16:23.608965 streamflow-0.2.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10253 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/bandit-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.576965 streamflow-0.2.0.dev9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/lint-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/report-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-10 08:16:23.608965 streamflow-0.2.0.dev9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.576965 streamflow-0.2.0.dev9/streamflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.580965 streamflow-0.2.0.dev9/streamflow/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/config/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.572965 streamflow-0.2.0.dev9/streamflow/config/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.580965 streamflow-0.2.0.dev9/streamflow/config/schemas/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/config/schemas/v1.0/config_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/config/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.584965 streamflow-0.2.0.dev9/streamflow/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/core/asyncache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9361 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/core/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7263 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/core/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/core/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/core/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7727 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/core/scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24159 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.584965 streamflow-0.2.0.dev9/streamflow/cwl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.588965 streamflow-0.2.0.dev9/streamflow/cwl/antlr/
+-rw-r--r--   0 runner    (1001) docker     (127)    52296 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/antlr/ECMAScriptLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33065 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/antlr/ECMAScriptListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)   228650 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/antlr/ECMAScriptParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/antlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/combinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53059 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49556 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.588965 streamflow-0.2.0.dev9/streamflow/cwl/requirement/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/requirement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.588965 streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15297 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/kubernetes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.588965 streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/schemas/docker.json
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/schemas/kubernetes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9310 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/schemas/singularity.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9715 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23143 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12751 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113838 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40610 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/cwl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.588965 streamflow-0.2.0.dev9/streamflow/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16179 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/data/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15071 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/data/remotepath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.588965 streamflow-0.2.0.dev9/streamflow/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/data/schemas/data_manager.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.592965 streamflow-0.2.0.dev9/streamflow/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36140 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/aiotarstream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.592965 streamflow-0.2.0.dev9/streamflow/deployment/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13661 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52606 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43802 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17390 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/occam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44839 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.596965 streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/docker-compose.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/docker.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/flux.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/helm3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/kubernetes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/local.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/occam.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/pbs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/queue_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/singularity.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21431 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/slurm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/ssh.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28835 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/connector/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.596965 streamflow-0.2.0.dev9/streamflow/deployment/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.596965 streamflow-0.2.0.dev9/streamflow/deployment/filter/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/filter/schemas/shuffle.json
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/filter/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.596965 streamflow-0.2.0.dev9/streamflow/deployment/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/schemas/deployment_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/deployment/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.596965 streamflow-0.2.0.dev9/streamflow/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/ext/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15356 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/ext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10162 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.596965 streamflow-0.2.0.dev9/streamflow/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/persistence/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/persistence/loading_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.600965 streamflow-0.2.0.dev9/streamflow/persistence/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/persistence/schemas/sqlite.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/persistence/schemas/sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    19346 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/persistence/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.600965 streamflow-0.2.0.dev9/streamflow/provenance/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64158 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/provenance/run_crate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.600965 streamflow-0.2.0.dev9/streamflow/recovery/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/recovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/recovery/checkpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11361 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/recovery/failure_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/recovery/recovery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.600965 streamflow-0.2.0.dev9/streamflow/recovery/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/recovery/schemas/default_checkpoint_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/recovery/schemas/default_failure_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/recovery/schemas/dummy_checkpoint_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/recovery/schemas/dummy_failure_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.600965 streamflow-0.2.0.dev9/streamflow/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/scheduling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.600965 streamflow-0.2.0.dev9/streamflow/scheduling/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/scheduling/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/scheduling/policy/data_locality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.600965 streamflow-0.2.0.dev9/streamflow/scheduling/policy/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/scheduling/policy/schemas/data_locality.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17129 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/scheduling/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.600965 streamflow-0.2.0.dev9/streamflow/scheduling/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/scheduling/schemas/scheduler.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.604966 streamflow-0.2.0.dev9/streamflow/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/workflow/combinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/workflow/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66334 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/workflow/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/workflow/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/workflow/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/streamflow/workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.580965 streamflow-0.2.0.dev9/streamflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12898 2023-09-10 08:16:23.000000 streamflow-0.2.0.dev9/streamflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2023-09-10 08:16:23.000000 streamflow-0.2.0.dev9/streamflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-10 08:16:23.000000 streamflow-0.2.0.dev9/streamflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2023-09-10 08:16:23.000000 streamflow-0.2.0.dev9/streamflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2023-09-10 08:16:23.000000 streamflow-0.2.0.dev9/streamflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-10 08:16:23.000000 streamflow-0.2.0.dev9/streamflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-10 08:16:23.000000 streamflow-0.2.0.dev9/streamflow.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 08:16:23.604966 streamflow-0.2.0.dev9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/tests/test_cwl_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24693 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/tests/test_cwl_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21328 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/tests/test_cwl_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/tests/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17890 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/tests/test_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/tests/test_remotepath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16712 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7508 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2023-09-10 08:16:03.000000 streamflow-0.2.0.dev9/tests/test_transfer.py
```

### Comparing `streamflow-0.2.0.dev8/LICENSE` & `streamflow-0.2.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/PKG-INFO` & `streamflow-0.2.0.dev9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow
-Version: 0.2.0.dev8
+Version: 0.2.0.dev9
 Summary: StreamFlow framework
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://streamflow.di.unito.it
 Project-URL: Package, https://pypi.org/project/streamflow
 Project-URL: Repository, https://github.com/alpha-unito/streamflow
 Project-URL: Docker, https://hub.docker.com/r/alphaunito/streamflow
@@ -20,20 +20,51 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp==3.8.5
+Requires-Dist: aiosqlite==0.19.0
+Requires-Dist: antlr4-python3-runtime==4.13.1
+Requires-Dist: asyncssh==2.13.2
+Requires-Dist: bcrypt==4.0.1
+Requires-Dist: cachetools==5.3.1
+Requires-Dist: cwltool==3.1.20230906142556
+Requires-Dist: cwl-utils==0.29
+Requires-Dist: importlib_metadata==6.8.0
+Requires-Dist: Jinja2==3.1.2
+Requires-Dist: jsonschema==4.19.0
+Requires-Dist: kubernetes_asyncio==25.11.0
+Requires-Dist: psutil==5.9.5
+Requires-Dist: rdflib==6.3.2
+Requires-Dist: yattag==1.15.1
 Provides-Extra: bandit
+Requires-Dist: bandit==1.7.5; extra == "bandit"
 Provides-Extra: docs
+Requires-Dist: sphinx==7.2.5; extra == "docs"
+Requires-Dist: sphinx-jsonschema==1.19.1; extra == "docs"
+Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "docs"
 Provides-Extra: lint
+Requires-Dist: black==23.7.0; extra == "lint"
+Requires-Dist: codespell==2.2.5; extra == "lint"
+Requires-Dist: flake8-bugbear==23.7.10; extra == "lint"
+Requires-Dist: pyupgrade==3.10.1; extra == "lint"
 Provides-Extra: report
+Requires-Dist: pandas==2.1.0; extra == "report"
+Requires-Dist: plotly==5.16.1; extra == "report"
+Requires-Dist: kaleido==0.2.1; extra == "report"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: cwltest==2.3.20230825125225; extra == "test"
+Requires-Dist: pytest==7.4.2; extra == "test"
+Requires-Dist: pytest-asyncio==0.21.1; extra == "test"
+Requires-Dist: pytest-cov==4.1.0; extra == "test"
+Requires-Dist: pytest-xdist==3.3.1; extra == "test"
 
 # StreamFlow
 
 [![CI Tests](https://github.com/alpha-unito/streamflow/actions/workflows/ci-tests.yaml/badge.svg?branch=master)](https://github.com/alpha-unito/streamflow/actions/workflows/ci-tests.yaml)
 
 The [StreamFlow](https://streamflow.di.unito.it/) framework is a container-native *Workflow Management System (WMS)* written in Python 3.
 It has been designed around two main principles:
```

### Comparing `streamflow-0.2.0.dev8/README.md` & `streamflow-0.2.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/pyproject.toml` & `streamflow-0.2.0.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/config/config.py` & `streamflow-0.2.0.dev9/streamflow/config/config.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/config/schema.py` & `streamflow-0.2.0.dev9/streamflow/config/schema.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/config/schemas/v1.0/config_schema.json` & `streamflow-0.2.0.dev9/streamflow/config/schemas/v1.0/config_schema.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/config/validator.py` & `streamflow-0.2.0.dev9/streamflow/config/validator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/core/asyncache.py` & `streamflow-0.2.0.dev9/streamflow/core/asyncache.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/core/config.py` & `streamflow-0.2.0.dev9/streamflow/core/config.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/core/context.py` & `streamflow-0.2.0.dev9/streamflow/core/context.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/core/data.py` & `streamflow-0.2.0.dev9/streamflow/core/data.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/core/deployment.py` & `streamflow-0.2.0.dev9/streamflow/core/deployment.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/core/exception.py` & `streamflow-0.2.0.dev9/streamflow/core/exception.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/core/persistence.py` & `streamflow-0.2.0.dev9/streamflow/core/persistence.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/core/provenance.py` & `streamflow-0.2.0.dev9/streamflow/core/provenance.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/core/recovery.py` & `streamflow-0.2.0.dev9/streamflow/core/recovery.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/core/scheduling.py` & `streamflow-0.2.0.dev9/streamflow/core/scheduling.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/core/utils.py` & `streamflow-0.2.0.dev9/streamflow/core/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,42 +51,68 @@
         for scope in self.stack:
             if name in scope:
                 return True
         return False
 
 
 def create_command(
+    class_name: str,
     command: MutableSequence[str],
     environment: MutableMapping[str, str] = None,
     workdir: str | None = None,
     stdin: int | str | None = None,
     stdout: int | str = asyncio.subprocess.STDOUT,
     stderr: int | str = asyncio.subprocess.STDOUT,
 ) -> str:
+    # Format stdin
+    stdin = (
+        f" < {shlex.quote(stdin)}"
+        if stdin is not None and stdin != asyncio.subprocess.DEVNULL
+        else ""
+    )
+    # Format stderr
+    if stderr == asyncio.subprocess.DEVNULL:
+        stderr = "/dev/null"
+    if stderr == stdout:
+        stderr = " 2>&1"
+    elif stderr != asyncio.subprocess.STDOUT:
+        stderr = f" 2>{shlex.quote(stderr)}"
+    else:
+        stderr = ""
+    # Format stdout
+    if stdout == asyncio.subprocess.PIPE:
+        raise WorkflowExecutionException(
+            f"The `{class_name}` does not support `stdout` pipe redirection."
+        )
+    elif stdout == asyncio.subprocess.DEVNULL:
+        stdout = "/dev/null"
+    elif stdout != asyncio.subprocess.STDOUT:
+        stdout = f" > {shlex.quote(stdout)}"
+    else:
+        stdout = ""
+    if stderr == asyncio.subprocess.PIPE:
+        raise WorkflowExecutionException(
+            f"The `{class_name}` does not support `stderr` pipe redirection."
+        )
+    # Build command
     command = "".join(
         "{workdir}" "{environment}" "{command}" "{stdin}" "{stdout}" "{stderr}"
     ).format(
         workdir=f"cd {workdir} && " if workdir is not None else "",
-        environment="".join(
-            [f'export {key}="{value}" && ' for (key, value) in environment.items()]
-        )
-        if environment is not None
-        else "",
-        command=" ".join(command),
-        stdin=f" < {shlex.quote(stdin)}" if stdin is not None else "",
-        stdout=f" > {shlex.quote(stdout)}"
-        if stdout != asyncio.subprocess.STDOUT
-        else "",
-        stderr=(
-            " 2>&1"
-            if stderr == stdout
-            else f" 2>{shlex.quote(stderr)}"
-            if stderr != asyncio.subprocess.STDOUT
+        environment=(
+            "".join(
+                [f'export {key}="{value}" && ' for (key, value) in environment.items()]
+            )
+            if environment is not None
             else ""
         ),
+        command=" ".join(command),
+        stdin=stdin,
+        stdout=stdout,
+        stderr=stderr,
     )
     return command
 
 
 def dict_product(**kwargs) -> MutableMapping[Any, Any]:
     keys = kwargs.keys()
     vals = kwargs.values()
```

### Comparing `streamflow-0.2.0.dev8/streamflow/core/workflow.py` & `streamflow-0.2.0.dev9/streamflow/core/workflow.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/antlr/ECMAScriptLexer.py` & `streamflow-0.2.0.dev9/streamflow/cwl/antlr/ECMAScriptLexer.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/antlr/ECMAScriptListener.py` & `streamflow-0.2.0.dev9/streamflow/cwl/antlr/ECMAScriptListener.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/antlr/ECMAScriptParser.py` & `streamflow-0.2.0.dev9/streamflow/cwl/antlr/ECMAScriptParser.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/combinator.py` & `streamflow-0.2.0.dev9/streamflow/cwl/combinator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/command.py` & `streamflow-0.2.0.dev9/streamflow/cwl/command.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/expression.py` & `streamflow-0.2.0.dev9/streamflow/cwl/expression.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/hardware.py` & `streamflow-0.2.0.dev9/streamflow/cwl/hardware.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/main.py` & `streamflow-0.2.0.dev9/streamflow/cwl/main.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/processor.py` & `streamflow-0.2.0.dev9/streamflow/cwl/processor.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/docker.py` & `streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/docker.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/kubernetes.py` & `streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/kubernetes.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/schemas/docker.json` & `streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/schemas/docker.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2` & `streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/schemas/kubernetes.json` & `streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/schemas/kubernetes.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/schemas/singularity.json` & `streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/schemas/singularity.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/singularity.py` & `streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/singularity.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/requirement/docker/translator.py` & `streamflow-0.2.0.dev9/streamflow/cwl/requirement/docker/translator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/runner.py` & `streamflow-0.2.0.dev9/streamflow/cwl/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,18 +51,18 @@
     "--streamflow-file",
     type=str,
     help="The path to a StreamFlow file specifying deployments and bindings for the workflow steps",
 )
 
 
 async def _async_main(args: argparse.Namespace):
+    load_extensions()
     validator = SfValidator()
     args.name = args.name or str(uuid.uuid4())
     if args.streamflow_file:
-        load_extensions()
         with open(args.streamflow_file) as f:
             streamflow_config = validator.yaml.load(f)
         workflows = streamflow_config.get("workflows", {})
         if len(workflows) == 1:
             workflow_name = list(workflows.keys())[0]
         elif len(workflows) == 0:
             workflow_name = "cwl-workflow"
```

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/step.py` & `streamflow-0.2.0.dev9/streamflow/cwl/step.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/token.py` & `streamflow-0.2.0.dev9/streamflow/cwl/token.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/transformer.py` & `streamflow-0.2.0.dev9/streamflow/cwl/transformer.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/translator.py` & `streamflow-0.2.0.dev9/streamflow/cwl/translator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/cwl/utils.py` & `streamflow-0.2.0.dev9/streamflow/cwl/utils.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/data/manager.py` & `streamflow-0.2.0.dev9/streamflow/data/manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/data/remotepath.py` & `streamflow-0.2.0.dev9/streamflow/data/remotepath.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/aiotarstream.py` & `streamflow-0.2.0.dev9/streamflow/deployment/aiotarstream.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/__init__.py` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/base.py` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,21 @@
         stdout: int | str = asyncio.subprocess.STDOUT,
         stderr: int | str = asyncio.subprocess.STDOUT,
         capture_output: bool = False,
         timeout: int | None = None,
         job_name: str | None = None,
     ) -> tuple[Any | None, int] | None:
         command = utils.create_command(
-            command, environment, workdir, stdin, stdout, stderr
+            self.__class__.__name__,
+            command,
+            environment,
+            workdir,
+            stdin,
+            stdout,
+            stderr,
         )
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(
                 "EXECUTING command {command} on {location} {job}".format(
                     command=command,
                     location=location,
                     job=f"for job {job_name}" if job_name else "",
```

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/container.py` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/container.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/kubernetes.py` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     cast,
 )
 
 import pkg_resources
 import yaml
 from cachetools import Cache, TTLCache
 from kubernetes_asyncio import client
-from kubernetes_asyncio.client import ApiClient, Configuration, V1Container
+from kubernetes_asyncio.client import ApiClient, Configuration, V1Container, V1PodList
 from kubernetes_asyncio.config import (
     ConfigException,
     load_incluster_config,
     load_kube_config,
 )
 from kubernetes_asyncio.stream import WsApiClient, ws_client
 from kubernetes_asyncio.utils import create_from_yaml
@@ -421,15 +421,15 @@
             f"exec {pod} "
             f"{get_option('i', interactive)}"
             f"{get_option('container', container)}"
             f"-- {command}"
         )
 
     @abstractmethod
-    async def _get_running_pods(self) -> MutableSequence[Any]:
+    async def _get_running_pods(self) -> V1PodList:
         ...
 
     def _get_stream_reader(self, location: Location, src: str) -> StreamWrapperContext:
         pod, container = location.name.split(":")
         dirname, basename = posixpath.split(src)
         return KubernetesResponseWrapperContext(
             coro=cast(
@@ -503,15 +503,21 @@
         stdout: int | str = asyncio.subprocess.STDOUT,
         stderr: int | str = asyncio.subprocess.STDOUT,
         capture_output: bool = False,
         timeout: int | None = None,
         job_name: str | None = None,
     ) -> tuple[Any | None, int] | None:
         command = utils.create_command(
-            command, environment, workdir, stdin, stdout, stderr
+            self.__class__.__name__,
+            command,
+            environment,
+            workdir,
+            stdin,
+            stdout,
+            stderr,
         )
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(
                 "EXECUTING command {command} on {location} {job}".format(
                     command=command,
                     location=location,
                     job=f"for job {job_name}" if job_name else "",
@@ -623,15 +629,15 @@
             version = group
             group = "core"
         group = "".join(group.rsplit(".k8s.io", 1))
         group = "".join(word.capitalize() for word in group.split("."))
         fcn_to_call = f"{group}{version.capitalize()}Api"
         return getattr(client, fcn_to_call)(self.client.api_client)
 
-    async def _get_running_pods(self) -> MutableSequence[Any]:
+    async def _get_running_pods(self) -> V1PodList:
         return await self.client.list_namespaced_pod(
             namespace=self.namespace or "default",
             field_selector="status.phase=Running",
         )
 
     async def _is_ready(self, k8s_object: Any) -> bool:
         kind = k8s_object.kind
@@ -982,15 +988,15 @@
             f"{get_option('kubeconfig', self.kubeconfig)}"
             f"{get_option('namespace', self.namespace)}"
             f"{get_option('registry-config', self.registryConfig)}"
             f"{get_option('repository-cache', self.repositoryCache)}"
             f"{get_option('repository-config', self.repositoryConfig)}"
         )
 
-    async def _get_running_pods(self) -> MutableSequence[Any]:
+    async def _get_running_pods(self) -> V1PodList:
         return await self.client.list_namespaced_pod(
             namespace=self.namespace or "default",
             label_selector=f"app.kubernetes.io/instance={self.releaseName}",
             field_selector="status.phase=Running",
         )
 
     async def deploy(self, external: bool) -> None:
```

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/local.py` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/local.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/occam.py` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/occam.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import asyncssh
 import pkg_resources
 from ruamel.yaml import YAML
 
 from streamflow.core import utils
 from streamflow.core.deployment import Location
+from streamflow.core.exception import WorkflowExecutionException
 from streamflow.core.scheduling import AvailableLocation
 from streamflow.core.utils import get_option
 from streamflow.deployment.connector.ssh import SSHConnector
 from streamflow.log_handler import logger
 
 
 class OccamConnector(SSHConnector):
@@ -94,16 +95,27 @@
         return None
 
     async def _get_tmpdir(self, location: str):
         scratch_home = f"/scratch/home/{self.username}"
         temp_dir = posixpath.join(
             scratch_home, "streamflow", "".join(utils.random_name())
         )
-        async with self._get_ssh_client(location) as ssh_client:
-            await ssh_client.run(f"mkdir -p {temp_dir}")
+        async with self._get_ssh_client_process(
+            location=location,
+            command=f"mkdir -p {temp_dir}",
+            stdout=asyncio.subprocess.STDOUT,
+            stderr=asyncio.subprocess.STDOUT,
+        ) as proc:
+            result = await proc.wait()
+            if result.returncode == 0:
+                return temp_dir
+            else:
+                raise WorkflowExecutionException(
+                    f"Error while creating directory {temp_dir}: {result.stdout.strip()}"
+                )
         return temp_dir
 
     def _get_volumes(self, location: str) -> MutableSequence[str]:
         for name in self.jobs_table:
             if location in self.jobs_table[name]:
                 service = name
                 return self.env_description[service].get("volumes", [])
@@ -144,16 +156,25 @@
                 )
                 for location in effective_locations
             )
         )
         # If a temporary location was created, delete it
         if temp_dir is not None:
             for location in effective_locations:
-                async with self._get_ssh_client(location.name) as ssh_client:
-                    await ssh_client.run(f"rm -rf {temp_dir}")
+                async with self._get_ssh_client_process(
+                    location=location.name,
+                    command=f"rm -rf {temp_dir}",
+                    stdout=asyncio.subprocess.STDOUT,
+                    stderr=asyncio.subprocess.STDOUT,
+                ) as proc:
+                    result = await proc.wait()
+                    if result.returncode != 0:
+                        raise WorkflowExecutionException(
+                            f"Error while removing directory {temp_dir}: {result.stdout.strip()}"
+                        )
 
     async def _copy_remote_to_remote_single(
         self,
         src: str,
         dst: str,
         location: Location,
         source_location: Location,
@@ -177,15 +198,15 @@
         effective_locations = self._get_effective_locations(locations, dst)
         # Check for the need of a temporary copy
         temp_dir = None
         for location in effective_locations:
             shared_path = self._get_shared_path(location.name, dst)
             if shared_path is None:
                 temp_dir = await self._get_tmpdir(location.name)
-                async with self._get_ssh_client(location.name) as ssh_client:
+                async with self._get_ssh_client_process(location.name) as ssh_client:
                     await asyncssh.scp(
                         src, (ssh_client, temp_dir), preserve=True, recurse=True
                     )
                 break
         # Perform the actual copies
         copy_tasks = []
         for location in effective_locations:
@@ -199,42 +220,46 @@
                         read_only=read_only,
                     )
                 )
             )
         await asyncio.gather(*copy_tasks)
         # If a temporary location was created, delete it
         if temp_dir is not None:
-            for location in effective_locations:
-                async with self._get_ssh_client(location.name) as ssh_client:
-                    await ssh_client.run(f"rm -rf {temp_dir}")
+            delete_command = ["rm", "-rf", temp_dir]
+            await asyncio.gather(
+                *(
+                    asyncio.create_task(self.run(location, delete_command))
+                    for location in effective_locations
+                )
+            )
 
     async def _copy_local_to_remote_single(
         self,
         src: str,
         dst: str,
         location: Location,
         temp_dir: str | None,
         read_only: bool = False,
     ) -> None:
         shared_path = self._get_shared_path(location.name, dst)
         if shared_path is not None:
-            async with self._get_ssh_client(location.name) as ssh_client:
+            async with self._get_ssh_client_process(location.name) as ssh_client:
                 await asyncssh.scp(
                     src, (ssh_client, shared_path), preserve=True, recurse=True
                 )
         else:
             copy_command = ["/bin/cp", "-rf", temp_dir + "/*", dst]
             await self.run(location, copy_command)
 
     async def _copy_remote_to_local(
         self, src: str, dst: str, location: Location, read_only: bool = False
     ) -> None:
         shared_path = self._get_shared_path(location.name, src)
         if shared_path is not None:
-            async with self._get_ssh_client(location.name) as ssh_client:
+            async with self._get_ssh_client_process(location.name) as ssh_client:
                 await asyncssh.scp(
                     (ssh_client, shared_path), dst, preserve=True, recurse=True
                 )
         else:
             temp_dir = await self._get_tmpdir(location.name)
             copy_command = [
                 "/bin/cp",
@@ -252,15 +277,15 @@
                 "basename",
                 "{}",
                 "\\;",
             ]
             contents, _ = await self.run(location, copy_command, capture_output=True)
             contents = contents.split()
             scp_tasks = []
-            async with self._get_ssh_client(location.name) as ssh_client:
+            async with self._get_ssh_client_process(location.name) as ssh_client:
                 for content in contents:
                     scp_tasks.append(
                         asyncio.create_task(
                             asyncssh.scp(
                                 (ssh_client, posixpath.join(temp_dir, content)),
                                 dst,
                                 preserve=True,
@@ -287,35 +312,55 @@
             f"{get_option('s', service.get('shmSize'))}"
             f"{get_option('v', service.get('volumes'))}"
             f"{service['image']} "
             f"{' '.join(service.get('command', ''))}"
         )
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(f"EXECUTING {deploy_command}")
-        async with self._get_ssh_client(name) as ssh_client:
-            result = await ssh_client.run(deploy_command)
-        output = result.stdout
-        search_result = re.findall(f"({node}-[0-9]+).*", output, re.MULTILINE)
-        if search_result:
-            if name not in self.jobs_table:
-                self.jobs_table[name] = []
-            self.jobs_table[name].append(search_result[0])
-            if logger.isEnabledFor(logging.INFO):
-                logger.info(f"Deployed {name} on {search_result[0]}")
-        else:
-            raise Exception
+        async with self._get_ssh_client_process(
+            location=name,
+            command=deploy_command,
+            stdout=asyncio.subprocess.STDOUT,
+            stderr=asyncio.subprocess.STDOUT,
+        ) as proc:
+            result = await proc.wait()
+            output = result.stdout.strip()
+            if result.returncode == 0:
+                search_result = re.findall(f"({node}-[0-9]+).*", output, re.MULTILINE)
+                if search_result:
+                    if name not in self.jobs_table:
+                        self.jobs_table[name] = []
+                    self.jobs_table[name].append(search_result[0])
+                    if logger.isEnabledFor(logging.INFO):
+                        logger.info(f"Deployed {name} on {search_result[0]}")
+                else:
+                    raise WorkflowExecutionException(
+                        f"Failed to deploy {name}: {output}"
+                    )
+            else:
+                raise WorkflowExecutionException(f"Failed to deploy {name}: {output}")
 
     async def _undeploy_node(self, name: str, job_id: str):
         undeploy_command = f"occam-kill {job_id}"
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(f"EXECUTING {undeploy_command}")
-        async with self._get_ssh_client(name) as ssh_client:
-            await ssh_client.run(undeploy_command)
-        if logger.isEnabledFor(logging.INFO):
-            logger.info(f"Killed {job_id}")
+        async with self._get_ssh_client_process(
+            location=name,
+            command=undeploy_command,
+            stdout=asyncio.subprocess.STDOUT,
+            stderr=asyncio.subprocess.STDOUT,
+        ) as proc:
+            result = await proc.wait()
+            if result.returncode == 0:
+                if logger.isEnabledFor(logging.INFO):
+                    logger.info(f"Killed {job_id}")
+            else:
+                raise WorkflowExecutionException(
+                    f"Failed to undeploy {name}: {result.stdout.strip()}"
+                )
 
     async def deploy(self, external: bool) -> None:
         await super().deploy(external)
         if not external:
             deploy_tasks = []
             for name, service in self.env_description.items():
                 nodes = service.get("nodes", ["node22"])
@@ -387,27 +432,30 @@
             workdir=workdir,
             stdin=stdin,
             stdout=stdout,
             stderr=stderr,
             job_name=job_name,
         )
         occam_command = f"occam-exec {location} sh -c '{command}'"
-        async with self._get_ssh_client(location.name) as ssh_client:
-            result = await asyncio.wait_for(
-                ssh_client.run(occam_command), timeout=timeout
-            )
-        if capture_output:
-            lines = (line for line in result.stdout.split("\n"))
-            out = ""
-            for line in lines:
-                if line.startswith("Trying to exec commands into container"):
-                    break
-            try:
-                line = next(lines)
-                out = line.strip(" \r\t")
-            except StopIteration:
-                return out
-            for line in lines:
-                out = "\n".join([out, line.strip(" \r\t")])
-            return out, result.returncode
-        else:
-            return None
+        async with self._get_ssh_client_process(
+            location=location.name,
+            command=occam_command,
+            stdout=asyncio.subprocess.STDOUT,
+            stderr=asyncio.subprocess.STDOUT,
+        ) as proc:
+            result = await proc.wait(timeout=timeout)
+            if capture_output:
+                lines = (line for line in result.stdout.split("\n"))
+                out = ""
+                for line in lines:
+                    if line.startswith("Trying to exec commands into container"):
+                        break
+                try:
+                    line = next(lines)
+                    out = line.strip(" \r\t")
+                except StopIteration:
+                    return out, result.returncode
+                for line in lines:
+                    out = "\n".join([out, line.strip(" \r\t")])
+                return out, result.returncode
+            else:
+                return None
```

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/queue_manager.py` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/queue_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,15 +111,16 @@
         reservation: str | None = None,
         signal: str | None = None,
         socketsPerNode: int | None = None,
         spreadJob: bool = False,
         switches: str | None = None,
         threadSpec: int | None = None,
         threadsPerCore: int | None = None,
-        timeMin: int | None = None,
+        time: str | None = None,
+        timeMin: str | None = None,
         tmp: int | None = None,
         tresPerTask: str | None = None,
         uid: int | str | None = None,
         useMinNodes: bool = False,
         waitAllNodes: bool = False,
         wckey: str | None = None,
     ):
@@ -198,14 +199,15 @@
         self.reservation: str | None = reservation
         self.signal: str | None = signal
         self.socketsPerNode: int | None = socketsPerNode
         self.spreadJob: bool = spreadJob
         self.switches: str | None = switches
         self.threadSpec: int | None = threadSpec
         self.threadsPerCore: int | None = threadsPerCore
+        self.time: str | None = time
         self.timeMin: str | None = timeMin
         self.tmp: int | None = tmp
         self.tresPerTask: str | None = tresPerTask
         self.uid: int | str | None = uid
         self.useMinNodes: bool = useMinNodes
         self.waitAllNodes: bool = waitAllNodes
         self.wckey: str | None = wckey
@@ -275,14 +277,15 @@
         requires: str | None = None,
         rlimit: MutableSequence[str] | None = None,
         setattr: MutableMapping[str, str] | None = None,
         setopt: MutableMapping[str, str] | None = None,
         taskmap: str | None = None,
         tasksPerCore: int | None = None,
         tasksPerNode: int | None = None,
+        timeLimit: str | None = None,
         unbuffered: bool = False,
         urgency: int | None = None,
     ):
         super().__init__(file)
         self.beginTime: str | None = beginTime
         self.brokerOpts: MutableSequence[str] | None = brokerOpts or []
         self.cores: int | None = cores
@@ -305,14 +308,15 @@
         self.requires: str | None = requires
         self.rlimit: MutableSequence[str] | None = rlimit or []
         self.setattr: MutableMapping[str, str] | None = setattr or {}
         self.setopt: MutableMapping[str, str] | None = setopt or {}
         self.taskmap: str | None = taskmap
         self.tasksPerCore: int | None = tasksPerCore
         self.tasksPerNode: int | None = tasksPerNode
+        self.timeLimit: str | None = timeLimit
         self.unbuffered: bool = unbuffered
         self.urgency: int | None = urgency
 
 
 class QueueManagerConnector(ConnectorWrapper, ABC):
     def __init__(
         self,
@@ -335,15 +339,16 @@
         transferBufferSize: int = 2**16,
     ) -> None:
         self._inner_ssh_connector: bool = False
         if hostname is not None:
             if logger.isEnabledFor(logging.WARN):
                 logger.warn(
                     "Inline SSH options are deprecated and will be removed in StreamFlow 0.3.0. "
-                    "Define a standalone SSH connector and link to it using the `connector` property."
+                    f"Define a standalone `SSHConnector` and link the `{self.__class__.__name__}` "
+                    "to it using the `wraps` property."
                 )
             self._inner_ssh_connector = True
             connector: Connector = SSHConnector(
                 deployment_name=f"{deployment_name}-ssh",
                 config_dir=config_dir,
                 checkHostKey=checkHostKey,
                 dataTransferConnection=dataTransferConnection,
@@ -387,14 +392,23 @@
         self.pollingInterval: int = pollingInterval
         self.scheduledJobs: MutableSequence[str] = []
         self.jobsCache: cachetools.Cache = cachetools.TTLCache(
             maxsize=1, ttl=self.pollingInterval
         )
         self.jobsCacheLock: asyncio.Lock = asyncio.Lock()
 
+    def _format_stream(self, stream: int | str) -> str:
+        if stream == asyncio.subprocess.DEVNULL:
+            stream = "/dev/null"
+        elif stream == asyncio.subprocess.PIPE:
+            raise WorkflowExecutionException(
+                f"The `{self.__class__.__name__}` does not support stream pipe redirection."
+            )
+        return shlex.quote(stream)
+
     async def _get_location(self):
         locations = await self.connector.get_available_locations()
         if len(locations) != 1:
             raise WorkflowDefinitionException(
                 f"QueueManager connectors support only nested connectors with a single location. "
                 f"{self.connector.deployment_name} returned {len(locations)} available locations."
             )
@@ -468,15 +482,18 @@
         stderr: int | str = asyncio.subprocess.STDOUT,
         capture_output: bool = False,
         timeout: int | None = None,
         job_name: str | None = None,
     ) -> tuple[Any | None, int] | None:
         if job_name:
             command = utils.create_command(
-                command=command, environment=environment, workdir=workdir
+                class_name=self.__class__.__name__,
+                command=command,
+                environment=environment,
+                workdir=workdir,
             )
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(
                     "EXECUTING command {command} on {location} {job}".format(
                         command=command,
                         location=location,
                         job=f"for job {job_name}" if job_name else "",
@@ -662,20 +679,20 @@
             "|",
             "base64",
             "-d",
             "|",
             "sbatch",
             "--parsable",
         ]
-        if stdin is not None:
+        if stdin is not None and stdin != asyncio.subprocess.DEVNULL:
             batch_command.append(get_option("input", shlex.quote(stdin)))
         if stderr != asyncio.subprocess.STDOUT and stderr != stdout:
-            batch_command.append(get_option("error", shlex.quote(stderr)))
+            batch_command.append(get_option("error", self._format_stream(stderr)))
         if stdout != asyncio.subprocess.STDOUT:
-            batch_command.append(get_option("output", shlex.quote(stdout)))
+            batch_command.append(get_option("output", self._format_stream(stdout)))
         if timeout:
             batch_command.append(
                 get_option("time", utils.format_seconds_to_hhmmss(timeout))
             )
         if service := cast(SlurmService, self.services.get(location.service)):
             batch_command.extend(
                 [
@@ -763,14 +780,16 @@
                     get_option("tres-per-task", service.tresPerTask),
                     get_option("uid", service.uid),
                     get_option("use-min_nodes", service.useMinNodes),
                     get_option("wait-all-nodes", 1 if service.waitAllNodes else 0),
                     get_option("wckey", service.wckey),
                 ]
             )
+            if not timeout:
+                batch_command.append(get_option("time", service.time))
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(f"Running command {' '.join(batch_command)}")
         stdout, returncode = await self.connector.run(
             location=location, command=batch_command, capture_output=True
         )
         if returncode == 0:
             return stdout.strip()
@@ -867,18 +886,18 @@
                         stdout
                         if stdout != asyncio.subprocess.STDOUT
                         else utils.random_name()
                     ),
                 ),
             ]
         )
-        if stdin is not None:
+        if stdin is not None and stdin != asyncio.subprocess.DEVNULL:
             batch_command.append(get_option("i", stdin))
         if stderr != asyncio.subprocess.STDOUT and stderr != stdout:
-            batch_command.append(get_option("e", stderr))
+            batch_command.append(get_option("e", self._format_stream(stderr)))
         if stderr == stdout:
             batch_command.append(get_option("j", "oe"))
         if service := cast(PBSService, self.services.get(location.service)):
             resources = {**service.resources, **resources}
             batch_command.extend(
                 [
                     get_option("a", service.begin),
@@ -1036,22 +1055,24 @@
             "-d",
             "|",
             "flux",
             "batch",
         ]
         if workdir is not None:
             batch_command.append(get_option("cwd", workdir))
-        if stdin is not None:
+        if stdin is not None and stdin != asyncio.subprocess.DEVNULL:
             batch_command.append(get_option("input", shlex.quote(stdin)))
         if stdout != asyncio.subprocess.STDOUT:
-            batch_command.append(get_option("output", shlex.quote(stdout)))
+            batch_command.append(get_option("output", self._format_stream(stdout)))
         if stderr != asyncio.subprocess.STDOUT and stderr != stdout:
-            batch_command.append(get_option("error", shlex.quote(stderr)))
+            batch_command.append(get_option("error", self._format_stream(stderr)))
         if timeout:
-            batch_command.extend(["-t", utils.format_seconds_to_hhmmss(timeout)])
+            batch_command.append(
+                get_option("time-limit", utils.format_seconds_to_hhmmss(timeout))
+            )
         nodes = 1
         if service := cast(FluxService, self.services.get(location.service)):
             nodes = service.nodes
             batch_command.extend(
                 [
                     get_option("begin-time", service.beginTime),
                     get_option("broker-opts", service.brokerOpts),
@@ -1082,14 +1103,16 @@
                     get_option("taskmap", service.taskmap),
                     get_option("tasks-per-core", service.tasksPerCore),
                     get_option("tasks-per-node", service.tasksPerNode),
                     get_option("unbuffered", service.unbuffered),
                     get_option("urgency", service.urgency),
                 ]
             )
+            if not timeout:
+                batch_command.append(get_option("time-limit", service.timeLimit))
         batch_command.append(get_option("nodes", nodes))
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(f"Running command {' '.join(batch_command)}")
         stdout, returncode = await self.connector.run(
             location=location, command=batch_command, capture_output=True
         )
         if returncode == 0:
```

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/docker-compose.json` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/docker-compose.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/docker.json` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/docker.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/flux.json` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/flux.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998511904761905%*

 * *Differences: {"'$defs'": "{'service': {'properties': {'timeLimit': OrderedDict([('type', 'string'), "*

 * *            "('description', 'Time limit in minutes when no units provided, otherwise in Flux "*

 * *            'standard duration (e.g., 30s, 2d, 1.5h). If a `timeout` value is defined directly in '*

 * *            "the workflow specification, it will override this value')])}}}"}*

```diff
@@ -122,14 +122,18 @@
                     "description": "Force a number of tasks per core",
                     "type": "integer"
                 },
                 "tasksPerNode": {
                     "description": "Set the number of tasks per node to run",
                     "type": "integer"
                 },
+                "timeLimit": {
+                    "description": "Time limit in minutes when no units provided, otherwise in Flux standard duration (e.g., 30s, 2d, 1.5h). If a `timeout` value is defined directly in the workflow specification, it will override this value",
+                    "type": "string"
+                },
                 "unbuffered": {
                     "description": "Disable buffering of standard input and output as much as practical",
                     "type": "boolean"
                 },
                 "urgency": {
                     "description": "Specify job urgency, which affects queue order. Numerically higher urgency jobs are considered by the scheduler first",
                     "type": "integer"
```

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/helm3.json` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/helm3.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/kubernetes.json` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/kubernetes.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/occam.json` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/occam.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/pbs.json` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/pbs.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/queue_manager.json` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/queue_manager.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/singularity.json` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/singularity.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/slurm.json` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/slurm.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999492694805195%*

 * *Differences: {"'$defs'": "{'service': {'properties': {'time': OrderedDict([('type', 'string'), ('description', "*

 * *            "'Set a limit on the total run time of the job allocation. If a `timeout` value is "*

 * *            "defined directly in the workflow specification, it will override this value')])}}}"}*

```diff
@@ -347,14 +347,18 @@
                     "description": "Count of specialized threads per node reserved by the job for system operations and not used by the application. The application will not use these threads, but will be charged for their allocation",
                     "type": "integer"
                 },
                 "threadsPerCore": {
                     "description": "Restrict node selection to nodes with at least the specified number of threads per core. In task layout, use the specified maximum number of threads per core",
                     "type": "integer"
                 },
+                "time": {
+                    "description": "Set a limit on the total run time of the job allocation. If a `timeout` value is defined directly in the workflow specification, it will override this value",
+                    "type": "string"
+                },
                 "timeMin": {
                     "description": "Set a minimum time limit on the job allocation. If specified, the job may have its time limit lowered to a value no lower than timeMin if doing so permits the job to begin execution earlier than otherwise possible",
                     "type": "string"
                 },
                 "tmp": {
                     "description": "Specify a minimum amount of temporary disk space per node. Default units are megabytes",
                     "type": "integer"
```

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/schemas/ssh.json` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/schemas/ssh.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'required'": '{delete: [1]}'}*

```diff
@@ -151,12 +151,11 @@
         },
         "username": {
             "description": "Username needed to connect with the SSH environment",
             "type": "string"
         }
     },
     "required": [
-        "nodes",
-        "username"
+        "nodes"
     ],
     "type": "object"
 }
```

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/connector/ssh.py` & `streamflow-0.2.0.dev9/streamflow/deployment/connector/ssh.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import posixpath
 import tarfile
 from pathlib import PurePosixPath
 from typing import Any, MutableMapping, MutableSequence
 
 import asyncssh
 import pkg_resources
+from asyncssh import ChannelOpenError
 from cachetools import Cache, LRUCache
 
 from streamflow.core import utils
 from streamflow.core.asyncache import cachedmethod
 from streamflow.core.data import StreamWrapperContext
 from streamflow.core.deployment import Connector, Location
 from streamflow.core.exception import WorkflowExecutionException
@@ -22,30 +23,14 @@
 from streamflow.deployment import aiotarstream
 from streamflow.deployment.connector.base import BaseConnector, extract_tar_stream
 from streamflow.deployment.stream import StreamReaderWrapper, StreamWriterWrapper
 from streamflow.deployment.template import CommandTemplateMap
 from streamflow.log_handler import logger
 
 
-async def _get_disk_usage(
-    ssh_client: asyncssh.SSHClientConnection, directory: str
-) -> float:
-    if directory:
-        result = await ssh_client.run(
-            f"df {directory} | tail -n 1 | awk '{{print $2}}'",
-            stderr=asyncio.subprocess.STDOUT,
-        )
-        if result.returncode == 0:
-            return float(result.stdout.strip()) / 2**10
-        else:
-            raise WorkflowExecutionException(result.returncode)
-    else:
-        return float("inf")
-
-
 def _parse_hostname(hostname):
     if ":" in hostname:
         hostname, port = hostname.split(":")
         port = int(port)
     else:
         port = 22
     return hostname, port
@@ -58,24 +43,29 @@
         config: SSHConfig,
         max_concurrent_sessions: int,
     ):
         self._streamflow_config_dir: str = streamflow_config_dir
         self._config: SSHConfig = config
         self._max_concurrent_sessions: int = max_concurrent_sessions
         self._ssh_connection: asyncssh.SSHClientConnection | None = None
-        self._sessions: int = 0
+        self._connecting = False
+        self._connect_event: asyncio.Event = asyncio.Event()
 
-    async def __aenter__(self):
+    async def get_connection(self) -> asyncssh.SSHClientConnection:
         if self._ssh_connection is None:
-            self._ssh_connection = await self._get_connection(self._config)
-        self._sessions += 1
+            if not self._connecting:
+                self._connecting = True
+                self._ssh_connection = await self._get_connection(self._config)
+                self._connect_event.set()
+            else:
+                await self._connect_event.wait()
         return self._ssh_connection
 
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        self._sessions -= 1
+    def get_hostname(self) -> str:
+        return self._config.hostname
 
     async def _get_connection(
         self, config: SSHConfig
     ) -> asyncssh.SSHClientConnection | None:
         if config is None:
             return None
         (hostname, port) = _parse_hostname(config.hostname)
@@ -114,39 +104,70 @@
             return f.read().strip()
 
     async def close(self):
         if self._ssh_connection is not None:
             self._ssh_connection.close()
 
     def full(self) -> bool:
-        return self._sessions == self._max_concurrent_sessions
+        if self._ssh_connection:
+            return len(self._ssh_connection._channels) >= self._max_concurrent_sessions
+        else:
+            return False
 
 
 class SSHContextManager:
     def __init__(
-        self, condition: asyncio.Condition, contexts: MutableSequence[SSHContext]
+        self,
+        condition: asyncio.Condition,
+        contexts: MutableSequence[SSHContext],
+        command: str,
+        stdin: int = asyncio.subprocess.PIPE,
+        stdout: int = asyncio.subprocess.PIPE,
+        stderr: int = asyncio.subprocess.PIPE,
+        encoding: str | None = "utf-8",
     ):
+        self.command: str = command
+        self.stdin: int = stdin
+        self.stdout: int = stdout
+        self.stderr: int = stderr
+        self.encoding: str | None = encoding
         self._condition: asyncio.Condition = condition
         self._contexts: MutableSequence[SSHContext] = contexts
         self._selected_context: SSHContext | None = None
+        self._proc: asyncssh.SSHClientProcess | None = None
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> asyncssh.SSHClientProcess:
         async with self._condition:
             while True:
                 for context in self._contexts:
                     if not context.full():
-                        ssh_connection = await context.__aenter__()
-                        self._selected_context = context
-                        return ssh_connection
+                        ssh_connection = await context.get_connection()
+                        try:
+                            self._selected_context = context
+                            self._proc = await ssh_connection.create_process(
+                                self.command,
+                                stdin=self.stdin,
+                                stdout=self.stdout,
+                                stderr=self.stderr,
+                                encoding=self.encoding,
+                            )
+                            await self._proc.__aenter__()
+                            return self._proc
+                        except ChannelOpenError as coe:
+                            logger.warning(
+                                f"Error opening SSH session to {context.get_hostname()} "
+                                f"to execute command `{self.command}`: [{coe.code}] {coe.reason}"
+                            )
                 await self._condition.wait()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         async with self._condition:
             if self._selected_context:
-                await self._selected_context.__aexit__(exc_type, exc_val, exc_tb)
+                if self._proc:
+                    await self._proc.__aexit__(exc_type, exc_val, exc_tb)
                 self._condition.notify_all()
 
 
 class SSHContextFactory:
     def __init__(
         self,
         streamflow_config_dir: str,
@@ -163,44 +184,55 @@
             )
             for _ in range(max_connections)
         ]
 
     async def close(self):
         await asyncio.gather(*(asyncio.create_task(c.close()) for c in self._contexts))
 
-    def get(self):
-        return SSHContextManager(condition=self._condition, contexts=self._contexts)
+    def get(
+        self,
+        command: str,
+        stdin: int = asyncio.subprocess.PIPE,
+        stdout: int = asyncio.subprocess.PIPE,
+        stderr: int = asyncio.subprocess.PIPE,
+        encoding: str | None = "utf-8",
+    ):
+        return SSHContextManager(
+            condition=self._condition,
+            contexts=self._contexts,
+            command=command,
+            stdin=stdin,
+            stdout=stdout,
+            stderr=stderr,
+            encoding=encoding,
+        )
 
 
 class SSHStreamWrapperContext(StreamWrapperContext):
-    def __init__(self, src: str, ssh_context: SSHContextManager):
+    def __init__(self, src: str, ssh_context_factory: SSHContextFactory):
         super().__init__()
         self.src: str = src
-        self.ssh_context: SSHContextManager = ssh_context
-        self.ssh_process: asyncssh.SSHClientProcess | None = None
+        self.ssh_context_factory: SSHContextFactory = ssh_context_factory
+        self.ssh_context: SSHContextManager | None = None
         self.stream: StreamReaderWrapper | None = None
 
     async def __aenter__(self):
-        ssh_client = await self.ssh_context.__aenter__()
         dirname, basename = posixpath.split(self.src)
-        self.ssh_process = await (
-            await ssh_client.create_process(
-                f"tar chf - -C {dirname} {basename}",
-                stdin=asyncio.subprocess.DEVNULL,
-                encoding=None,
-            )
-        ).__aenter__()
-        self.stream = StreamReaderWrapper(self.ssh_process.stdout)
+        self.ssh_context = self.ssh_context_factory.get(
+            command=f"tar chf - -C {dirname} {basename}",
+            stdin=asyncio.subprocess.DEVNULL,
+            encoding=None,
+        )
+        proc = await self.ssh_context.__aenter__()
+        self.stream = StreamReaderWrapper(proc.stdout)
         return self.stream
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         if self.stream:
             await self.stream.close()
-        if self.ssh_process:
-            await self.ssh_process.__aexit__(exc_type, exc_val, exc_tb)
         await self.ssh_context.__aexit__(exc_type, exc_val, exc_tb)
 
 
 class SSHConfig:
     def __init__(
         self,
         check_host_key: bool,
@@ -217,47 +249,20 @@
         self.password_file: str | None = password_file
         self.ssh_key_passphrase_file: str | None = ssh_key_passphrase_file
         self.tunnel: SSHConfig | None = tunnel
         self.username: str = username
 
 
 class SSHConnector(BaseConnector):
-    @staticmethod
-    def _get_command(
-        location: Location,
-        command: MutableSequence[str],
-        environment: MutableMapping[str, str] = None,
-        workdir: str | None = None,
-        stdin: int | str | None = None,
-        stdout: int | str = asyncio.subprocess.STDOUT,
-        stderr: int | str = asyncio.subprocess.STDOUT,
-        job_name: str | None = None,
-    ):
-        command = utils.create_command(
-            command=command,
-            environment=environment,
-            workdir=workdir,
-            stdin=stdin,
-            stdout=stdout,
-            stderr=stderr,
-        )
-        if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(
-                f"EXECUTING command {command} on {location}" f" for job {job_name}"
-                if job_name
-                else ""
-            )
-        return utils.encode_command(command)
-
     def __init__(
         self,
         deployment_name: str,
         config_dir: str,
         nodes: MutableSequence[Any],
-        username: str,
+        username: str | None = None,
         checkHostKey: bool = True,
         dataTransferConnection: str | MutableMapping[str, Any] | None = None,
         file: str | None = None,
         maxConcurrentSessions: int = 10,
         maxConnections: int = 1,
         passwordFile: str | None = None,
         services: MutableMapping[str, str] | None = None,
@@ -312,56 +317,56 @@
             n.hostname: n for n in [self._get_config(n) for n in nodes]
         }
         self.hardwareCache: Cache = LRUCache(maxsize=len(self.nodes))
 
     async def _copy_local_to_remote_single(
         self, src: str, dst: str, location: Location, read_only: bool = False
     ):
-        async with self._get_data_transfer_client(location.name) as ssh_client:
-            async with ssh_client.create_process(
-                "tar xf - -C /",
-                stderr=asyncio.subprocess.DEVNULL,
-                stdout=asyncio.subprocess.DEVNULL,
-                encoding=None,
-            ) as proc:
-                try:
-                    async with aiotarstream.open(
-                        stream=StreamWriterWrapper(proc.stdin),
-                        format=tarfile.GNU_FORMAT,
-                        mode="w",
-                        dereference=True,
-                        copybufsize=self.transferBufferSize,
-                    ) as tar:
-                        await tar.add(src, arcname=dst)
-                except tarfile.TarError as e:
-                    raise WorkflowExecutionException(
-                        f"Error copying {src} to {dst} on location {location}: {e}"
-                    ) from e
+        async with self._get_data_transfer_process(
+            location=location.name,
+            command="tar xf - -C /",
+            stderr=asyncio.subprocess.DEVNULL,
+            stdout=asyncio.subprocess.DEVNULL,
+            encoding=None,
+        ) as proc:
+            try:
+                async with aiotarstream.open(
+                    stream=StreamWriterWrapper(proc.stdin),
+                    format=tarfile.GNU_FORMAT,
+                    mode="w",
+                    dereference=True,
+                    copybufsize=self.transferBufferSize,
+                ) as tar:
+                    await tar.add(src, arcname=dst)
+            except tarfile.TarError as e:
+                raise WorkflowExecutionException(
+                    f"Error copying {src} to {dst} on location {location}: {e}"
+                ) from e
 
     async def _copy_remote_to_local(
         self, src: str, dst: str, location: Location, read_only: bool = False
     ) -> None:
         dirname, basename = posixpath.split(src)
-        async with self._get_data_transfer_client(location.name) as ssh_client:
-            async with ssh_client.create_process(
-                f"tar chf - -C {dirname} {basename}",
-                stdin=asyncio.subprocess.DEVNULL,
-                encoding=None,
-            ) as proc:
-                try:
-                    async with aiotarstream.open(
-                        stream=StreamReaderWrapper(proc.stdout),
-                        mode="r",
-                        copybufsize=self.transferBufferSize,
-                    ) as tar:
-                        await extract_tar_stream(tar, src, dst, self.transferBufferSize)
-                except tarfile.TarError as e:
-                    raise WorkflowExecutionException(
-                        f"Error copying {src} from location {location} to {dst}: {e}"
-                    ) from e
+        async with self._get_data_transfer_process(
+            location=location.name,
+            command=f"tar chf - -C {dirname} {basename}",
+            stdin=asyncio.subprocess.DEVNULL,
+            encoding=None,
+        ) as proc:
+            try:
+                async with aiotarstream.open(
+                    stream=StreamReaderWrapper(proc.stdout),
+                    mode="r",
+                    copybufsize=self.transferBufferSize,
+                ) as tar:
+                    await extract_tar_stream(tar, src, dst, self.transferBufferSize)
+            except tarfile.TarError as e:
+                raise WorkflowExecutionException(
+                    f"Error copying {src} from location {location} to {dst}: {e}"
+                ) from e
 
     async def _copy_remote_to_remote(
         self,
         src: str,
         dst: str,
         locations: MutableSequence[Location],
         source_location: Location,
@@ -383,43 +388,41 @@
                 src=src,
                 dst_connector=self,
                 dst_locations=locations,
                 dst=dst,
             )
         )
         if locations:
-            async with source_connector._get_stream_reader(
-                source_location, src
-            ) as reader:
-                async with contextlib.AsyncExitStack() as exit_stack:
-                    # Open a target StreamWriter for each location
-                    writer_clients = await asyncio.gather(
-                        *(
-                            asyncio.create_task(
-                                exit_stack.enter_async_context(
-                                    self._get_data_transfer_client(location.name)
-                                )
-                            )
-                            for location in locations
-                        )
-                    )
-                    async with contextlib.AsyncExitStack() as writers_stack:
+            conn_per_round = min(len(locations), self.maxConcurrentSessions)
+            rounds = self.maxConcurrentSessions // conn_per_round
+            if len(locations) % conn_per_round != 0:
+                rounds += 1
+            location_groups = [
+                locations[i : i + rounds] for i in range(0, len(locations), rounds)
+            ]
+            for location_group in location_groups:
+                async with source_connector._get_stream_reader(
+                    source_location, src
+                ) as reader:
+                    async with contextlib.AsyncExitStack() as exit_stack:
+                        # Open a target StreamWriter for each location
                         writers = await asyncio.gather(
                             *(
                                 asyncio.create_task(
-                                    writers_stack.enter_async_context(
-                                        client.create_process(
-                                            write_command,
+                                    exit_stack.enter_async_context(
+                                        self._get_data_transfer_process(
+                                            location=location.name,
+                                            command=write_command,
                                             stderr=asyncio.subprocess.DEVNULL,
                                             stdout=asyncio.subprocess.DEVNULL,
                                             encoding=None,
                                         )
                                     )
                                 )
-                                for client in writer_clients
+                                for location in location_group
                             )
                         )
                         # Multiplex the reader output to all the writers
                         while content := await reader.read(
                             source_connector.transferBufferSize
                         ):
                             for writer in writers:
@@ -427,14 +430,42 @@
                             await asyncio.gather(
                                 *(
                                     asyncio.create_task(writer.stdin.drain())
                                     for writer in writers
                                 )
                             )
 
+    def _get_command(
+        self,
+        location: Location,
+        command: MutableSequence[str],
+        environment: MutableMapping[str, str] = None,
+        workdir: str | None = None,
+        stdin: int | str | None = None,
+        stdout: int | str = asyncio.subprocess.STDOUT,
+        stderr: int | str = asyncio.subprocess.STDOUT,
+        job_name: str | None = None,
+    ):
+        command = utils.create_command(
+            class_name=self.__class__.__name__,
+            command=command,
+            environment=environment,
+            workdir=workdir,
+            stdin=stdin,
+            stdout=stdout,
+            stderr=stderr,
+        )
+        if logger.isEnabledFor(logging.DEBUG):
+            logger.debug(
+                f"EXECUTING command {command} on {location}" f" for job {job_name}"
+                if job_name
+                else ""
+            )
+        return utils.encode_command(command)
+
     def _get_config(self, node: str | MutableMapping[str, Any]):
         if node is None:
             return None
         elif isinstance(node, str):
             node = {"hostname": node}
         ssh_key = node["sshKey"] if "sshKey" in node else self.sshKey
         return SSHConfig(
@@ -457,36 +488,83 @@
                 if "tunnel" in node
                 else self.tunnel
                 if hasattr(self, "tunnel")
                 else None
             ),
         )
 
-    def _get_data_transfer_client(self, location: str) -> SSHContextManager:
+    async def _get_cores(self, location: str) -> float:
+        async with self._get_ssh_client_process(
+            location=location, command="nproc", stderr=asyncio.subprocess.STDOUT
+        ) as proc:
+            result = await proc.wait()
+            if result.returncode == 0:
+                return float(result.stdout.strip())
+            else:
+                raise WorkflowExecutionException(result.returncode)
+
+    def _get_data_transfer_process(
+        self,
+        location: str,
+        command: str,
+        stdin: int = asyncio.subprocess.PIPE,
+        stdout: int = asyncio.subprocess.PIPE,
+        stderr: int = asyncio.subprocess.PIPE,
+        encoding: str | None = "utf-8",
+    ) -> SSHContextManager:
         if self.dataTransferConfig:
             if location not in self.data_transfer_context_factories:
                 self.data_transfer_context_factories[location] = SSHContextFactory(
                     streamflow_config_dir=self.config_dir,
                     config=self.dataTransferConfig,
                     max_concurrent_sessions=self.maxConcurrentSessions,
                     max_connections=self.maxConnections,
                 )
-            return self.data_transfer_context_factories[location].get()
+            return self.data_transfer_context_factories[location].get(
+                command=command,
+                stdin=stdin,
+                stdout=stdout,
+                stderr=stderr,
+                encoding=encoding,
+            )
         else:
-            return self._get_ssh_client(location)
+            return self._get_ssh_client_process(
+                location=location,
+                command=command,
+                stdin=stdin,
+                stdout=stdout,
+                stderr=stderr,
+                encoding=encoding,
+            )
+
+    async def _get_disk_usage(self, location: str, directory: str) -> float:
+        async with self._get_ssh_client_process(
+            location=location,
+            command=f"df {directory} | tail -n 1 | awk '{{print $2}}'",
+            stderr=asyncio.subprocess.STDOUT,
+        ) as proc:
+            if directory:
+                result = await proc.wait()
+                if result.returncode == 0:
+                    return float(result.stdout.strip()) / 2**10
+                else:
+                    raise WorkflowExecutionException(result.returncode)
+            else:
+                return float("inf")
 
     async def _get_existing_parent(self, location: str, directory: str):
         if directory is None:
             return None
-        async with self._get_ssh_client(location) as ssh_client:
+        async with self._get_ssh_client_process(
+            location=location,
+            command=f'test -e "{directory}"',
+            stderr=asyncio.subprocess.STDOUT,
+        ) as proc:
             while True:
-                result = await ssh_client.run(
-                    f'test -e "{directory}"',
-                    stderr=asyncio.subprocess.STDOUT,
-                )
+                result = await proc.wait()
                 if result.returncode == 0:
                     return directory
                 elif result.returncode == 1:
                     directory = PurePosixPath(directory).parent
                 else:
                     raise WorkflowExecutionException(result.stdout.strip())
 
@@ -494,72 +572,83 @@
     async def _get_location_hardware(
         self,
         location: str,
         input_directory: str,
         output_directory: str,
         tmp_directory: str,
     ) -> Hardware:
-        try:
-            async with self._get_ssh_client(location) as ssh_client:
-                (
-                    cores,
-                    memory,
-                    input_directory,
-                    output_directory,
-                    tmp_directory,
-                ) = await asyncio.gather(
-                    asyncio.create_task(
-                        ssh_client.run("nproc", stderr=asyncio.subprocess.STDOUT)
-                    ),
-                    asyncio.create_task(
-                        ssh_client.run(
-                            "free | grep Mem | awk '{print $2}'",
-                            stderr=asyncio.subprocess.STDOUT,
-                        )
-                    ),
-                    asyncio.create_task(_get_disk_usage(ssh_client, input_directory)),
-                    asyncio.create_task(_get_disk_usage(ssh_client, output_directory)),
-                    asyncio.create_task(_get_disk_usage(ssh_client, tmp_directory)),
-                )
-                if cores.returncode == 0 and memory.returncode == 0:
-                    return Hardware(
-                        cores=float(cores.stdout.strip()),
-                        memory=float(memory.stdout.strip()) / 2**10,
-                        input_directory=input_directory,
-                        output_directory=output_directory,
-                        tmp_directory=tmp_directory,
-                    )
-                else:
-                    raise WorkflowExecutionException(
-                        f"Impossible to retrieve locations for {location}"
-                    )
-        except WorkflowExecutionException:
-            raise WorkflowExecutionException(
-                f"Impossible to retrieve locations for {location}"
-            )
+        return Hardware(
+            await self._get_cores(location),
+            await self._get_memory(location),
+            await self._get_disk_usage(location, input_directory),
+            await self._get_disk_usage(location, output_directory),
+            await self._get_disk_usage(location, tmp_directory),
+        )
+
+    async def _get_memory(self, location: str) -> float:
+        async with self._get_ssh_client_process(
+            location=location,
+            command="free | grep Mem | awk '{print $2}'",
+            stderr=asyncio.subprocess.STDOUT,
+        ) as proc:
+            result = await proc.wait()
+            if result.returncode == 0:
+                return float(result.stdout.strip()) / 2**10
+            else:
+                raise WorkflowExecutionException(result.returncode)
 
     def _get_run_command(
         self, command: str, location: Location, interactive: bool = False
     ):
         return f"ssh {location.name} {command}"
 
-    def _get_ssh_client(self, location: str) -> SSHContextManager:
+    def _get_ssh_client_process(
+        self,
+        location: str,
+        command: str,
+        stdin: int = asyncio.subprocess.PIPE,
+        stdout: int = asyncio.subprocess.PIPE,
+        stderr: int = asyncio.subprocess.PIPE,
+        encoding: str | None = "utf-8",
+    ) -> SSHContextManager:
         if location not in self.ssh_context_factories:
             self.ssh_context_factories[location] = SSHContextFactory(
                 streamflow_config_dir=self.config_dir,
                 config=self.nodes[location],
                 max_concurrent_sessions=self.maxConcurrentSessions,
                 max_connections=self.maxConnections,
             )
-        return self.ssh_context_factories[location].get()
+        return self.ssh_context_factories[location].get(
+            command=command,
+            stdin=stdin,
+            stdout=stdout,
+            stderr=stderr,
+            encoding=encoding,
+        )
 
     def _get_stream_reader(self, location: Location, src: str) -> StreamWrapperContext:
-        return SSHStreamWrapperContext(
-            src=src, ssh_context=self._get_data_transfer_client(location.name)
-        )
+        if self.dataTransferConfig:
+            if location not in self.data_transfer_context_factories:
+                self.data_transfer_context_factories[location.name] = SSHContextFactory(
+                    streamflow_config_dir=self.config_dir,
+                    config=self.dataTransferConfig,
+                    max_concurrent_sessions=self.maxConcurrentSessions,
+                    max_connections=self.maxConnections,
+                )
+            ssh_context_factory = self.data_transfer_context_factories[location.name]
+        else:
+            if location not in self.ssh_context_factories:
+                self.ssh_context_factories[location.name] = SSHContextFactory(
+                    streamflow_config_dir=self.config_dir,
+                    config=self.nodes[location.name],
+                    max_concurrent_sessions=self.maxConcurrentSessions,
+                    max_connections=self.maxConnections,
+                )
+            ssh_context_factory = self.ssh_context_factories[location.name]
+        return SSHStreamWrapperContext(src=src, ssh_context_factory=ssh_context_factory)
 
     async def deploy(self, external: bool) -> None:
         pass
 
     async def get_available_locations(
         self,
         service: str | None = None,
@@ -628,28 +717,27 @@
             command = self.template_map.get_command(
                 command=command,
                 template=location.service,
                 environment=environment,
                 workdir=workdir,
             )
             command = utils.encode_command(command)
-            async with self._get_ssh_client(location.name) as ssh_client:
-                result = await asyncio.wait_for(
-                    ssh_client.run(command, stderr=asyncio.subprocess.STDOUT),
-                    timeout=timeout,
-                )
+            async with self._get_ssh_client_process(
+                location=location.name,
+                command=command,
+                stderr=asyncio.subprocess.STDOUT,
+            ) as proc:
+                result = await proc.wait(timeout=timeout)
         else:
-            async with self._get_ssh_client(location.name) as ssh_client:
-                result = await asyncio.wait_for(
-                    ssh_client.run(
-                        command,
-                        stderr=asyncio.subprocess.STDOUT,
-                    ),
-                    timeout=timeout,
-                )
+            async with self._get_ssh_client_process(
+                location=location.name,
+                command=command,
+                stderr=asyncio.subprocess.STDOUT,
+            ) as proc:
+                result = await proc.wait(timeout=timeout)
         return result.stdout.strip(), result.returncode if capture_output else None
 
     async def undeploy(self, external: bool) -> None:
         for ssh_context in self.ssh_context_factories.values():
             await ssh_context.close()
         self.ssh_context_factories = {}
         for ssh_context in self.data_transfer_context_factories.values():
```

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/filter/shuffle.py` & `streamflow-0.2.0.dev9/streamflow/deployment/filter/shuffle.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/future.py` & `streamflow-0.2.0.dev9/streamflow/deployment/future.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/manager.py` & `streamflow-0.2.0.dev9/streamflow/deployment/manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/stream.py` & `streamflow-0.2.0.dev9/streamflow/deployment/stream.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/template.py` & `streamflow-0.2.0.dev9/streamflow/deployment/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,13 +22,13 @@
         self,
         command: str,
         template: str | None = None,
         environment: MutableMapping[str, str] = None,
         workdir: str = None,
         **kwargs,
     ) -> str:
-        return self.templates[template or "__DEFAULT__"].render(
+        return self.templates.get(template, self.templates["__DEFAULT__"]).render(
             streamflow_command=command,
             streamflow_environment=environment,
             streamflow_workdir=workdir,
             **kwargs,
         )
```

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/utils.py` & `streamflow-0.2.0.dev9/streamflow/deployment/utils.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/deployment/wrapper.py` & `streamflow-0.2.0.dev9/streamflow/deployment/wrapper.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/ext/plugin.py` & `streamflow-0.2.0.dev9/streamflow/ext/plugin.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/ext/utils.py` & `streamflow-0.2.0.dev9/streamflow/ext/utils.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/log_handler.py` & `streamflow-0.2.0.dev9/streamflow/log_handler.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/main.py` & `streamflow-0.2.0.dev9/streamflow/main.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/parser.py` & `streamflow-0.2.0.dev9/streamflow/parser.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/persistence/base.py` & `streamflow-0.2.0.dev9/streamflow/persistence/base.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/persistence/loading_context.py` & `streamflow-0.2.0.dev9/streamflow/persistence/loading_context.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/persistence/schemas/sqlite.json` & `streamflow-0.2.0.dev9/streamflow/persistence/schemas/sqlite.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/persistence/schemas/sqlite.sql` & `streamflow-0.2.0.dev9/streamflow/persistence/schemas/sqlite.sql`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/persistence/sqlite.py` & `streamflow-0.2.0.dev9/streamflow/persistence/sqlite.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 class SqliteConnection:
     def __init__(self, connection: str, timeout: int, init_db: bool):
         self.connection: str = connection
         self.timeout: int = timeout
         self.init_db: bool = init_db
         self._connection: aiosqlite.Connection | None = None
-        self.__row_factory = None
 
     async def __aenter__(self):
         if not self._connection:
             self._connection = await aiosqlite.connect(
                 database=self.connection, timeout=self.timeout
             )
             if self.init_db:
@@ -41,19 +40,19 @@
                     __name__, os.path.join("schemas", "sqlite.sql")
                 )
                 with open(schema_path) as f:
                     async with self._connection.cursor() as cursor:
                         await cursor.execute("PRAGMA journal_mode = WAL")
                         await cursor.execute("PRAGMA wal_autocheckpoint = 10")
                         await cursor.executescript(f.read())
-        self.__row_factory = self._connection.row_factory
+            self._connection.row_factory = aiosqlite.Row
         return self._connection
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
-        self._connection.row_factory = self.__row_factory
+        pass
 
     async def close(self):
         if self._connection:
             await self._connection.close()
 
 
 class SqliteDatabase(CachedDatabase):
@@ -240,102 +239,93 @@
             ) as cursor:
                 return cursor.lastrowid
 
     async def get_dependees(
         self, token_id: int
     ) -> MutableSequence[MutableMapping[str, Any]]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM provenance WHERE depender = :depender",
                 {"depender": token_id},
             ) as cursor:
                 return await cursor.fetchall()
 
     async def get_dependers(
         self, token_id: int
     ) -> MutableSequence[MutableMapping[str, Any]]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM provenance WHERE dependee = :dependee",
                 {"dependee": token_id},
             ) as cursor:
                 return await cursor.fetchall()
 
     async def get_command(self, command_id: int) -> MutableMapping[str, Any]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM command WHERE id = :id", {"id": command_id}
             ) as cursor:
                 return await cursor.fetchone()
 
     async def get_commands_by_step(
         self, step_id: int
     ) -> MutableSequence[MutableMapping[str, Any]]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM command WHERE step = :id", {"id": step_id}
             ) as cursor:
                 return await cursor.fetchall()
 
     @cachedmethod(lambda self: self.deployment_cache)
     async def get_deployment(self, deplyoment_id: int) -> MutableMapping[str, Any]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM deployment WHERE id = :id", {"id": deplyoment_id}
             ) as cursor:
                 return await cursor.fetchone()
 
     async def get_input_ports(
         self, step_id: int
     ) -> MutableSequence[MutableMapping[str, Any]]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM dependency WHERE step = :step AND type = :type",
                 {"step": step_id, "type": DependencyType.INPUT.value},
             ) as cursor:
                 return await cursor.fetchall()
 
     async def get_output_ports(
         self, step_id: int
     ) -> MutableSequence[MutableMapping[str, Any]]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM dependency WHERE step = :step AND type = :type",
                 {"step": step_id, "type": DependencyType.OUTPUT.value},
             ) as cursor:
                 return await cursor.fetchall()
 
     @cachedmethod(lambda self: self.port_cache)
     async def get_port(self, port_id: int) -> MutableMapping[str, Any]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM port WHERE id = :id", {"id": port_id}
             ) as cursor:
                 return await cursor.fetchone()
 
     async def get_port_tokens(self, port_id: int) -> MutableSequence[int]:
         async with self.connection as db:
             async with db.execute(
                 "SELECT id FROM token WHERE port = :port", {"port": port_id}
             ) as cursor:
-                return [row[0] for row in await cursor.fetchall()]
+                return [row["id"] for row in await cursor.fetchall()]
 
     async def get_reports(
         self, workflow: str, last_only: bool = False
     ) -> MutableSequence[MutableSequence[MutableMapping[str, Any]]]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             if last_only:
                 async with db.execute(
                     "SELECT c.id, s.name, c.start_time, c.end_time "
                     "FROM step AS s, command AS c "
                     "WHERE s.id = c.step "
                     "AND s.workflow = (SELECT id FROM workflow WHERE name = :workflow ORDER BY id DESC LIMIT 1)",
                     {"workflow": workflow},
@@ -356,73 +346,66 @@
                             {k: row[k] for k in row.keys() if k != "workflow"}
                         )
                     return list(result.values())
 
     @cachedmethod(lambda self: self.step_cache)
     async def get_step(self, step_id: int) -> MutableMapping[str, Any]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM step WHERE id = :id", {"id": step_id}
             ) as cursor:
                 return await cursor.fetchone()
 
     @cachedmethod(lambda self: self.target_cache)
     async def get_target(self, target_id: int) -> MutableMapping[str, Any]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM target WHERE id = :id", {"id": target_id}
             ) as cursor:
                 return await cursor.fetchone()
 
     @cachedmethod(lambda self: self.token_cache)
     async def get_token(self, token_id: int) -> MutableMapping[str, Any]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM token WHERE id = :id", {"id": token_id}
             ) as cursor:
                 return await cursor.fetchone()
 
     async def get_workflow(self, workflow_id: int) -> MutableMapping[str, Any]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM workflow WHERE id = :id", {"id": workflow_id}
             ) as cursor:
                 return await cursor.fetchone()
 
     async def get_workflow_ports(
         self, workflow_id: int
     ) -> MutableSequence[MutableMapping[str, Any]]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM port WHERE workflow = :workflow",
                 {"workflow": workflow_id},
             ) as cursor:
                 return await cursor.fetchall()
 
     async def get_workflow_steps(
         self, workflow_id: int
     ) -> MutableSequence[MutableMapping[str, Any]]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM step WHERE workflow = :workflow",
                 {"workflow": workflow_id},
             ) as cursor:
                 return await cursor.fetchall()
 
     async def get_workflows_by_name(
         self, workflow_name: str, last_only: bool = False
     ) -> MutableSequence[MutableMapping[str, Any]]:
         async with self.connection as db:
-            db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM workflow WHERE name = :name ORDER BY id desc",
                 {"name": workflow_name},
             ) as cursor:
                 return (
                     [await cursor.fetchone()] if last_only else await cursor.fetchall()
                 )
@@ -438,15 +421,14 @@
                         "start_time": get_date_from_ns(row["start_time"]),
                         "status": Status(row["status"]).name,
                         "type": row["type"],
                     }
                     for row in await self.get_workflows_by_name(name, last_only=False)
                 ]
             else:
-                db.row_factory = aiosqlite.Row
                 async with db.execute(
                     "SELECT name, type, COUNT(*) AS num FROM workflow GROUP BY name, type ORDER BY name DESC"
                 ) as cursor:
                     return await cursor.fetchall()
 
     async def update_command(
         self, command_id: int, updates: MutableMapping[str, Any]
```

### Comparing `streamflow-0.2.0.dev8/streamflow/provenance/run_crate.py` & `streamflow-0.2.0.dev9/streamflow/provenance/run_crate.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/recovery/checkpoint_manager.py` & `streamflow-0.2.0.dev9/streamflow/recovery/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/recovery/failure_manager.py` & `streamflow-0.2.0.dev9/streamflow/recovery/failure_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/recovery/recovery.py` & `streamflow-0.2.0.dev9/streamflow/recovery/recovery.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/recovery/schemas/default_failure_manager.json` & `streamflow-0.2.0.dev9/streamflow/recovery/schemas/default_failure_manager.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/report.py` & `streamflow-0.2.0.dev9/streamflow/report.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/scheduling/policy/data_locality.py` & `streamflow-0.2.0.dev9/streamflow/scheduling/policy/data_locality.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/scheduling/scheduler.py` & `streamflow-0.2.0.dev9/streamflow/scheduling/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     def __init__(
         self, context: StreamFlowContext, retry_delay: int | None = None
     ) -> None:
         super().__init__(context)
         self.allocation_groups: MutableMapping[str, MutableSequence[Job]] = {}
         self.binding_filter_map: MutableMapping[str, BindingFilter] = {}
         self.policy_map: MutableMapping[str, Policy] = {}
-        self.retry_interval: int | None = retry_delay
+        self.retry_interval: int | None = retry_delay if retry_delay != 0 else None
         self.scheduling_groups: MutableMapping[str, MutableSequence[str]] = {}
         self.wait_queues: MutableMapping[str, asyncio.Condition] = {}
 
     def _allocate_job(
         self,
         job: Job,
         hardware: Hardware,
@@ -317,17 +317,29 @@
                                 "No location available for job {} on deployment {}.".format(
                                     job_context.job.name,
                                     posixpath.join(deployment, target.service)
                                     if target.service
                                     else deployment,
                                 )
                             )
-                await asyncio.wait_for(
-                    self.wait_queues[deployment].wait(), timeout=self.retry_interval
-                )
+                try:
+                    await asyncio.wait_for(
+                        self.wait_queues[deployment].wait(), timeout=self.retry_interval
+                    )
+                except TimeoutError:
+                    if logger.isEnabledFor(logging.DEBUG):
+                        target_name = (
+                            "/".join([target.deployment.name, target.service])
+                            if target.service is not None
+                            else target.deployment.name
+                        )
+                        logger.debug(
+                            f"No locations available for job {job_context.job.name} "
+                            f"in target {target_name}. Waiting {self.retry_interval} seconds."
+                        )
 
     async def close(self):
         pass
 
     @classmethod
     def get_schema(cls) -> str:
         return pkg_resources.resource_filename(
```

### Comparing `streamflow-0.2.0.dev8/streamflow/workflow/combinator.py` & `streamflow-0.2.0.dev9/streamflow/workflow/combinator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/workflow/executor.py` & `streamflow-0.2.0.dev9/streamflow/workflow/executor.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/workflow/port.py` & `streamflow-0.2.0.dev9/streamflow/workflow/port.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/workflow/step.py` & `streamflow-0.2.0.dev9/streamflow/workflow/step.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/workflow/token.py` & `streamflow-0.2.0.dev9/streamflow/workflow/token.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/workflow/transformer.py` & `streamflow-0.2.0.dev9/streamflow/workflow/transformer.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow/workflow/utils.py` & `streamflow-0.2.0.dev9/streamflow/workflow/utils.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow.egg-info/PKG-INFO` & `streamflow-0.2.0.dev9/streamflow.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow
-Version: 0.2.0.dev8
+Version: 0.2.0.dev9
 Summary: StreamFlow framework
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://streamflow.di.unito.it
 Project-URL: Package, https://pypi.org/project/streamflow
 Project-URL: Repository, https://github.com/alpha-unito/streamflow
 Project-URL: Docker, https://hub.docker.com/r/alphaunito/streamflow
@@ -20,20 +20,51 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp==3.8.5
+Requires-Dist: aiosqlite==0.19.0
+Requires-Dist: antlr4-python3-runtime==4.13.1
+Requires-Dist: asyncssh==2.13.2
+Requires-Dist: bcrypt==4.0.1
+Requires-Dist: cachetools==5.3.1
+Requires-Dist: cwltool==3.1.20230906142556
+Requires-Dist: cwl-utils==0.29
+Requires-Dist: importlib_metadata==6.8.0
+Requires-Dist: Jinja2==3.1.2
+Requires-Dist: jsonschema==4.19.0
+Requires-Dist: kubernetes_asyncio==25.11.0
+Requires-Dist: psutil==5.9.5
+Requires-Dist: rdflib==6.3.2
+Requires-Dist: yattag==1.15.1
 Provides-Extra: bandit
+Requires-Dist: bandit==1.7.5; extra == "bandit"
 Provides-Extra: docs
+Requires-Dist: sphinx==7.2.5; extra == "docs"
+Requires-Dist: sphinx-jsonschema==1.19.1; extra == "docs"
+Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "docs"
 Provides-Extra: lint
+Requires-Dist: black==23.7.0; extra == "lint"
+Requires-Dist: codespell==2.2.5; extra == "lint"
+Requires-Dist: flake8-bugbear==23.7.10; extra == "lint"
+Requires-Dist: pyupgrade==3.10.1; extra == "lint"
 Provides-Extra: report
+Requires-Dist: pandas==2.1.0; extra == "report"
+Requires-Dist: plotly==5.16.1; extra == "report"
+Requires-Dist: kaleido==0.2.1; extra == "report"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: cwltest==2.3.20230825125225; extra == "test"
+Requires-Dist: pytest==7.4.2; extra == "test"
+Requires-Dist: pytest-asyncio==0.21.1; extra == "test"
+Requires-Dist: pytest-cov==4.1.0; extra == "test"
+Requires-Dist: pytest-xdist==3.3.1; extra == "test"
 
 # StreamFlow
 
 [![CI Tests](https://github.com/alpha-unito/streamflow/actions/workflows/ci-tests.yaml/badge.svg?branch=master)](https://github.com/alpha-unito/streamflow/actions/workflows/ci-tests.yaml)
 
 The [StreamFlow](https://streamflow.di.unito.it/) framework is a container-native *Workflow Management System (WMS)* written in Python 3.
 It has been designed around two main principles:
```

### Comparing `streamflow-0.2.0.dev8/streamflow.egg-info/SOURCES.txt` & `streamflow-0.2.0.dev9/streamflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/streamflow.egg-info/requires.txt` & `streamflow-0.2.0.dev9/streamflow.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 aiohttp==3.8.5
 aiosqlite==0.19.0
-antlr4-python3-runtime==4.13.0
+antlr4-python3-runtime==4.13.1
 asyncssh==2.13.2
 bcrypt==4.0.1
 cachetools==5.3.1
-cwltool==3.1.20230719185429
-cwl-utils==0.28
+cwltool==3.1.20230906142556
+cwl-utils==0.29
 importlib_metadata==6.8.0
 Jinja2==3.1.2
 jsonschema==4.19.0
 kubernetes_asyncio==25.11.0
 psutil==5.9.5
 rdflib==6.3.2
 yattag==1.15.1
 
 [bandit]
 bandit==1.7.5
 
 [docs]
-sphinx==7.2.3
+sphinx==7.2.5
 sphinx-jsonschema==1.19.1
 sphinx-rtd-theme==1.3.0
 
 [lint]
 black==23.7.0
 codespell==2.2.5
 flake8-bugbear==23.7.10
 pyupgrade==3.10.1
 
 [report]
-pandas==2.0.3
+pandas==2.1.0
 plotly==5.16.1
 kaleido==0.2.1
 
 [test]
 cwltest==2.3.20230825125225
-pytest==7.4.0
+pytest==7.4.2
 pytest-asyncio==0.21.1
 pytest-cov==4.1.0
 pytest-xdist==3.3.1
```

### Comparing `streamflow-0.2.0.dev8/tests/test_cwl_loop.py` & `streamflow-0.2.0.dev9/tests/test_cwl_loop.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/tests/test_cwl_persistence.py` & `streamflow-0.2.0.dev9/tests/test_cwl_persistence.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/tests/test_cwl_provenance.py` & `streamflow-0.2.0.dev9/tests/test_cwl_provenance.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/tests/test_persistence.py` & `streamflow-0.2.0.dev9/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/tests/test_provenance.py` & `streamflow-0.2.0.dev9/tests/test_provenance.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/tests/test_remotepath.py` & `streamflow-0.2.0.dev9/tests/test_remotepath.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/tests/test_scheduler.py` & `streamflow-0.2.0.dev9/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/tests/test_schema.py` & `streamflow-0.2.0.dev9/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev8/tests/test_transfer.py` & `streamflow-0.2.0.dev9/tests/test_transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import os
 import posixpath
 import tempfile
 
 import pytest
 import pytest_asyncio
 
@@ -162,15 +163,20 @@
     else:
         src_path = posixpath.join("/tmp", utils.random_name())
     if isinstance(dst_connector, LocalConnector):
         dst_path = os.path.join(tempfile.gettempdir(), utils.random_name())
     else:
         dst_path = posixpath.join("/tmp", utils.random_name())
     try:
-        await remotepath.write(src_connector, src_location, src_path, "StreamFlow")
+        await remotepath.write(
+            src_connector,
+            src_location,
+            src_path,
+            "StreamFlow",
+        )
         src_path = await remotepath.follow_symlink(
             context, src_connector, src_location, src_path
         )
         src_digest = await remotepath.checksum(
             context, src_connector, src_location, src_path
         )
         context.data_manager.register_path(
@@ -192,7 +198,24 @@
         dst_digest = await remotepath.checksum(
             context, dst_connector, dst_location, dst_path
         )
         assert src_digest == dst_digest
     finally:
         await remotepath.rm(src_connector, src_location, src_path)
         await remotepath.rm(dst_connector, dst_location, dst_path)
+
+
+@pytest.mark.asyncio
+async def test_multiple_files(
+    context, src_connector, src_location, dst_connector, dst_location
+):
+    """Test transferring multiple files simultaneously from one location to another."""
+    await asyncio.gather(
+        *(
+            asyncio.create_task(
+                test_file_to_file(
+                    context, src_connector, src_location, dst_connector, dst_location
+                )
+            )
+            for _ in range(20)
+        )
+    )
```

