# Comparing `tmp/contrast_agent-8.0.0.tar.gz` & `tmp/contrast_agent-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contrast_agent-8.0.0.tar", last modified: Wed Apr 24 20:53:53 2024, max compression
+gzip compressed data, was "contrast_agent-8.1.0.tar", last modified: Tue May  7 15:59:08 2024, max compression
```

## Comparing `contrast_agent-8.0.0.tar` & `contrast_agent-8.1.0.tar`

### file list

```diff
@@ -1,788 +1,788 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.332630 contrast_agent-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-24 20:53:53.332630 contrast_agent-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.192628 contrast_agent-8.0.0/hookspy/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.192628 contrast_agent-8.0.0/hookspy/ext/
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/ext/hookspy.c
--rwxr-xr-x   0 runner    (1001) docker     (127)      952 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.176628 contrast_agent-8.0.0/hookspy/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.192628 contrast_agent-8.0.0/hookspy/src/hookspy/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/src/hookspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/src/hookspy/autogen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/src/hookspy/body.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/src/hookspy/signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/src/hookspy/spy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 20:53:53.332630 contrast_agent-8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.188629 contrast_agent-8.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.192628 contrast_agent-8.0.0/src/contrast/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.200629 contrast_agent-8.0.0/src/contrast/agent/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.200629 contrast_agent-8.0.0/src/contrast/agent/agent_lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/agent_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/agent_lib/input_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/agent_lib/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/agent_lib/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/agent_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.204629 contrast_agent-8.0.0/src/contrast/agent/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/adjusted_span.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/apply_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/assess_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15343 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/contrast_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.204629 contrast_agent-8.0.0/src/contrast/agent/assess/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/deadzone_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/preshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagation_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagation_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.208629 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/append_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/base_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/center_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/codecs_splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/format_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/join_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/json_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/keep_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/split_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/tagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/source_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/source_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10799 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/string_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.212629 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.212629 contrast_agent-8.0.0/src/contrast/agent/assess/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/base_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.216629 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/base_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/django_httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/django_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/django_session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/flask_httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/flask_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/flask_session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/dataflow_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/non_dataflow_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.216629 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/enable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.220629 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/base_response_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/xss.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/static_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/trigger_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.220629 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/string_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/truncate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/disable_reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/exclusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/heartbeat_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.220629 contrast_agent-8.0.0/src/contrast/agent/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/app_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14116 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/base_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/environ_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.220629 contrast_agent-8.0.0/src/contrast/agent/middlewares/response_wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/response_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.224629 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/django_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/patch_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.224629 contrast_agent-8.0.0/src/contrast/agent/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/applicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/patch_location_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/policy_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/trigger_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.228629 contrast_agent-8.0.0/src/contrast/agent/protect/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/input_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.228629 contrast_agent-8.0.0/src/contrast/agent/protect/policy/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.228629 contrast_agent-8.0.0/src/contrast/agent/protect/rule/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/base_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/bot_blocker_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/cmdi_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.232629 contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/http_method_tampering.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/malformed_header.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/mode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.232629 contrast_agent-8.0.0/src/contrast/agent/protect/rule/nosql_injection/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/nosql_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/nosqli_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/path_traversal_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/rules_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/sqli_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/ssrf_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/unsafe_file_upload_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/xss_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.232629 contrast_agent-8.0.0/src/contrast/agent/protect/rule/xxe/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/xxe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/xxe_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/reaction_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/request_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/request_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/server_settings_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)    24894 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/sys_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    12551 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/thread_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.232629 contrast_agent-8.0.0/src/contrast/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/aiohttp/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/aiohttp/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.232629 contrast_agent-8.0.0/src/contrast/api/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/architecture_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/route_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/trace_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/type_checked_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.232629 contrast_agent-8.0.0/src/contrast/applies/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/applies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.236629 contrast_agent-8.0.0/src/contrast/applies/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/applies/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/applies/assess/unsafe_code_execution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.236629 contrast_agent-8.0.0/src/contrast/applies/common/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/applies/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.236629 contrast_agent-8.0.0/src/contrast/applies/protect/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/applies/protect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/applies/sqli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.236629 contrast_agent-8.0.0/src/contrast/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.236629 contrast_agent-8.0.0/src/contrast/assess_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/build_funchook.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.240629 contrast_agent-8.0.0/src/contrast/assess_extensions/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/cast.c
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/format.c
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/intern.c
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/logging.c
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/patches.c
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/propagate.c
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/repeat.c
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/repr.c
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/scope.c
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/streams.c
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/subscript.c
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/trace.c
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/cs_str.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.240629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 20:53:42.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.git
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.gitmodules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.240629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.travis/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.travis/Dockerfile-alpine-test
--rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.travis/run-test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/appveyor.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/autogen.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    44826 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/config.guess
--rwxr-xr-x   0 runner    (1001) docker     (127)    35454 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/config.sub
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/configure.ac
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.244629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/.git
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.244629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/include/
--rw-r--r--   0 runner    (1001) docker     (127)    19536 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h
--rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.180628 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.244629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.244629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/mac/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.244629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/
--rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.h
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.248629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/config.h
--rw-r--r--   0 runner    (1001) docker     (127)    25059 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c
--rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c
--rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h
--rw-r--r--   0 runner    (1001) docker     (127)   209309 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h
--rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c
--rw-r--r--   0 runner    (1001) docker     (127)    45685 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.248629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/include/
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/include/funchook.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    13998 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/install-sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.252629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/__strerror.h
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook.c
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_io.c
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_io.h
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S
--rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c
--rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c
--rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func.c
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func.h
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c
--rw-r--r--   0 runner    (1001) docker     (127)    43872 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/printf_base.c
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/printf_base.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.252629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/libfunchook_test.c
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/libfunchook_test2.c
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/suffix.list
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/test_main.c
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/x86_64_test.S
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/x86_test.S
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.256629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook.sln
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test_exe.def
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.180628 contrast_agent-8.0.0/src/contrast/assess_extensions/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.180628 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.256629 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/intern.h
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/logging.h
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/patches.h
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/scope.h
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/trace.h
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.256629 contrast_agent-8.0.0/src/contrast/assess_extensions/py3/
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py3/patches.c
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py3/str_concat.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.260629 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.260629 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.260629 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.264629 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.264629 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.264629 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.264629 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/
--rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.268629 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.268629 contrast_agent-8.0.0/src/contrast/bottle/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/bottle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/bottle/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/agent_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/assess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/protect.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/django/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/django/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/django_asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/django_asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/django_asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/falcon/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/falcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/falcon/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/falcon_asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/falcon_asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/falcon_asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/fastapi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/flask/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/flask/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/loader/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/loader/sitecustomize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.276629 contrast_agent-8.0.0/src/contrast/patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/cgi_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/concurrent_futures_thread_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/cs_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/cs_str.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.280629 contrast_agent-8.0.0/src/contrast/patches/databases/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/dbapi2.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/mysql_connector_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/psycopg2_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/pymysql_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/sqlalchemy_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/sqlite3_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/encodings_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/exec_and_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.280629 contrast_agent-8.0.0/src/contrast/patches/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/bottle_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/django_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/drf_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/falcon_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/flask_and_quart_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/pyramid_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/starlette_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/genshi_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/import_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/lxml_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.280629 contrast_agent-8.0.0/src/contrast/patches/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/middleware/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/middleware/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/middleware/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/middleware/mod_wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/pathlib_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/re_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/str_new.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/sys_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/threading_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/urllib_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.280629 contrast_agent-8.0.0/src/contrast/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/deadzones.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.284629 contrast_agent-8.0.0/src/contrast/policy/propagators/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/frameworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/re.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.284629 contrast_agent-8.0.0/src/contrast/policy/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/cgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/quart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/webob.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.288629 contrast_agent-8.0.0/src/contrast/policy/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/cmd_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/httponly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/nosql_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/path_traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/prompt_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/redos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/reflected_xss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/secure_flag_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/session_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/session_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/sql_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/ssrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/trust_boundary_violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/unsafe_code_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/untrusted_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/unvalidated_redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/xpath_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/xxe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.288629 contrast_agent-8.0.0/src/contrast/pyramid/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/pyramid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/pyramid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.288629 contrast_agent-8.0.0/src/contrast/quart/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/quart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/quart/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.288629 contrast_agent-8.0.0/src/contrast/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/activity_masker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/reporting_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/request_audit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.292629 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/agent_startup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/application_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/application_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/application_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/base_ts_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/effective_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/library_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/observed_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/server_activity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.292629 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/application_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/ng_application_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/ng_server_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/protect_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/server_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.296629 contrast_agent-8.0.0/src/contrast/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/scripts/fix_interpreter_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/scripts/propagator_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/scripts/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/scripts/validate_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.300629 contrast_agent-8.0.0/src/contrast/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.300629 contrast_agent-8.0.0/src/contrast/utils/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/duck_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.300629 contrast_agent-8.0.0/src/contrast/utils/assess/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/formatting/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/formatting/tokenize_cformat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/formatting/tokenize_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/tag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/tracking_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/base64_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/configuration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/context_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/deprecated_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/digest_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/environ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.300629 contrast_agent-8.0.0/src/contrast/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/exceptions/deprecation_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/exceptions/wsgi_compliance_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/ignored_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.304629 contrast_agent-8.0.0/src/contrast/utils/library_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/library_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/library_reader/library_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/library_reader/patched_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/library_reader/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/locale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.304629 contrast_agent-8.0.0/src/contrast/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/loggers/structlog.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/module_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/patch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/pattern_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/safe_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/stack_trace_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/stdlib_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 20:53:52.000000 contrast_agent-8.0.0/src/contrast/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.304629 contrast_agent-8.0.0/src/contrast/wsgi/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/wsgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/wsgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.328630 contrast_agent-8.0.0/src/contrast_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    32206 2024-04-24 20:53:53.000000 contrast_agent-8.0.0/src/contrast_agent.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.304629 contrast_agent-8.0.0/src/contrast_rewriter/
--rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_rewriter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.304629 contrast_agent-8.0.0/src/contrast_vendor/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.308629 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    34323 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.308629 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/compat/py39.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/diagnose.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.308629 contrast_agent-8.0.0/src/contrast_vendor/isort/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.308629 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/all.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py27.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py311.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py312.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py36.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py37.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py39.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.308629 contrast_agent-8.0.0/src/contrast_vendor/ported_cpython_code/
--rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ported_cpython_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ported_cpython_code/import_functionality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.188629 contrast_agent-8.0.0/src/contrast_vendor/ruamel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.316630 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/anchor.py
--rw-r--r--   0 runner    (1001) docker     (127)    37673 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/composer.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/configobjwalker.py
--rw-r--r--   0 runner    (1001) docker     (127)    70392 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/cyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)    67960 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    59457 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    36019 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/representer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarbool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarstring.py
--rw-r--r--   0 runner    (1001) docker     (127)    87945 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.324630 contrast_agent-8.0.0/src/contrast_vendor/structlog/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_greenlets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_log_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_native.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (127)    23428 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    37555 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/threadlocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/tracebacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/twisted.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/vendor-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.328630 contrast_agent-8.0.0/src/contrast_vendor/webob/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   210210 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/acceptparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/byterange.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/cachecontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/dec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/etag.py
--rw-r--r--   0 runner    (1001) docker     (127)    38268 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/multidict.py
--rw-r--r--   0 runner    (1001) docker     (127)    59159 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    55423 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.328630 contrast_agent-8.0.0/src/contrast_vendor/wrapt/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/__wrapt__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/weakrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27137 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.328630 contrast_agent-8.0.0/src/contrast_vendor/zipp/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/zipp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/zipp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.328630 contrast_agent-8.0.0/src/contrast_vendor/zipp/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/zipp/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/zipp/compat/py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/zipp/glob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.642629 contrast_agent-8.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-07 15:59:08.642629 contrast_agent-8.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.510628 contrast_agent-8.1.0/hookspy/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.510628 contrast_agent-8.1.0/hookspy/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/ext/hookspy.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)      952 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.498628 contrast_agent-8.1.0/hookspy/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.514628 contrast_agent-8.1.0/hookspy/src/hookspy/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/src/hookspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/src/hookspy/autogen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/src/hookspy/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/src/hookspy/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/src/hookspy/spy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:59:08.642629 contrast_agent-8.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.510628 contrast_agent-8.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.514628 contrast_agent-8.1.0/src/contrast/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.518628 contrast_agent-8.1.0/src/contrast/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.518628 contrast_agent-8.1.0/src/contrast/agent/agent_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/agent_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/agent_lib/input_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/agent_lib/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/agent_lib/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16006 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/agent_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.522628 contrast_agent-8.1.0/src/contrast/agent/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/adjusted_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/apply_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/assess_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/contrast_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.522628 contrast_agent-8.1.0/src/contrast/agent/assess/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/deadzone_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/preshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagation_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagation_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.526628 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/append_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/base_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/center_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/codecs_splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/format_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/join_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/json_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/keep_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/split_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/tagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/source_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/source_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/string_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.530628 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.530628 contrast_agent-8.1.0/src/contrast/agent/assess/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/base_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.534628 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/base_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/django_httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/django_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/django_session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/flask_httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/flask_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/flask_session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/dataflow_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/non_dataflow_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.534628 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.538628 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/base_response_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/xss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/static_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/trigger_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.538628 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/string_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/disable_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/heartbeat_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.538628 contrast_agent-8.1.0/src/contrast/agent/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/app_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14101 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/base_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/environ_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.538628 contrast_agent-8.1.0/src/contrast/agent/middlewares/response_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/response_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.542628 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/django_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/patch_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.542628 contrast_agent-8.1.0/src/contrast/agent/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/applicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/patch_location_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/policy_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/trigger_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.542628 contrast_agent-8.1.0/src/contrast/agent/protect/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/input_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.542628 contrast_agent-8.1.0/src/contrast/agent/protect/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.546628 contrast_agent-8.1.0/src/contrast/agent/protect/rule/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13381 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/base_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/bot_blocker_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/cmdi_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.546628 contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/http_method_tampering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/malformed_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/mode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.546628 contrast_agent-8.1.0/src/contrast/agent/protect/rule/nosql_injection/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/nosql_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/nosqli_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/path_traversal_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/rules_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/sqli_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/ssrf_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/unsafe_file_upload_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/xss_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/agent/protect/rule/xxe/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/xxe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/xxe_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/reaction_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/request_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/request_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/server_settings_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24894 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/sys_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12551 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/thread_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/aiohttp/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/aiohttp/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/architecture_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/route_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/trace_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/type_checked_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/applies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/applies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/applies/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/applies/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/applies/assess/unsafe_code_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/applies/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/applies/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/applies/protect/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/applies/protect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/applies/sqli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.554628 contrast_agent-8.1.0/src/contrast/assess_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/build_funchook.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.554628 contrast_agent-8.1.0/src/contrast/assess_extensions/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/cast.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/format.c
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/intern.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/logging.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/patches.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/propagate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/repeat.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/repr.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/scope.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/streams.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/subscript.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/trace.c
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/cs_str.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.558628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.git
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.gitmodules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.558628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.travis/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.travis/Dockerfile-alpine-test
+-rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.travis/run-test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/appveyor.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/autogen.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44826 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/config.guess
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35454 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/config.sub
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/configure.ac
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.558628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/.git
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.558628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    19536 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.502628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.558628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.558628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/mac/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.562628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.566628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25059 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c
+-rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   209309 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45685 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.566628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/include/funchook.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13998 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/install-sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.570628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/__strerror.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_io.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_io.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c
+-rw-r--r--   0 runner    (1001) docker     (127)    43872 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/printf_base.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/printf_base.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.570628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/libfunchook_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/libfunchook_test2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/suffix.list
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/test_main.c
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/x86_64_test.S
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/x86_test.S
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.570628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook.sln
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test_exe.def
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.502628 contrast_agent-8.1.0/src/contrast/assess_extensions/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.502628 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.574628 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/intern.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/logging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/patches.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/scope.h
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/trace.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.574628 contrast_agent-8.1.0/src/contrast/assess_extensions/py3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py3/patches.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py3/str_concat.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.574628 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.574628 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.578628 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.578628 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.578628 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.578628 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.582628 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.582628 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.582628 contrast_agent-8.1.0/src/contrast/bottle/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/bottle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/bottle/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/assess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/protect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/django/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/django_asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/django_asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/django_asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/falcon/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/falcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/falcon/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/falcon_asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/falcon_asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/falcon_asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/fastapi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/flask/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/loader/sitecustomize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.590628 contrast_agent-8.1.0/src/contrast/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/cgi_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/concurrent_futures_thread_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/cs_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/cs_str.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.590628 contrast_agent-8.1.0/src/contrast/patches/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/dbapi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/mysql_connector_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/psycopg2_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/pymysql_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/sqlalchemy_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/sqlite3_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/encodings_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/exec_and_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.594628 contrast_agent-8.1.0/src/contrast/patches/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/bottle_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/django_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/drf_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/falcon_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/flask_and_quart_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/pyramid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/starlette_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/genshi_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/import_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/lxml_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.594628 contrast_agent-8.1.0/src/contrast/patches/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/middleware/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/middleware/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/middleware/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/middleware/mod_wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/pathlib_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/re_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/str_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/sys_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/threading_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/urllib_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.594628 contrast_agent-8.1.0/src/contrast/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/deadzones.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.598628 contrast_agent-8.1.0/src/contrast/policy/propagators/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/frameworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.598628 contrast_agent-8.1.0/src/contrast/policy/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/cgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/quart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/webob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.602628 contrast_agent-8.1.0/src/contrast/policy/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/cmd_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/httponly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/nosql_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/path_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/prompt_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/redos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/reflected_xss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/secure_flag_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/session_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/session_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/sql_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/ssrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/trust_boundary_violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/unsafe_code_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/untrusted_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/unvalidated_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/xpath_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/xxe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.602628 contrast_agent-8.1.0/src/contrast/pyramid/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/pyramid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/pyramid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.602628 contrast_agent-8.1.0/src/contrast/quart/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/quart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/quart/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.602628 contrast_agent-8.1.0/src/contrast/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/activity_masker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/reporting_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/request_audit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.606628 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/agent_startup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/application_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/application_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/application_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/base_ts_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/effective_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/library_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/observed_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/server_activity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.606628 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/ng_application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/ng_server_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/protect_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/server_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.606628 contrast_agent-8.1.0/src/contrast/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/scripts/fix_interpreter_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/scripts/propagator_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/scripts/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/scripts/validate_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.610628 contrast_agent-8.1.0/src/contrast/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast/utils/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/duck_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast/utils/assess/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/formatting/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/formatting/tokenize_cformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/formatting/tokenize_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/tag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/tracking_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/base64_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/context_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/deprecated_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/digest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/environ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/exceptions/deprecation_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/exceptions/wsgi_compliance_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/ignored_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast/utils/library_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/library_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/library_reader/library_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/library_reader/patched_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/library_reader/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/locale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/loggers/structlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/module_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/patch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/pattern_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/safe_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/stack_trace_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/stdlib_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 15:59:08.000000 contrast_agent-8.1.0/src/contrast/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast/wsgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/wsgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/wsgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.638629 contrast_agent-8.1.0/src/contrast_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32206 2024-05-07 15:59:08.000000 contrast_agent-8.1.0/src/contrast_agent.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast_rewriter/
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_rewriter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.618628 contrast_agent-8.1.0/src/contrast_vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.618628 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    34323 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.618628 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/compat/py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/diagnose.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.618628 contrast_agent-8.1.0/src/contrast_vendor/isort/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.622628 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py27.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py311.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py39.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.622628 contrast_agent-8.1.0/src/contrast_vendor/ported_cpython_code/
+-rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ported_cpython_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ported_cpython_code/import_functionality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.510628 contrast_agent-8.1.0/src/contrast_vendor/ruamel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.630628 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37673 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/configobjwalker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70392 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/cyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67960 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59457 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36019 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/representer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarbool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87945 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.634628 contrast_agent-8.1.0/src/contrast_vendor/structlog/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_greenlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23428 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    37555 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/threadlocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/tracebacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/twisted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/vendor-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.638629 contrast_agent-8.1.0/src/contrast_vendor/webob/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   210210 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/acceptparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/byterange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/cachecontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/etag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38268 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/multidict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59159 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55423 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.638629 contrast_agent-8.1.0/src/contrast_vendor/wrapt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/__wrapt__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/weakrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27137 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.638629 contrast_agent-8.1.0/src/contrast_vendor/zipp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/zipp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/zipp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.638629 contrast_agent-8.1.0/src/contrast_vendor/zipp/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/zipp/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/zipp/compat/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/zipp/glob.py
```

### Comparing `contrast_agent-8.0.0/LICENSE.txt` & `contrast_agent-8.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/MANIFEST.in` & `contrast_agent-8.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/PKG-INFO` & `contrast_agent-8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contrast-agent
-Version: 8.0.0
+Version: 8.1.0
 Summary: Contrast Security's agent for Python web frameworks
 Author-email: "Contrast Security, Inc." <python@contrastsecurity.com>
 License: Copyright: 2024 Contrast Security, Inc
         Contact: support@contrastsecurity.com
         License: Commercial
         
         NOTICE: This Software and the patented inventions embodied within may only be used as
