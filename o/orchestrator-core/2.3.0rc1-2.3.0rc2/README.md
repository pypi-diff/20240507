# Comparing `tmp/orchestrator_core-2.3.0rc1.tar.gz` & `tmp/orchestrator_core-2.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrator_core-2.3.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orchestrator_core-2.3.0rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orchestrator_core-2.3.0rc1.tar` & `orchestrator_core-2.3.0rc2.tar`

### file list

```diff
@@ -1,560 +1,560 @@
--rw-r--r--   0        0        0      342 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.bumpversion.cfg
--rw-r--r--   0        0        0       33 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.coveragerc
--rw-r--r--   0        0        0     1564 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0     1149 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0      502 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/dependabot.yml
--rw-r--r--   0        0        0     2620 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/README.md
--rw-r--r--   0        0        0     1851 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/build-push-container.yml
--rw-r--r--   0        0        0      291 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2341 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      346 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      583 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/issues.yml
--rw-r--r--   0        0        0      550 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1221 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     2426 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1985 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1809 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.gitignore
--rw-r--r--   0        0        0     2599 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2024-05-06 11:29:57.990776 orchestrator_core-2.3.0rc1/.stignore
--rw-r--r--   0        0        0    30927 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0      333 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/Dockerfile
--rw-r--r--   0        0        0    11409 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/LICENSE
--rw-r--r--   0        0        0      150 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/NOTICE
--rw-r--r--   0        0        0     5595 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/README.md
--rw-r--r--   0        0        0      196 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/codecov.yml
--rw-r--r--   0        0        0    10746 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/application/domainmodels.md
--rw-r--r--   0        0        0     9277 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/application/forms-frontend.md
--rw-r--r--   0        0        0     5514 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/application/tasks.md
--rw-r--r--   0        0        0    11462 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/application/workflow.md
--rw-r--r--   0        0        0        0 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/orchestration/philosophy.md
--rw-r--r--   0        0        0      668 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/context.md
--rw-r--r--   0        0        0     4226 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/imports.md
--rw-r--r--   0        0        0      802 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/introduction.md
--rw-r--r--   0        0        0     1671 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/ip_static.md
--rw-r--r--   0        0        0    84576 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/ip_static.png
--rw-r--r--   0        0        0     1311 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_point_to_point.md
--rw-r--r--   0        0        0    55937 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_point_to_point.png
--rw-r--r--   0        0        0      854 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_vpn.md
--rw-r--r--   0        0        0    29551 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_vpn.png
--rw-r--r--   0        0        0     1398 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/modelling.md
--rw-r--r--   0        0        0     1138 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/node.md
--rw-r--r--   0        0        0    23110 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/node.png
--rw-r--r--   0        0        0     1147 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/port.md
--rw-r--r--   0        0        0    37248 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/port.png
--rw-r--r--   0        0        0     1694 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/product_block_graph.md
--rw-r--r--   0        0        0    78824 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/product_block_graph.png
--rw-r--r--   0        0        0      989 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/standards.md
--rw-r--r--   0        0        0     1114 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/terminology.md
--rw-r--r--   0        0        0     2080 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/architecture/tldr.md
--rw-r--r--   0        0        0      443 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/contributing/documentation.md
--rw-r--r--   0        0        0     1771 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/contributing/guidelines.md
--rw-r--r--   0        0        0     9997 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/contributing/testing.md
--rw-r--r--   0        0        0      452 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/css/custom.css
--rw-r--r--   0        0        0      656 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/css/style.css
--rw-r--r--   0        0        0     2165 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/css/termynal.css
--rw-r--r--   0        0        0     2135 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/getting-started/base.md
--rw-r--r--   0        0        0      928 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/getting-started/development.md
--rw-r--r--   0        0        0     3438 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/getting-started/prepare-source-folder.md
--rw-r--r--   0        0        0    17905 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/img/WFO-Emblem-White.png
--rw-r--r--   0        0        0      842 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/img/favicon.ico
--rw-r--r--   0        0        0     4005 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/index.md
--rw-r--r--   0        0        0     3897 2024-05-06 11:29:57.994776 orchestrator_core-2.3.0rc1/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/js/termynal.js
--rw-r--r--   0        0        0    11084 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/migration-guide/2.0.md
--rw-r--r--   0        0        0      600 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/api.md
--rw-r--r--   0        0        0     1026 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/app/app.md
--rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/app/runtimes.md
--rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/auth.md
--rw-r--r--   0        0        0    29652 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/cli.md
--rw-r--r--   0        0        0     2241 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/database.md
--rw-r--r--   0        0        0      359 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/generator.md
--rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/instantiating.md
--rw-r--r--   0        0        0     3867 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/model_attributes.md
--rw-r--r--   0        0        0      543 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/overview.md
--rw-r--r--   0        0        0     3863 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/product_blocks.md
--rw-r--r--   0        0        0     4030 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/product_types.md
--rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/properties.md
--rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/pydantic_hooks.md
--rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/type_casting.md
--rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/union_types.md
--rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/validation.md
--rw-r--r--   0        0        0    15366 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/forms.md
--rw-r--r--   0        0        0    27254 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/graphql.md
--rw-r--r--   0        0        0     1565 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/python.md
--rw-r--r--   0        0        0     5585 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/scaling.md
--rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/serialization.md
--rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/tasks.md
--rw-r--r--   0        0        0        0 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/tests.md
--rw-r--r--   0        0        0      499 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/tldr.md
--rw-r--r--   0        0        0     2500 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/websockets.md
--rw-r--r--   0        0        0     5505 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/workflows/callbacks.md
--rw-r--r--   0        0        0       73 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/workflows/workflow-lifecycles.md
--rw-r--r--   0        0        0     1472 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/reference-docs/workflows/workflow-steps.md
--rw-r--r--   0        0        0     9063 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/circuit-workflow.md
--rw-r--r--   0        0        0      254 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/database-migration.md
--rw-r--r--   0        0        0     3719 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/docker-installation.md
--rw-r--r--   0        0        0     2563 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/domain-models.md
--rw-r--r--   0        0        0     6048 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/node-workflow.md
--rw-r--r--   0        0        0     3087 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/overview.md
--rw-r--r--   0        0        0     1750 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/scenario.md
--rw-r--r--   0        0        0     4369 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/advanced/workflow-introduction.md
--rw-r--r--   0        0        0     5602 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/create-user-group.md
--rw-r--r--   0        0        0     4623 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/create-user.md
--rw-r--r--   0        0        0     7447 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/database-migration.md
--rw-r--r--   0        0        0     3697 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/debian.md
--rw-r--r--   0        0        0     3051 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/docker.md
--rw-r--r--   0        0        0     6157 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/domain-models.md
--rw-r--r--   0        0        0     1953 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/explore.md
--rw-r--r--   0        0        0     3991 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/input-forms.md
--rw-r--r--   0        0        0     3596 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/macos.md
--rw-r--r--   0        0        0     3411 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/modify-user-group.md
--rw-r--r--   0        0        0     2141 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/modify-user.md
--rw-r--r--   0        0        0     2878 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/overview.md
--rw-r--r--   0        0        0     4547 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/register-workflows.md
--rw-r--r--   0        0        0      785 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/scenario.md
--rw-r--r--   0        0        0     1013 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/start-applications.md
--rw-r--r--   0        0        0     2988 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/terminate-user-group.md
--rw-r--r--   0        0        0     1332 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/terminate-user.md
--rw-r--r--   0        0        0     3632 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/beginner/workflow-introduction.md
--rw-r--r--   0        0        0    46296 2024-05-06 11:29:57.998776 orchestrator_core-2.3.0rc1/docs/workshops/images/metadata_products.png
--rw-r--r--   0        0        0   983304 2024-05-06 11:29:58.002776 orchestrator_core-2.3.0rc1/docs/workshops/images/netbox_devices_active.png
--rw-r--r--   0        0        0      312 2024-05-06 11:29:58.002776 orchestrator_core-2.3.0rc1/includes/abbreviations.md
--rw-r--r--   0        0        0     8030 2024-05-06 11:29:58.002776 orchestrator_core-2.3.0rc1/mkdocs.yml
--rw-r--r--   0        0        0     1262 2024-05-06 11:29:58.002776 orchestrator_core-2.3.0rc1/mutmut_config.py
--rw-r--r--   0        0        0       70 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/nitpick-style.toml
--rw-r--r--   0        0        0     1098 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/__init__.py
--rw-r--r--   0        0        0      571 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/__init__.py
--rw-r--r--   0        0        0      571 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/__init__.py
--rw-r--r--   0        0        0     2415 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/api.py
--rw-r--r--   0        0        0      571 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     1284 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/health.py
--rw-r--r--   0        0        0    12428 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/processes.py
--rw-r--r--   0        0        0     2143 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/products.py
--rw-r--r--   0        0        0     6106 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/settings.py
--rw-r--r--   0        0        0     3081 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
--rw-r--r--   0        0        0     8861 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/subscriptions.py
--rw-r--r--   0        0        0      963 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/translations.py
--rw-r--r--   0        0        0     1827 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/user.py
--rw-r--r--   0        0        0     1722 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/ws.py
--rw-r--r--   0        0        0     1502 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/error_handling.py
--rw-r--r--   0        0        0     6933 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/helpers.py
--rw-r--r--   0        0        0     5996 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/api/models.py
--rw-r--r--   0        0        0     8886 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/app.py
--rw-r--r--   0        0        0      571 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0    16226 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/database.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/__init__.py
--rw-r--r--   0        0        0     6775 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
--rw-r--r--   0        0        0     2172 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/helpers.py
--rw-r--r--   0        0        0    10474 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
--rw-r--r--   0        0        0     9379 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py
--rw-r--r--   0        0        0    23981 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
--rw-r--r--   0        0        0     1399 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/types.py
--rw-r--r--   0        0        0     7377 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generate.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/__init__.py
--rw-r--r--   0        0        0      173 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/README
--rw-r--r--   0        0        0      307 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_create_imports.j2
--rw-r--r--   0        0        0      115 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_create_input_fields.j2
--rw-r--r--   0        0        0       82 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_create_steps.j2
--rw-r--r--   0        0        0      307 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_modify_imports.j2
--rw-r--r--   0        0        0      115 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_modify_input_fields.j2
--rw-r--r--   0        0        0       82 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_modify_steps.j2
--rw-r--r--   0        0        0      234 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_terminate_imports.j2
--rw-r--r--   0        0        0      131 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_terminate_input_fields.j2
--rw-r--r--   0        0        0       82 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/custom_templates/additional_terminate_steps.j2
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/__init__.py
--rw-r--r--   0        0        0     2007 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/enums.py
--rw-r--r--   0        0        0     5452 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/helpers.py
--rw-r--r--   0        0        0     6341 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/migration.py
--rw-r--r--   0        0        0     2073 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/product.py
--rw-r--r--   0        0        0     5285 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/product_block.py
--rw-r--r--   0        0        0     1379 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/settings.py
--rw-r--r--   0        0        0     1878 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/translations.py
--rw-r--r--   0        0        0     4541 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/unittest.py
--rw-r--r--   0        0        0     1815 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/validations.py
--rw-r--r--   0        0        0     8026 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/workflow.py
--rw-r--r--   0        0        0      759 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/circuit.yaml
--rw-r--r--   0        0        0      538 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/node.yaml
--rw-r--r--   0        0        0      532 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/user.yaml
--rw-r--r--   0        0        0      361 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/user_group.yaml
--rw-r--r--   0        0        0      431 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/additional_create_imports.j2
--rw-r--r--   0        0        0       25 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/additional_create_steps.j2
--rw-r--r--   0        0        0      394 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/additional_modify_imports.j2
--rw-r--r--   0        0        0       25 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/additional_modify_steps.j2
--rw-r--r--   0        0        0       25 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/additional_terminate_steps.j2
--rw-r--r--   0        0        0      282 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/constrained_int_definitions.j2
--rw-r--r--   0        0        0      361 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/create_data_head.j2
--rw-r--r--   0        0        0     4806 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/create_product.j2
--rw-r--r--   0        0        0      298 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/enums.j2
--rw-r--r--   0        0        0      523 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/lazy_workflow_instance.j2
--rw-r--r--   0        0        0      277 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/list_definitions.j2
--rw-r--r--   0        0        0      904 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/macros.j2
--rw-r--r--   0        0        0     4719 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/modify_product.j2
--rw-r--r--   0        0        0     2901 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/new_product_migration.j2
--rw-r--r--   0        0        0     1365 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/product.j2
--rw-r--r--   0        0        0     2454 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/product_block.j2
--rw-r--r--   0        0        0      545 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/shared_forms.j2
--rw-r--r--   0        0        0     1274 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/shared_workflows.j2
--rw-r--r--   0        0        0      291 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/subscription_model_registry.j2
--rw-r--r--   0        0        0     1883 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/terminate_product.j2
--rw-r--r--   0        0        0     1802 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_create_workflow.j2
--rw-r--r--   0        0        0     1677 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_modify_workflow.j2
--rw-r--r--   0        0        0     1860 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_product_type.j2
--rw-r--r--   0        0        0     1518 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_terminate_workflow.j2
--rw-r--r--   0        0        0      985 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_validate_workflow.j2
--rw-r--r--   0        0        0     2315 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/validate_product.j2
--rw-r--r--   0        0        0      571 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1139 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/helpers/input_helpers.py
--rw-r--r--   0        0        0      857 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/helpers/print_helpers.py
--rw-r--r--   0        0        0      983 2024-05-06 11:29:58.006776 orchestrator_core-2.3.0rc1/orchestrator/cli/main.py
--rwxr-xr-x   0        0        0    20371 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/cli/migrate_domain_models.py
--rwxr-xr-x   0        0        0     8979 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/cli/migrate_workflows.py
--rw-r--r--   0        0        0     4110 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/cli/migration_helpers.py
--rw-r--r--   0        0        0     1896 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/cli/scheduler.py
--rw-r--r--   0        0        0      571 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/config/__init__.py
--rw-r--r--   0        0        0      770 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/config/assignee.py
--rw-r--r--   0        0        0     2970 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/__init__.py
--rw-r--r--   0        0        0    10269 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/database.py
--rw-r--r--   0        0        0      371 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/__init__.py
--rw-r--r--   0        0        0     5020 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/filters.py
--rw-r--r--   0        0        0     4144 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/process.py
--rw-r--r--   0        0        0      899 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/product.py
--rw-r--r--   0        0        0     1089 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/product_block.py
--rw-r--r--   0        0        0      889 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/resource_type.py
--rw-r--r--   0        0        0      562 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/search_filters/__init__.py
--rw-r--r--   0        0        0     5591 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/search_filters/inferred_filter.py
--rw-r--r--   0        0        0     1466 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/subscription.py
--rw-r--r--   0        0        0     1276 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/filters/workflow.py
--rw-r--r--   0        0        0      831 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/helpers.py
--rw-r--r--   0        0        0    24900 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/models.py
--rw-r--r--   0        0        0      162 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/range/__init__.py
--rw-r--r--   0        0        0     2175 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/range/range.py
--rw-r--r--   0        0        0      353 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/__init__.py
--rw-r--r--   0        0        0     1987 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/process.py
--rw-r--r--   0        0        0      570 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/product.py
--rw-r--r--   0        0        0      617 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/product_block.py
--rw-r--r--   0        0        0      617 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/resource_type.py
--rw-r--r--   0        0        0     4455 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/sorting.py
--rw-r--r--   0        0        0     1441 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/subscription.py
--rw-r--r--   0        0        0      576 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/db/sorting/workflow.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/devtools/__init__.py
--rw-r--r--   0        0        0    18847 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/devtools/populator.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/devtools/scripts/__init__.py
--rw-r--r--   0        0        0     8359 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/devtools/scripts/migrate_20.py
--rw-r--r--   0        0        0     2494 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/distlock/__init__.py
--rw-r--r--   0        0        0     2508 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/distlock/distlock_manager.py
--rw-r--r--   0        0        0      571 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/distlock/managers/__init__.py
--rw-r--r--   0        0        0     3114 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/distlock/managers/memory_distlock_manager.py
--rw-r--r--   0        0        0     3271 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/distlock/managers/redis_distlock_manager.py
--rw-r--r--   0        0        0      894 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/domain/__init__.py
--rw-r--r--   0        0        0    59707 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/domain/base.py
--rw-r--r--   0        0        0     2732 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/domain/customer_description.py
--rw-r--r--   0        0        0      989 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/domain/helpers.py
--rw-r--r--   0        0        0     2882 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/domain/lifecycle.py
--rw-r--r--   0        0        0     1268 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/exception_handlers.py
--rw-r--r--   0        0        0     1168 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/__init__.py
--rw-r--r--   0        0        0     1906 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/validators/__init__.py
--rw-r--r--   0        0        0     1505 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/validators/customer_contact_list.py
--rw-r--r--   0        0        0      708 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/validators/customer_id.py
--rw-r--r--   0        0        0      779 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/validators/display_subscription.py
--rw-r--r--   0        0        0      571 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/validators/network_type_validators.py
--rw-r--r--   0        0        0     2114 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/forms/validators/product_id.py
--rw-r--r--   0        0        0     1482 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/__init__.py
--rw-r--r--   0        0        0     6413 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/autoregistration.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/__init__.py
--rw-r--r--   0        0        0     4304 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py
--rw-r--r--   0        0        0     1746 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/error_collector_extension.py
--rw-r--r--   0        0        0     5826 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/error_handler_extension.py
--rw-r--r--   0        0        0     3100 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/mutations/customer_description.py
--rw-r--r--   0        0        0     1553 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/mutations/start_process.py
--rw-r--r--   0        0        0     2413 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/pagination.py
--rw-r--r--   0        0        0      851 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/__init__.py
--rw-r--r--   0        0        0      934 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/customer.py
--rw-r--r--   0        0        0      636 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/helpers.py
--rw-r--r--   0        0        0     4491 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/process.py
--rw-r--r--   0        0        0     2562 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/product.py
--rw-r--r--   0        0        0     2748 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/product_block.py
--rw-r--r--   0        0        0     2741 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/resource_type.py
--rw-r--r--   0        0        0     3700 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/settings.py
--rw-r--r--   0        0        0     5888 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/subscription.py
--rw-r--r--   0        0        0     2681 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/workflow.py
--rw-r--r--   0        0        0     7736 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schema.py
--rw-r--r--   0        0        0      798 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/__init__.py
--rw-r--r--   0        0        0      147 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/customer.py
--rw-r--r--   0        0        0      213 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/customer_description.py
--rw-r--r--   0        0        0      203 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/errors.py
--rw-r--r--   0        0        0      513 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/fixed_input.py
--rw-r--r--   0        0        0     3482 2024-05-06 11:29:58.010776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/process.py
--rw-r--r--   0        0        0     2430 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/product.py
--rw-r--r--   0        0        0     2414 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/product_block.py
--rw-r--r--   0        0        0      755 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/resource_type.py
--rw-r--r--   0        0        0      999 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/settings.py
--rw-r--r--   0        0        0     7838 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/subscription.py
--rw-r--r--   0        0        0     1140 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/workflow.py
--rw-r--r--   0        0        0     4905 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/types.py
--rw-r--r--   0        0        0      524 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/__init__.py
--rw-r--r--   0        0        0     1191 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/create_resolver_error_handler.py
--rw-r--r--   0        0        0     1002 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/get_selected_fields.py
--rw-r--r--   0        0        0     4374 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/get_subscription_product_blocks.py
--rw-r--r--   0        0        0     2156 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/is_query_detailed.py
--rw-r--r--   0        0        0     1370 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/override_class.py
--rw-r--r--   0        0        0      902 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/to_graphql_result_page.py
--rw-r--r--   0        0        0       39 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/README
--rw-r--r--   0        0        0      873 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/alembic.ini
--rwxr-xr-x   0        0        0     3382 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/env.py
--rw-r--r--   0        0        0    40911 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/helpers.py
--rw-r--r--   0        0        0      510 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/script.py.mako
--rw-r--r--   0        0        0      905 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/templates/alembic.ini.j2
--rwxr-xr-x   0        0        0     2821 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/templates/env.py.j2
--rw-r--r--   0        0        0       98 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/templates/helpers.py.j2
--rw-r--r--   0        0        0     2698 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
--rw-r--r--   0        0        0     1265 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
--rw-r--r--   0        0        0    39307 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
--rw-r--r--   0        0        0      950 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
--rw-r--r--   0        0        0     1214 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
--rw-r--r--   0        0        0     1603 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
--rw-r--r--   0        0        0     5106 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
--rw-r--r--   0        0        0     7964 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
--rw-r--r--   0        0        0     1014 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
--rw-r--r--   0        0        0      591 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py
--rw-r--r--   0        0        0      755 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql
--rw-r--r--   0        0        0      967 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py
--rw-r--r--   0        0        0     4491 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql
--rw-r--r--   0        0        0     1036 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py
--rw-r--r--   0        0        0     5383 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql
--rw-r--r--   0        0        0     2246 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/py.typed
--rw-r--r--   0        0        0     1066 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schedules/__init__.py
--rw-r--r--   0        0        0      832 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schedules/resume_workflows.py
--rw-r--r--   0        0        0     1526 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schedules/scheduling.py
--rw-r--r--   0        0        0      821 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schedules/task_vacuum.py
--rw-r--r--   0        0        0     1234 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schedules/validate_products.py
--rw-r--r--   0        0        0     2195 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schedules/validate_subscriptions.py
--rw-r--r--   0        0        0     2326 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/__init__.py
--rw-r--r--   0        0        0      930 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/base.py
--rw-r--r--   0        0        0     1286 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/engine_settings.py
--rw-r--r--   0        0        0     1214 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/fixed_input.py
--rw-r--r--   0        0        0      802 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/problem_detail.py
--rw-r--r--   0        0        0     2354 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/process.py
--rw-r--r--   0        0        0     1484 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/product.py
--rw-r--r--   0        0        0     1428 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/product_block.py
--rw-r--r--   0        0        0      973 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/resource_type.py
--rw-r--r--   0        0        0     3366 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/subscription.py
--rw-r--r--   0        0        0     1030 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/subscription_descriptions.py
--rw-r--r--   0        0        0     1890 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/schemas/workflow.py
--rw-r--r--   0        0        0     1744 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/security.py
--rw-r--r--   0        0        0      571 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/__init__.py
--rw-r--r--   0        0        0     3635 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/celery.py
--rw-r--r--   0        0        0      876 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/fixed_inputs.py
--rw-r--r--   0        0        0     3710 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/process_broadcast_thread.py
--rw-r--r--   0        0        0    26253 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/processes.py
--rw-r--r--   0        0        0     1933 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/products.py
--rw-r--r--   0        0        0      884 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/resource_types.py
--rw-r--r--   0        0        0     2723 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/settings.py
--rw-r--r--   0        0        0    25733 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/subscriptions.py
--rw-r--r--   0        0        0     5867 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/tasks.py
--rw-r--r--   0        0        0     1713 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/translations.py
--rw-r--r--   0        0        0     1638 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/services/workflows.py
--rw-r--r--   0        0        0     3634 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/settings.py
--rw-r--r--   0        0        0      766 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/targets.py
--rw-r--r--   0        0        0    16236 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/types.py
--rw-r--r--   0        0        0      571 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/utils/__init__.py
--rw-r--r--   0        0        0     5584 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/utils/crypt.py
--rw-r--r--   0        0        0     1477 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/utils/datetime.py
--rw-r--r--   0        0        0      875 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/utils/deprecation_logger.py
--rw-r--r--   0        0        0     6172 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/utils/docs.py
--rw-r--r--   0        0        0     4658 2024-05-06 11:29:58.014776 orchestrator_core-2.3.0rc1/orchestrator/utils/enrich_process.py
--rw-r--r--   0        0        0     4250 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/errors.py
--rw-r--r--   0        0        0     2665 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/fixed_inputs.py
--rw-r--r--   0        0        0     8063 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/functional.py
--rw-r--r--   0        0        0     1322 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/get_updated_properties.py
--rw-r--r--   0        0        0     3212 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/helpers.py
--rw-r--r--   0        0        0     8341 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/json.py
--rw-r--r--   0        0        0     6378 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/redis.py
--rw-r--r--   0        0        0    17039 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/search_query.py
--rw-r--r--   0        0        0    13011 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/state.py
--rw-r--r--   0        0        0     1077 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/utils/strings.py
--rw-r--r--   0        0        0     1366 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/version.py
--rw-r--r--   0        0        0     4828 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/websocket/__init__.py
--rw-r--r--   0        0        0     4596 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py
--rw-r--r--   0        0        0     3324 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/websocket/managers/memory_websocket_manager.py
--rw-r--r--   0        0        0     2924 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/websocket/websocket_manager.py
--rw-r--r--   0        0        0    42689 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflow.py
--rw-r--r--   0        0        0     4048 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2175 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/modify_note.py
--rw-r--r--   0        0        0      909 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/removed_workflow.py
--rw-r--r--   0        0        0     9528 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/steps.py
--rw-r--r--   0        0        0      571 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     1614 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py
--rw-r--r--   0        0        0     2349 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/resume_workflows.py
--rw-r--r--   0        0        0     8511 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/validate_products.py
--rw-r--r--   0        0        0      684 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/translations/en-GB.json
--rw-r--r--   0        0        0    12929 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/orchestrator/workflows/utils.py
--rw-r--r--   0        0        0     5208 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2725 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/setup.cfg
--rw-r--r--   0        0        0      665 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/setup.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/__init__.py
--rw-r--r--   0        0        0     3199 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/conftest.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
--rw-r--r--   0        0        0     1851 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
--rw-r--r--   0        0        0     1544 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
--rw-r--r--   0        0        0     1529 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
--rw-r--r--   0        0        0     1210 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2887 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
--rw-r--r--   0        0        0      588 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/acceptance_tests/test_test_product.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/__init__.py
--rw-r--r--   0        0        0     5160 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_caching.py
--rw-r--r--   0        0        0     1139 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_health.py
--rw-r--r--   0        0        0     3055 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_helpers.py
--rw-r--r--   0        0        0     1747 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_models.py
--rw-r--r--   0        0        0    19442 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_processes.py
--rw-r--r--   0        0        0    15509 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_processes_ws.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_product_blocks.py
--rw-r--r--   0        0        0     5841 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_products.py
--rw-r--r--   0        0        0     3000 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_settings.py
--rw-r--r--   0        0        0     3038 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_subscription_customer_descriptions.py
--rw-r--r--   0        0        0    29171 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_subscriptions.py
--rw-r--r--   0        0        0     3777 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/api/test_ws.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/__init__.py
--rw-r--r--   0        0        0      744 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate.sh
--rw-r--r--   0        0        0      885 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/alembic.ini
--rw-r--r--   0        0        0      233 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/main.py
--rw-r--r--   0        0        0     2821 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/env.py
--rw-r--r--   0        0        0       98 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/helpers.py
--rw-r--r--   0        0        0      510 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/script.py.mako
--rw-r--r--   0        0        0      315 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_59e1199aff7f_create_data_head.py
--rw-r--r--   0        0        0     2227 2024-05-06 11:29:58.018776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py
--rw-r--r--   0        0        0     3852 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py
--rw-r--r--   0        0        0      467 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1995 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_blocks/example1.py
--rw-r--r--   0        0        0      812 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_blocks/example2.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_types/__init__.py
--rw-r--r--   0        0        0      764 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_types/example1.py
--rw-r--r--   0        0        0      559 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_types/example2.py
--rw-r--r--   0        0        0     1499 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py
--rw-r--r--   0        0        0     1499 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py
--rw-r--r--   0        0        0     2442 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py
--rw-r--r--   0        0        0     2014 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py
--rw-r--r--   0        0        0     1345 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py
--rw-r--r--   0        0        0     1010 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py
--rw-r--r--   0        0        0      902 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py
--rw-r--r--   0        0        0      872 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py
--rw-r--r--   0        0        0      755 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py
--rw-r--r--   0        0        0      405 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_validate_example2.py
--rw-r--r--   0        0        0      415 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/translations/en-GB.json
--rw-r--r--   0        0        0      701 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/__init__.py
--rw-r--r--   0        0        0     3940 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py
--rw-r--r--   0        0        0     3602 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py
--rw-r--r--   0        0        0      620 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py
--rw-r--r--   0        0        0     1560 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py
--rw-r--r--   0        0        0     1025 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py
--rw-r--r--   0        0        0     2683 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py
--rw-r--r--   0        0        0     2508 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py
--rw-r--r--   0        0        0        1 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/shared/forms.py
--rw-r--r--   0        0        0     1220 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py
--rw-r--r--   0        0        0     1273 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/shared.py
--rw-r--r--   0        0        0     2656 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/product_config1.yaml
--rw-r--r--   0        0        0      549 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/product_config2.yaml
--rw-r--r--   0        0        0      590 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/product_config3.yaml
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/generator/__init__.py
--rw-r--r--   0        0        0      812 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/generator/test_enums.py
--rw-r--r--   0        0        0     2509 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_cli_generate.py
--rw-r--r--   0        0        0     2930 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_generate_code.py
--rw-r--r--   0        0        0    26343 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
--rw-r--r--   0        0        0    27644 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
--rw-r--r--   0        0        0      511 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/config.py
--rw-r--r--   0        0        0    23677 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/conftest.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/domain/__init__.py
--rw-r--r--   0        0        0    53002 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_base.py
--rw-r--r--   0        0        0     8230 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_base_with_list_union.py
--rw-r--r--   0        0        0     4670 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_base_with_union.py
--rw-r--r--   0        0        0     1992 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_lifecycle.py
--rw-r--r--   0        0        0     2841 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/__init__.py
--rw-r--r--   0        0        0     7794 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/processes.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1645 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
--rw-r--r--   0        0        0     2970 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
--rw-r--r--   0        0        0     1606 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
--rw-r--r--   0        0        0     2573 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
--rw-r--r--   0        0        0     2518 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
--rw-r--r--   0        0        0     1194 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
--rw-r--r--   0        0        0     1123 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/__init__.py
--rw-r--r--   0        0        0     2372 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
--rw-r--r--   0        0        0     2172 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
--rw-r--r--   0        0        0     4217 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
--rw-r--r--   0        0        0     3428 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py
--rw-r--r--   0        0        0     2341 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
--rw-r--r--   0        0        0     2951 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
--rw-r--r--   0        0        0     2272 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
--rw-r--r--   0        0        0     2256 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
--rw-r--r--   0        0        0     1639 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
--rw-r--r--   0        0        0     1838 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py
--rw-r--r--   0        0        0      644 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/resource_types.py
--rw-r--r--   0        0        0      451 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/workflows.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/forms/__init__.py
--rw-r--r--   0        0        0     4706 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_customer_contact_list.py
--rw-r--r--   0        0        0      495 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_customer_id.py
--rw-r--r--   0        0        0     1746 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_display_subscription.py
--rw-r--r--   0        0        0     4109 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_generic_validators.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.022776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/__init__.py
--rw-r--r--   0        0        0     1424 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/conftest.py
--rw-r--r--   0        0        0      488 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/mutations/helpers.py
--rw-r--r--   0        0        0     6235 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/mutations/test_customer_description.py
--rw-r--r--   0        0        0     2449 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/mutations/test_start_process.py
--rw-r--r--   0        0        0     2316 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_customer.py
--rw-r--r--   0        0        0    18677 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_processes.py
--rw-r--r--   0        0        0     8514 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_product.py
--rw-r--r--   0        0        0    10211 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_product_blocks.py
--rw-r--r--   0        0        0     5635 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_resource_types.py
--rw-r--r--   0        0        0     5179 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_settings.py
--rw-r--r--   0        0        0     2939 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_sort_and_filter_fields.py
--rw-r--r--   0        0        0     3239 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_subscription.py
--rw-r--r--   0        0        0    48814 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_subscriptions.py
--rw-r--r--   0        0        0     6682 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_workflows.py
--rw-r--r--   0        0        0      608 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_autoregistration.py
--rw-r--r--   0        0        0     7669 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_is_query_detailed.py
--rw-r--r--   0        0        0     3042 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_is_querying_page_data.py
--rw-r--r--   0        0        0     8760 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_override_class.py
--rw-r--r--   0        0        0      631 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/helpers.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/schedules/__init__.py
--rw-r--r--   0        0        0      807 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/schedules/test_scheduling.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/services/__init__.py
--rw-r--r--   0        0        0    28556 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/services/test_processes.py
--rw-r--r--   0        0        0     1155 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/services/test_products.py
--rw-r--r--   0        0        0     6171 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/services/test_subscriptions.py
--rw-r--r--   0        0        0     2100 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/services/test_translations.py
--rw-r--r--   0        0        0     6852 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/test_db.py
--rw-r--r--   0        0        0      379 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/test_types.py
--rw-r--r--   0        0        0    17406 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/test_workflow.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/__init__.py
--rw-r--r--   0        0        0      163 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1891 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_errors.py
--rw-r--r--   0        0        0     3486 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_functional.py
--rw-r--r--   0        0        0     3529 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_get_updated_properties.py
--rw-r--r--   0        0        0     3907 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_json.py
--rw-r--r--   0        0        0     5867 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_search_query.py
--rw-r--r--   0        0        0    11471 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_state.py
--rw-r--r--   0        0        0      192 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_strings.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/websocket/__init__.py
--rw-r--r--   0        0        0     3561 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/websocket/test_broadcast.py
--rw-r--r--   0        0        0    14040 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/conftest.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/shared/__init__.py
--rw-r--r--   0        0        0     2094 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py
--rw-r--r--   0        0        0        0 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     2443 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
--rw-r--r--   0        0        0     2746 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py
--rw-r--r--   0        0        0      288 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/tasks/test_validate_products.py
--rw-r--r--   0        0        0     5378 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_async_workflow.py
--rw-r--r--   0        0        0     3495 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_config_db_code.py
--rw-r--r--   0        0        0     1884 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_generic_workflow_steps.py
--rw-r--r--   0        0        0      987 2024-05-06 11:29:58.026776 orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_modify_note.py
--rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 orchestrator_core-2.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      342 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.bumpversion.cfg
+-rw-r--r--   0        0        0       33 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.coveragerc
+-rw-r--r--   0        0        0     1564 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0     1149 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      502 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2620 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.github/workflows/README.md
+-rw-r--r--   0        0        0     1851 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.github/workflows/build-push-container.yml
+-rw-r--r--   0        0        0      291 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2341 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      346 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      583 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.github/workflows/issues.yml
+-rw-r--r--   0        0        0      550 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1221 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     2426 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1985 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1809 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.gitignore
+-rw-r--r--   0        0        0     2599 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/.stignore
+-rw-r--r--   0        0        0    30927 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/Dockerfile
+-rw-r--r--   0        0        0    11409 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/LICENSE
+-rw-r--r--   0        0        0      150 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/NOTICE
+-rw-r--r--   0        0        0     5595 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/README.md
+-rw-r--r--   0        0        0      196 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/codecov.yml
+-rw-r--r--   0        0        0    10746 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/application/domainmodels.md
+-rw-r--r--   0        0        0     9277 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/application/forms-frontend.md
+-rw-r--r--   0        0        0     5514 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/application/tasks.md
+-rw-r--r--   0        0        0    11462 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/application/workflow.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/orchestration/philosophy.md
+-rw-r--r--   0        0        0      668 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/context.md
+-rw-r--r--   0        0        0     4226 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/imports.md
+-rw-r--r--   0        0        0      802 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/introduction.md
+-rw-r--r--   0        0        0     1671 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/ip_static.md
+-rw-r--r--   0        0        0    84576 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/ip_static.png
+-rw-r--r--   0        0        0     1311 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/l2_point_to_point.md
+-rw-r--r--   0        0        0    55937 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/l2_point_to_point.png
+-rw-r--r--   0        0        0      854 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/l2_vpn.md
+-rw-r--r--   0        0        0    29551 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/l2_vpn.png
+-rw-r--r--   0        0        0     1398 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/modelling.md
+-rw-r--r--   0        0        0     1138 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/node.md
+-rw-r--r--   0        0        0    23110 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/node.png
+-rw-r--r--   0        0        0     1147 2024-05-06 11:41:27.107505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/port.md
+-rw-r--r--   0        0        0    37248 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/port.png
+-rw-r--r--   0        0        0     1694 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/product_block_graph.md
+-rw-r--r--   0        0        0    78824 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/product_block_graph.png
+-rw-r--r--   0        0        0      989 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/standards.md
+-rw-r--r--   0        0        0     1114 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/terminology.md
+-rw-r--r--   0        0        0     2080 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/architecture/tldr.md
+-rw-r--r--   0        0        0      443 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/contributing/documentation.md
+-rw-r--r--   0        0        0     1771 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/contributing/guidelines.md
+-rw-r--r--   0        0        0     9997 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/contributing/testing.md
+-rw-r--r--   0        0        0      452 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/css/custom.css
+-rw-r--r--   0        0        0      656 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/css/style.css
+-rw-r--r--   0        0        0     2165 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/css/termynal.css
+-rw-r--r--   0        0        0     2135 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/getting-started/base.md
+-rw-r--r--   0        0        0      928 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/getting-started/development.md
+-rw-r--r--   0        0        0     3438 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/getting-started/prepare-source-folder.md
+-rw-r--r--   0        0        0    17905 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/img/WFO-Emblem-White.png
+-rw-r--r--   0        0        0      842 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/img/favicon.ico
+-rw-r--r--   0        0        0     4005 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/index.md
+-rw-r--r--   0        0        0     3897 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/js/termynal.js
+-rw-r--r--   0        0        0    11084 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/migration-guide/2.0.md
+-rw-r--r--   0        0        0      600 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/api.md
+-rw-r--r--   0        0        0     1026 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/app/app.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/app/runtimes.md
+-rw-r--r--   0        0        0     4966 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/auth.md
+-rw-r--r--   0        0        0    29652 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/cli.md
+-rw-r--r--   0        0        0     2241 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/database.md
+-rw-r--r--   0        0        0      359 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/generator.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/instantiating.md
+-rw-r--r--   0        0        0     3867 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/model_attributes.md
+-rw-r--r--   0        0        0      543 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/overview.md
+-rw-r--r--   0        0        0     3863 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/product_blocks.md
+-rw-r--r--   0        0        0     4030 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/product_types.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/properties.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/pydantic_hooks.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/type_casting.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/union_types.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/validation.md
+-rw-r--r--   0        0        0    15366 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/forms.md
+-rw-r--r--   0        0        0    27254 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/graphql.md
+-rw-r--r--   0        0        0     1565 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/python.md
+-rw-r--r--   0        0        0     5585 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/scaling.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/serialization.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/tasks.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/tests.md
+-rw-r--r--   0        0        0      499 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/tldr.md
+-rw-r--r--   0        0        0     2500 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/websockets.md
+-rw-r--r--   0        0        0     5505 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/workflows/callbacks.md
+-rw-r--r--   0        0        0       73 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/workflows/workflow-lifecycles.md
+-rw-r--r--   0        0        0     1472 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/reference-docs/workflows/workflow-steps.md
+-rw-r--r--   0        0        0     9063 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/advanced/circuit-workflow.md
+-rw-r--r--   0        0        0      254 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/advanced/database-migration.md
+-rw-r--r--   0        0        0     3719 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/advanced/docker-installation.md
+-rw-r--r--   0        0        0     2563 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/advanced/domain-models.md
+-rw-r--r--   0        0        0     6048 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/advanced/node-workflow.md
+-rw-r--r--   0        0        0     3087 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/advanced/overview.md
+-rw-r--r--   0        0        0     1750 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/advanced/scenario.md
+-rw-r--r--   0        0        0     4369 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/advanced/workflow-introduction.md
+-rw-r--r--   0        0        0     5602 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/create-user-group.md
+-rw-r--r--   0        0        0     4623 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/create-user.md
+-rw-r--r--   0        0        0     7447 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/database-migration.md
+-rw-r--r--   0        0        0     3697 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/debian.md
+-rw-r--r--   0        0        0     3051 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/docker.md
+-rw-r--r--   0        0        0     6157 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/domain-models.md
+-rw-r--r--   0        0        0     1953 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/explore.md
+-rw-r--r--   0        0        0     3991 2024-05-06 11:41:27.111505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/input-forms.md
+-rw-r--r--   0        0        0     3596 2024-05-06 11:41:27.115505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/macos.md
+-rw-r--r--   0        0        0     3411 2024-05-06 11:41:27.115505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/modify-user-group.md
+-rw-r--r--   0        0        0     2141 2024-05-06 11:41:27.115505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/modify-user.md
+-rw-r--r--   0        0        0     2878 2024-05-06 11:41:27.115505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/overview.md
+-rw-r--r--   0        0        0     4547 2024-05-06 11:41:27.115505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/register-workflows.md
+-rw-r--r--   0        0        0      785 2024-05-06 11:41:27.115505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/scenario.md
+-rw-r--r--   0        0        0     1013 2024-05-06 11:41:27.115505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/start-applications.md
+-rw-r--r--   0        0        0     2988 2024-05-06 11:41:27.115505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/terminate-user-group.md
+-rw-r--r--   0        0        0     1332 2024-05-06 11:41:27.115505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/terminate-user.md
+-rw-r--r--   0        0        0     3632 2024-05-06 11:41:27.115505 orchestrator_core-2.3.0rc2/docs/workshops/beginner/workflow-introduction.md
+-rw-r--r--   0        0        0    46296 2024-05-06 11:41:27.115505 orchestrator_core-2.3.0rc2/docs/workshops/images/metadata_products.png
+-rw-r--r--   0        0        0   983304 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/docs/workshops/images/netbox_devices_active.png
+-rw-r--r--   0        0        0      312 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/includes/abbreviations.md
+-rw-r--r--   0        0        0     8030 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/mkdocs.yml
+-rw-r--r--   0        0        0     1262 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/mutmut_config.py
+-rw-r--r--   0        0        0       70 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/nitpick-style.toml
+-rw-r--r--   0        0        0     1058 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/__init__.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/__init__.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     2466 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/api.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     1284 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/health.py
+-rw-r--r--   0        0        0    12517 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/processes.py
+-rw-r--r--   0        0        0     2143 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/products.py
+-rw-r--r--   0        0        0     6113 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/settings.py
+-rw-r--r--   0        0        0     3081 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
+-rw-r--r--   0        0        0     8867 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/subscriptions.py
+-rw-r--r--   0        0        0      963 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/translations.py
+-rw-r--r--   0        0        0     1827 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/user.py
+-rw-r--r--   0        0        0     1722 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/ws.py
+-rw-r--r--   0        0        0     1502 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/error_handling.py
+-rw-r--r--   0        0        0     6933 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/helpers.py
+-rw-r--r--   0        0        0     5996 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/api/models.py
+-rw-r--r--   0        0        0    10987 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/app.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0    16226 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/database.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/domain_gen_helpers/__init__.py
+-rw-r--r--   0        0        0     6775 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
+-rw-r--r--   0        0        0     2172 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/domain_gen_helpers/helpers.py
+-rw-r--r--   0        0        0    10474 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
+-rw-r--r--   0        0        0     9379 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py
+-rw-r--r--   0        0        0    23981 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
+-rw-r--r--   0        0        0     1399 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/domain_gen_helpers/types.py
+-rw-r--r--   0        0        0     7377 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generate.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/__init__.py
+-rw-r--r--   0        0        0      173 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/custom_templates/README
+-rw-r--r--   0        0        0      307 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/custom_templates/additional_create_imports.j2
+-rw-r--r--   0        0        0      115 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/custom_templates/additional_create_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/custom_templates/additional_create_steps.j2
+-rw-r--r--   0        0        0      307 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/custom_templates/additional_modify_imports.j2
+-rw-r--r--   0        0        0      115 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/custom_templates/additional_modify_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/custom_templates/additional_modify_steps.j2
+-rw-r--r--   0        0        0      234 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/custom_templates/additional_terminate_imports.j2
+-rw-r--r--   0        0        0      131 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/custom_templates/additional_terminate_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/custom_templates/additional_terminate_steps.j2
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/__init__.py
+-rw-r--r--   0        0        0     2007 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/enums.py
+-rw-r--r--   0        0        0     5452 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/helpers.py
+-rw-r--r--   0        0        0     6341 2024-05-06 11:41:27.119505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/migration.py
+-rw-r--r--   0        0        0     2073 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/product.py
+-rw-r--r--   0        0        0     5285 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/product_block.py
+-rw-r--r--   0        0        0     1379 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/settings.py
+-rw-r--r--   0        0        0     1878 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/translations.py
+-rw-r--r--   0        0        0     4541 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/unittest.py
+-rw-r--r--   0        0        0     1815 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/validations.py
+-rw-r--r--   0        0        0     8026 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/workflow.py
+-rw-r--r--   0        0        0      759 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/products/workshop/circuit.yaml
+-rw-r--r--   0        0        0      538 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/products/workshop/node.yaml
+-rw-r--r--   0        0        0      532 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/products/workshop/user.yaml
+-rw-r--r--   0        0        0      361 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/products/workshop/user_group.yaml
+-rw-r--r--   0        0        0      431 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/additional_create_imports.j2
+-rw-r--r--   0        0        0       25 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/additional_create_steps.j2
+-rw-r--r--   0        0        0      394 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/additional_modify_imports.j2
+-rw-r--r--   0        0        0       25 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/additional_modify_steps.j2
+-rw-r--r--   0        0        0       25 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/additional_terminate_steps.j2
+-rw-r--r--   0        0        0      282 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/constrained_int_definitions.j2
+-rw-r--r--   0        0        0      361 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/create_data_head.j2
+-rw-r--r--   0        0        0     4806 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/create_product.j2
+-rw-r--r--   0        0        0      298 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/enums.j2
+-rw-r--r--   0        0        0      523 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/lazy_workflow_instance.j2
+-rw-r--r--   0        0        0      277 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/list_definitions.j2
+-rw-r--r--   0        0        0      904 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/macros.j2
+-rw-r--r--   0        0        0     4719 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/modify_product.j2
+-rw-r--r--   0        0        0     2901 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/new_product_migration.j2
+-rw-r--r--   0        0        0     1365 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/product.j2
+-rw-r--r--   0        0        0     2454 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/product_block.j2
+-rw-r--r--   0        0        0      545 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/shared_forms.j2
+-rw-r--r--   0        0        0     1274 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/shared_workflows.j2
+-rw-r--r--   0        0        0      291 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/subscription_model_registry.j2
+-rw-r--r--   0        0        0     1883 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/terminate_product.j2
+-rw-r--r--   0        0        0     1802 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/test_create_workflow.j2
+-rw-r--r--   0        0        0     1677 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/test_modify_workflow.j2
+-rw-r--r--   0        0        0     1860 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/test_product_type.j2
+-rw-r--r--   0        0        0     1518 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/test_terminate_workflow.j2
+-rw-r--r--   0        0        0      985 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/test_validate_workflow.j2
+-rw-r--r--   0        0        0     2315 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/validate_product.j2
+-rw-r--r--   0        0        0      571 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1139 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/helpers/input_helpers.py
+-rw-r--r--   0        0        0      857 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/helpers/print_helpers.py
+-rw-r--r--   0        0        0      983 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/main.py
+-rwxr-xr-x   0        0        0    20371 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/migrate_domain_models.py
+-rwxr-xr-x   0        0        0     8979 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/migrate_workflows.py
+-rw-r--r--   0        0        0     4110 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/migration_helpers.py
+-rw-r--r--   0        0        0     1896 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/cli/scheduler.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/config/__init__.py
+-rw-r--r--   0        0        0      770 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/config/assignee.py
+-rw-r--r--   0        0        0     2970 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0    10269 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/database.py
+-rw-r--r--   0        0        0      371 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/filters/__init__.py
+-rw-r--r--   0        0        0     5020 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/filters/filters.py
+-rw-r--r--   0        0        0     4144 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/filters/process.py
+-rw-r--r--   0        0        0      899 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/filters/product.py
+-rw-r--r--   0        0        0     1089 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/filters/product_block.py
+-rw-r--r--   0        0        0      889 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/filters/resource_type.py
+-rw-r--r--   0        0        0      562 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/filters/search_filters/__init__.py
+-rw-r--r--   0        0        0     5591 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/filters/search_filters/inferred_filter.py
+-rw-r--r--   0        0        0     1466 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/filters/subscription.py
+-rw-r--r--   0        0        0     1276 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/filters/workflow.py
+-rw-r--r--   0        0        0      831 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/helpers.py
+-rw-r--r--   0        0        0    24900 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/models.py
+-rw-r--r--   0        0        0      162 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/range/__init__.py
+-rw-r--r--   0        0        0     2175 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/range/range.py
+-rw-r--r--   0        0        0      353 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/sorting/__init__.py
+-rw-r--r--   0        0        0     1987 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/sorting/process.py
+-rw-r--r--   0        0        0      570 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/sorting/product.py
+-rw-r--r--   0        0        0      617 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/sorting/product_block.py
+-rw-r--r--   0        0        0      617 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/sorting/resource_type.py
+-rw-r--r--   0        0        0     4455 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/sorting/sorting.py
+-rw-r--r--   0        0        0     1441 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/sorting/subscription.py
+-rw-r--r--   0        0        0      576 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/db/sorting/workflow.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/devtools/__init__.py
+-rw-r--r--   0        0        0    18847 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/devtools/populator.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/devtools/scripts/__init__.py
+-rw-r--r--   0        0        0     8359 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/devtools/scripts/migrate_20.py
+-rw-r--r--   0        0        0     2494 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/distlock/__init__.py
+-rw-r--r--   0        0        0     2508 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/distlock/distlock_manager.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/distlock/managers/__init__.py
+-rw-r--r--   0        0        0     3114 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/distlock/managers/memory_distlock_manager.py
+-rw-r--r--   0        0        0     3271 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/distlock/managers/redis_distlock_manager.py
+-rw-r--r--   0        0        0      894 2024-05-06 11:41:27.123505 orchestrator_core-2.3.0rc2/orchestrator/domain/__init__.py
+-rw-r--r--   0        0        0    59707 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/domain/base.py
+-rw-r--r--   0        0        0     2732 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/domain/customer_description.py
+-rw-r--r--   0        0        0      989 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/domain/helpers.py
+-rw-r--r--   0        0        0     2882 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/domain/lifecycle.py
+-rw-r--r--   0        0        0     1268 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/exception_handlers.py
+-rw-r--r--   0        0        0     1168 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/forms/__init__.py
+-rw-r--r--   0        0        0     1906 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/forms/validators/__init__.py
+-rw-r--r--   0        0        0     1505 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/forms/validators/customer_contact_list.py
+-rw-r--r--   0        0        0      708 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/forms/validators/customer_id.py
+-rw-r--r--   0        0        0      779 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/forms/validators/display_subscription.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/forms/validators/network_type_validators.py
+-rw-r--r--   0        0        0     2114 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/forms/validators/product_id.py
+-rw-r--r--   0        0        0     1418 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/__init__.py
+-rw-r--r--   0        0        0     6413 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/autoregistration.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/extensions/__init__.py
+-rw-r--r--   0        0        0     4304 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py
+-rw-r--r--   0        0        0     1746 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/extensions/error_collector_extension.py
+-rw-r--r--   0        0        0     5826 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/extensions/error_handler_extension.py
+-rw-r--r--   0        0        0     3100 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/mutations/customer_description.py
+-rw-r--r--   0        0        0     1553 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/mutations/start_process.py
+-rw-r--r--   0        0        0     2413 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/pagination.py
+-rw-r--r--   0        0        0      851 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/__init__.py
+-rw-r--r--   0        0        0      934 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/customer.py
+-rw-r--r--   0        0        0      636 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/helpers.py
+-rw-r--r--   0        0        0     4491 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/process.py
+-rw-r--r--   0        0        0     2562 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/product.py
+-rw-r--r--   0        0        0     2748 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/product_block.py
+-rw-r--r--   0        0        0     2741 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/resource_type.py
+-rw-r--r--   0        0        0     3700 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/settings.py
+-rw-r--r--   0        0        0     5888 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/subscription.py
+-rw-r--r--   0        0        0     2681 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/workflow.py
+-rw-r--r--   0        0        0     7343 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/schema.py
+-rw-r--r--   0        0        0      798 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/__init__.py
+-rw-r--r--   0        0        0      147 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/customer.py
+-rw-r--r--   0        0        0      213 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/customer_description.py
+-rw-r--r--   0        0        0      203 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/errors.py
+-rw-r--r--   0        0        0      513 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/fixed_input.py
+-rw-r--r--   0        0        0     3482 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/process.py
+-rw-r--r--   0        0        0     2430 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/product.py
+-rw-r--r--   0        0        0     2414 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/product_block.py
+-rw-r--r--   0        0        0      755 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/resource_type.py
+-rw-r--r--   0        0        0      999 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/settings.py
+-rw-r--r--   0        0        0     7838 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/subscription.py
+-rw-r--r--   0        0        0     1140 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/workflow.py
+-rw-r--r--   0        0        0     4674 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/types.py
+-rw-r--r--   0        0        0      524 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/__init__.py
+-rw-r--r--   0        0        0     1191 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/create_resolver_error_handler.py
+-rw-r--r--   0        0        0     1002 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/get_selected_fields.py
+-rw-r--r--   0        0        0     4374 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/get_subscription_product_blocks.py
+-rw-r--r--   0        0        0     2156 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/is_query_detailed.py
+-rw-r--r--   0        0        0     1370 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/override_class.py
+-rw-r--r--   0        0        0      902 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/to_graphql_result_page.py
+-rw-r--r--   0        0        0       39 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/README
+-rw-r--r--   0        0        0      873 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/alembic.ini
+-rwxr-xr-x   0        0        0     3382 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/env.py
+-rw-r--r--   0        0        0    40911 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/script.py.mako
+-rw-r--r--   0        0        0      905 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/templates/alembic.ini.j2
+-rwxr-xr-x   0        0        0     2821 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/templates/env.py.j2
+-rw-r--r--   0        0        0       98 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/templates/helpers.py.j2
+-rw-r--r--   0        0        0     2698 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
+-rw-r--r--   0        0        0     1265 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
+-rw-r--r--   0        0        0    39307 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
+-rw-r--r--   0        0        0      950 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
+-rw-r--r--   0        0        0     1214 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
+-rw-r--r--   0        0        0     1603 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
+-rw-r--r--   0        0        0     5106 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
+-rw-r--r--   0        0        0     7964 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
+-rw-r--r--   0        0        0     1014 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
+-rw-r--r--   0        0        0      591 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py
+-rw-r--r--   0        0        0      755 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql
+-rw-r--r--   0        0        0      967 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py
+-rw-r--r--   0        0        0     4491 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql
+-rw-r--r--   0        0        0     1036 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py
+-rw-r--r--   0        0        0     5383 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql
+-rw-r--r--   0        0        0     2246 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/py.typed
+-rw-r--r--   0        0        0     1066 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/schedules/__init__.py
+-rw-r--r--   0        0        0      832 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/schedules/resume_workflows.py
+-rw-r--r--   0        0        0     1526 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/schedules/scheduling.py
+-rw-r--r--   0        0        0      821 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/schedules/task_vacuum.py
+-rw-r--r--   0        0        0     1234 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/schedules/validate_products.py
+-rw-r--r--   0        0        0     2195 2024-05-06 11:41:27.127505 orchestrator_core-2.3.0rc2/orchestrator/schedules/validate_subscriptions.py
+-rw-r--r--   0        0        0     2326 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/schemas/__init__.py
+-rw-r--r--   0        0        0      930 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/schemas/base.py
+-rw-r--r--   0        0        0     1286 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/schemas/engine_settings.py
+-rw-r--r--   0        0        0     1214 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/schemas/fixed_input.py
+-rw-r--r--   0        0        0      802 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/schemas/problem_detail.py
+-rw-r--r--   0        0        0     2354 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/schemas/process.py
+-rw-r--r--   0        0        0     1484 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/schemas/product.py
+-rw-r--r--   0        0        0     1428 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/schemas/product_block.py
+-rw-r--r--   0        0        0      973 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/schemas/resource_type.py
+-rw-r--r--   0        0        0     3366 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/schemas/subscription.py
+-rw-r--r--   0        0        0     1030 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/schemas/subscription_descriptions.py
+-rw-r--r--   0        0        0     1890 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/schemas/workflow.py
+-rw-r--r--   0        0        0     2071 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/security.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0     3635 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/services/celery.py
+-rw-r--r--   0        0        0      876 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/services/fixed_inputs.py
+-rw-r--r--   0        0        0     3710 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/services/process_broadcast_thread.py
+-rw-r--r--   0        0        0    26253 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/services/processes.py
+-rw-r--r--   0        0        0     1933 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/services/products.py
+-rw-r--r--   0        0        0      884 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/services/resource_types.py
+-rw-r--r--   0        0        0     2723 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/services/settings.py
+-rw-r--r--   0        0        0    25733 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/services/subscriptions.py
+-rw-r--r--   0        0        0     5867 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/services/tasks.py
+-rw-r--r--   0        0        0     1713 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/services/translations.py
+-rw-r--r--   0        0        0     1638 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/services/workflows.py
+-rw-r--r--   0        0        0     3325 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/settings.py
+-rw-r--r--   0        0        0      766 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/targets.py
+-rw-r--r--   0        0        0    16236 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/types.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/__init__.py
+-rw-r--r--   0        0        0     5584 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/crypt.py
+-rw-r--r--   0        0        0     1477 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/datetime.py
+-rw-r--r--   0        0        0      875 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/deprecation_logger.py
+-rw-r--r--   0        0        0     6172 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/docs.py
+-rw-r--r--   0        0        0     4658 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/enrich_process.py
+-rw-r--r--   0        0        0     4250 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/errors.py
+-rw-r--r--   0        0        0     2665 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/fixed_inputs.py
+-rw-r--r--   0        0        0     8063 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/functional.py
+-rw-r--r--   0        0        0     1322 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/get_updated_properties.py
+-rw-r--r--   0        0        0     3212 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/helpers.py
+-rw-r--r--   0        0        0     8341 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/json.py
+-rw-r--r--   0        0        0     6378 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/redis.py
+-rw-r--r--   0        0        0    17039 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/search_query.py
+-rw-r--r--   0        0        0    13011 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/state.py
+-rw-r--r--   0        0        0     1077 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/utils/strings.py
+-rw-r--r--   0        0        0     1366 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/version.py
+-rw-r--r--   0        0        0     4828 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/websocket/__init__.py
+-rw-r--r--   0        0        0     4596 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py
+-rw-r--r--   0        0        0     3324 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/websocket/managers/memory_websocket_manager.py
+-rw-r--r--   0        0        0     2755 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/websocket/websocket_manager.py
+-rw-r--r--   0        0        0    42689 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/workflow.py
+-rw-r--r--   0        0        0     4048 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2175 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/workflows/modify_note.py
+-rw-r--r--   0        0        0      909 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/workflows/removed_workflow.py
+-rw-r--r--   0        0        0     9528 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/workflows/steps.py
+-rw-r--r--   0        0        0      571 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     1614 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py
+-rw-r--r--   0        0        0     2349 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/workflows/tasks/resume_workflows.py
+-rw-r--r--   0        0        0     8511 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/workflows/tasks/validate_products.py
+-rw-r--r--   0        0        0      684 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/workflows/translations/en-GB.json
+-rw-r--r--   0        0        0    12929 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/orchestrator/workflows/utils.py
+-rw-r--r--   0        0        0     5208 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     2725 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/setup.cfg
+-rw-r--r--   0        0        0      665 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/setup.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/test/acceptance_tests/__init__.py
+-rw-r--r--   0        0        0     3199 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/test/acceptance_tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.131505 orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
+-rw-r--r--   0        0        0     1851 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
+-rw-r--r--   0        0        0     1544 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1529 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
+-rw-r--r--   0        0        0     1210 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2887 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
+-rw-r--r--   0        0        0      588 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/acceptance_tests/test_test_product.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0     5160 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/api/test_caching.py
+-rw-r--r--   0        0        0     1139 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/api/test_health.py
+-rw-r--r--   0        0        0     3055 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/api/test_helpers.py
+-rw-r--r--   0        0        0     1747 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/api/test_models.py
+-rw-r--r--   0        0        0    19442 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/api/test_processes.py
+-rw-r--r--   0        0        0    15509 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/api/test_processes_ws.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/api/test_product_blocks.py
+-rw-r--r--   0        0        0     5841 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/api/test_products.py
+-rw-r--r--   0        0        0     3000 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/api/test_settings.py
+-rw-r--r--   0        0        0     3038 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/api/test_subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    29171 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/api/test_subscriptions.py
+-rw-r--r--   0        0        0     3999 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/api/test_ws.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/__init__.py
+-rw-r--r--   0        0        0      744 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate.sh
+-rw-r--r--   0        0        0      885 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/alembic.ini
+-rw-r--r--   0        0        0      233 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/main.py
+-rw-r--r--   0        0        0     2821 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/migrations/env.py
+-rw-r--r--   0        0        0       98 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/migrations/script.py.mako
+-rw-r--r--   0        0        0      315 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_59e1199aff7f_create_data_head.py
+-rw-r--r--   0        0        0     2227 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py
+-rw-r--r--   0        0        0     3852 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py
+-rw-r--r--   0        0        0      467 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/products/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1995 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/products/product_blocks/example1.py
+-rw-r--r--   0        0        0      812 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/products/product_blocks/example2.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/products/product_types/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/products/product_types/example1.py
+-rw-r--r--   0        0        0      559 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/products/product_types/example2.py
+-rw-r--r--   0        0        0     1499 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py
+-rw-r--r--   0        0        0     1499 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py
+-rw-r--r--   0        0        0     2442 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py
+-rw-r--r--   0        0        0     2014 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py
+-rw-r--r--   0        0        0     1345 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py
+-rw-r--r--   0        0        0     1010 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py
+-rw-r--r--   0        0        0      902 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py
+-rw-r--r--   0        0        0      872 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py
+-rw-r--r--   0        0        0      755 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py
+-rw-r--r--   0        0        0      405 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_validate_example2.py
+-rw-r--r--   0        0        0      415 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/translations/en-GB.json
+-rw-r--r--   0        0        0      701 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/__init__.py
+-rw-r--r--   0        0        0     3940 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py
+-rw-r--r--   0        0        0     3602 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py
+-rw-r--r--   0        0        0      620 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py
+-rw-r--r--   0        0        0     1560 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py
+-rw-r--r--   0        0        0     1025 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py
+-rw-r--r--   0        0        0     2683 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py
+-rw-r--r--   0        0        0     2508 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py
+-rw-r--r--   0        0        0        1 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example2/shared/forms.py
+-rw-r--r--   0        0        0     1220 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py
+-rw-r--r--   0        0        0     1273 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/shared.py
+-rw-r--r--   0        0        0     2656 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/product_config1.yaml
+-rw-r--r--   0        0        0      549 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/product_config2.yaml
+-rw-r--r--   0        0        0      590 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/product_config3.yaml
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/generator/__init__.py
+-rw-r--r--   0        0        0      812 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/generator/test_enums.py
+-rw-r--r--   0        0        0     2509 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/test_cli_generate.py
+-rw-r--r--   0        0        0     2930 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/test_generate_code.py
+-rw-r--r--   0        0        0    26343 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
+-rw-r--r--   0        0        0    27644 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
+-rw-r--r--   0        0        0      511 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/config.py
+-rw-r--r--   0        0        0    23677 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.135505 orchestrator_core-2.3.0rc2/test/unit_tests/domain/__init__.py
+-rw-r--r--   0        0        0    53002 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/domain/test_base.py
+-rw-r--r--   0        0        0     8230 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/domain/test_base_with_list_union.py
+-rw-r--r--   0        0        0     4670 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/domain/test_base_with_union.py
+-rw-r--r--   0        0        0     1992 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/domain/test_lifecycle.py
+-rw-r--r--   0        0        0     2841 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     7794 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/processes.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1645 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
+-rw-r--r--   0        0        0     2970 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
+-rw-r--r--   0        0        0     1606 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
+-rw-r--r--   0        0        0     2573 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
+-rw-r--r--   0        0        0     2518 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
+-rw-r--r--   0        0        0     1194 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
+-rw-r--r--   0        0        0     1123 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/__init__.py
+-rw-r--r--   0        0        0     2372 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
+-rw-r--r--   0        0        0     2172 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
+-rw-r--r--   0        0        0     4217 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
+-rw-r--r--   0        0        0     3428 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py
+-rw-r--r--   0        0        0     2341 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
+-rw-r--r--   0        0        0     2951 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
+-rw-r--r--   0        0        0     2272 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
+-rw-r--r--   0        0        0     2256 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
+-rw-r--r--   0        0        0     1639 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
+-rw-r--r--   0        0        0     1838 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py
+-rw-r--r--   0        0        0      644 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/resource_types.py
+-rw-r--r--   0        0        0      451 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/workflows.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/forms/__init__.py
+-rw-r--r--   0        0        0     4706 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/forms/test_customer_contact_list.py
+-rw-r--r--   0        0        0      495 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/forms/test_customer_id.py
+-rw-r--r--   0        0        0     1746 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/forms/test_display_subscription.py
+-rw-r--r--   0        0        0     4109 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/forms/test_generic_validators.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/__init__.py
+-rw-r--r--   0        0        0     1424 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/conftest.py
+-rw-r--r--   0        0        0      488 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/mutations/helpers.py
+-rw-r--r--   0        0        0     6235 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/mutations/test_customer_description.py
+-rw-r--r--   0        0        0     2449 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/mutations/test_start_process.py
+-rw-r--r--   0        0        0     2316 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_customer.py
+-rw-r--r--   0        0        0    18677 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_processes.py
+-rw-r--r--   0        0        0     8514 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_product.py
+-rw-r--r--   0        0        0    10211 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_product_blocks.py
+-rw-r--r--   0        0        0     5635 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_resource_types.py
+-rw-r--r--   0        0        0     5179 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_settings.py
+-rw-r--r--   0        0        0     2939 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_sort_and_filter_fields.py
+-rw-r--r--   0        0        0     3239 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_subscription.py
+-rw-r--r--   0        0        0    48814 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_subscriptions.py
+-rw-r--r--   0        0        0     6682 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_workflows.py
+-rw-r--r--   0        0        0      608 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/utils/test_autoregistration.py
+-rw-r--r--   0        0        0     7669 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/utils/test_is_query_detailed.py
+-rw-r--r--   0        0        0     3042 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/utils/test_is_querying_page_data.py
+-rw-r--r--   0        0        0     8760 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/graphql/utils/test_override_class.py
+-rw-r--r--   0        0        0      631 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/schedules/__init__.py
+-rw-r--r--   0        0        0      807 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/schedules/test_scheduling.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/services/__init__.py
+-rw-r--r--   0        0        0    28556 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/services/test_processes.py
+-rw-r--r--   0        0        0     1155 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/services/test_products.py
+-rw-r--r--   0        0        0     6171 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/services/test_subscriptions.py
+-rw-r--r--   0        0        0     2100 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/services/test_translations.py
+-rw-r--r--   0        0        0     6852 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/test_db.py
+-rw-r--r--   0        0        0      379 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/test_types.py
+-rw-r--r--   0        0        0    17406 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/utils/__init__.py
+-rw-r--r--   0        0        0      163 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1891 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_errors.py
+-rw-r--r--   0        0        0     3486 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_functional.py
+-rw-r--r--   0        0        0     3529 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_get_updated_properties.py
+-rw-r--r--   0        0        0     3907 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_json.py
+-rw-r--r--   0        0        0     5867 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_search_query.py
+-rw-r--r--   0        0        0    11471 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_state.py
+-rw-r--r--   0        0        0      192 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_strings.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/websocket/__init__.py
+-rw-r--r--   0        0        0     3561 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/websocket/test_broadcast.py
+-rw-r--r--   0        0        0    14040 2024-05-06 11:41:27.139505 orchestrator_core-2.3.0rc2/test/unit_tests/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.143505 orchestrator_core-2.3.0rc2/test/unit_tests/workflows/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.143505 orchestrator_core-2.3.0rc2/test/unit_tests/workflows/shared/__init__.py
+-rw-r--r--   0        0        0     2094 2024-05-06 11:41:27.143505 orchestrator_core-2.3.0rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:27.143505 orchestrator_core-2.3.0rc2/test/unit_tests/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     2443 2024-05-06 11:41:27.143505 orchestrator_core-2.3.0rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
+-rw-r--r--   0        0        0     2746 2024-05-06 11:41:27.143505 orchestrator_core-2.3.0rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py
+-rw-r--r--   0        0        0      288 2024-05-06 11:41:27.143505 orchestrator_core-2.3.0rc2/test/unit_tests/workflows/tasks/test_validate_products.py
+-rw-r--r--   0        0        0     5378 2024-05-06 11:41:27.143505 orchestrator_core-2.3.0rc2/test/unit_tests/workflows/test_async_workflow.py
+-rw-r--r--   0        0        0     3495 2024-05-06 11:41:27.143505 orchestrator_core-2.3.0rc2/test/unit_tests/workflows/test_config_db_code.py
+-rw-r--r--   0        0        0     1884 2024-05-06 11:41:27.143505 orchestrator_core-2.3.0rc2/test/unit_tests/workflows/test_generic_workflow_steps.py
+-rw-r--r--   0        0        0      987 2024-05-06 11:41:27.143505 orchestrator_core-2.3.0rc2/test/unit_tests/workflows/test_modify_note.py
+-rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 orchestrator_core-2.3.0rc2/PKG-INFO
```

