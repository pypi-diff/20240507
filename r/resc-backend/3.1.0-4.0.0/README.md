# Comparing `tmp/resc_backend-3.1.0.tar.gz` & `tmp/resc_backend-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_backend-3.1.0.tar", last modified: Tue May  7 09:23:53 2024, max compression
+gzip compressed data, was "resc_backend-4.0.0.tar", last modified: Tue Apr 30 15:21:35 2024, max compression
```

## Comparing `resc_backend-3.1.0.tar` & `resc_backend-4.0.0.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.809822 resc_backend-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 09:23:49.000000 resc_backend-3.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-07 09:23:53.809822 resc_backend-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-07 09:23:49.000000 resc_backend-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-07 09:23:49.000000 resc_backend-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-07 09:23:53.809822 resc_backend-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 09:23:49.000000 resc_backend-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.789822 resc_backend-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.793822 resc_backend-3.1.0/src/resc_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.793822 resc_backend-3.1.0/src/resc_backend/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/bin/rabbitmq_bootup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.793822 resc_backend-3.1.0/src/resc_backend/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/engine_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.797822 resc_backend-3.1.0/src/resc_backend/db/model/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/model/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/model/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/model/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/model/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/model/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/model/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/db/model/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.797822 resc_backend-3.1.0/src/resc_backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/helpers/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/helpers/environment_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.797822 resc_backend-3.1.0/src/resc_backend/helpers/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/helpers/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/helpers/rabbitmq/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.797822 resc_backend-3.1.0/src/resc_backend/resc_web_service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.801822 resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    34210 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    16397 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.801822 resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
--rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20677 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.801822 resc_backend-3.1.0/src/resc_backend/resc_web_service/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/helpers/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/helpers/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.805822 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/date_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/date_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/finding_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/finding_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/pagination_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/repository_enriched.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/rule_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/status_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/time_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/vcs_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.809822 resc_backend-3.1.0/src/resc_backend/resc_web_service_interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service_interface/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service_interface/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service_interface/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service_interface/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-07 09:23:49.000000 resc_backend-3.1.0/src/resc_backend/resc_web_service_interface/vcs_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:53.809822 resc_backend-3.1.0/src/resc_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-07 09:23:53.000000 resc_backend-3.1.0/src/resc_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-07 09:23:53.000000 resc_backend-3.1.0/src/resc_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:23:53.000000 resc_backend-3.1.0/src/resc_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-07 09:23:53.000000 resc_backend-3.1.0/src/resc_backend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:23:53.000000 resc_backend-3.1.0/src/resc_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-07 09:23:53.000000 resc_backend-3.1.0/src/resc_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 09:23:53.000000 resc_backend-3.1.0/src/resc_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.881999 resc_backend-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 15:21:29.000000 resc_backend-4.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-04-30 15:21:35.881999 resc_backend-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-30 15:21:29.000000 resc_backend-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-30 15:21:29.000000 resc_backend-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 15:21:35.885999 resc_backend-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 15:21:29.000000 resc_backend-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.865998 resc_backend-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.865998 resc_backend-4.0.0/src/resc_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.869998 resc_backend-4.0.0/src/resc_backend/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/bin/rabbitmq_bootup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.869998 resc_backend-4.0.0/src/resc_backend/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/engine_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.869998 resc_backend-4.0.0/src/resc_backend/db/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.869998 resc_backend-4.0.0/src/resc_backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/environment_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.873998 resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.873998 resc_backend-4.0.0/src/resc_backend/resc_web_service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.873998 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34253 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16397 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.877998 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20677 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.877998 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.881999 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/date_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/date_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/pagination_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/repository_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/status_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/time_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/vcs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.881999 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/vcs_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.881999 resc_backend-4.0.0/src/resc_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/top_level.txt
```

### Comparing `resc_backend-3.1.0/LICENSE.md` & `resc_backend-4.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/PKG-INFO` & `resc_backend-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: resc_backend
-Version: 3.1.0
+Version: 4.0.0
 Summary: Repository Scanner - Backend