```

### Comparing `contrast_agent-8.0.0/hookspy/README.md` & `contrast_agent-8.1.0/hookspy/README.md`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/hookspy/ext/hookspy.c` & `contrast_agent-8.1.0/hookspy/ext/hookspy.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/hookspy/setup.py` & `contrast_agent-8.1.0/hookspy/setup.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/hookspy/src/hookspy/autogen.py` & `contrast_agent-8.1.0/hookspy/src/hookspy/autogen.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/hookspy/src/hookspy/body.py` & `contrast_agent-8.1.0/hookspy/src/hookspy/body.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/hookspy/src/hookspy/signatures.py` & `contrast_agent-8.1.0/hookspy/src/hookspy/signatures.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/hookspy/src/hookspy/spy.py` & `contrast_agent-8.1.0/hookspy/src/hookspy/spy.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/pyproject.toml` & `contrast_agent-8.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -58,27 +58,27 @@
 '''
 
 [tool.ruff]
 line-length = 88
 target-version = "py38"
 extend-exclude = [
   "src/contrast_vendor/",
-  "tests/agent/data/rewriter/golden/",
+  "*.golden",
   "tests/agent/data/rewriter/source/",
   "tests/extern/",
 ]
 
 [tool.ruff.lint]
 extend-select = [
     "E",
     "W",
     "PLE",
     "PLC",
+    "B",
     # we may want to add these eventually
-    # "B",
     # "PLW",
     # "RUF",
     # "PERF",
     # "UP",
     # "RET",
 ]
 # we may want to remove this eventually
```

### Comparing `contrast_agent-8.0.0/setup.py` & `contrast_agent-8.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/__init__.py` & `contrast_agent-8.1.0/src/contrast/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/agent_lib/__init__.py` & `contrast_agent-8.1.0/src/contrast/agent/agent_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/agent_lib/input_tracing.py` & `contrast_agent-8.1.0/src/contrast/agent/agent_lib/input_tracing.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/agent_lib/main.py` & `contrast_agent-8.1.0/src/contrast/agent/agent_lib/main.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/agent_state.py` & `contrast_agent-8.1.0/src/contrast/agent/agent_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 from contrast.utils.namespace import Namespace
 from contrast.utils.decorators import fail_loudly, fail_quietly
 from contrast_rewriter import (
     process_rewriter_logs,
     set_rewriter_logger,
 )
 from contrast.agent.runner import is_runner_in_use
+from contrast_rewriter import is_rewriter_enabled
+from contrast_vendor.structlog._log_levels import LEVEL_TO_NAME
 
 # NOTE: policy is currently loaded/generated on import. It is applied explicitly in
 # policy/applicator.py
 from contrast import policy  # noqa: F401
 
 logger = setup_basic_agent_logger()
 LOGS_SEPARATOR = "-" * 120
@@ -105,57 +107,59 @@
     app_name: Optional[str] = None
 
 
 def _log_environment(settings: Settings):
     """
     Log current working directory, python version and pip version
     """
-    banner = f"{'-' * 50}ENVIRONMENT{'-' * 50}"
-    logger.debug(banner)
-    logger.debug("Current Working Dir: %s", AGENT_CURR_WORKING_DIR)
-    logger.debug("Python Version: %s", sys.version)
-    logger.debug("Detected Framework: %s", settings.framework)
-    logger.debug("Detected application name: %s", module.app_name)
-    logger.debug("Configured application name: %s", settings.app_name)
-    logger.debug("Server Version: %s", settings.server)
-    logger.debug("Contrast Python Agent Version: %s", __version__)
-    logger.debug("Executable: %s", sys.executable)
-    logger.debug("Default encoding %s", DEFAULT_ENCODING)
-    logger.debug("Using runner: %s", is_runner_in_use())
-    logger.debug("Has funchook: %s", cs_str.has_funchook())
-    logger.debug("Enabled sys.monitoring: %s", sys_monitoring.is_enabled())
-
-    # TODO: PYT-3116 uncomment with deprecation of 3.8
-    # if sys.version_info[:2] == (3, 8):
-    #     logger.warn(
-    #         "Support for Python 3.8 is deprecated and will be removed in a future release"
-    #     )
-
     try:
         platform_str = platform.platform()
     except Exception:
         try:
             platform_str = platform.platform(terse=True)
         except Exception:
             platform_str = "unknown"
+    log_level = logger.getEffectiveLevel()
+    logger.info(
+        "ENVIRONMENT",
+        python_version=sys.version,
+        agent_version=__version__,
+        assess_enabled=settings.is_assess_enabled(),
+        protect_enabled=settings.is_protect_enabled(),
+        using_runner=is_runner_in_use(),
+        using_rewriter=is_rewriter_enabled(),
+        has_funchook=cs_str.has_funchook(),
+        using_sys_monitoring=sys_monitoring.is_enabled(),
+        log_level=LEVEL_TO_NAME.get(log_level, str(log_level)).upper(),
+        configured_application_name=settings.app_name,
+        detected_application_name=module.app_name,
+        detected_framework=module.framework,
+        installed_framework=settings.framework,
+        installed_webserver=settings.server,
+        cwd=AGENT_CURR_WORKING_DIR,
+        executable=sys.executable,
+        platform=platform_str,
+        default_encoding=DEFAULT_ENCODING,
+    )
 