### Comparing `orchestrator_core-2.3.0rc1/.github/ISSUE_TEMPLATE/bug-report.yml` & `orchestrator_core-2.3.0rc2/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/.github/ISSUE_TEMPLATE/feature-request.yml` & `orchestrator_core-2.3.0rc2/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/.github/workflows/README.md` & `orchestrator_core-2.3.0rc2/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/.github/workflows/build-push-container.yml` & `orchestrator_core-2.3.0rc2/.github/workflows/build-push-container.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/.github/workflows/codeql-analysis.yml` & `orchestrator_core-2.3.0rc2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/.github/workflows/issues.yml` & `orchestrator_core-2.3.0rc2/.github/workflows/issues.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/.github/workflows/publish-package.yml` & `orchestrator_core-2.3.0rc2/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/.github/workflows/run-linting-tests.yml` & `orchestrator_core-2.3.0rc2/.github/workflows/run-linting-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/.github/workflows/run-unit-tests.yml` & `orchestrator_core-2.3.0rc2/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/.github/workflows/scheduled-build.yml` & `orchestrator_core-2.3.0rc2/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/.gitignore` & `orchestrator_core-2.3.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/.pre-commit-config.yaml` & `orchestrator_core-2.3.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/.stignore` & `orchestrator_core-2.3.0rc2/.stignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/CHANGELOG.md` & `orchestrator_core-2.3.0rc2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/LICENSE` & `orchestrator_core-2.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/README.md` & `orchestrator_core-2.3.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/application/domainmodels.md` & `orchestrator_core-2.3.0rc2/docs/architecture/application/domainmodels.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/application/forms-frontend.md` & `orchestrator_core-2.3.0rc2/docs/architecture/application/forms-frontend.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/application/tasks.md` & `orchestrator_core-2.3.0rc2/docs/architecture/application/tasks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/application/workflow.md` & `orchestrator_core-2.3.0rc2/docs/architecture/application/workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/context.md` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/context.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/imports.md` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/imports.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/introduction.md` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/ip_static.md` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/ip_static.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/ip_static.png` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/ip_static.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_point_to_point.md` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/l2_point_to_point.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_point_to_point.png` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/l2_point_to_point.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_vpn.md` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/l2_vpn.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/l2_vpn.png` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/l2_vpn.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/modelling.md` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/modelling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/node.md` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/node.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/node.png` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/node.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/port.md` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/port.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/port.png` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/port.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/product_block_graph.md` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/product_block_graph.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/product_block_graph.png` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/product_block_graph.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/standards.md` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/standards.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/product_modelling/terminology.md` & `orchestrator_core-2.3.0rc2/docs/architecture/product_modelling/terminology.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/architecture/tldr.md` & `orchestrator_core-2.3.0rc2/docs/architecture/tldr.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/contributing/guidelines.md` & `orchestrator_core-2.3.0rc2/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/contributing/testing.md` & `orchestrator_core-2.3.0rc2/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/css/style.css` & `orchestrator_core-2.3.0rc2/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/css/termynal.css` & `orchestrator_core-2.3.0rc2/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/getting-started/base.md` & `orchestrator_core-2.3.0rc2/docs/getting-started/base.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/getting-started/development.md` & `orchestrator_core-2.3.0rc2/docs/getting-started/development.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/getting-started/prepare-source-folder.md` & `orchestrator_core-2.3.0rc2/docs/getting-started/prepare-source-folder.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/img/WFO-Emblem-White.png` & `orchestrator_core-2.3.0rc2/docs/img/WFO-Emblem-White.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/img/favicon.ico` & `orchestrator_core-2.3.0rc2/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/index.md` & `orchestrator_core-2.3.0rc2/docs/index.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/js/custom.js` & `orchestrator_core-2.3.0rc2/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/js/termynal.js` & `orchestrator_core-2.3.0rc2/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/migration-guide/2.0.md` & `orchestrator_core-2.3.0rc2/docs/migration-guide/2.0.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/api.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/api.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/app/app.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/app/app.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/cli.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/cli.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/database.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/database.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/model_attributes.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/model_attributes.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/overview.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/product_blocks.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/product_blocks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/domain_models/product_types.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/domain_models/product_types.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/forms.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/graphql.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/graphql.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/python.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/python.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/scaling.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/scaling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/websockets.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/websockets.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/workflows/callbacks.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/workflows/callbacks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/reference-docs/workflows/workflow-steps.md` & `orchestrator_core-2.3.0rc2/docs/reference-docs/workflows/workflow-steps.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/advanced/circuit-workflow.md` & `orchestrator_core-2.3.0rc2/docs/workshops/advanced/circuit-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/advanced/docker-installation.md` & `orchestrator_core-2.3.0rc2/docs/workshops/advanced/docker-installation.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/advanced/domain-models.md` & `orchestrator_core-2.3.0rc2/docs/workshops/advanced/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/advanced/node-workflow.md` & `orchestrator_core-2.3.0rc2/docs/workshops/advanced/node-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/advanced/overview.md` & `orchestrator_core-2.3.0rc2/docs/workshops/advanced/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/advanced/scenario.md` & `orchestrator_core-2.3.0rc2/docs/workshops/advanced/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/advanced/workflow-introduction.md` & `orchestrator_core-2.3.0rc2/docs/workshops/advanced/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/create-user-group.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/create-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/create-user.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/create-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/database-migration.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/database-migration.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/debian.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/debian.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/docker.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/docker.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/domain-models.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/explore.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/explore.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/input-forms.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/input-forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/macos.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/macos.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/modify-user-group.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/modify-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/modify-user.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/modify-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/overview.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/register-workflows.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/register-workflows.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/scenario.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/start-applications.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/start-applications.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/terminate-user-group.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/terminate-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/terminate-user.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/terminate-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/beginner/workflow-introduction.md` & `orchestrator_core-2.3.0rc2/docs/workshops/beginner/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/images/metadata_products.png` & `orchestrator_core-2.3.0rc2/docs/workshops/images/metadata_products.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/docs/workshops/images/netbox_devices_active.png` & `orchestrator_core-2.3.0rc2/docs/workshops/images/netbox_devices_active.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/mkdocs.yml` & `orchestrator_core-2.3.0rc2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/mutmut_config.py` & `orchestrator_core-2.3.0rc2/mutmut_config.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the orchestrator workflow engine."""
 