-Home-page: https://github.com/abnamro/resc-backend
+Home-page: https://github.com/ABNAMRO/repository-scanner
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: celery==5.3.1
```

### Comparing `resc_backend-3.1.0/README.md` & `resc_backend-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/bin/rabbitmq_bootup.py` & `resc_backend-4.0.0/src/resc_backend/bin/rabbitmq_bootup.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/common.py` & `resc_backend-4.0.0/src/resc_backend/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/constants.py` & `resc_backend-4.0.0/src/resc_backend/constants.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/db/connection.py` & `resc_backend-4.0.0/src/resc_backend/db/connection.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/db/engine_azure.py` & `resc_backend-4.0.0/src/resc_backend/db/engine_azure.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/db/model/__init__.py` & `resc_backend-4.0.0/src/resc_backend/db/model/__init__.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/db/model/audit.py` & `resc_backend-4.0.0/src/resc_backend/db/model/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/db/model/finding.py` & `resc_backend-4.0.0/src/resc_backend/db/model/finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/db/model/repository.py` & `resc_backend-4.0.0/src/resc_backend/db/model/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/db/model/rule.py` & `resc_backend-4.0.0/src/resc_backend/db/model/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/db/model/rule_allow_list.py` & `resc_backend-4.0.0/src/resc_backend/db/model/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/db/model/rule_pack.py` & `resc_backend-4.0.0/src/resc_backend/db/model/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/db/model/scan.py` & `resc_backend-4.0.0/src/resc_backend/db/model/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/db/model/vcs_instance.py` & `resc_backend-4.0.0/src/resc_backend/db/model/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/helpers/dict_remapper.py` & `resc_backend-4.0.0/src/resc_backend/helpers/dict_remapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/helpers/environment_wrapper.py` & `resc_backend-4.0.0/src/resc_backend/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/helpers/rabbitmq/configuration.py` & `resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py` & `resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/api.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/api.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/cache_manager.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/cache_manager.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/configuration.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/audit.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/detailed_finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/detailed_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/finding.py`

 * *Files 0% similar despite different names*

```diff
@@ -632,16 +632,16 @@
         )
     elif date_type == DateFilter.DAY:
         query: Query = db_connection.query(
             extract("year", DBscan.timestamp),
             extract("month", DBscan.timestamp),
             extract("day", DBscan.timestamp),
         )
-
-    query = query.join(DBscanFinding, DBscan.id_ == DBscanFinding.scan_id)
+    # To check later if it fixes the bug.
+    # query = query.join(DBscanFinding, DBscan.id_ == DBscanFinding.scan_id)
 
     if start_date_time:
         query = query.where(DBscan.timestamp >= start_date_time)
     if end_date_time:
         query = query.where(DBscan.timestamp <= end_date_time)
 
     query = query.distinct()
```

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/repository.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/rule.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/rule_pack.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/rule_tag.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule_tag.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/scan.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/scan_finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/scan_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/crud/vcs_instance.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/dependencies.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/dependencies.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/common.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/findings.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/health.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/metrics.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/metrics.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/repositories.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/repositories.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/rules.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/rules.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/scans.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/scans.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/filters.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/filters.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/helpers/exception_handler.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/exception_handler.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/helpers/rule.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/audit.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/detailed_finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/detailed_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/finding_count_model.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding_count_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/pagination_model.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/pagination_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/repository.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/repository_enriched.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/repository_enriched.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/rule.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/rule_count_model.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_count_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/rule_pack.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/scan.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service/schema/vcs_instance.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service_interface/findings.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service_interface/repositories.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/repositories.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service_interface/rule_packs.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend/resc_web_service_interface/vcs_instances.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.0/src/resc_backend.egg-info/PKG-INFO` & `resc_backend-4.0.0/src/resc_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: resc_backend
-Version: 3.1.0
+Version: 4.0.0
 Summary: Repository Scanner - Backend
-Home-page: https://github.com/abnamro/resc-backend
+Home-page: https://github.com/ABNAMRO/repository-scanner
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: celery==5.3.1
```

### Comparing `resc_backend-3.1.0/src/resc_backend.egg-info/SOURCES.txt` & `resc_backend-4.0.0/src/resc_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