-    logger.debug("Platform %s", platform_str)
-    logger.debug(banner)
+    # TODO: PYT-3116 uncomment with deprecation of py38
+    # if sys.version_info[:2] == (3, 8):
+    #     logger.warn(
+    #         "Support for Python 3.8 is deprecated and will be removed in a future release"
+    #     )
 
 
 def _warn_for_misleading_config(settings: Settings):
     protect_option = settings.config.get("protect.enable")
     protect_enabled = protect_option.value()
-    logger.info("Protect: %s", protect_enabled)
     if protect_enabled and not protect_option.ui_value:
         logger.warning(PROTECT_MISMATCH_MESSAGE)
 
     assess_option = settings.config.get("assess.enable")
     assess_enabled = assess_option.value()
-    logger.info("Assess: %s", assess_enabled)
     if assess_enabled and not assess_option.ui_value:
         logger.warning(ASSESS_MISMATCH_MESSAGE)
 
     if (
         settings.is_agent_config_enabled()
         and not protect_enabled
         and not assess_enabled
@@ -275,15 +279,15 @@
     order to be effective, this method should be called prior to middleware
     initialization.
     """
     module.app_name = name
 
 
 def _log_and_warn(msg):
-    warnings.warn(msg, ContrastDeprecationWarning)
+    warnings.warn(msg, ContrastDeprecationWarning, stacklevel=2)
     logger.warning(msg)
 
 
 def _check_middleware_warnings():
     # NOTE: currently, we are skipping framework-specific middleware deprecation
     # warnings. In the future, we might want to actually deprecate these. For now,
     # however, we are holding off.
@@ -320,15 +324,15 @@
     else:
         logger.debug("Not checking for deferred rewriter logs")
 
     logger.debug("Setting rewriter logger to agent logger")
     set_rewriter_logger(logger)
 
 
-def initialize(name: Optional[str] = None):
+def initialize():
     """
     If this method is called more than once per process, we use the is_initialized
     flag to only run the following work once:
         - library analysis thread initialization
         - turning on patches
         - hardcoded rule providers
         - scanning config rules
@@ -342,28 +346,31 @@
     with module.init_lock:
         if module.is_initialized:
             _check_middleware_warnings()
             logger.warning("Attempted to initialize agent state more than once")
             return
 
         module.id = id(module)
-        name = name or __name__
 
-        logger.info('Initializing Contrast Agent "%s" [id=%s]', name, module.id)
-        logger.info("Contrast Python Agent Version: %s\n", __version__)
+        logger.info(
+            "Initializing Contrast Agent %s",
+            __name__,
+            id=module.id,
+            version=__version__,
+        )
 
         if not initialize_settings():
             return
 
         if module.settings is None:
             logger.warning("Contrast Agent is not enabled.")
             return
 
         if not module.settings.is_agent_config_enabled():
-            logger.warning("Contrast Agent is not enabled.")
+            logger.warning("Contrast Agent is disabled by local configuration.")
             module.settings.log_effective_config()
             return
 
         setup_agent_logger(module.settings.config)
         setup_security_logger(module.settings.config)
         module.settings.config.log_config()
 
@@ -371,17 +378,16 @@
             if module.settings.config.should_enable_sys_monitoring:
                 sys_monitoring.enable()
             else:
                 logger.debug(
                     "sys.monitoring explicitly disabled in local config - will not enable"
                 )
 
-        _log_environment(module.settings)
-
-        # NOTE: This assumes that initialize is only ever called from middleware.
+        # NOTE (TODO: PYT-3016)
+        # This assumes that initialize is only ever called from middleware.
         # If at some point this no longer holds, it may be necessary to pass a
         # flag to initialize indicating whether these warnings should be
         # processed or not.
         _check_middleware_warnings()
 
         # The rewriter is applied long before we have any settings or logger so
         # the deferred logs are finally processed here
@@ -413,28 +419,28 @@
         if module.settings.is_assess_enabled():
             # For now agent runtime starts before config scanning
             # this will be reset when time_limit_threshold is reached,
             # it doesn't symbolize the total agent runtime for all time.
             module.settings.agent_runtime_window = timer.now_ms()
 
             enable_providers()
-            # NOTE: This should stay in middleware
+            # NOTE (TODO: PYT-3016) This should stay in middleware
             # scan_configs_in_thread()
 
         if module.settings.is_protect_enabled() and not agent_lib.initialize():
             logger.error("Fatal: Unable to initialize agent-lib. Disabling Contrast.")
             enable_option = module.settings.config.get("enable")
             enable_option.override_value = False
             return
 
+        _log_environment(module.settings)
         logger.info(
-            "Finished Initializing Contrast Agent %s [id=%s] \n\n%s\n",
-            name,
-            module.id,
-            LOGS_SEPARATOR,
+            "Finished Initializing Contrast Agent %s",
+            __name__,
+            id=module.id,
         )
 
         if Telemetry is not None:
             contrast.TELEMETRY = Telemetry()
             contrast.TELEMETRY.start()
             atexit.register(contrast.TELEMETRY.stop)
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/asgi.py` & `contrast_agent-8.1.0/src/contrast/agent/asgi.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/adjusted_span.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/adjusted_span.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/apply_trigger.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/apply_trigger.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,40 +87,40 @@
         # If the target is a stream that is being treated as a source, then we
         # build a new Properties object for it and add the stream's source
         # event to it. In this case the stream object itself is actually
         # triggering the rule, which means that no data was necessarily read
         # from the stream before triggering the rule.
         if safe_getattr(target, "cs__source", False):
             target_properties = Properties(target)
-            target_properties.add_event(target.cs__source_event)
+            target_properties.event = target.cs__source_event
         else:
             target_properties = get_properties(target)
 
     if target_properties is not None:
         events = [event.to_reportable_event() for event in target_properties.events]
 
         target_props = target_properties.dynamic_source_metadata
         if target_props:
             for key, value in target_props.items():
                 properties[key] = value
 
-    parent_ids = (
-        [target_properties.events[-1].event_id]
-        if target_properties and target_properties.events
+    parents = (
+        [target_properties.event]
+        if target_properties and target_properties.event
         else []
     )
 
     contrast_event = ContrastEvent(
         node,
         target,
         self_obj,
         ret,
         args,
         kwargs,
-        parent_ids,
+        parents,
         possible_key,
     ).to_reportable_event()
 
     events.append(contrast_event)
 
     rule.build_and_append_finding(
         context, properties, node, target, events=events, source=target
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/contrast_event.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/contrast_event.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import copy
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from itertools import chain
 from pathlib import PurePath
 import re
 import reprlib
 import threading
+import time
 from typing import Any, Callable, Dict, List, Optional, Sequence, Type
 from contrast.agent.assess.tag import Tag
 
 from contrast.agent.policy.constants import (
     OBJECT,
     RETURN,
     TRIGGER_TYPE,
@@ -27,19 +28,20 @@
     TraceEventObject,
     ParentObjectId,
     TraceEventSource,
 )
 from contrast.utils.assess.duck_utils import len_or_zero
 from contrast.utils.base64_utils import B64_NONE_STRING, base64_encode
 from contrast.utils.stack_trace_utils import (
+    acceptable_frame,
     build_stack,
     clean_stack,
 )
-from contrast.utils.timer import now_ms
 from contrast_vendor import structlog as logging
+from contrast_vendor.webob.util import html_escape
 
 logger = logging.getLogger("contrast")
 
 INIT = "__init__"
 INITIALIZERS = (INIT, "__new__")
 NONE_STRING = str(None)
 
@@ -136,36 +138,36 @@
         self,
         node: PolicyNode,
         tagged: Any,
         self_obj: Optional[Any],
         ret: Optional[Any],
         args: Sequence[Any],
         kwargs: Dict[str, Any],
-        parent_ids: List[int],
+        parents: List["ContrastEvent"],
         possible_key=None,
         source_type=None,
         source_name=None,
     ):
         self.node = node
         self._init_tagged(tagged, possible_key, args, kwargs)
         self.source_type = source_type
         self.source_name = source_name
-        self.parent_ids = parent_ids
+        self.parents = parents or []
         ret = self._update_init_return(node, self_obj, ret)
         self.obj = Field(self_obj) if self_obj is not None else None
         self.ret = Field(ret) if ret is not None else None
         self.args = [Field(arg) for arg in args] if args is not None else None
         self.kwargs = (
             [Field(f"{k}={obj_repr.repr(v)}", typ=type(v)) for k, v in kwargs.items()]
             if kwargs is not None
             else None
         )
 
         # These are needed only at trigger-time but values must be set at init.
-        self.time = now_ms()
+        self.time_ns = time.time_ns()
         self.thread = threading.current_thread().ident
         self.event_id = ContrastEvent._atomic_id()
 
         self.event_action = self.node.build_action()
 
         self._raw_stack = build_stack() if self._should_get_stack else []
 
@@ -195,14 +197,18 @@
             self.tags_override = (
                 None
                 if len(self.tagged.value) == len_or_zero(tagged)
                 else (Tag(len(self.tagged.value), 0),)
             )
 
     @property
+    def parent_ids(self):
+        return [parent.event_id for parent in self.parents]
+
+    @property
     def _should_get_stack(self):
         """
         Determine if event.stack should be populated or not.
 
         Get stacktrace for the event EXCEPT if
           1. the node explicitly indicates not to collect a stacktrace, which is the
                 case for WSGI environ sources
@@ -278,15 +284,15 @@
         """
         Convert a ContrastEvent to a TraceEvent.
         """
         event = TraceEvent()
 
         event.type = self.node.node_type
         event.action = self.event_action
-        event.timestamp_ms = self.time
+        event.timestamp_ms = self.time_ns // 1_000_000
         event.thread = str(self.thread)
         event.tags = self.node.tags
 
         self._build_all_event_objects(event)
 
         event.stack = clean_stack(self._raw_stack, depth=20)
 
@@ -294,19 +300,18 @@
         event.field_name = safe_source_name
 
         if self.source_type:
             event.event_sources.append(self.build_source_event(safe_source_name))
 
         event.object_id = int(self.event_id)
 
-        if self.parent_ids:
-            for parent_id in self.parent_ids:
-                parent = ParentObjectId()
-                parent.id = parent_id
-                event.parent_object_ids.append(parent)
+        for parent_id in self.parent_ids:
+            parent = ParentObjectId()
+            parent.id = parent_id
+            event.parent_object_ids.append(parent)
 
         self._build_complete_signature(event)
         self._validate_event(event)
 
         return event
 
     def _update_init_return(self, node, obj, ret):
@@ -447,7 +452,94 @@
         if (
             event.action == TraceEvent.Action[TRIGGER_TYPE]
             and event.source[0] not in allowed_trigger_sources
         ):
             # If this is logged, check the node in policy.json corresponding to
             # this event and how the agent has transformed the source string
             logger.debug("WARNING: trigger event TS-invalid source %s", event.source)
+
+    def history(self: "ContrastEvent"):
+        """
+        Return a generator that yields all the events in the history of this event,
+        starting with the event itself and then its parents, and so on.
+
+        Events are yielded in depth-first order, so the event itself is yielded first,
+        then its last parent, then the last parent of that parent, and so on.
+
+        Events are deduplicated, so if an event is seen more than once, it will not be
+        yielded again.
+        """
+        seen = set()
+        queue = [self]
+        while queue:
+            event = queue.pop()
+            seen.add(event)
+            yield event
+            queue.extend(event for event in event.parents if event not in seen)
+
+    def dot_repr(self: "ContrastEvent") -> str:
+        """
+        Returns a DOT graph representation of self's history.
+        """
+        return str(DotGraph(self))
+
+
+@dataclass
+class DotGraph:
+    event: ContrastEvent
+    normalize: bool = False
+    _seen_events: Dict[ContrastEvent, int] = field(default_factory=dict, init=False)
+
+    def __str__(self):
+        dot_lines = [
+            "digraph {",
+            "   node [shape=plain];",
+        ]
+        for event in self.event.history():
+            dot_lines.append(self._node(event))
+            dot_lines.extend(self._edge(parent, event) for parent in event.parents)
+        dot_lines.append("}")
+        return "\n".join(dot_lines)
+
+    def _node(self, event: ContrastEvent) -> str:
+        return f"""{self._event_id(event)} [label=<
+        <table cellborder="0" cellspacing="10" style="rounded" {self._tooltip(event)}>
+        <tr><td align="text" cellpadding="1"><b>{event.node}</b></td></tr>
+        <tr><td><table cellborder="1" cellspacing="0" cellpadding="15">
+            <tr><td align="text">data</td><td align="text"><font face="Monospace">{html_escape(event.tagged.value)}</font></td></tr>
+            {"".join(f"<tr><td align='text'>{tag}</td><td align='text'><font face='Monospace'>{self._tagrng_markup(rngs, len(event.tagged.value), untagged_marker='&nbsp;')}</font></td></tr>" for tag, rngs in (event.tagged_props.tags.items() if event.tagged_props else []) )}
+        </table></td></tr>
+        </table>>];"""
+
+    def _edge(self, parent: ContrastEvent, child: ContrastEvent) -> str:
+        return f"{self._event_id(parent)} -> {self._event_id(child)};"
+
+    def _event_id(self, event: ContrastEvent) -> int:
+        if self.normalize:
+            if event not in self._seen_events:
+                self._seen_events[event] = len(self._seen_events) + 1
+            return self._seen_events[event]
+
+        return event.event_id
+
+    def _tooltip(self, event: ContrastEvent) -> str:
+        if self.normalize:
+            return ""
+
+        # intentionally avoid using clean_stack because it formats filenames
+        # replacing / with ., which makes them unusable as links.
+        frame = next(
+            (frame for frame in reversed(event._raw_stack) if acceptable_frame(frame)),
+            None,
+        )
+
+        return (
+            f'tooltip="{html_escape(frame.line)}" href="file://{frame.filename}"'
+            if frame
+            else ""
+        )
+
+    def _tagrng_markup(self, rngs, length, tag_marker="*", untagged_marker=" ") -> str:
+        return "".join(
+            tag_marker if any(rng.covers(i) for rng in rngs) else untagged_marker
+            for i in range(length)
+        )
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/analysis.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/analysis.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/deadzone_node.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/deadzone_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/patches.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/preshift.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/preshift.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagation_node.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagation_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagation_policy.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagation_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         copy_from(target, self_obj, 0, set())
 
 
 STREAM_SOURCES = ["read", "read1", "readline", "readlines", "getvalue"]
 STREAM_WRITE_METHODS = ["write", "writelines"]
 
 
-def create_stream_event(node_type, stream, args, kwargs):
+def create_stream_event(node_type, parents, stream, args, kwargs):
     context = contrast.CS__CONTEXT_TRACKER.current()
     if context is None or not Settings().is_assess_enabled():
         return None
 
     module = stream.__class__.__module__
     class_name = stream.__class__.__name__
 
@@ -101,28 +101,28 @@
             "__init__",
             "ARG_0,KWARG:initial_value",
             "RETURN",
             source_type,
             None,
         )
 
-    return ContrastEvent(node, stream, stream, None, args, kwargs, [], 0, None)
+    return ContrastEvent(node, stream, stream, None, args, kwargs, parents, 0, None)
 
 
 def create_stream_source_event(stream, args, kwargs):
     """
     Called directly from C extensions to create source events for __init__
     """
     context = contrast.CS__CONTEXT_TRACKER.current()
     if context is None:
         return
 
     source_type = safe_getattr(stream, "cs__source_type", None) or "BODY"
 
-    init_event = create_stream_event("source", stream, args, kwargs)
+    init_event = create_stream_event("source", [], stream, args, kwargs)
     stream.cs__source_event = init_event
 
     if context.stop_source_creation(context, source_type, None):
         return
 
     if len(args) > 0:
         properties = get_properties(args[0])
@@ -136,19 +136,18 @@
 
 
 def _add_and_track_event_to_stream(stream, properties, args, kwargs):
     stream_props = Properties(stream)
     set_properties(stream, stream_props)
     copy_tags_to_offset(stream_props, properties.tags, 0)
     copy_events(stream_props, properties)
-    prop_event = create_stream_event("propagation", stream, args, kwargs)
+    parents = [properties.event] if properties.event else []
+    prop_event = create_stream_event("propagation", parents, stream, args, kwargs)
     if prop_event is not None:
-        if len(properties.events) > 0:
-            prop_event.parent_ids = [properties.events[-1].event_id]
-        stream_props.add_event(prop_event)
+        stream_props.event = prop_event
     stream.cs__tracked = True
 
 
 def propagate_stream(method_name, target, self_obj, ret, args, kwargs):
     """
     Called directly from C extensions to propagate stream operations.
     """
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/__init__.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/append_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/append_propagator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 from contrast.agent.assess.policy.propagators.base_propagator import BasePropagator
 from contrast.agent.assess.utils import (
     copy_events,
     copy_tags_to_offset,
     copy_from,
+    get_last_event_from_sources,
     get_properties,
 )
 
 from contrast_vendor import structlog as logging
 
 logger = logging.getLogger("contrast")
 
 
 class AppendPropagator(BasePropagator):
+    def get_parents(self, ret):
+        return get_last_event_from_sources(self.sources)
+
     def _propagate(self):
         second_source = None
 
         if len(self.sources) > 1:
             second_source = self.sources[1]
 
         # if the object and the return are the same length just copy the tags
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/base_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/base_propagator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 from contrast.agent.assess.adjusted_span import AdjustedSpan
-from contrast.agent.assess.policy.source_policy import get_parent_ids
+from contrast.agent.assess.policy.source_policy import get_parents
 from contrast.agent.assess.tag import Tag
 from contrast.utils.assess import tracking_util
 from contrast.utils.assess.tag_utils import combine, is_covered
 from contrast.utils.decorators import cached_property, fail_quietly
 from contrast.agent.assess.utils import (
     is_tracked,
     get_properties,
@@ -20,14 +20,15 @@
         """
         :param node: instance of PropagationNode
         """
         self.node = node
         self.preshift = preshift
         self.target = target
         self.target_properties = None
+        self._splat_parents = []
 
     @cached_property
     def sources(self):
         """
         Get all the sources for the propagation node.
         """
         return self.node.get_matching_sources(self.preshift)
@@ -69,30 +70,30 @@
         if self.target_properties is None:
             return
 
         self.first_source = self.sources[0]
         self._propagate()
         self.target_properties.cleanup_tags()
 
-    def get_parent_ids(self, ret):
+    def get_parents(self, ret):
         """Some derived classes may need to override this method"""
-        return get_parent_ids(
+        return self._splat_parents or get_parents(
             self.node, self.preshift.obj, ret, self.preshift.args, self.preshift.kwargs
         )
 
     def build_event(self, target_properties, ret):
-        parent_ids = self.get_parent_ids(ret)
+        parents = self.get_parents(ret)
         target_properties.build_event(
             self.node,
             self.target,
             self.preshift.obj,
             ret,
             self.preshift.args,
             self.preshift.kwargs,
-            parent_ids,
+            parents,
             None,
         )
 
     def splat_tags(self, source, ret):
         """
         SPLAT copies tags for cases where the string transformation is unknown
 
@@ -115,14 +116,17 @@
 
         ret_props = get_properties(ret)
         if ret_props is None:
             return
 
         ret_length = len(ret)
 
+        if source_props.event:
+            self._splat_parents.append(source_props.event)
+
         untrusted_ranges = source_props.tags.get("UNTRUSTED") or []
         if untrusted_ranges:
             # splat UNTRUSTED ranges across the entire output
             ret_props.add_tag("UNTRUSTED", AdjustedSpan(0, ret_length))
 
         for name, ranges in source_props.tags.items():
             if name == "UNTRUSTED":
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,11 +84,11 @@
             col_value_properties.build_event(
                 self.node,
                 col_value_properties.origin,
                 self.preshift.obj,
                 self.target,
                 self.preshift.args,
                 self.preshift.kwargs,
-                [],
+                [col_value_properties.event] if col_value_properties.event else [],
                 0,
                 None,
             )
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/format_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/format_propagator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 from contrast.agent.assess.adjusted_span import AdjustedSpan
 from contrast.agent.assess.policy.propagators import BasePropagator
 from contrast.agent.assess.utils import (
     copy_events,
-    get_last_event_ids_from_sources,
+    get_last_event_from_sources,
     get_properties,
     track_string,
 )
 from contrast.utils.assess import tracking_util
 from contrast.utils.assess.tag_utils import merge_tags
 from contrast.utils.assess.formatting import FormatToken, StringToken
 from contrast.utils.assess.formatting.tokenize_format import tokenize_format
@@ -36,16 +36,16 @@
                 sources.append(token.get_arg(self.preshift.args, self.preshift.kwargs))
         return sources + [self.preshift.obj]
 
     @cached_property
     def tracked_sources(self):
         return any(tracking_util.recursive_is_tracked(src) for src in self.sources)
 
-    def get_parent_ids(self, *args):
-        return get_last_event_ids_from_sources(self.sources)
+    def get_parents(self, *args):
+        return get_last_event_from_sources(self.sources)
 
     @property
     def inputs_require_propagation(self):
         if tracking_util.recursive_is_tracked(self.preshift.obj):
             return True
 
         return self.tracked_sources
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/join_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/join_propagator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 from contrast.agent.assess.policy.propagators import SUPPORTED_TYPES, BasePropagator
 from contrast.utils.assess.tag_utils import merge_tags
 from contrast.agent.assess.utils import (
     copy_events,
-    get_last_event_ids_from_sources,
+    get_last_event_from_sources,
     get_properties,
     is_tracked,
 )
 from contrast.utils.decorators import cached_property
 from contrast.utils.string_utils import ensure_string
 
 
@@ -20,16 +20,16 @@
                 target_props.add_existing_tag(label, new_tag)
 
     def __init__(self, node, preshift, target):
         super().__init__(node, preshift, target)
         self.strings_to_join = self.preshift.args[0] if self.preshift.args else []
         self.separator = self.preshift.obj
 
-    def get_parent_ids(self, *args):
-        return get_last_event_ids_from_sources(self.sources)
+    def get_parents(self, *args):
+        return get_last_event_from_sources(self.sources)
 
     @cached_property
     def sources(self):
         return [self.preshift.obj] + self.preshift.args[0]
 
     @property
     def needs_propagation(self):
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/json_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/json_propagator.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,17 +65,14 @@
         """
         target = self.target
 
         item_properties = get_properties(item)
         target_properties = get_properties(target) or track_string(target)
 
         if item_properties and target_properties:
-            for event in item_properties.events:
-                target_properties.events.append(event)
-
             self.splat_tags(item, target)
 
             target_properties.cleanup_tags()
 
         return target_properties
 
     def track_target(self):
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from contrast.agent.policy import registry
 from contrast.agent.assess.policy.preshift import Preshift
 from contrast.agent.assess.utils import (
     copy_events,
     copy_tags_in_span,
     copy_tags_to_offset,
     get_properties,
-    get_last_event_id,
     track_string,
 )
 from contrast.utils.decorators import fail_quietly
 
 from functools import lru_cache
 
 from .split_propagator import SplitPropagator
@@ -35,26 +34,26 @@
         return
 
     target_properties = copy_tags_in_span(target, source_properties, span)
     # This can be None if len(target) < 2
     if target_properties is None:
         return
 
-    parent_ids = [get_last_event_id(source_properties)]
+    parents = [source_properties.event] if source_properties.event else []
 
     copy_events(target_properties, source_properties)
 
     target_properties.build_event(
         policy_node,
         target,
         preshift.obj,
         retval,
         preshift.args,
         preshift.kwargs,
-        parent_ids,
+        parents,
     )
 
 
 @fail_quietly("Failed to propagate regex group")
 def propagate_group(self_obj, target, *args):
     """
     Propagator for re.Match.group()
@@ -180,26 +179,26 @@
     target_properties,
     orig_properties,
     repl_properties,
     target,
     args,
     kwargs,
 ):
-    parent_ids = []
-    if orig_properties is not None:
-        parent_ids.append(get_last_event_id(orig_properties))
+    parents = []
+    if orig_properties is not None and orig_properties.event:
+        parents.append(orig_properties.event)
 
     copy_events(target_properties, orig_properties)
 
     for props in repl_properties:
         copy_events(target_properties, props)
-        if props is not None:
-            parent_ids.append(get_last_event_id(props))
+        if props is not None and props.event:
+            parents.append(props.event)
 
-    target_properties.build_event(node, target, None, target, args, kwargs, parent_ids)
+    target_properties.build_event(node, target, None, target, args, kwargs, parents)
 
 
 @fail_quietly("Failed to propagate regex sub(n)")
 def propagate_sub(node, target, repl_results, pattern, repl, string, count=0, **kwargs):
     """
     Propagator for re.sub and re.subn
     """
@@ -311,19 +310,19 @@
                 target_index += 1
 
     def propagate(self):
         string = self.sources[0]
         flags = self._get_flags()
         pattern = self._get_pattern()
 
-        source_properties = get_properties(string)
-        if source_properties is None:
+        self.source_properties = get_properties(string)
+        if self.source_properties is None:
             return
 
-        self._propagate(string, flags, pattern, source_properties)
+        self._propagate(string, flags, pattern, self.source_properties)
 
 
 class RegexFindallPropagator(RegexSplitPropagator):
     def propagate(self):
         """
         Propagation action for re.findall and re.Pattern.findall
 
@@ -334,50 +333,54 @@
 
         When the number of groups is greater than 1, findall returns a list of tuples
         where each tuple represents the groups corresponding to a given match. In this
         case, we use finditer to get the corresponding Match instances in order to
         determine the spans to use for propagation.
         """
         string = self.sources[0]
-        source_props = get_properties(string)
-        if source_props is None:
+        self.source_properties = get_properties(string)
+        if self.source_properties is None:
             return
 
         flags = self._get_flags()
         pattern = re.compile(self._get_pattern())
         if pattern.groups < 2:
-            self._propagate(string, flags, pattern, source_props)
+            self._propagate(string, flags, pattern, self.source_properties)
             return
 
         # We know we're in scope here, so we're safe to call finditer
         matches = (
             pattern.finditer(string)
             if self.is_pattern_method
             else re.finditer(pattern, string, flags)
         )
 
         for target, match in zip(self.target, matches):
             for i, result in enumerate(target):
                 target_properties = copy_tags_in_span(
                     result,
-                    source_props,
+                    self.source_properties,
                     # skip the first span since it duplicates the entire match
                     match.span(i + 1),
                 )
 
                 # This can be None if len(target) < 2
                 if target_properties is None:
                     continue
 
-                parent_ids = [get_last_event_id(source_props)]
+                parents = (
+                    [self.source_properties.event]
+                    if self.source_properties.event
+                    else []
+                )
 
-                copy_events(target_properties, source_props)
+                copy_events(target_properties, self.source_properties)
 
                 target_properties.build_event(
                     self.node,
                     result,
                     self.preshift.obj,
                     result,
                     self.preshift.args,
                     self.preshift.kwargs,
-                    parent_ids,
+                    parents,
                 )
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,18 +93,10 @@
                     _append_if_tracked(item)
 
         return tracked_inputs
 
     def _apply_splat_tags(self, tracked_inputs):
         for item in tracked_inputs:
             if item is not self.target:
-                item_properties = get_properties(item)
-
-                if not item_properties:
-                    continue
-
-                for event in item_properties.events:
-                    self.target_properties.events.append(event)
-
                 self.splat_tags(item, self.target)
 
         self.target_properties.cleanup_tags()
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/split_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/split_propagator.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,30 +21,33 @@
     def needs_propagation(self):
         if not self.preshift:
             return False
 
         return tracking_util.recursive_is_tracked(self.preshift.obj)
 
     def build_event(self, target_properties, tagged):
-        parent_ids = self.get_parent_ids(tagged)
+        parents = [self.source_properties.event] if self.source_properties.event else []
         # For split, the tagged individual string is passed when building the
         # event, but the target is actually the array of strings that was
         # returned by split.
         target_properties.build_event(
             self.node,
             tagged,
             self.preshift.obj,
             self.target,
             self.preshift.args,
             self.preshift.kwargs,
-            parent_ids,
+            parents,
             None,
         )
 
     def add_tags_and_properties(self, ret):
+        if self.source_properties is None:
+            return
+
         for target in self.target:
             if self.node.tags:
                 self.apply_tags(self.node, target)
 
             if self.node.untags:
                 self.apply_untags(self.node, target)
 
@@ -53,42 +56,44 @@
                 continue
 
             target_properties.add_properties(self.node.properties)
 
             self.build_event(target_properties, target)
 
     def propagate(self):
-        reverse = self.node.method_name in self.REVERSE_METHODS
-
-        if self.node.method_name in self.PARTITION_METHODS:
-            partition = self.preshift.args[0]
-        else:
-            partition = None
-
         source = self.preshift.obj
-        source_properties = get_properties(source)
+        self.source_properties = get_properties(source)
+        if self.source_properties is None:
+            return
 
         # Offset in the original string
         source_offset = 0
 
+        reverse = self.node.method_name in self.REVERSE_METHODS
+
         # The target (result of split) is an array of strings
         target = self.target[::-1] if reverse else self.target
 
+        if self.node.method_name in self.PARTITION_METHODS:
+            partition = self.preshift.args[0]
+        else:
+            partition = None
+
         for newstr in target:
             if reverse:
                 source_offset = source.rfind(newstr)
                 source = source[:source_offset]
             else:
                 source_offset = source.find(newstr, source_offset)
 
             if partition and newstr == partition:
                 # Make sure that we don't skip another string that just happens
                 # to be the same as the partition string.
                 partition = None
                 continue
 
             span = (source_offset, source_offset + len(newstr))
-            copy_tags_in_span(newstr, source_properties, span)
+            copy_tags_in_span(newstr, self.source_properties, span)
 
             target_properties = get_properties(newstr)
             if target_properties is not None:
-                copy_events(target_properties, source_properties)
+                copy_events(target_properties, self.source_properties)
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from contrast.agent.assess.adjusted_span import AdjustedSpan
 from contrast.agent.assess.policy.propagation_node import PropagationNode
 from contrast.agent.assess.utils import (
     copy_events,
     copy_tags_in_span,
     copy_tags_to_offset,
-    get_last_event_id,
     get_properties,
     set_properties,
 )
 
 
 from contrast_vendor import structlog as logging
 
@@ -34,17 +33,17 @@
     """Copies tags and creates event for stream read operations"""
     source_properties = get_properties(preshift.obj)
     target_properties = copy_tags_in_span(target, source_properties, tag_span)
     if target_properties is None:
         return
 
     copy_events(target_properties, source_properties)
-    parent_ids = [get_last_event_id(source_properties)]
+    parents = [source_properties.event] if source_properties.event else []
     target_properties.build_event(
-        node, target, preshift.obj, ret, preshift.args, preshift.kwargs, parent_ids
+        node, target, preshift.obj, ret, preshift.args, preshift.kwargs, parents
     )
 
 
 def propagate_stream_read(method_name, preshift, target, ret):
     class_name = _get_class_name(preshift.obj)
     node = PropagationNode(
         "io", class_name, True, method_name, "OBJ", "RETURN", "STREAM_READ"
@@ -135,44 +134,44 @@
     curpos = preshift.obj.tell()
     # Compute the position of the stream cursor before the write occurred
     startpos = curpos - sum([len(line) for line in lines])
 
     # Copy any tags from the original stream outside of the span of newly written data
     new_props = _copy_old_props_from_stream(preshift.obj, startpos, curpos)
 
-    parent_ids = []
+    parents = []
 
     # TODO: PYT-911 this is not quite right. We make it look like the most recent event on
     # the original string contributes to the `write` event, but that's not really
     # accurate. Instead, the write event and the stream event should contribute to any
     # subsequent `read` events. But this requires an additional level of bookkeeping.
     # We'll pass for now since it only affects trace reports, and not accuracy.
-    if new_props is not None and new_props.events:
-        parent_ids.append(new_props.events[-1].event_id)
+    if new_props is not None and new_props.event:
+        parents.append(new_props.event)
 
     # Iterate over all newly written lines and copy tags if the line is tracked
     for line, source_props in zip(lines, props):
         if source_props is not None:
             # This means that the original stream was not tracked at all
             if new_props is None:
                 new_props = source_props.copy(tag_offset=startpos)
             else:
                 copy_tags_to_offset(new_props, source_props.tags, startpos)
                 copy_events(new_props, source_props)
 
-            if source_props.events:
-                parent_ids.append(source_props.events[-1].event_id)
+            if source_props.event:
+                parents.append(source_props.event)
 
         startpos += len(line)
 
     # Update with new properties on stream object
     preshift.obj.cs__tracked = True
     set_properties(preshift.obj, new_props)
 
     # Add event
     class_name = _get_class_name(preshift.obj)
     node = PropagationNode(
         "io", class_name, True, method_name, "ARG_0", "OBJ", "STREAM_WRITE"
     )
     new_props.build_event(
-        node, target, preshift.obj, ret, preshift.args, preshift.kwargs, parent_ids
+        node, target, preshift.obj, ret, preshift.args, preshift.kwargs, parents
     )
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/source_node.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/source_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/source_policy.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/source_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import contrast
 from contrast.agent.assess.adjusted_span import AdjustedSpan
 from contrast.agent.assess.policy.source_node import SourceNode
 from contrast.agent.assess.properties import Properties
 from contrast.agent.assess.utils import (
     get_properties,
-    get_last_event_ids_from_sources,
+    get_last_event_from_sources,
     is_trackable,
     set_properties,
     track_string,
 )
 from contrast.agent.policy.constants import OBJECT, RETURN
 from contrast.agent.settings import Settings
 from contrast.utils.assess.duck_utils import is_iterable, safe_getattr, safe_iterator
@@ -274,24 +274,18 @@
     if not context or not node or target is None:
         return
 
     if context.stop_source_creation(context, source_type, source_name):
         return
 
     target_properties = get_properties(target)
-    if target_properties is not None:
-        all_cookie_sources = all(
-            [
-                e.source_type == "COOKIE"
-                for e in target_properties.events
-                if e.source_type is not None
-            ]
-        )
-        if all_cookie_sources:
-            source_type = "COOKIE"
+    if target_properties is not None and all(
+        e.source_type == "COOKIE" for e in target_properties.events if e.source_type
+    ):
+        source_type = "COOKIE"
         # Discard any preexisting tags or events for this string. This greatly
         # simplifies reporting by retaining only the most recent source event for each
         # string
         target_properties.reset()
     if target_properties is None and is_trackable(target):
         target_properties = track_string(target)
     if target_properties is not None:
@@ -306,23 +300,23 @@
                 logger.debug(
                     "Source %s detected: %s tagged with %s",
                     node.name,
                     truncated_signature(target),
                     str(tag),
                 )
 
-        parent_ids = get_parent_ids(node, self_obj, ret, args, kwargs)
+        parents = get_parents(node, self_obj, ret, args, kwargs)
         target_properties.build_event(
             node,
             target,
             self_obj,
             ret,
             args,
             kwargs,
-            parent_ids,
+            parents,
             possible_key=None,
             source_type=source_type,
             source_name=source_name,
         )
 
         context.source_created()
 
@@ -419,22 +413,22 @@
 
     if kwargs and source in kwargs:
         return kwargs[source]
 
     return None
 
 
-def get_parent_ids(node, self_obj, ret, args, kwargs):
+def get_parents(node, self_obj, ret, args, kwargs):
     if isinstance(node, SourceNode):
         return []
 
     sources = [
         value_of_source(source, self_obj, ret, args, kwargs) for source in node.sources
     ]
-    return get_last_event_ids_from_sources(sources)
+    return get_last_event_from_sources(sources)
 
 
 def build_source_node(source_dict, method_name, source_type):
     """
     Useful for explicit source tracking, ie scope tracking / aiohttp request tracking.
 
     Note that headers (including cookies) should not trigger XSS, per labs
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/string_propagation.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/string_propagation.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 Builds/defines propagation functions to be called from C extension hooks
 
 NOTE: This module will need to be loaded before the extension executes
 """
 import sys
 
+from contrast.agent.assess.utils import is_tracked
 from contrast_vendor import structlog as logging
 
 import contrast
 from contrast.agent.assess.policy.preshift import Preshift
 from contrast.agent.assess.policy.propagation_policy import track_copy_without_new_event
 
 # We call these from the C extension - they're import aliases
@@ -202,15 +203,21 @@
 
     Having a separate builder here allows us to optimize for the translate special case
     without imposing a blanket performance overhead on all other unicode/bytes methods.
     """
     propagator_class = PROPAGATOR_ACTIONS.get(policy_node.action, BasePropagator)
 
     def propagate_cast(target, self_obj, ret, args, kwargs):
-        if ret is (args and args[0]):
+        if ret is (args and args[0]) or is_tracked(ret):
+            # If the return value is the same as the first argument,
+            # then no new object was created and we'll already be tracking
+            # the return value (or not).
+            # If the return value is already tracked, we already propagated
+            # to it (likely via a custom __str__ or __bytes__ method) and
+            # don't need to do so again.
             return
 
         context = contrast.CS__CONTEXT_TRACKER.current()
         if context is None or context.stop_propagation:
             return
 
         preshift = Preshift(self_obj, args or [], kwargs or {})
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_policy.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_policy.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/preflight.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/preflight.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/properties.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,30 +28,49 @@
     @property
     def timestamp(self):
         # NOTE: timestamp must not be modified. This affects string tracker age-off.
         return self._timestamp
 
     def reset(self):
         self.tags = {}
-        self.events = []
+        self._event = None
         self.dynamic_source_metadata = {}
 
+    def _get_event(self):
+        return self._event
+
+    def _set_event(self, event):
+        self._event = event
+        for parent in event.parents:
+            self.report_source(parent)
+
+    event = property(_get_event, _set_event)
+
+    @property
+    def events(self):
+        if self.event:
+            history = list(self.event.history())
+            history.reverse()
+            history.sort(key=lambda e: e.time_ns)
+            return history
+        return []
+
     def copy(self, tag_offset=0):
         """
         Return a (shallow) copy of this object
         """
         new = self.__class__(self.origin)
 
         # Copy tags to given offset
         new.tags = {}
         for name, tag_list in self.tags.items():
             new.tags[name] = [tag.copy_modified(tag_offset) for tag in tag_list]
 
-        # Creating copies of the events themselves should not be necessary
-        new.events = self.events[:]
+        # Creating a copy of the event itself should not be necessary
+        new._event = self._event
         new.dynamic_source_metadata = dict(self.dynamic_source_metadata)
 
         return new
 
     def __repr__(self):
         return f"Properties({repr(self.origin)}, {self.tags})"
 
@@ -279,57 +298,46 @@
         current tags: 0-15
         range:        5-10
         result:       0-5, 10-20
         """
         for item in ranges:
             self.shift_tags_for_insertion(item)
 
-    def add_event(self, event):
-        """
-        Add event to properties
-        """
-        self.events.append(event)
-
-        self.report_source()
-
-        return self
-
     def build_event(
         self,
         policy_node,
         tagged,
         self_obj,
         ret,
         args,
         kwargs,
-        parent_ids,
+        parents,
         possible_key=None,
         source_type=None,
         source_name=None,
     ):
         """
         Build ContrastEvent from an applied policy method
 
         After creation of the ContrastEvent, report the event to the observed_route in the RequestContext
         """
-        event = ContrastEvent(
+        self.event = ContrastEvent(
             policy_node,
             tagged,
             self_obj,
             ret,
             args,
             kwargs,
-            parent_ids,
+            parents,
             possible_key,
             source_type,
             source_name,
         )
-        self.add_event(event)
 
-    def report_source(self):
+    def report_source(self, event):
         """
         This is for Route-based Auto-remediation
 
         We want to associate source events with routes. However, we only want to record
         sources if they are actually used. The reason for this is that the Python agent
         is fairly aggressive with source tracking, and so we preemptively track many
         sources even if they are never used. But to avoid inaccurate RBAV reports, we
@@ -340,24 +348,16 @@
         - Previous event doesn't have a source type, do nothing
         - No current context and therefore no observed route, do nothing
         - There is an event of the same name and type, do nothing
         - Can create the TraceEventSource, append to the observed route sources
 
         :return: None
         """
-        if len(self.events) < 2:
-            return
-
-        # Check whether the last event before the newest one was a source event.
-        # Before this method is called, we add the newest event, which is now
-        # self.events[-1]. So we check the event prior to that to see whether it's a
-        # source event.
-        event = self.events[-2]
 
-        if not event.source_type:
+        if event is None or not event.source_type:
             return
 
         context = contrast.CS__CONTEXT_TRACKER.current()
 
         if not context:
             return
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/base_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/base_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/base_config_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/base_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/session_age_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/session_age_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/dataflow_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/dataflow_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/non_dataflow_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/non_dataflow_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/enable.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/enable.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/analyze.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/analyze.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     ]
 
     if not valid_response_rules:
         return
 
     form_tags, meta_tags = get_tags(body, content_type)
 
+    logger.debug("Analyzing response rules", response_rules=valid_response_rules)
+
     for rule in valid_response_rules:
         violated, properties = rule.is_violated(
             response.headers, body, form_tags, meta_tags
         )
         if violated:
             rule.build_and_append_finding(properties, context)
 
@@ -79,14 +81,16 @@
     except AssertionError as exc:
         # Invalid HTML throws assertion errors. HTMLParser doesn't expose an API
         # to disable these assertions.
         # We don't validate that the body is HTML, and the error can be ignored
         # if the body isn't HTML. If the body is HTML or we partially parsed
         # tags, throw the exception so that we can investigate the issue.
         if "html" in content_type:
-            raise Exception(f"Failed to parse response body {content_type=}") from exc
+            raise RuntimeError(
+                f"Failed to parse response body {content_type=}"
+            ) from exc
         if parser.form_tags or parser.meta_tags:
-            raise Exception(
+            raise RuntimeError(
                 f"Partially parsed response body {parser.form_tags=} {parser.meta_tags=}"
             ) from exc
 
     return parser.form_tags, parser.meta_tags
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/base_response_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/base_response_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/xss.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/xss.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/static_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/static_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/trigger_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/sampling.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/sampling.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/string_tracker.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/string_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/tag.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/tag.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/truncate.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/truncate.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/assess/utils.py` & `contrast_agent-8.1.0/src/contrast/agent/assess/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -41,19 +41,23 @@
         end = len(value)
 
     properties.add_tag(label, AdjustedSpan(start, end))
     return properties
 
 
 def copy_events(target_props, source_props):
-    if source_props is None or target_props is None or target_props is source_props:
+    if (
+        source_props is None
+        or target_props is None
+        or target_props is source_props
+        or source_props.event is None
+    ):
         return
 
-    for event in source_props.events:
-        target_props.events.append(event)
+    target_props.event = source_props.event
 
 
 def copy_from(to_obj, from_obj, shift=0, skip_tags=None):
     """Copy events and tags from from_obj to to_obj"""
     if from_obj is to_obj:
         return
 
@@ -98,37 +102,23 @@
     for node in patch_policy.all_nodes:
         if not node.instance_method:
             return None
 
     return args[0] if args else None
 
 
-def get_last_event_id(source_properties):
-    if source_properties.events and source_properties.events[-1]:
-        last_event = source_properties.events[-1]
-        return last_event.event_id
-    return None
-
-
-def get_last_event_ids_from_sources(sources):
+def get_last_event_from_sources(sources):
     """
     Gathers from given sources the parent IDs that should be used for an event
     """
-    id_list = []
-
-    for source in sources:
-        source_properties = get_properties(source)
-        if source_properties is None:
-            continue
-
-        event_id = get_last_event_id(source_properties)
-        if event_id is not None and event_id not in id_list:
-            id_list.append(event_id)
-
-    return id_list
+    return [
+        props.event
+        for source in sources
+        if (props := get_properties(source)) and props.event
+    ]
 
 
 def copy_tags_in_span(target, source_properties, span, offset=0):
     """
     Given source properties, copies tags at a given span to the target
     """
     span = AdjustedSpan(*tuple(x + offset for x in span))
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/disable_reaction.py` & `contrast_agent-8.1.0/src/contrast/agent/disable_reaction.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/events.py` & `contrast_agent-8.1.0/src/contrast/agent/events.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/exceptions.py` & `contrast_agent-8.1.0/src/contrast/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/exclusions.py` & `contrast_agent-8.1.0/src/contrast/agent/exclusions.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/framework.py` & `contrast_agent-8.1.0/src/contrast/agent/framework.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/heartbeat_thread.py` & `contrast_agent-8.1.0/src/contrast/agent/heartbeat_thread.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/metrics.py` & `contrast_agent-8.1.0/src/contrast/agent/metrics.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/app_finder.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/app_finder.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/base_middleware.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/base_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,19 +44,19 @@
         yield
     finally:
         logger.debug(
             "Ending request analysis",
             request_method=request_method,
             request_path=request_path,
         )
-        logger.debug(
-            "elapsed time request analysis ms",
-            elapsed_time=timer.now_ms() - start_time,
-            request_method=request_method,
+        logger.info(
+            "request summary",
             request_path=request_path,
+            request_method=request_method,
+            elapsed_time_ms=timer.now_ms() - start_time,
         )
 
 
 def _log_response_info(response: BaseResponseWrapper):
     if response is None:
         logger.debug("No response info for this request")
         return
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/environ_tracker.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/environ_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/common.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/common.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/django_routes.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/django_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py` & `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/patch_controller.py` & `contrast_agent-8.1.0/src/contrast/agent/patch_controller.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/policy/applicator.py` & `contrast_agent-8.1.0/src/contrast/agent/policy/applicator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/policy/constants.py` & `contrast_agent-8.1.0/src/contrast/agent/policy/constants.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/policy/patch_location_policy.py` & `contrast_agent-8.1.0/src/contrast/agent/policy/patch_location_policy.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/policy/patch_manager.py` & `contrast_agent-8.1.0/src/contrast/agent/policy/patch_manager.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/policy/policy_node.py` & `contrast_agent-8.1.0/src/contrast/agent/policy/policy_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/policy/registry.py` & `contrast_agent-8.1.0/src/contrast/agent/policy/registry.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/policy/rewriter.py` & `contrast_agent-8.1.0/src/contrast/agent/policy/rewriter.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/policy/trigger_node.py` & `contrast_agent-8.1.0/src/contrast/agent/policy/trigger_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/policy/utils.py` & `contrast_agent-8.1.0/src/contrast/agent/policy/utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/input_analysis.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/input_analysis.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/policy/__init__.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/base_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/base_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from contrast.utils.string_utils import ensure_string
 
 logger = logging.getLogger("contrast")
 
 
 BLOCKING_RULES = frozenset([Mode.BLOCK, Mode.BLOCK_AT_PERIMETER])
 PREFILTER_RULES = frozenset([Mode.BLOCK_AT_PERIMETER])
-POSTFILTER_RULES = frozenset([Mode.BLOCK, Mode.MONITOR, Mode.PERMIT])
+POSTFILTER_RULES = frozenset([Mode.BLOCK, Mode.MONITOR])
 
 PREFILTER = "prefilter"
 INFILTER = "infilter"
 POSTFILTER = "postfilter"
 
 
 class BaseRule:
@@ -132,15 +132,15 @@
             raise contrast.SecurityException(rule_name=self.name)
 
     def _infilter(self, match_string, **kwargs):
         """
         Scans the input analysis for the rule and looks for matched attack signatures. The call to this method may be
         rule specific and include additional context in a args list.
         """
-        if self.mode in [Mode.OFF, Mode.PERMIT]:
+        if self.mode == Mode.OFF:
             return
 
         logger.debug("PROTECT: Infilter for %s", self.name)
 
         attack = self.find_attack(match_string, analysis_stage=INFILTER, **kwargs)
         if attack is None or len(attack.samples) == 0:
             return
@@ -199,15 +199,15 @@
         """
         Scans the input analysis for the rule and looks for matched attack signatures
 
         Appends attacker to the context if a positive evaluation is found
         """
         logger.debug("PROTECT: Postfilter for %s", self.name)
 
-        if self.mode in [Mode.OFF, Mode.PERMIT]:
+        if self.mode == Mode.OFF:
             return
 
         attack = self.find_attack(analysis_stage=POSTFILTER)
         if attack is None or len(attack.samples) == 0:
             return
 
         self._append_to_context(attack)
@@ -367,15 +367,14 @@
         context.attacks.append(attack)
 
     _RESPONSE_MAP = {
         Mode.MONITOR: ProtectResponse.MONITORED,
         Mode.BLOCK: ProtectResponse.BLOCKED,
         Mode.BLOCK_AT_PERIMETER: ProtectResponse.BLOCKED_AT_PERIMETER,
         Mode.OFF: ProtectResponse.NO_ACTION,
-        Mode.PERMIT: ProtectResponse.NO_ACTION,
     }
 
     def response_from_mode(self, mode):
         return self._RESPONSE_MAP.get(mode)
 
     def evaluations_for_rule(self, context=None):
         if context is None:
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/cmdi_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/cmdi_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/http_method_tampering.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/http_method_tampering.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/nosqli_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/nosqli_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/path_traversal_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/path_traversal_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/rules_builder.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/rules_builder.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/sqli_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/sqli_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/ssrf_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/ssrf_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/xss_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/xss_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/protect/rule/xxe_rule.py` & `contrast_agent-8.1.0/src/contrast/agent/protect/rule/xxe_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/reaction_processor.py` & `contrast_agent-8.1.0/src/contrast/agent/reaction_processor.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/request.py` & `contrast_agent-8.1.0/src/contrast/agent/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,27 +36,32 @@
         self._masked_query_string = None
         self._parsed_http = None
 
         self.timestamp_ms = now_ms()
 
     @property
     def reportable_format(self):
+
         return {
             "body": truncate(ensure_string(self._reportable_body), length=4096),
             # the WSGI environ supports only one value per request header. However
             # the server decides to handle multiple headers, we're guaranteed to
             # have only unique keys in request.request_headers (since we iterate
             # over webob's EnvironHeaders). Thus, each value list here is length-1.
             "headers": {
-                ensure_string(k): [ensure_string(v)]
+                ensure_string(k): (
+                    ensure_string(v) if isinstance(v, list) else [ensure_string(v)]
+                )
                 for k, v in self._reportable_headers.items()
             },
             "method": ensure_string(self.method),
             "parameters": {
-                ensure_string(k): [ensure_string(v)]
+                ensure_string(k): (
+                    ensure_string(v) if isinstance(v, list) else [ensure_string(v)]
+                )
                 for k, v in self._reportable_params.items()
             },
             "port": int(self.host_port),
             "protocol": ensure_string(self.scheme),
             "queryString": ensure_string(self._reportable_query_string),
             "uri": ensure_string(self.path),
             "version": ensure_string(self._get_http_version()),
```

### Comparing `contrast_agent-8.0.0/src/contrast/agent/request_context.py` & `contrast_agent-8.1.0/src/contrast/agent/request_context.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/request_state.py` & `contrast_agent-8.1.0/src/contrast/agent/request_state.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/runner.py` & `contrast_agent-8.1.0/src/contrast/agent/runner.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/scope.py` & `contrast_agent-8.1.0/src/contrast/agent/scope.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/server_settings_poll.py` & `contrast_agent-8.1.0/src/contrast/agent/server_settings_poll.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/settings.py` & `contrast_agent-8.1.0/src/contrast/agent/settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/sys_monitoring.py` & `contrast_agent-8.1.0/src/contrast/agent/sys_monitoring.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/telemetry.py` & `contrast_agent-8.1.0/src/contrast/agent/telemetry.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/thread_watcher.py` & `contrast_agent-8.1.0/src/contrast/agent/thread_watcher.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/agent/validator.py` & `contrast_agent-8.1.0/src/contrast/agent/validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,18 @@
         """
         assert self.VALIDATIONS, "Child class must implement VALIDATIONS"
 
         for field_name, validations in self.VALIDATIONS.items():
             # The field_name we're validating must be defined as an attr to the class.
             try:
                 field_value = getattr(self, field_name)
-            except AttributeError:
+            except AttributeError as e:
                 raise ValidationException(
                     self, field_name, "field is not an attr of the class"
-                )
+                ) from e
 
             required = validations.get("required")
 
             # if field is required but it isn't populated.
             if required and not field_value:
                 raise ValidationException(
                     self, field_name, "field is required but empty"
```

### Comparing `contrast_agent-8.0.0/src/contrast/aiohttp/middleware.py` & `contrast_agent-8.1.0/src/contrast/aiohttp/middleware.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/aiohttp/sources.py` & `contrast_agent-8.1.0/src/contrast/aiohttp/sources.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/api/architecture_component.py` & `contrast_agent-8.1.0/src/contrast/api/architecture_component.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/api/attack.py` & `contrast_agent-8.1.0/src/contrast/api/attack.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/api/finding.py` & `contrast_agent-8.1.0/src/contrast/api/finding.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/api/library.py` & `contrast_agent-8.1.0/src/contrast/api/library.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/api/route_coverage.py` & `contrast_agent-8.1.0/src/contrast/api/route_coverage.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/api/trace_event.py` & `contrast_agent-8.1.0/src/contrast/api/trace_event.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/api/type_checked_property.py` & `contrast_agent-8.1.0/src/contrast/api/type_checked_property.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/api/user_input.py` & `contrast_agent-8.1.0/src/contrast/api/user_input.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/applies/__init__.py` & `contrast_agent-8.1.0/src/contrast/applies/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/applies/assess/unsafe_code_execution.py` & `contrast_agent-8.1.0/src/contrast/applies/assess/unsafe_code_execution.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/applies/sqli.py` & `contrast_agent-8.1.0/src/contrast/applies/sqli.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/asgi/middleware.py` & `contrast_agent-8.1.0/src/contrast/asgi/middleware.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/__init__.py` & `contrast_agent-8.1.0/src/contrast/assess_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/common/cast.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/common/cast.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/common/format.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/common/format.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/common/logging.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/common/logging.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/common/patches.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/common/patches.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/common/propagate.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/common/propagate.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/common/repeat.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/common/repeat.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/common/repr.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/common/repr.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/common/scope.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/common/scope.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/common/streams.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/common/streams.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/common/subscript.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/common/subscript.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/common/trace.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/common/trace.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/cs_str.pyi` & `contrast_agent-8.1.0/src/contrast/assess_extensions/cs_str.pyi`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.travis.yml` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.travis.yml`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/LICENSE` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/Makefile.in` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/README.md` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/README.md`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/appveyor.yml` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/appveyor.yml`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/config.guess` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/config.guess`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/config.sub` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/config.sub`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/configure.ac` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/configure.ac`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/COPYING` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/COPYING`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/README.md` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/README.md`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/setup.py` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/setup.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/config.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/config.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/include/funchook.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/include/funchook.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/install-sh` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/install-sh`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/Makefile.in` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/__strerror.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/__strerror.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_io.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_io.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_io.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_io.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/printf_base.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/printf_base.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/printf_base.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/printf_base.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/Makefile.in` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/suffix.list` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/suffix.list`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/test_main.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/test_main.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/x86_test.S` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/x86_test.S`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook.sln` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook.sln`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters` & `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/logging.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/logging.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/patches.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/patches.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/scope.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/scope.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/utils.h` & `contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/utils.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py3/patches.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py3/patches.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py3/str_concat.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py3/str_concat.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py310/bytearray.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py310/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py310/bytes.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py310/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py310/bytesio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py310/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py310/iobase.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py310/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py310/stringio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py310/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py310/unicode.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py310/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py311/bytearray.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py311/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py311/bytes.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py311/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py311/bytesio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py311/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py311/iobase.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py311/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py311/stringio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py311/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py311/unicode.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py311/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py312/bytearray.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py312/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py312/bytes.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py312/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py312/bytesio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py312/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py312/iobase.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py312/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py312/stringio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py312/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py312/unicode.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py312/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py35/bytearray.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py35/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py35/bytes.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py35/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py35/bytesio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py35/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py35/iobase.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py35/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py35/stringio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py35/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py35/unicode.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py35/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py36/bytearray.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py36/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py36/bytes.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py36/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py36/bytesio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py36/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py36/iobase.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py36/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py36/stringio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py36/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py36/unicode.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py36/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py37/bytearray.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py37/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py37/bytes.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py37/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py37/bytesio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py37/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py37/iobase.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py37/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py37/stringio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py37/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py37/unicode.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py37/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py38/bytearray.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py38/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py38/bytes.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py38/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py38/bytesio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py38/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py38/iobase.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py38/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py38/stringio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py38/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py38/unicode.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py38/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py39/bytearray.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py39/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py39/bytes.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py39/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py39/bytesio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py39/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py39/iobase.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py39/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py39/stringio.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py39/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/assess_extensions/py39/unicode.c` & `contrast_agent-8.1.0/src/contrast/assess_extensions/py39/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/configuration/__init__.py` & `contrast_agent-8.1.0/src/contrast/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/configuration/agent.py` & `contrast_agent-8.1.0/src/contrast/configuration/agent.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/configuration/agent_config.py` & `contrast_agent-8.1.0/src/contrast/configuration/agent_config.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/configuration/api.py` & `contrast_agent-8.1.0/src/contrast/configuration/api.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/configuration/application.py` & `contrast_agent-8.1.0/src/contrast/configuration/application.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/configuration/assess.py` & `contrast_agent-8.1.0/src/contrast/configuration/assess.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/configuration/config_builder.py` & `contrast_agent-8.1.0/src/contrast/configuration/config_builder.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/configuration/config_option.py` & `contrast_agent-8.1.0/src/contrast/configuration/config_option.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/configuration/inventory.py` & `contrast_agent-8.1.0/src/contrast/configuration/inventory.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/configuration/protect.py` & `contrast_agent-8.1.0/src/contrast/configuration/protect.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/configuration/server.py` & `contrast_agent-8.1.0/src/contrast/configuration/server.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/loader/sitecustomize.py` & `contrast_agent-8.1.0/src/contrast/loader/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/__init__.py` & `contrast_agent-8.1.0/src/contrast/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/cgi_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/cgi_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/concurrent_futures_thread_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/concurrent_futures_thread_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/cs_io.py` & `contrast_agent-8.1.0/src/contrast/patches/cs_io.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/cs_str.py` & `contrast_agent-8.1.0/src/contrast/patches/cs_str.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/databases/dbapi2.py` & `contrast_agent-8.1.0/src/contrast/patches/databases/dbapi2.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/databases/mysql_connector_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/databases/mysql_connector_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/databases/psycopg2_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/databases/psycopg2_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/databases/sqlalchemy_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/databases/sqlalchemy_patch.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     if module.unpatched_method is not None:
         return
 
     orig_method = sqlalchemy_engine_default.DefaultDialect.__init__
     module.unpatched_method = orig_method
     wrapped_method = CustomFunctionWrapper(orig_method, dialect_init_wrapper)
 
-    setattr(sqlalchemy_engine_default.DefaultDialect, "__init__", wrapped_method)
+    sqlalchemy_engine_default.DefaultDialect.__init__ = wrapped_method
 
 
 def register_patches():
     wrapt.register_post_import_hook(patch_sqlalchemy, ENGINE_DEFAULT_MODULE)
 
 
 def reverse_patches():
@@ -110,11 +110,9 @@
     Note: this doesn't reverse-patch any dbapi2 adapters that were patched as a
     result of this module's patch.
     """
     sqlalchemy_engine_default = sys.modules.get(ENGINE_DEFAULT_MODULE)
     if None in (sqlalchemy_engine_default, module.unpatched_method):
         return
 
-    setattr(
-        sqlalchemy_engine_default.DefaultDialect, "__init__", module.unpatched_method
-    )
+    sqlalchemy_engine_default.DefaultDialect.__init__ = module.unpatched_method
     module.unpatched_method = None
```

### Comparing `contrast_agent-8.0.0/src/contrast/patches/databases/sqlite3_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/databases/sqlite3_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/encodings_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/encodings_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/exec_and_eval.py` & `contrast_agent-8.1.0/src/contrast/patches/exec_and_eval.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/frameworks/bottle_patches.py` & `contrast_agent-8.1.0/src/contrast/patches/frameworks/bottle_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/frameworks/django_patches.py` & `contrast_agent-8.1.0/src/contrast/patches/frameworks/django_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/frameworks/drf_patches.py` & `contrast_agent-8.1.0/src/contrast/patches/frameworks/drf_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/frameworks/falcon_patches.py` & `contrast_agent-8.1.0/src/contrast/patches/frameworks/falcon_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/frameworks/flask_and_quart_patches.py` & `contrast_agent-8.1.0/src/contrast/patches/frameworks/flask_and_quart_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/frameworks/pyramid_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/frameworks/pyramid_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/frameworks/starlette_patches.py` & `contrast_agent-8.1.0/src/contrast/patches/frameworks/starlette_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/genshi_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/genshi_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/import_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/import_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,21 +142,16 @@
     )
 
     return True, possible_sys_module_keys, before_import_sys_modules
 
 
 @fail_quietly("Failed to analyze assess")
 def analyze_assess(method_name, result, args, kwargs):
-    if scope.in_trigger_scope() or scope.in_contrast_scope():
-        return
-
     trigger_rule = registry.get_triggers_by_rule("unsafe-code-execution")
-
     trigger_nodes = trigger_rule.find_trigger_nodes("importlib", method_name)
-
     trigger_policy.apply(trigger_rule, trigger_nodes, result, args, kwargs)
 
 
 @fail_quietly("Failed to determine loaded files")
 def post__import__analysis(
     req_context, before_import_sys_modules, possible_sys_module_keys
 ):
@@ -184,48 +179,52 @@
         for dist_hash, loaded_files in loaded_files_dict.items():
             if len(loaded_files) > 0:
                 observation = {"id": dist_hash, "names": loaded_files}
                 msg.body["observations"].append(observation)
 
 
 def build_import_patch(orig_func, _):
+    @scope.with_contrast_scope
     def import_patch(wrapped, instance, args, kwargs):
         del instance
 
         context = contrast.CS__CONTEXT_TRACKER.current()
         settings = Settings()
 
         perform_analysis = False
         possible_sys_module_keys = None
         before_import_sys_modules = None
         result = None
 
         # We only support reporting this information in the context of a request.
         # Verify we can get request context before doing any processing
         if context is not None and settings.is_analyze_libs_enabled() and args:
-            with scope.contrast_scope():
-                (
-                    perform_analysis,
-                    possible_sys_module_keys,
-                    before_import_sys_modules,
-                ) = pre__import__analysis(*args, **kwargs)
+            (
+                perform_analysis,
+                possible_sys_module_keys,
+                before_import_sys_modules,
+            ) = pre__import__analysis(*args, **kwargs)
 
+        imported_in_contrast_scope = False
         try:
-            # Don't perform import in contrast scope because there may be analysis we can
-            # do during import (i.e first time executing + caching the module)
-            result = wrapped(*args, **kwargs)
+            # Don't enter contrast scope here because there may be analysis that should
+            # happen during import (i.e first time executing + caching the module).
+            # Note that it is still possible for the wrapped func to run in scope if
+            # the caller was in scope.
+            with scope.pop_contrast_scope():
+                imported_in_contrast_scope = scope.in_contrast_scope()
+                result = wrapped(*args, **kwargs)
         finally:
-            if settings.is_assess_enabled():
+            if settings.is_assess_enabled() and not imported_in_contrast_scope:
                 analyze_assess("__import__", result, args, kwargs)
 
         if perform_analysis:
-            with scope.contrast_scope():
-                post__import__analysis(
-                    context, before_import_sys_modules, possible_sys_module_keys
-                )
+            post__import__analysis(
+                context, before_import_sys_modules, possible_sys_module_keys
+            )
 
         return result
 
     return wrap_and_watermark(orig_func, import_patch)
 
 
 def patch_import(module):
```

### Comparing `contrast_agent-8.0.0/src/contrast/patches/lxml_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/lxml_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/middleware/aiohttp.py` & `contrast_agent-8.1.0/src/contrast/patches/middleware/aiohttp.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/middleware/common.py` & `contrast_agent-8.1.0/src/contrast/patches/middleware/common.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/middleware/django.py` & `contrast_agent-8.1.0/src/contrast/patches/middleware/django.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/middleware/mod_wsgi.py` & `contrast_agent-8.1.0/src/contrast/patches/middleware/mod_wsgi.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/operator.py` & `contrast_agent-8.1.0/src/contrast/patches/operator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/pathlib_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/pathlib_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/re_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/re_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/str_new.py` & `contrast_agent-8.1.0/src/contrast/patches/str_new.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/sys_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/sys_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/threading_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/threading_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/urllib_patch.py` & `contrast_agent-8.1.0/src/contrast/patches/urllib_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/patches/utils.py` & `contrast_agent-8.1.0/src/contrast/patches/utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/deadzones.py` & `contrast_agent-8.1.0/src/contrast/policy/deadzones.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/propagators/codecs.py` & `contrast_agent-8.1.0/src/contrast/policy/propagators/codecs.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/propagators/encodings.py` & `contrast_agent-8.1.0/src/contrast/policy/propagators/encodings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/propagators/frameworks.py` & `contrast_agent-8.1.0/src/contrast/policy/propagators/frameworks.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/propagators/paths.py` & `contrast_agent-8.1.0/src/contrast/policy/propagators/paths.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/propagators/re.py` & `contrast_agent-8.1.0/src/contrast/policy/propagators/re.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/propagators/serialize.py` & `contrast_agent-8.1.0/src/contrast/policy/propagators/serialize.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/propagators/string.py` & `contrast_agent-8.1.0/src/contrast/policy/propagators/string.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/sources/asgi.py` & `contrast_agent-8.1.0/src/contrast/policy/sources/asgi.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/sources/cgi.py` & `contrast_agent-8.1.0/src/contrast/policy/sources/cgi.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/sources/django.py` & `contrast_agent-8.1.0/src/contrast/policy/sources/django.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/sources/falcon.py` & `contrast_agent-8.1.0/src/contrast/policy/sources/falcon.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/sources/flask.py` & `contrast_agent-8.1.0/src/contrast/policy/sources/flask.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/sources/quart.py` & `contrast_agent-8.1.0/src/contrast/policy/sources/quart.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/sources/webob.py` & `contrast_agent-8.1.0/src/contrast/policy/sources/webob.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/__init__.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/cmd_injection.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/cmd_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/crypto.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/crypto.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/httponly.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/httponly.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/nosql_injection.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/nosql_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/path_traversal.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/path_traversal.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/prompt_injection.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/prompt_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/redos.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/redos.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/reflected_xss.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/reflected_xss.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/secure_flag_missing.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/secure_flag_missing.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/session_rewriting.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/session_rewriting.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/session_timeout.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/session_timeout.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/sql_injection.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/sql_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/ssrf.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/ssrf.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/trust_boundary_violation.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/trust_boundary_violation.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/unsafe_code_execution.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/unsafe_code_execution.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/untrusted_deserialization.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/untrusted_deserialization.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/unvalidated_redirect.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/unvalidated_redirect.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/xpath_injection.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/xpath_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/policy/triggers/xxe.py` & `contrast_agent-8.1.0/src/contrast/policy/triggers/xxe.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/activity_masker.py` & `contrast_agent-8.1.0/src/contrast/reporting/activity_masker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
+from copy import copy
 from urllib.parse import parse_qs, urlencode, unquote
 
 from contrast.agent.settings import Settings
 from contrast.api.attack import ProtectResponse
 from contrast_vendor import structlog as logging
+from contrast_vendor.webob.multidict import MultiDict
 
 logger = logging.getLogger("contrast")
 
 MASK = "contrast-redacted-{}"
 BODY_MASK = b"contrast-redacted-body"
 SEMICOLON_URL_ENCODE_VAL = "%25"
 
@@ -51,16 +53,16 @@
     def mask_query_string(self):
         query_string = self.http_request.query_string
         if query_string:
             self.http_request._masked_query_string = self.mask_raw_query(query_string)
 
     def mask_raw_query(self, query_string):
         qs_dict = parse_qs(query_string)
-        self.mask_dictionary(qs_dict)
-        return urlencode(qs_dict, doseq=True)
+        masked_qs_dict = self.mask_dictionary(qs_dict)
+        return urlencode(masked_qs_dict, doseq=True)
 
     def mask_request_params(self):
         params = self.http_request.params
         if not params:
             return
 
         self.http_request._masked_params = self.mask_dictionary(params)
@@ -79,18 +81,21 @@
 
         self.http_request._masked_headers = self.mask_dictionary(headers)
 
     def mask_dictionary(self, d):
         if not d:
             return None
 
-        d_copy = dict(d).copy()
+        if isinstance(d, MultiDict):
+            d = d.mixed()
+
+        d_copy = {k: copy(v) for k, v in d.items()}
 
         for k, v in d_copy.items():
-            if self.find_value_index_in_rules(k.lower()) == -1:
+            if k is None or self.find_value_index_in_rules(k.lower()) == -1:
                 continue
 
             if isinstance(v, list):
                 self.mask_values(k, v, d_copy, self.ctx.attacks)
             else:
                 self.mask_hash(k, v, d_copy, self.ctx.attacks)
         return d_copy
```

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/reporting_client.py` & `contrast_agent-8.1.0/src/contrast/reporting/reporting_client.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/request_audit.py` & `contrast_agent-8.1.0/src/contrast/reporting/request_audit.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/__init__.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/_traces.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/_traces.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/agent_startup.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/agent_startup.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/application_activity.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/application_activity.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/application_inventory.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/application_inventory.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/application_update.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/application_update.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/base_ts_message.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/base_ts_message.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/effective_config.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/effective_config.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/heartbeat.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/heartbeat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/library_usage.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/library_usage.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/observed_route.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/observed_route.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/preflight.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/preflight.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/server_activity.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/server_activity.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/__init__.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/application_settings.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/application_settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/ng_application_settings.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/ng_application_settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/ng_server_settings.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/ng_server_settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/protect_rule.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/protect_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/sampling.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/sampling.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/server_settings.py` & `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/server_settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/scripts/fix_interpreter_permissions.py` & `contrast_agent-8.1.0/src/contrast/scripts/fix_interpreter_permissions.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/scripts/propagator_check.py` & `contrast_agent-8.1.0/src/contrast/scripts/propagator_check.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/scripts/runner.py` & `contrast_agent-8.1.0/src/contrast/scripts/runner.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/scripts/validate_config.py` & `contrast_agent-8.1.0/src/contrast/scripts/validate_config.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/assess/duck_utils.py` & `contrast_agent-8.1.0/src/contrast/utils/assess/duck_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/assess/formatting/base.py` & `contrast_agent-8.1.0/src/contrast/utils/assess/formatting/base.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/assess/formatting/tokenize_cformat.py` & `contrast_agent-8.1.0/src/contrast/utils/assess/formatting/tokenize_cformat.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     consts = dict(wildcard="*", empty="", dot=".", percent="%", formatter="%s%s")
     for name, val in consts.items():
         setattr(cls, name, encoder(val))
 
     def encode(self, val):
         return encoder(val)
 
-    setattr(cls, "encode", encode)
+    cls.encode = encode
 
     return cls
 
 
 StrFormatToken = _build_token_class("StrFormatToken", ensure_string)
 BytesFormatToken = _build_token_class("BytesFormatToken", ensure_binary)
```

### Comparing `contrast_agent-8.0.0/src/contrast/utils/assess/formatting/tokenize_format.py` & `contrast_agent-8.1.0/src/contrast/utils/assess/formatting/tokenize_format.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/assess/stream_utils.py` & `contrast_agent-8.1.0/src/contrast/utils/assess/stream_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/assess/tag_utils.py` & `contrast_agent-8.1.0/src/contrast/utils/assess/tag_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/assess/tracking_util.py` & `contrast_agent-8.1.0/src/contrast/utils/assess/tracking_util.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/base64_utils.py` & `contrast_agent-8.1.0/src/contrast/utils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/configuration_utils.py` & `contrast_agent-8.1.0/src/contrast/utils/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/context_tracker.py` & `contrast_agent-8.1.0/src/contrast/utils/context_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/decorators.py` & `contrast_agent-8.1.0/src/contrast/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/deprecated_middleware.py` & `contrast_agent-8.1.0/src/contrast/utils/deprecated_middleware.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/environ.py` & `contrast_agent-8.1.0/src/contrast/utils/environ.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py` & `contrast_agent-8.1.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/ignored_modules.py` & `contrast_agent-8.1.0/src/contrast/utils/ignored_modules.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/library_reader/library_reader.py` & `contrast_agent-8.1.0/src/contrast/utils/library_reader/library_reader.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/library_reader/patched_state.py` & `contrast_agent-8.1.0/src/contrast/utils/library_reader/patched_state.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/library_reader/utils.py` & `contrast_agent-8.1.0/src/contrast/utils/library_reader/utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/loggers/logger.py` & `contrast_agent-8.1.0/src/contrast/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/loggers/structlog.py` & `contrast_agent-8.1.0/src/contrast/utils/loggers/structlog.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/module_parser.py` & `contrast_agent-8.1.0/src/contrast/utils/module_parser.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/namespace.py` & `contrast_agent-8.1.0/src/contrast/utils/namespace.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/object_utils.py` & `contrast_agent-8.1.0/src/contrast/utils/object_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/patch_utils.py` & `contrast_agent-8.1.0/src/contrast/utils/patch_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/pattern_builder.py` & `contrast_agent-8.1.0/src/contrast/utils/pattern_builder.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/profiler.py` & `contrast_agent-8.1.0/src/contrast/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/safe_import.py` & `contrast_agent-8.1.0/src/contrast/utils/safe_import.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/singleton.py` & `contrast_agent-8.1.0/src/contrast/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/stack_trace_utils.py` & `contrast_agent-8.1.0/src/contrast/utils/stack_trace_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/stdlib_modules.py` & `contrast_agent-8.1.0/src/contrast/utils/stdlib_modules.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast/utils/string_utils.py` & `contrast_agent-8.1.0/src/contrast/utils/string_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,16 +73,18 @@
 def ends_with_any(value, strings):
     """
     Returns True if any of the strings are at the end of the value
     """
     return any(value.endswith(item) for item in strings)
 
 
-def equals_ignore_case(this, that):
-    return this.lower() == that.lower()
+def equals_ignore_case(this: str, that: str) -> bool:
+    # PERF: this function is hot. Pre-checking str lengths is an optimization that
+    # often prevents unnecessary (and slower) calls to lower().
+    return len(this) == len(that) and this.lower() == that.lower()
 
 
 def ensure_string(value, encoding=None, errors="ignore") -> str:
     """
     Convert `value` of any type to a string, even if empty string.
 
     On failure given a custom encoding or using DEFAULT_ENCODING we
```

### Comparing `contrast_agent-8.0.0/src/contrast/wsgi/middleware.py` & `contrast_agent-8.1.0/src/contrast/wsgi/middleware.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_agent.egg-info/SOURCES.txt` & `contrast_agent-8.1.0/src/contrast_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_rewriter/__init__.py` & `contrast_agent-8.1.0/src/contrast_rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/__init__.py` & `contrast_agent-8.1.0/src/contrast_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/LICENSE` & `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/__init__.py` & `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_adapters.py` & `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_collections.py` & `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_compat.py` & `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_functools.py` & `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_itertools.py` & `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_meta.py` & `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_text.py` & `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/compat/py39.py` & `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/compat/py39.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/isort/LICENSE` & `contrast_agent-8.1.0/src/contrast_vendor/isort/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py27.py` & `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py27.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py310.py` & `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py310.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py311.py` & `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py311.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py312.py` & `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py312.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py36.py` & `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py36.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py37.py` & `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py37.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py38.py` & `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py38.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py39.py` & `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py39.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE` & `contrast_agent-8.1.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ported_cpython_code/import_functionality.py` & `contrast_agent-8.1.0/src/contrast_vendor/ported_cpython_code/import_functionality.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/LICENSE` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/__init__.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/comments.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/comments.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/compat.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/compat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/composer.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/constructor.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/cyaml.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/dumper.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/emitter.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/error.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/error.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/events.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/events.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/loader.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/main.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/main.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/nodes.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/parser.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/reader.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/representer.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/resolver.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarbool.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarbool.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarint.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarint.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarstring.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarstring.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scanner.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/serializer.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/tag.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/tag.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/timestamp.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/timestamp.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/tokens.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/util.py` & `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/util.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/LICENSE-APACHE` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/LICENSE-MIT` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/__init__.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/_base.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/_base.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/_config.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/_config.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/_frames.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/_frames.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/_generic.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/_generic.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/_greenlets.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/_greenlets.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/_log_levels.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/_log_levels.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/_native.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/_native.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/_output.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/_output.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/_utils.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/contextvars.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/contextvars.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/dev.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/dev.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/processors.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/stdlib.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/stdlib.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/testing.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/testing.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/threadlocal.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/threadlocal.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/tracebacks.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/tracebacks.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/twisted.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/twisted.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/types.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/types.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/structlog/typing.py` & `contrast_agent-8.1.0/src/contrast_vendor/structlog/typing.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/__init__.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/acceptparse.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/acceptparse.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/byterange.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/byterange.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/cachecontrol.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/cachecontrol.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/client.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/client.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/compat.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/compat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/cookies.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/cookies.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/datetime_utils.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/dec.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/dec.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/descriptors.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/descriptors.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/etag.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/etag.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/exc.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/exc.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/headers.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/headers.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/license.txt` & `contrast_agent-8.1.0/src/contrast_vendor/webob/license.txt`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/multidict.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/multidict.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/request.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/request.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/response.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/response.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/static.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/static.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/webob/util.py` & `contrast_agent-8.1.0/src/contrast_vendor/webob/util.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/wrapt/LICENSE` & `contrast_agent-8.1.0/src/contrast_vendor/wrapt/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/wrapt/__init__.py` & `contrast_agent-8.1.0/src/contrast_vendor/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/wrapt/arguments.py` & `contrast_agent-8.1.0/src/contrast_vendor/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/wrapt/decorators.py` & `contrast_agent-8.1.0/src/contrast_vendor/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/wrapt/importer.py` & `contrast_agent-8.1.0/src/contrast_vendor/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/wrapt/patches.py` & `contrast_agent-8.1.0/src/contrast_vendor/wrapt/patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/wrapt/weakrefs.py` & `contrast_agent-8.1.0/src/contrast_vendor/wrapt/weakrefs.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/wrapt/wrappers.py` & `contrast_agent-8.1.0/src/contrast_vendor/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/zipp/LICENSE` & `contrast_agent-8.1.0/src/contrast_vendor/zipp/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/zipp/__init__.py` & `contrast_agent-8.1.0/src/contrast_vendor/zipp/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.0.0/src/contrast_vendor/zipp/glob.py` & `contrast_agent-8.1.0/src/contrast_vendor/zipp/glob.py`

 * *Files identical despite different names*