-__version__ = "2.3.0rc1"
+__version__ = "2.3.0rc2"
 
 from orchestrator.app import OrchestratorCore
-from orchestrator.settings import app_settings, oauth2_settings
+from orchestrator.settings import app_settings
 from orchestrator.workflow import begin, conditional, done, focussteps, inputstep, retrystep, step, steplens, workflow
 
 __all__ = [
     "OrchestratorCore",
     "app_settings",
-    "oauth2_settings",
     "step",
     "inputstep",
     "workflow",
     "retrystep",
     "begin",
     "done",
     "conditional",
```

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/api.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,42 +23,43 @@
     settings,
     subscription_customer_descriptions,
     subscriptions,
     translations,
     user,
     ws,
 )
-from orchestrator.security import opa_security_default
+from orchestrator.security import authorize
 
 api_router = APIRouter()
 
 api_router.include_router(
-    processes.router, prefix="/processes", tags=["Core", "Processes"], dependencies=[Depends(opa_security_default)]
+    processes.router, prefix="/processes", tags=["Core", "Processes"], dependencies=[Depends(authorize)]
 )
 api_router.include_router(processes.ws_router, prefix="/processes", tags=["Core", "Processes"])
 api_router.include_router(
-    products.router, prefix="/products", tags=["Core", "Product"], dependencies=[Depends(opa_security_default)]
+    products.router, prefix="/products", tags=["Core", "Product"], dependencies=[Depends(authorize)]
 )
 api_router.include_router(
     subscriptions.router,
     prefix="/subscriptions",
     tags=["Core", "Subscriptions"],
-    dependencies=[Depends(opa_security_default)],
+    dependencies=[Depends(authorize)],
 )
 api_router.include_router(
     subscription_customer_descriptions.router,
     prefix="/subscription_customer_descriptions",
     tags=["Core", "Subscription Customer Descriptions"],
-    dependencies=[Depends(opa_security_default)],
+    dependencies=[Depends(authorize)],
 )
+api_router.include_router(user.router, prefix="/user", tags=["Core", "User"], dependencies=[Depends(authorize)])
 api_router.include_router(
-    user.router, prefix="/user", tags=["Core", "User"], dependencies=[Depends(opa_security_default)]
+    workflows.router, prefix="/workflows", tags=["Core", "Workflows"], dependencies=[Depends(authorize)]
 )
 api_router.include_router(
-    settings.router, prefix="/settings", tags=["Core", "Settings"], dependencies=[Depends(opa_security_default)]
+    settings.router, prefix="/settings", tags=["Core", "Settings"], dependencies=[Depends(authorize)]
 )
 api_router.include_router(settings.ws_router, prefix="/settings", tags=["Core", "Settings"])
 api_router.include_router(health.router, prefix="/health", tags=["Core"])
 api_router.include_router(
     translations.router,
     prefix="/translations",
     tags=["Core", "Translations"],
```

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/health.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/processes.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/processes.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from orchestrator.schemas import (
     ProcessIdSchema,
     ProcessResumeAllSchema,
     ProcessSchema,
     ProcessStatusCounts,
     Reporter,
 )
-from orchestrator.security import oidc_user
+from orchestrator.security import authenticate
 from orchestrator.services.process_broadcast_thread import api_broadcast_process_data
 from orchestrator.services.processes import (
     SYSTEM_USER,
     _async_resume_processes,
     _get_process,
     abort_process,
     continue_awaiting_process,
@@ -83,23 +83,30 @@
         logger.info("Unable to interact with processes at this time. Engine StatusEnum is locked")
         raise_status(
             HTTPStatus.SERVICE_UNAVAILABLE, detail="Engine is locked cannot accept changes on processes at this time"
         )
 
 
 def resolve_user_name(
-    reporter: Reporter | None = None, resolved_user: OIDCUserModel | None = Depends(oidc_user)
+    reporter: Reporter | None = None,
+    resolved_user: OIDCUserModel | None = None,
 ) -> str:
     if reporter:
         return reporter
+
     if resolved_user:
         return resolved_user.name if resolved_user.name else resolved_user.user_name
+
     return SYSTEM_USER
 
 
+def user_name(user: OIDCUserModel | None = Depends(authenticate)) -> str:
+    return resolve_user_name(resolved_user=user)
+
+
 @router.delete("/{process_id}", response_model=None, status_code=HTTPStatus.NO_CONTENT)
 def delete(process_id: UUID) -> None:
     stmt = select(ProcessTable).filter_by(process_id=process_id)
     process = db.session.execute(stmt).scalar_one_or_none()
 
     if not process:
         raise_status(HTTPStatus.NOT_FOUND)
@@ -117,30 +124,30 @@
     status_code=HTTPStatus.CREATED,
     dependencies=[Depends(check_global_lock, use_cache=False)],
 )
 def new_process(
     workflow_key: str,
     request: Request,
     json_data: list[dict[str, Any]] | None = Body(...),
-    user: str = Depends(resolve_user_name),
+    user: str = Depends(user_name),
 ) -> dict[str, UUID]:
     broadcast_func = api_broadcast_process_data(request)
     process_id = start_process(workflow_key, user_inputs=json_data, user=user, broadcast_func=broadcast_func)
 
     return {"id": process_id}
 
 
 @router.put(
     "/{process_id}/resume",
     response_model=None,
     status_code=HTTPStatus.NO_CONTENT,
     dependencies=[Depends(check_global_lock, use_cache=False)],
 )
 def resume_process_endpoint(
-    process_id: UUID, request: Request, json_data: JSON = Body(...), user: str = Depends(resolve_user_name)
+    process_id: UUID, request: Request, json_data: JSON = Body(...), user: str = Depends(user_name)
 ) -> None:
     process = _get_process(process_id)
 
     if process.last_status == ProcessStatus.COMPLETED:
         raise_status(HTTPStatus.CONFLICT, "Resuming a completed workflow is not possible")
 
     if process.last_status == ProcessStatus.RUNNING:
@@ -177,15 +184,15 @@
     except AssertionError as e:
         raise_status(HTTPStatus.NOT_FOUND, str(e))
 
 
 @router.put(
     "/resume-all", response_model=ProcessResumeAllSchema, dependencies=[Depends(check_global_lock, use_cache=False)]
 )
-async def resume_all_processess_endpoint(request: Request, user: str = Depends(resolve_user_name)) -> dict[str, int]:
+async def resume_all_processess_endpoint(request: Request, user: str = Depends(user_name)) -> dict[str, int]:
     """Retry all task processes in status Failed, Waiting, API Unavailable or Inconsistent Data.
 
     The retry is started in the background, returning status 200 and number of processes in message.
     When it is already running, refuse and return status 409 instead.
     """
 
     # Retrieve processes eligible for resuming
@@ -211,15 +218,15 @@
 
     logger.info("Resuming all processes", count=len(processes_to_resume))
 
     return {"count": len(processes_to_resume)}
 
 
 @router.put("/{process_id}/abort", response_model=None, status_code=HTTPStatus.NO_CONTENT)
-def abort_process_endpoint(process_id: UUID, request: Request, user: str = Depends(resolve_user_name)) -> None:
+def abort_process_endpoint(process_id: UUID, request: Request, user: str = Depends(user_name)) -> None:
     process = _get_process(process_id)
 
     broadcast_func = api_broadcast_process_data(request)
     try:
         abort_process(process, user, broadcast_func=broadcast_func)
         return
     except Exception as e:
```

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/products.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/settings.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,25 @@
 from redis.asyncio import Redis as AIORedis
 from sqlalchemy.exc import SQLAlchemyError
 
 from oauth2_lib.fastapi import OIDCUserModel
 from orchestrator.api.error_handling import raise_status
 from orchestrator.db import EngineSettingsTable
 from orchestrator.schemas import EngineSettingsBaseSchema, EngineSettingsSchema, GlobalStatusEnum, WorkerStatus
-from orchestrator.security import oidc_user
+from orchestrator.security import authenticate
 from orchestrator.services import processes, settings
 from orchestrator.settings import ExecutorType, app_settings
 from orchestrator.utils.json import json_dumps
 from orchestrator.utils.redis import delete_keys_matching_pattern
 from orchestrator.websocket import WS_CHANNELS, broadcast_invalidate_cache, websocket_manager
 
 router = APIRouter()
 logger = structlog.get_logger()
 
+
 CACHE_FLUSH_OPTIONS: dict[str, str] = {
     "all": "All caches",
 }
 
 
 @router.delete("/cache/{name}")
 async def clear_cache(name: str) -> int | None:
@@ -59,15 +60,15 @@
         settings.reset_search_index(tx_commit=True)
     except SQLAlchemyError:
         raise_status(HTTPStatus.INTERNAL_SERVER_ERROR)
 
 
 @router.put("/status", response_model=EngineSettingsSchema)
 async def set_global_status(
-    body: EngineSettingsBaseSchema, user: OIDCUserModel | None = Depends(oidc_user)
+    body: EngineSettingsBaseSchema, user: OIDCUserModel | None = Depends(authenticate)
 ) -> EngineSettingsSchema:
     """Update the global status of the engine to a new state.
 
     Args:
         body: The GlobalStatus object
         user: The OIDCUser model
```

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/subscriptions.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/subscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     SubscriptionMetadataTable,
     SubscriptionTable,
     db,
 )
 from orchestrator.domain import SubscriptionModel
 from orchestrator.schemas import SubscriptionWorkflowListsSchema
 from orchestrator.schemas.subscription import SubscriptionDomainModelSchema, SubscriptionWithMetadata
-from orchestrator.security import oidc_user
+from orchestrator.security import authenticate
 from orchestrator.services.subscriptions import (
     _generate_etag,
     build_extended_domain_model,
     format_extended_domain_model,
     format_special_types,
     get_subscription,
     subscription_workflows,
@@ -187,15 +187,15 @@
     if not subscription:
         raise_status(HTTPStatus.NOT_FOUND)
 
     return subscription_workflows(subscription)
 
 
 @router.put("/{subscription_id}/set_in_sync", response_model=None, status_code=HTTPStatus.OK)
-def subscription_set_in_sync(subscription_id: UUID, current_user: OIDCUserModel | None = Depends(oidc_user)) -> None:
+def subscription_set_in_sync(subscription_id: UUID, current_user: OIDCUserModel | None = Depends(authenticate)) -> None:
     def failed_processes() -> list[str]:
         if app_settings.DISABLE_INSYNC_CHECK:
             return []
         stmt = (
             select(ProcessSubscriptionTable)
             .join(ProcessTable)
             .filter(ProcessSubscriptionTable.subscription_id == subscription_id)
```

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/translations.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/user.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/api_v1/endpoints/ws.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/api_v1/endpoints/ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/error_handling.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/error_handling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/api/models.py` & `orchestrator_core-2.3.0rc2/orchestrator/api/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/database.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/domain_gen_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/domain_gen_helpers/types.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/domain_gen_helpers/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generate.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/enums.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/enums.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/migration.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/product.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/product_block.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/settings.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/translations.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/unittest.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/unittest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/validations.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/validations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/generator/workflow.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/generator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/circuit.yaml` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/products/workshop/circuit.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/node.yaml` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/products/workshop/node.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/products/workshop/user.yaml` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/products/workshop/user.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/create_product.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/create_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/lazy_workflow_instance.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/lazy_workflow_instance.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/macros.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/macros.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/modify_product.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/modify_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/new_product_migration.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/new_product_migration.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/product.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/product_block.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/product_block.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/shared_forms.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/shared_forms.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/shared_workflows.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/shared_workflows.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/terminate_product.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/terminate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_create_workflow.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/test_create_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_modify_workflow.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/test_modify_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_product_type.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/test_product_type.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_terminate_workflow.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/test_terminate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/test_validate_workflow.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/test_validate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/generator/templates/validate_product.j2` & `orchestrator_core-2.3.0rc2/orchestrator/cli/generator/templates/validate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/helpers/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/helpers/input_helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/helpers/input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/helpers/print_helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/helpers/print_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/main.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/migrate_domain_models.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/migrate_domain_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/migrate_workflows.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/migrate_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/migration_helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/cli/scheduler.py` & `orchestrator_core-2.3.0rc2/orchestrator/cli/scheduler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/config/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/config/assignee.py` & `orchestrator_core-2.3.0rc2/orchestrator/config/assignee.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/database.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/filters/filters.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/filters/filters.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/filters/process.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/filters/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/filters/product.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/filters/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/filters/product_block.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/filters/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/filters/resource_type.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/filters/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/filters/search_filters/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/filters/search_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/filters/search_filters/inferred_filter.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/filters/search_filters/inferred_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/filters/subscription.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/filters/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/filters/workflow.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/filters/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/models.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/range/range.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/range/range.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/process.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/sorting/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/product.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/sorting/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/product_block.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/sorting/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/resource_type.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/sorting/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/sorting.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/sorting/sorting.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/subscription.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/sorting/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/db/sorting/workflow.py` & `orchestrator_core-2.3.0rc2/orchestrator/db/sorting/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/devtools/populator.py` & `orchestrator_core-2.3.0rc2/orchestrator/devtools/populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/devtools/scripts/migrate_20.py` & `orchestrator_core-2.3.0rc2/orchestrator/devtools/scripts/migrate_20.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/distlock/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/distlock/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/distlock/distlock_manager.py` & `orchestrator_core-2.3.0rc2/orchestrator/distlock/distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/distlock/managers/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/distlock/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/distlock/managers/memory_distlock_manager.py` & `orchestrator_core-2.3.0rc2/orchestrator/distlock/managers/memory_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/distlock/managers/redis_distlock_manager.py` & `orchestrator_core-2.3.0rc2/orchestrator/distlock/managers/redis_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/domain/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/domain/base.py` & `orchestrator_core-2.3.0rc2/orchestrator/domain/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/domain/customer_description.py` & `orchestrator_core-2.3.0rc2/orchestrator/domain/customer_description.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/domain/helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/domain/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/domain/lifecycle.py` & `orchestrator_core-2.3.0rc2/orchestrator/domain/lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/exception_handlers.py` & `orchestrator_core-2.3.0rc2/orchestrator/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/forms/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/forms/validators/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/forms/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/forms/validators/customer_contact_list.py` & `orchestrator_core-2.3.0rc2/orchestrator/forms/validators/customer_contact_list.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/forms/validators/customer_id.py` & `orchestrator_core-2.3.0rc2/orchestrator/forms/validators/customer_id.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/forms/validators/display_subscription.py` & `orchestrator_core-2.3.0rc2/orchestrator/forms/validators/display_subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/forms/validators/network_type_validators.py` & `orchestrator_core-2.3.0rc2/orchestrator/forms/validators/network_type_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/forms/validators/product_id.py` & `orchestrator_core-2.3.0rc2/orchestrator/forms/validators/product_id.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,30 +20,28 @@
     CustomerQuery,
     Mutation,
     OrchestratorGraphqlRouter,
     OrchestratorQuery,
     OrchestratorSchema,
     Query,
     create_graphql_router,
-    custom_context_dependency,
     get_context,
 )
 from orchestrator.graphql.schemas import DEFAULT_GRAPHQL_MODELS
 from orchestrator.graphql.types import SCALAR_OVERRIDES
 
 __all__ = [
     "DEFAULT_GRAPHQL_MODELS",
     "SCALAR_OVERRIDES",
     "Query",
     "OrchestratorQuery",
     "CustomerQuery",
     "Mutation",
     "OrchestratorGraphqlRouter",
     "OrchestratorSchema",
-    "custom_context_dependency",
     "get_context",
     "create_graphql_router",
     "EnumDict",
     "add_class_to_strawberry",
     "graphql_subscription_name",
     "register_domain_models",
 ]
```

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/autoregistration.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/autoregistration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/error_collector_extension.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/extensions/error_collector_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/extensions/error_handler_extension.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/extensions/error_handler_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/mutations/customer_description.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/mutations/customer_description.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/mutations/start_process.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/mutations/start_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/pagination.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/customer.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/customer.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/process.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/product.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/product_block.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/resource_type.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/settings.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/subscription.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/resolvers/workflow.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/resolvers/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/schema.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 # limitations under the License.
 from collections.abc import Callable
 from http import HTTPStatus
 from typing import Any, Coroutine
 
 import strawberry
 import structlog
-from fastapi import Depends
 from fastapi.routing import APIRouter
 from graphql import GraphQLError
 from httpx import HTTPStatusError
 from strawberry.fastapi import GraphQLRouter
 from strawberry.tools import merge_types
 from strawberry.types import ExecutionContext
 from strawberry.utils.logging import StrawberryLogger
 
+from oauth2_lib.fastapi import AuthManager
 from oauth2_lib.strawberry import authenticated_field
 from orchestrator.domain.base import SubscriptionModel
 from orchestrator.graphql.autoregistration import create_subscription_strawberry_type, register_domain_models
 from orchestrator.graphql.extensions.deprecation_checker_extension import make_deprecation_checker_extension
 from orchestrator.graphql.extensions.error_handler_extension import ErrorHandlerExtension
 from orchestrator.graphql.mutations.customer_description import CustomerSubscriptionDescriptionMutation
 from orchestrator.graphql.mutations.start_process import ProcessMutation
@@ -51,15 +51,14 @@
 from orchestrator.graphql.schemas.product import ProductType
 from orchestrator.graphql.schemas.product_block import ProductBlock
 from orchestrator.graphql.schemas.resource_type import ResourceType
 from orchestrator.graphql.schemas.settings import StatusType
 from orchestrator.graphql.schemas.subscription import SubscriptionInterface
 from orchestrator.graphql.schemas.workflow import Workflow
 from orchestrator.graphql.types import SCALAR_OVERRIDES, OrchestratorContext, ScalarOverrideType, StrawberryModelType
-from orchestrator.security import get_oidc_user, get_opa_security_graphql
 from orchestrator.services.process_broadcast_thread import ProcessDataBroadcastThread
 from orchestrator.settings import app_settings
 
 api_router = APIRouter()
 
 logger = structlog.get_logger(__name__)
 
@@ -123,36 +122,29 @@
             ):
                 message = str(error.original_error).splitlines()[0]  # Strip "For more info"
                 StrawberryLogger.logger.debug(message)
             else:
                 StrawberryLogger.error(error, execution_context)
 
 
-def custom_context_dependency(
-    get_current_user: Callable = Depends(get_oidc_user),  # noqa: B008
-    get_opa_decision: Callable = Depends(get_opa_security_graphql),  # noqa: B008
-) -> OrchestratorContext:
-    return OrchestratorContext(get_current_user=get_current_user, get_opa_decision=get_opa_decision)
-
-
 def get_context(
+    auth_manager: AuthManager,
     graphql_models: StrawberryModelType,
     broadcast_thread: ProcessDataBroadcastThread | None = None,
-) -> Callable[[OrchestratorContext], Coroutine[Any, Any, OrchestratorContext]]:
-    async def _get_context(
-        custom_context: OrchestratorContext = Depends(custom_context_dependency),  # noqa: B008
-    ) -> OrchestratorContext:
-        custom_context.broadcast_thread = broadcast_thread
-        custom_context.graphql_models = graphql_models
-        return custom_context
+) -> Callable[[], Coroutine[Any, Any, OrchestratorContext]]:
+    async def _get_context() -> OrchestratorContext:
+        return OrchestratorContext(
+            auth_manager=auth_manager, graphql_models=graphql_models, broadcast_thread=broadcast_thread
+        )
 
     return _get_context
 
 
 def create_graphql_router(
+    auth_manager: AuthManager,
     query: Any = Query,
     mutation: Any = Mutation,
     register_models: bool = True,
     subscription_interface: type = SubscriptionInterface,
     broadcast_thread: ProcessDataBroadcastThread | None = None,
     graphql_models: StrawberryModelType | None = None,
     scalar_overrides: ScalarOverrideType | None = None,
@@ -172,9 +164,11 @@
         enable_federation_2=app_settings.FEDERATION_ENABLED,
         types=tuple(models.values()),
         extensions=[ErrorHandlerExtension, make_deprecation_checker_extension(query=query)],
         scalar_overrides=scalar_overrides,
     )
 
     return OrchestratorGraphqlRouter(
-        schema, context_getter=get_context(models, broadcast_thread), graphiql=app_settings.SERVE_GRAPHQL_UI
+        schema,
+        context_getter=get_context(auth_manager, models, broadcast_thread),
+        graphiql=app_settings.SERVE_GRAPHQL_UI,
     )
```

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/fixed_input.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/process.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/product.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/product_block.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/resource_type.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/settings.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/subscription.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/schemas/workflow.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/types.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,31 +7,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from collections.abc import Awaitable, Callable
 from ipaddress import IPv4Address, IPv4Interface, IPv6Address, IPv6Interface
 
 # Map some Orchestrator types to scalars
 from typing import Any, NewType, TypeVar
 
 import strawberry
 from graphql import GraphQLError
-from starlette.requests import Request
 from strawberry.custom_scalar import ScalarDefinition, ScalarWrapper
 from strawberry.experimental.pydantic.conversion_types import StrawberryTypeFromPydantic
 from strawberry.scalars import JSON
 from strawberry.types import Info
 from strawberry.types.info import RootValueType
 
 from nwastdlib.vlans import VlanRanges
-from oauth2_lib.fastapi import OIDCUserModel
+from oauth2_lib.fastapi import AuthManager
 from oauth2_lib.strawberry import OauthContext
 from orchestrator.db.filters import Filter
 from orchestrator.db.sorting import Sort, SortOrder
 from orchestrator.services.process_broadcast_thread import ProcessDataBroadcastThread
 
 StrawberryPydanticModel = TypeVar("StrawberryPydanticModel", bound=StrawberryTypeFromPydantic)
 StrawberryModelType = dict[str, StrawberryPydanticModel]
@@ -47,23 +45,22 @@
 
 class OrchestratorContext(OauthContext):
     broadcast_thread: ProcessDataBroadcastThread | None
     graphql_models: StrawberryModelType
 
     def __init__(
         self,
-        get_current_user: Callable[[Request], Awaitable[OIDCUserModel]],
-        get_opa_decision: Callable[[str, OIDCUserModel], Awaitable[bool | None]],
+        auth_manager: AuthManager,
         broadcast_thread: ProcessDataBroadcastThread | None = None,
         graphql_models: StrawberryModelType | None = None,
     ):
         self.errors: list[GraphQLError] = []
         self.broadcast_thread = broadcast_thread
         self.graphql_models = graphql_models or {}
-        super().__init__(get_current_user, get_opa_decision)
+        super().__init__(auth_manager)
 
 
 OrchestratorInfo = Info[OrchestratorContext, RootValueType]
 
 
 @strawberry.experimental.pydantic.input(model=Sort)
 class GraphqlSort:
```

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/create_resolver_error_handler.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/create_resolver_error_handler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/get_selected_fields.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/get_selected_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/get_subscription_product_blocks.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/get_subscription_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/is_query_detailed.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/is_query_detailed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/override_class.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/override_class.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/graphql/utils/to_graphql_result_page.py` & `orchestrator_core-2.3.0rc2/orchestrator/graphql/utils/to_graphql_result_page.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/alembic.ini` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/env.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/templates/alembic.ini.j2` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/templates/alembic.ini.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/templates/env.py.j2` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/templates/env.py.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py` & `orchestrator_core-2.3.0rc2/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schedules/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schedules/resume_workflows.py` & `orchestrator_core-2.3.0rc2/orchestrator/schedules/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schedules/scheduling.py` & `orchestrator_core-2.3.0rc2/orchestrator/schedules/scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schedules/task_vacuum.py` & `orchestrator_core-2.3.0rc2/orchestrator/schedules/task_vacuum.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schedules/validate_products.py` & `orchestrator_core-2.3.0rc2/orchestrator/schedules/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schedules/validate_subscriptions.py` & `orchestrator_core-2.3.0rc2/orchestrator/schedules/validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schemas/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schemas/base.py` & `orchestrator_core-2.3.0rc2/orchestrator/schemas/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schemas/engine_settings.py` & `orchestrator_core-2.3.0rc2/orchestrator/schemas/engine_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schemas/fixed_input.py` & `orchestrator_core-2.3.0rc2/orchestrator/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schemas/problem_detail.py` & `orchestrator_core-2.3.0rc2/orchestrator/schemas/problem_detail.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schemas/process.py` & `orchestrator_core-2.3.0rc2/orchestrator/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schemas/product.py` & `orchestrator_core-2.3.0rc2/orchestrator/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schemas/product_block.py` & `orchestrator_core-2.3.0rc2/orchestrator/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schemas/resource_type.py` & `orchestrator_core-2.3.0rc2/orchestrator/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schemas/subscription.py` & `orchestrator_core-2.3.0rc2/orchestrator/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schemas/subscription_descriptions.py` & `orchestrator_core-2.3.0rc2/orchestrator/schemas/subscription_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/schemas/workflow.py` & `orchestrator_core-2.3.0rc2/orchestrator/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/services/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/services/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/services/celery.py` & `orchestrator_core-2.3.0rc2/orchestrator/services/celery.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/services/fixed_inputs.py` & `orchestrator_core-2.3.0rc2/orchestrator/services/fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/services/process_broadcast_thread.py` & `orchestrator_core-2.3.0rc2/orchestrator/services/process_broadcast_thread.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/services/processes.py` & `orchestrator_core-2.3.0rc2/orchestrator/services/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/services/products.py` & `orchestrator_core-2.3.0rc2/orchestrator/services/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/services/resource_types.py` & `orchestrator_core-2.3.0rc2/orchestrator/services/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/services/settings.py` & `orchestrator_core-2.3.0rc2/orchestrator/services/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/services/subscriptions.py` & `orchestrator_core-2.3.0rc2/orchestrator/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/services/tasks.py` & `orchestrator_core-2.3.0rc2/orchestrator/services/tasks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/services/translations.py` & `orchestrator_core-2.3.0rc2/orchestrator/services/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/services/workflows.py` & `orchestrator_core-2.3.0rc2/orchestrator/services/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/settings.py` & `orchestrator_core-2.3.0rc2/orchestrator/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,21 +76,12 @@
     FEDERATION_ENABLED: bool = False
     DEFAULT_CUSTOMER_FULLNAME: str = "Default::Orchestrator-Core Customer"
     DEFAULT_CUSTOMER_SHORTCODE: str = "default-cust"
     DEFAULT_CUSTOMER_IDENTIFIER: str = "59289a57-70fb-4ff5-9c93-10fe67b12434"
     TASK_LOG_RETENTION_DAYS: int = 3
 
 
-class Oauth2Settings(BaseSettings):
-    OAUTH2_RESOURCE_SERVER_ID: str = ""
-    OAUTH2_RESOURCE_SERVER_SECRET: str = ""
-    OAUTH2_TOKEN_URL: str = ""
-    OIDC_CONF_WELL_KNOWN_URL: str = ""
-    OPA_URL: str = "http://127.0.0.1:8181/v1/data/automation/authorization/allow"
-
-
 app_settings = AppSettings()
-oauth2_settings = Oauth2Settings()
 
 # Set oauth2lib_settings variables to the same (default) value of settings
 oauth2lib_settings.SERVICE_NAME = app_settings.SERVICE_NAME
 oauth2lib_settings.ENVIRONMENT = app_settings.ENVIRONMENT
```

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/targets.py` & `orchestrator_core-2.3.0rc2/orchestrator/targets.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/types.py` & `orchestrator_core-2.3.0rc2/orchestrator/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/crypt.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/datetime.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/deprecation_logger.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/deprecation_logger.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/docs.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/docs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/enrich_process.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/enrich_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/errors.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/fixed_inputs.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/functional.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/get_updated_properties.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/get_updated_properties.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/helpers.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/json.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/redis.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/redis.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/search_query.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/search_query.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/state.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/utils/strings.py` & `orchestrator_core-2.3.0rc2/orchestrator/utils/strings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/version.py` & `orchestrator_core-2.3.0rc2/orchestrator/version.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/websocket/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py` & `orchestrator_core-2.3.0rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/websocket/managers/memory_websocket_manager.py` & `orchestrator_core-2.3.0rc2/orchestrator/websocket/managers/memory_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/websocket/websocket_manager.py` & `orchestrator_core-2.3.0rc2/orchestrator/websocket/websocket_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,19 +11,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from urllib.parse import urlparse
 
 from fastapi import WebSocket, status
 from fastapi.exceptions import HTTPException
-from httpx import AsyncClient
 from structlog import get_logger
 
-from oauth2_lib.fastapi import HTTPX_SSL_CONTEXT
-from orchestrator.security import oidc_user, opa_security_default
+from orchestrator.security import authenticate_websocket, authorize_websocket
 from orchestrator.websocket.managers.broadcast_websocket_manager import BroadcastWebsocketManager
 from orchestrator.websocket.managers.memory_websocket_manager import MemoryWebsocketManager
 
 logger = get_logger(__name__)
 
 
 class WebSocketManager:
@@ -36,18 +34,17 @@
         if self.broadcaster_type in ("redis", "rediss"):
             self._backend = BroadcastWebsocketManager(broadcast_url)
         else:
             self._backend = MemoryWebsocketManager()
 
     async def authorize(self, websocket: WebSocket, token: str) -> dict | None:
         try:
-            async with AsyncClient(verify=HTTPX_SSL_CONTEXT) as client:
-                user = await oidc_user(websocket, token=token)  # type: ignore
-                if user:
-                    await opa_security_default(websocket, user, client)  # type: ignore
+            user = await authenticate_websocket(websocket=websocket, token=token)
+            if user:
+                await authorize_websocket(websocket, user)
         except HTTPException as e:
             return {"error": vars(e)}
         return None
 
     async def connect_redis(self) -> None:
         if not self.connected:
             await self._backend.connect_redis()
```

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/workflow.py` & `orchestrator_core-2.3.0rc2/orchestrator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/workflows/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/workflows/modify_note.py` & `orchestrator_core-2.3.0rc2/orchestrator/workflows/modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/workflows/removed_workflow.py` & `orchestrator_core-2.3.0rc2/orchestrator/workflows/removed_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/workflows/steps.py` & `orchestrator_core-2.3.0rc2/orchestrator/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/__init__.py` & `orchestrator_core-2.3.0rc2/orchestrator/workflows/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py` & `orchestrator_core-2.3.0rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/resume_workflows.py` & `orchestrator_core-2.3.0rc2/orchestrator/workflows/tasks/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/workflows/tasks/validate_products.py` & `orchestrator_core-2.3.0rc2/orchestrator/workflows/tasks/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/workflows/translations/en-GB.json` & `orchestrator_core-2.3.0rc2/orchestrator/workflows/translations/en-GB.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/orchestrator/workflows/utils.py` & `orchestrator_core-2.3.0rc2/orchestrator/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/pyproject.toml` & `orchestrator_core-2.3.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     "sentry-sdk[fastapi]==2.0.1",
     "SQLAlchemy==2.0.29",
     "SQLAlchemy-Utils==0.41.2",
     "structlog",
     "typer==0.12.3",
     "uvicorn[standard]~=0.29.0",
     "nwa-stdlib~=1.7.0",
-    "oauth2-lib~=1.5.0",
+    "oauth2-lib~=2.0.0",
     "tabulate==0.9.0",
     "strawberry-graphql==0.210.0",
     "pydantic-forms~=1.0.3",
     "ruff",
 ]
 
 description-file = "README.md"
```

### Comparing `orchestrator_core-2.3.0rc1/setup.cfg` & `orchestrator_core-2.3.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/setup.py` & `orchestrator_core-2.3.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/acceptance_tests/conftest.py` & `orchestrator_core-2.3.0rc2/test/acceptance_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py` & `orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py` & `orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py` & `orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py` & `orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py` & `orchestrator_core-2.3.0rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/acceptance_tests/test_test_product.py` & `orchestrator_core-2.3.0rc2/test/acceptance_tests/test_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_caching.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/api/test_caching.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_health.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/api/test_health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_helpers.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/api/test_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_models.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/api/test_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_processes.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/api/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_processes_ws.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/api/test_processes_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_products.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_settings.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/api/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_subscription_customer_descriptions.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/api/test_subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_subscriptions.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/api/test_ws.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/api/test_ws.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,61 +21,63 @@
 
 async def test_websocket_events_invalidate_cache_async(test_client):
     with test_client.websocket_connect("api/ws/events") as websocket:
         await broadcast_invalidate_cache("foo", "bar")
         assert websocket.receive_json() == {"name": "invalidateCache", "value": ["foo", "bar"]}
 
 
-@mock.patch("orchestrator.websocket.websocket_manager.opa_security_default")
-@mock.patch("orchestrator.websocket.websocket_manager.oidc_user")
-async def test_websocket_events_not_authenticated(mock_user, mock_security, test_client):
+@mock.patch("orchestrator.websocket.websocket_manager.authorize_websocket")
+@mock.patch("orchestrator.websocket.websocket_manager.authenticate_websocket")
+async def test_websocket_events_not_authenticated(mock_authenticate_websocket, mock_authorize_websocket, test_client):
     # given: the user is not authenticated
-    mock_user.side_effect = AsyncMock(side_effect=HTTPException(status_code=401))
-    mock_security.side_effect = AsyncMock(side_effect=Exception("This should not be called"))
+    mock_authenticate_websocket.side_effect = AsyncMock(side_effect=HTTPException(status_code=401))
+    mock_authorize_websocket.side_effect = AsyncMock(side_effect=Exception("This should not be called"))
 
     # when: we create a websocket connection and ping it
     with test_client.websocket_connect("api/ws/events") as websocket:
         websocket.send_text("__ping__")
         reply = websocket.receive_text()
 
     # then: it does not reply with pong and returns 401
     assert reply != "__pong__"
     assert json.loads(reply) == {"error": {"detail": "Unauthorized", "headers": None, "status_code": 401}}
-    assert mock_user.call_args[1] == {"token": ""}
-    assert len(mock_security.mock_calls) == 0
+    assert mock_authenticate_websocket.call_count == 1
+    assert mock_authenticate_websocket.call_args[1]["token"] == ""
+    assert mock_authorize_websocket.call_count == 0
 
 
-@mock.patch("orchestrator.websocket.websocket_manager.opa_security_default")
-@mock.patch("orchestrator.websocket.websocket_manager.oidc_user")
+@mock.patch("orchestrator.websocket.websocket_manager.authorize_websocket")
+@mock.patch("orchestrator.websocket.websocket_manager.authenticate_websocket")
 async def test_websocket_events_not_authorized(mock_user, mock_security, test_client):
     # given: the user is authenticated but not authorized
     mock_user.side_effect = AsyncMock(return_value={"active": True})
     mock_security.side_effect = AsyncMock(side_effect=HTTPException(status_code=403))
 
     # when: we create a websocket connection and ping it
     with test_client.websocket_connect("api/ws/events", headers={"sec-websocket-protocol": "my token"}) as websocket:
         websocket.send_text("__ping__")
         reply = websocket.receive_text()
 
     # then: it does not reply with pong and returns 403
     assert reply != "__pong__"
     assert json.loads(reply) == {"error": {"detail": "Forbidden", "headers": None, "status_code": 403}}
-    assert mock_user.call_args[1] == {"token": "my token"}
-    assert len(mock_security.mock_calls) == 1
+    assert mock_user.call_count == 1
+    assert mock_user.call_args[1]["token"] == "my token"  # noqa: S105
+    assert mock_security.call_count == 1
 
 
-@mock.patch("orchestrator.websocket.websocket_manager.opa_security_default")
-@mock.patch("orchestrator.websocket.websocket_manager.oidc_user")
+@mock.patch("orchestrator.websocket.websocket_manager.authorize_websocket")
+@mock.patch("orchestrator.websocket.websocket_manager.authenticate_websocket")
 async def test_websocket_events_authorized(mock_user, mock_security, test_client):
     # given: the user is authenticated and authorized
     mock_user.side_effect = AsyncMock(return_value={"active": True})
     mock_security.side_effect = AsyncMock(return_value=True)
 
     # when: we create a websocket connection and ping it
     with test_client.websocket_connect("api/ws/events", headers={"sec-websocket-protocol": "my token"}) as websocket:
         websocket.send_text("__ping__")
         reply = websocket.receive_text()
 
     # then: it replies with pong
     assert reply == "__pong__"
-    assert mock_user.call_args[1] == {"token": "my token"}
-    assert len(mock_security.mock_calls) == 1
+    assert mock_user.call_args[1]["token"] == "my token"  # noqa: S105
+    assert mock_security.call_count == 1
```

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate.sh` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate.sh`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/alembic.ini` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/env.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_blocks/example1.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/products/product_blocks/example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_blocks/example2.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/products/product_blocks/example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_types/example1.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/products/product_types/example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/products/product_types/example2.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/products/product_types/example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/__init__.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/generate/workflows/shared.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/generate/workflows/shared.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/product_config1.yaml` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/product_config1.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/product_config2.yaml` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/product_config2.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/data/product_config3.yaml` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/data/product_config3.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/generator/test_enums.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/generator/test_enums.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_cli_generate.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/test_cli_generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_generate_code.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/test_generate_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/conftest.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_base.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/domain/test_base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_base_with_list_union.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/domain/test_base_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_base_with_union.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/domain/test_base_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/domain/test_lifecycle.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/domain/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/__init__.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/processes.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/fixtures/products/resource_types.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/fixtures/products/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_customer_contact_list.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/forms/test_customer_contact_list.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_display_subscription.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/forms/test_display_subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/forms/test_generic_validators.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/forms/test_generic_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/conftest.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/mutations/test_customer_description.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/mutations/test_customer_description.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/mutations/test_start_process.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/mutations/test_start_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_customer.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_customer.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_processes.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_product.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_product_blocks.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_resource_types.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_settings.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_sort_and_filter_fields.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_sort_and_filter_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_subscription.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_subscriptions.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/test_workflows.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_autoregistration.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/utils/test_autoregistration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_is_query_detailed.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/utils/test_is_query_detailed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_is_querying_page_data.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/utils/test_is_querying_page_data.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/graphql/utils/test_override_class.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/graphql/utils/test_override_class.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/helpers.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/schedules/test_scheduling.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/schedules/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/services/test_processes.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/services/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/services/test_products.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/services/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/services/test_subscriptions.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/services/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/services/test_translations.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/services/test_translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/test_db.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/test_db.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/test_workflow.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_errors.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_functional.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_get_updated_properties.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_get_updated_properties.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_json.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_search_query.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_search_query.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/utils/test_state.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/utils/test_state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/websocket/test_broadcast.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/websocket/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/__init__.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_async_workflow.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/workflows/test_async_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_config_db_code.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/workflows/test_config_db_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_generic_workflow_steps.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/workflows/test_generic_workflow_steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/test/unit_tests/workflows/test_modify_note.py` & `orchestrator_core-2.3.0rc2/test/unit_tests/workflows/test_modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.3.0rc1/PKG-INFO` & `orchestrator_core-2.3.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrator-core
-Version: 2.3.0rc1
+Version: 2.3.0rc2
 Summary: This is the orchestrator workflow engine.
 Requires-Python: >=3.11,<3.13
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
@@ -48,15 +48,15 @@
 Requires-Dist: sentry-sdk[fastapi]==2.0.1
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: SQLAlchemy-Utils==0.41.2
 Requires-Dist: structlog
 Requires-Dist: typer==0.12.3
 Requires-Dist: uvicorn[standard]~=0.29.0
 Requires-Dist: nwa-stdlib~=1.7.0
-Requires-Dist: oauth2-lib~=1.5.0
+Requires-Dist: oauth2-lib~=2.0.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: strawberry-graphql==0.210.0
 Requires-Dist: pydantic-forms~=1.0.3
 Requires-Dist: ruff
 Requires-Dist: celery~=5.4.0 ; extra == "celery"
 Requires-Dist: toml ; extra == "dev"
 Requires-Dist: bumpversion ; extra == "dev"
```

