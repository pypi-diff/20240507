# Comparing `tmp/nebari-2024.4.1rc1.tar.gz` & `tmp/nebari-2024.5.1rc1.tar.gz`

## Comparing `nebari-2024.4.1rc1.tar` & `nebari-2024.5.1rc1.tar`

### file list

```diff
@@ -1,429 +1,429 @@
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.cirun.yml
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/MANIFEST.in
--rw-r--r--   0        0        0    87041 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/RELEASE.md
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/SECURITY.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/flake.lock
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/flake.nix
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/pytest.ini
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/release-notes-sync-config.yaml
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/actions/publish-from-template/action.yml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/actions/publish-from-template/render_template.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/failed-workflow-issue-templates/test-provider.md
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/generate_cli_doc.yml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/release-notes-sync.yaml
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/release.yaml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/run-precommit.yaml
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test-provider.yaml
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_aws_integration.yaml
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_conda_build.yaml
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_do_integration.yaml
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_gcp_integration.yaml
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_helm_charts.yaml
--rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_local_integration.yaml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/typing.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/Makefile
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/README.md
--rw-r--r--   0        0        0    46502 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/cli.html
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/cli.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/conf.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/index.rst
--rw-r--r--   0        0        0    14306 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/scripts/aws-force-destroy.py
--rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/scripts/aws-force-destroy.sh
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/scripts/helm-validate.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/scripts/keycloak-export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/__init__.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/_version.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/cli.py
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/config.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/constants.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/deploy.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/deprecate.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/destroy.py
--rw-r--r--   0        0        0    11250 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/initialize.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/keycloak.py
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/render.py
--rw-r--r--   0        0        0    31183 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/upgrade.py
--rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/utils.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/__init__.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/git.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/terraform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/common.py
--rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/github.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/gitlab.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/linter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/__init__.py
--rw-r--r--   0        0        0    38296 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/amazon_web_services.py
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/azure_cloud.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/commons.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/digital_ocean.py
--rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/google_cloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/dns/__init__.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/dns/cloudflare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/oauth/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/oauth/auth0.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/__init__.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/base.py
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/tf_objects.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/bootstrap/__init__.py
--rw-r--r--   0        0        0    32085 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/locals.tf
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/main.tf
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/versions.tf
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/variables.tf
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/main.tf
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/outputs.tf
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/outputs.tf
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/outputs.tf
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/outputs.tf
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/outputs.tf
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/outputs.tf
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/variables.tf
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/main.tf
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/outputs.tf
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/variables.tf
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/main.tf
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/outputs.tf
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/providers.tf
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/versions.tf
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/main.tf
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/variables.tf
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/providers.tf
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/main.tf
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/variable.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/versions.tf
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/existing/main.tf
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/versions.tf
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/service_account.tf
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/templates/kubeconfig.yaml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/main.tf
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/variables.tf
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/main.tf
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/variables.tf
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/main.tf
--rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/variables.tf
--rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/locals.tf
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/outputs.tf
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/versions.tf
--rw-r--r--   0        0        0     9777 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/outputs.tf
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/external-container-registry.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/locals.tf
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/versions.tf
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/variables.tf
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/main.tf
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/variables.tf
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/variables.tf
--rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf
--rw-r--r--   0        0        0     9398 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/main.tf
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/outputs.tf
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/versions.tf
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/outputs.tf
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/outputs.tf
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/providers.tf
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/versions.tf
--rw-r--r--   0        0        0    22258 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/__init__.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/forward-auth.tf
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub_ssh.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/locals.tf
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/providers.tf
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/versions.tf
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/outputs.tf
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/variables.tf
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/output.tf
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/variables.tf
--rw-r--r--   0        0        0    16354 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/values.yaml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/versions.tf
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/outputs.tf
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py
--rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/middleware.tf
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/outputs.tf
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
--rw-r--r--   0        0        0    19781 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/versions.tf
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/values.yaml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf
--rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/values.yaml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/versions.tf
--rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json
--rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json
--rw-r--r--   0        0        0    34598 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json
--rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json
--rw-r--r--   0        0        0    28438 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_minio.yaml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_promtail.yaml
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/outputs.tf
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/values.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/values.yaml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/helm-extension.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/nebari-config.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/providers.tf
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/versions.tf
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/main.tf
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf
--rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/main.tf
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/output.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/main.tf
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/main.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/main.tf
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/versions.tf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/versions.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/existing/main.tf
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/main.tf
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/local/main.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/__init__.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/deploy.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/destroy.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/dev.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/info.py
--rw-r--r--   0        0        0    36979 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/init.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/keycloak.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/render.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/support.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/upgrade.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/__init__.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/__main__.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/hookspecs.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/plugins.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/conftest.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/__init__.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/config_mod_utils.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/kube_api.py
--rw-r--r--   0        0        0    16519 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/navigator.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/playwright_fixtures.py
--rw-r--r--   0        0        0    10512 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/run_notebook.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/notebooks/test_notebook_output.ipynb
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/tests/test_notebook.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/constants.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/test_dask_gateway.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/test_grafana_api.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/test_jupyterhub_ssh.py
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/test_loki_deployment.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/utils.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/assets/notebook/simple.ipynb
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/.gitignore
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress.json
--rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/package-lock.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/package.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/.gitignore
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/integration/main.js
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/plugins/index.js
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/support/index.js
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/playwright/.env.tpl
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/playwright/README.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/playwright/test_playwright.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/__init__.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/conftest.py
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/deployment_fixtures.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/test_all_clouds.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/test_gpu.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/test_preemptible.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/__init__.py
--rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/conftest.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_deploy.py
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_dev.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_init.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_init_repository.py
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_keycloak.py
--rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_support.py
--rw-r--r--   0        0        0    18509 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_upgrade.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_validate.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_commons.py
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_config.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_dependencies.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_init.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_links.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_provider.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_render.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_schema.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_upgrade.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/utils.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/aws.error.kubernetes-version.yaml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/aws.happy.yaml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/azure.happy.yaml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/do.happy.yaml
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/gcp.happy.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.authentication-type-called-custom.yaml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.extra-fields.yaml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.project_name.ends_with_special.yaml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.project_name.starts_with_number.yaml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.project_name.too_long.yaml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.auth0.yaml
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.github.yaml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.project_name.with_numbers.yaml
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/min.happy.jupyterlab.default_settings.yaml
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/min.happy.monitoring.overrides.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/min.happy.yaml
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/LICENSE
--rw-r--r--   0        0        0     9814 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/README.md
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/pyproject.toml
--rw-r--r--   0        0        0    12409 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.cirun.yml
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/MANIFEST.in
+-rw-r--r--   0        0        0    88441 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/RELEASE.md
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/SECURITY.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/flake.lock
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/flake.nix
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/pytest.ini
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/release-notes-sync-config.yaml
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/actions/publish-from-template/action.yml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/actions/publish-from-template/render_template.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/failed-workflow-issue-templates/test-provider.md
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/generate_cli_doc.yml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/release-notes-sync.yaml
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/run-precommit.yaml
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test-provider.yaml
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test_aws_integration.yaml
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test_conda_build.yaml
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test_do_integration.yaml
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test_gcp_integration.yaml
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test_helm_charts.yaml
+-rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test_local_integration.yaml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/typing.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/docs-sphinx/Makefile
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/docs-sphinx/README.md
+-rw-r--r--   0        0        0    46502 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/docs-sphinx/cli.html
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/docs-sphinx/cli.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/docs-sphinx/conf.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/docs-sphinx/index.rst
+-rw-r--r--   0        0        0    14306 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/scripts/aws-force-destroy.py
+-rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/scripts/aws-force-destroy.sh
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/scripts/helm-validate.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/scripts/keycloak-export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/__init__.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/_version.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/cli.py
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/config.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/constants.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/deploy.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/deprecate.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/destroy.py
+-rw-r--r--   0        0        0    11202 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/initialize.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/keycloak.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/render.py
+-rw-r--r--   0        0        0    32645 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/upgrade.py
+-rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/utils.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/__init__.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/git.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/terraform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cicd/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cicd/common.py
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cicd/github.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cicd/gitlab.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cicd/linter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cloud/__init__.py
+-rw-r--r--   0        0        0    38090 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cloud/amazon_web_services.py
+-rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cloud/azure_cloud.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cloud/commons.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cloud/digital_ocean.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cloud/google_cloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/dns/__init__.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/dns/cloudflare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/oauth/__init__.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/oauth/auth0.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/__init__.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/base.py
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/tf_objects.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/bootstrap/__init__.py
+-rw-r--r--   0        0        0    33679 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/locals.tf
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/main.tf
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/versions.tf
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/variables.tf
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/main.tf
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/outputs.tf
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/outputs.tf
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/outputs.tf
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/outputs.tf
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/outputs.tf
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/outputs.tf
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/variables.tf
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/main.tf
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/outputs.tf
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/variables.tf
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/main.tf
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/outputs.tf
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/providers.tf
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/versions.tf
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/main.tf
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/variables.tf
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/providers.tf
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/main.tf
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/variable.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/versions.tf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/existing/main.tf
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/versions.tf
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/service_account.tf
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/templates/kubeconfig.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/main.tf
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/variables.tf
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/main.tf
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/variables.tf
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/main.tf
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/variables.tf
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/locals.tf
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/outputs.tf
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/versions.tf
+-rw-r--r--   0        0        0     9777 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/outputs.tf
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/__init__.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/external-container-registry.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/locals.tf
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/versions.tf
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/variables.tf
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/main.tf
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/variables.tf
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/variables.tf
+-rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf
+-rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/main.tf
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/outputs.tf
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/versions.tf
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/outputs.tf
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/outputs.tf
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/providers.tf
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/versions.tf
+-rw-r--r--   0        0        0    22150 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/__init__.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/forward-auth.tf
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub_ssh.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/locals.tf
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/providers.tf
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/versions.tf
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/outputs.tf
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/variables.tf
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/output.tf
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/variables.tf
+-rw-r--r--   0        0        0    16354 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/values.yaml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/versions.tf
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/outputs.tf
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py
+-rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf
+-rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/middleware.tf
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/outputs.tf
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
+-rw-r--r--   0        0        0    20109 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/versions.tf
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/values.yaml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf
+-rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/values.yaml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/versions.tf
+-rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json
+-rw-r--r--   0        0        0    34598 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json
+-rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json
+-rw-r--r--   0        0        0    28438 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_minio.yaml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_promtail.yaml
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/outputs.tf
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/values.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/values.yaml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/helm-extension.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/nebari-config.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/providers.tf
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/versions.tf
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/main.tf
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf
+-rw-r--r--   0        0        0     9983 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/aws/main.tf
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/output.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/azure/main.tf
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/main.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/main.tf
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/versions.tf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/versions.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/existing/main.tf
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/main.tf
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/local/main.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/__init__.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/deploy.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/destroy.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/dev.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/info.py
+-rw-r--r--   0        0        0    37041 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/init.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/keycloak.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/render.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/support.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/upgrade.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/nebari/__init__.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/nebari/__main__.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/nebari/hookspecs.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/nebari/plugins.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/nebari/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/conftest.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/__init__.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/config_mod_utils.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/kube_api.py
+-rw-r--r--   0        0        0    16519 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/navigator.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/playwright_fixtures.py
+-rw-r--r--   0        0        0    10512 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/run_notebook.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/notebooks/test_notebook_output.ipynb
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/tests/test_notebook.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/constants.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/test_dask_gateway.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/test_grafana_api.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/test_jupyterhub_ssh.py
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/test_loki_deployment.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/utils.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/assets/notebook/simple.ipynb
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/.gitignore
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/cypress.json
+-rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/package-lock.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/package.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/cypress/.gitignore
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/cypress/integration/main.js
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/cypress/plugins/index.js
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/cypress/support/index.js
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/playwright/.env.tpl
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/playwright/README.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/playwright/test_playwright.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/__init__.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/conftest.py
+-rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/deployment_fixtures.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/test_all_clouds.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/test_gpu.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/test_preemptible.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/__init__.py
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/conftest.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_deploy.py
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_dev.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_init.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_init_repository.py
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_keycloak.py
+-rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_support.py
+-rw-r--r--   0        0        0    18509 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_upgrade.py
+-rw-r--r--   0        0        0    10490 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_validate.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_commons.py
+-rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_config.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_dependencies.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_init.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_links.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_provider.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_render.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_schema.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_upgrade.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/utils.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/aws.error.kubernetes-version.yaml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/aws.happy.yaml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/azure.happy.yaml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/do.happy.yaml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/gcp.happy.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.error.authentication-type-custom.yaml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.error.extra-inputs.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.error.project_name.ends_with_special.yaml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.error.project_name.starts_with_number.yaml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.error.project_name.too_long.yaml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.happy.auth0.yaml
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.happy.github.yaml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.happy.project_name.with_numbers.yaml
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.happy.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/min.happy.jupyterlab.default_settings.yaml
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/min.happy.monitoring.overrides.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/min.happy.yaml
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/LICENSE
+-rw-r--r--   0        0        0     9814 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/README.md
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    12422 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/PKG-INFO
```

### Comparing `nebari-2024.4.1rc1/.cirun.yml` & `nebari-2024.5.1rc1/.cirun.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.pre-commit-config.yaml` & `nebari-2024.5.1rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/CODE_OF_CONDUCT.md` & `nebari-2024.5.1rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/CONTRIBUTING.md` & `nebari-2024.5.1rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/RELEASE.md` & `nebari-2024.5.1rc1/RELEASE.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,34 @@
 <!-- Note:
 The RELEASE.md file at the root of the Nebari codebase is the source of truth for all release notes.
 If you want to update the release notes, open a PR against nebari-dev/nebari.
 This file is copied to nebari-dev/nebari-docs using a GitHub Action. -->
 
 ---
 
+## Release 2024.4.1 - April 20, 2024
+
+### What's Changed
+* update azurerm version by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2370
+* Get JupyterHub `groups` from Keycloak, support `oauthenticator` 16.3+ by @krassowski in https://github.com/nebari-dev/nebari/pull/2361
+* add full names for cloud providers in guided init by @exitflynn in https://github.com/nebari-dev/nebari/pull/2375
+* Add middleware to prefix JupyterHub navbar items with /hub. by @marcelovilla in https://github.com/nebari-dev/nebari/pull/2360
+* CLN: split #1928, refactor render test by @fangchenli in https://github.com/nebari-dev/nebari/pull/2246
+* add trailing slash for jupyterhub proxy paths by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2387
+* remove references to deprecated cdsdashboards by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2390
+* add default node groups to config by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2398
+* Update concurrency settings for Integration tests by @viniciusdc in https://github.com/nebari-dev/nebari/pull/2393
+* Make CI/CD Cloud Provider Test Conditional by @tylergraff in https://github.com/nebari-dev/nebari/pull/2369
+
+### New Contributors
+* @exitflynn made their first contribution in https://github.com/nebari-dev/nebari/pull/2375
+
+**Full Changelog**: https://github.com/nebari-dev/nebari/compare/2024.3.3...2024.4.1
+
+
 ## Release 2024.3.3 - March 27, 2024
 
 ### What's Changed
 * get default variable value when following a terraform variable by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2322
 * Upgrade Actions versions by @isumitjha in https://github.com/nebari-dev/nebari/pull/2291
 * Cleanup spawner logs by @krassowski in https://github.com/nebari-dev/nebari/pull/2328
 * Fix loki gateway url when deployed on non-dev namespace by @aktech in https://github.com/nebari-dev/nebari/pull/2327
```

### Comparing `nebari-2024.4.1rc1/SECURITY.md` & `nebari-2024.5.1rc1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/flake.lock` & `nebari-2024.5.1rc1/flake.lock`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/flake.nix` & `nebari-2024.5.1rc1/flake.nix`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/PULL_REQUEST_TEMPLATE.md` & `nebari-2024.5.1rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml` & `nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/config.yml` & `nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml` & `nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml` & `nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md` & `nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md` & `nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/actions/publish-from-template/action.yml` & `nebari-2024.5.1rc1/.github/actions/publish-from-template/action.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/workflows/generate_cli_doc.yml` & `nebari-2024.5.1rc1/.github/workflows/generate_cli_doc.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/workflows/release-notes-sync.yaml` & `nebari-2024.5.1rc1/.github/workflows/release-notes-sync.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/workflows/release.yaml` & `nebari-2024.5.1rc1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/workflows/run-precommit.yaml` & `nebari-2024.5.1rc1/.github/workflows/run-precommit.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/workflows/test-provider.yaml` & `nebari-2024.5.1rc1/.github/workflows/test-provider.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -28,16 +28,21 @@
     inputs:
       pr_number:
         required: true
         type: string
 
 jobs:
   test-render-providers:
-    # avoid running on PRs coming from a fork
-    if: github.event.pull_request.head.repo.full_name == github.repository || github.event_name != 'pull_request'
+    # Prevents the execution of this test under the following conditions:
+    # 1. When the 'NO_PROVIDER_CREDENTIALS' GitHub variable is set, indicating the absence of provider credentials.
+    # 2. For pull requests (PRs) originating from a fork, since GitHub does not provide the fork's credentials to the destination repository.
+    # ref. https://github.com/nebari-dev/nebari/issues/2379
+    if: |
+      vars.NO_PROVIDER_CREDENTIALS == '' &&
+      (github.event.pull_request.head.repo.full_name == github.repository || github.event_name != 'pull_request')
     name: "Test Nebari Provider"
     runs-on: ubuntu-latest
     permissions:
       id-token: write
       contents: read
       pull-requests: write
     strategy:
```

### Comparing `nebari-2024.4.1rc1/.github/workflows/test.yaml` & `nebari-2024.5.1rc1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/workflows/test_aws_integration.yaml` & `nebari-2024.5.1rc1/.github/workflows/test_aws_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/workflows/test_conda_build.yaml` & `nebari-2024.5.1rc1/.github/workflows/test_conda_build.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/workflows/test_do_integration.yaml` & `nebari-2024.5.1rc1/.github/workflows/test_do_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/workflows/test_gcp_integration.yaml` & `nebari-2024.5.1rc1/.github/workflows/test_gcp_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/workflows/test_helm_charts.yaml` & `nebari-2024.5.1rc1/.github/workflows/test_helm_charts.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.github/workflows/test_local_integration.yaml` & `nebari-2024.5.1rc1/.github/workflows/test_local_integration.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -30,22 +30,27 @@
       - ".cirun.yml"
   workflow_call:
     inputs:
       pr_number:
         required: true
         type: string
 
+# When the cancel-in-progress: true option is specified, any concurrent jobs or workflows using the same
+# concurrency group will cancel both the pending and currently running jobs or workflows. This allows only
+# one job or workflow in the concurrency group to be in progress at a time.
+concurrency:
+  group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
+  cancel-in-progress: true
+
 jobs:
   test-local-integration:
     runs-on: "cirun-runner--${{ github.run_id }}"
     defaults:
       run:
         shell: bash -l {0}
-    concurrency:
-      group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
     steps:
       - name: 'Checkout Infrastructure'
         uses: actions/checkout@main
         with:
           fetch-depth: 0
 
       - name: Checkout the branch from the PR that triggered the job
```

### Comparing `nebari-2024.4.1rc1/.github/workflows/typing.yaml` & `nebari-2024.5.1rc1/.github/workflows/typing.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/docs-sphinx/Makefile` & `nebari-2024.5.1rc1/docs-sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/docs-sphinx/README.md` & `nebari-2024.5.1rc1/docs-sphinx/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/docs-sphinx/cli.html` & `nebari-2024.5.1rc1/docs-sphinx/cli.html`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/scripts/aws-force-destroy.py` & `nebari-2024.5.1rc1/scripts/aws-force-destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/scripts/aws-force-destroy.sh` & `nebari-2024.5.1rc1/scripts/aws-force-destroy.sh`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/scripts/helm-validate.py` & `nebari-2024.5.1rc1/scripts/helm-validate.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/scripts/keycloak-export.py` & `nebari-2024.5.1rc1/scripts/keycloak-export.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/cli.py` & `nebari-2024.5.1rc1/src/_nebari/cli.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/config.py` & `nebari-2024.5.1rc1/src/_nebari/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import os
 import pathlib
 import re
 import sys
-import typing
+from typing import Any, Dict, List, Union
 
 import pydantic
 
 from _nebari.utils import yaml
 
 
-def set_nested_attribute(data: typing.Any, attrs: typing.List[str], value: typing.Any):
+def set_nested_attribute(data: Any, attrs: List[str], value: Any):
     """Takes an arbitrary set of attributes and accesses the deep
     nested object config to set value
     """
 
-    def _get_attr(d: typing.Any, attr: str):
+    def _get_attr(d: Any, attr: str):
         if isinstance(d, list) and re.fullmatch(r"\d+", attr):
             return d[int(attr)]
         elif hasattr(d, "__getitem__"):
             return d[attr]
         else:
             return getattr(d, attr)
 
-    def _set_attr(d: typing.Any, attr: str, value: typing.Any):
+    def _set_attr(d: Any, attr: str, value: Any):
         if isinstance(d, list) and re.fullmatch(r"\d+", attr):
             d[int(attr)] = value
         elif hasattr(d, "__getitem__"):
             d[attr] = value
         else:
             setattr(d, attr, value)
 
@@ -59,46 +59,57 @@
                 f"ERROR: the provided environment variable {secret} causes the following error:\n\n",
                 e,
             )
             sys.exit(1)
     return config
 
 
+def dump_nested_model(model_dict: Dict[str, Union[pydantic.BaseModel, str]]):
+    result = {}
+    for key, value in model_dict.items():
+        result[key] = (
+            value.model_dump() if isinstance(value, pydantic.BaseModel) else value
+        )
+    return result
+
+
 def read_configuration(
     config_filename: pathlib.Path,
     config_schema: pydantic.BaseModel,
     read_environment: bool = True,
 ):
     """Read the nebari configuration from disk and apply validation"""
     filename = pathlib.Path(config_filename)
 
     if not filename.is_file():
         raise ValueError(
             f"passed in configuration filename={config_filename} does not exist"
         )
 
     with filename.open() as f:
-        config = config_schema(**yaml.load(f.read()))
+        config_dict = yaml.load(f)
+        config = config_schema(**config_dict)
 
     if read_environment:
         config = set_config_from_environment_variables(config)
 
     return config
 
 
 def write_configuration(
     config_filename: pathlib.Path,
-    config: typing.Union[pydantic.BaseModel, typing.Dict],
+    config: Union[pydantic.BaseModel, Dict],
     mode: str = "w",
 ):
     """Write the nebari configuration file to disk"""
     with config_filename.open(mode) as f:
         if isinstance(config, pydantic.BaseModel):
-            yaml.dump(config.dict(), f)
+            yaml.dump(config.model_dump(), f)
         else:
+            config = dump_nested_model(config)
             yaml.dump(config, f)
 
 
 def backup_configuration(filename: pathlib.Path, extrasuffix: str = ""):
     if not filename.exists():
         return
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/constants.py` & `nebari-2024.5.1rc1/src/_nebari/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CURRENT_RELEASE = "2024.3.3"
+CURRENT_RELEASE = "2024.4.1"
 
 # NOTE: Terraform cannot be upgraded further due to Hashicorp licensing changes
 # implemented in August 2023.
 # https://www.hashicorp.com/license-faq
 TERRAFORM_VERSION = "1.5.7"
 
 # 04-kubernetes-ingress
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/deploy.py` & `nebari-2024.5.1rc1/src/_nebari/deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/destroy.py` & `nebari-2024.5.1rc1/src/_nebari/destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/initialize.py` & `nebari-2024.5.1rc1/src/_nebari/initialize.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,704 +1,701 @@
 00000000: 696d 706f 7274 206c 6f67 6769 6e67 0a69  import logging.i
 00000010: 6d70 6f72 7420 6f73 0a69 6d70 6f72 7420  mport os.import 
 00000020: 7265 0a69 6d70 6f72 7420 7465 6d70 6669  re.import tempfi
 00000030: 6c65 0a66 726f 6d20 7061 7468 6c69 6220  le.from pathlib 
-00000040: 696d 706f 7274 2050 6174 680a 0a69 6d70  import Path..imp
-00000050: 6f72 7420 7079 6461 6e74 6963 0a69 6d70  ort pydantic.imp
-00000060: 6f72 7420 7265 7175 6573 7473 0a0a 6672  ort requests..fr
-00000070: 6f6d 205f 6e65 6261 7269 2069 6d70 6f72  om _nebari impor
-00000080: 7420 636f 6e73 7461 6e74 730a 6672 6f6d  t constants.from
-00000090: 205f 6e65 6261 7269 2e70 726f 7669 6465   _nebari.provide
-000000a0: 7220 696d 706f 7274 2067 6974 0a66 726f  r import git.fro
-000000b0: 6d20 5f6e 6562 6172 692e 7072 6f76 6964  m _nebari.provid
-000000c0: 6572 2e63 6963 6420 696d 706f 7274 2067  er.cicd import g
-000000d0: 6974 6875 620a 6672 6f6d 205f 6e65 6261  ithub.from _neba
-000000e0: 7269 2e70 726f 7669 6465 722e 636c 6f75  ri.provider.clou
-000000f0: 6420 696d 706f 7274 2028 0a20 2020 2061  d import (.    a
-00000100: 6d61 7a6f 6e5f 7765 625f 7365 7276 6963  mazon_web_servic
-00000110: 6573 2c0a 2020 2020 617a 7572 655f 636c  es,.    azure_cl
-00000120: 6f75 642c 0a20 2020 2064 6967 6974 616c  oud,.    digital
-00000130: 5f6f 6365 616e 2c0a 2020 2020 676f 6f67  _ocean,.    goog
-00000140: 6c65 5f63 6c6f 7564 2c0a 290a 6672 6f6d  le_cloud,.).from
-00000150: 205f 6e65 6261 7269 2e70 726f 7669 6465   _nebari.provide
-00000160: 722e 6f61 7574 682e 6175 7468 3020 696d  r.oauth.auth0 im
-00000170: 706f 7274 2063 7265 6174 655f 636c 6965  port create_clie
-00000180: 6e74 0a66 726f 6d20 5f6e 6562 6172 692e  nt.from _nebari.
-00000190: 7374 6167 6573 2e62 6f6f 7473 7472 6170  stages.bootstrap
-000001a0: 2069 6d70 6f72 7420 4369 456e 756d 0a66   import CiEnum.f
-000001b0: 726f 6d20 5f6e 6562 6172 692e 7374 6167  rom _nebari.stag
-000001c0: 6573 2e69 6e66 7261 7374 7275 6374 7572  es.infrastructur
-000001d0: 6520 696d 706f 7274 2028 0a20 2020 2044  e import (.    D
-000001e0: 4546 4155 4c54 5f41 5753 5f4e 4f44 455f  EFAULT_AWS_NODE_
-000001f0: 4752 4f55 5053 2c0a 2020 2020 4445 4641  GROUPS,.    DEFA
-00000200: 554c 545f 415a 5552 455f 4e4f 4445 5f47  ULT_AZURE_NODE_G
-00000210: 524f 5550 532c 0a20 2020 2044 4546 4155  ROUPS,.    DEFAU
-00000220: 4c54 5f44 4f5f 4e4f 4445 5f47 524f 5550  LT_DO_NODE_GROUP
-00000230: 532c 0a20 2020 2044 4546 4155 4c54 5f47  S,.    DEFAULT_G
-00000240: 4350 5f4e 4f44 455f 4752 4f55 5053 2c0a  CP_NODE_GROUPS,.
-00000250: 290a 6672 6f6d 205f 6e65 6261 7269 2e73  ).from _nebari.s
-00000260: 7461 6765 732e 6b75 6265 726e 6574 6573  tages.kubernetes
-00000270: 5f69 6e67 7265 7373 2069 6d70 6f72 7420  _ingress import 
-00000280: 4365 7274 6966 6963 6174 6545 6e75 6d0a  CertificateEnum.
-00000290: 6672 6f6d 205f 6e65 6261 7269 2e73 7461  from _nebari.sta
-000002a0: 6765 732e 6b75 6265 726e 6574 6573 5f6b  ges.kubernetes_k
-000002b0: 6579 636c 6f61 6b20 696d 706f 7274 2041  eycloak import A
-000002c0: 7574 6865 6e74 6963 6174 696f 6e45 6e75  uthenticationEnu
-000002d0: 6d0a 6672 6f6d 205f 6e65 6261 7269 2e73  m.from _nebari.s
-000002e0: 7461 6765 732e 7465 7272 6166 6f72 6d5f  tages.terraform_
-000002f0: 7374 6174 6520 696d 706f 7274 2054 6572  state import Ter
-00000300: 7261 666f 726d 5374 6174 6545 6e75 6d0a  raformStateEnum.
-00000310: 6672 6f6d 205f 6e65 6261 7269 2e75 7469  from _nebari.uti
-00000320: 6c73 2069 6d70 6f72 7420 6765 745f 6c61  ls import get_la
-00000330: 7465 7374 5f6b 7562 6572 6e65 7465 735f  test_kubernetes_
-00000340: 7665 7273 696f 6e2c 2072 616e 646f 6d5f  version, random_
-00000350: 7365 6375 7265 5f73 7472 696e 670a 6672  secure_string.fr
-00000360: 6f6d 205f 6e65 6261 7269 2e76 6572 7369  om _nebari.versi
-00000370: 6f6e 2069 6d70 6f72 7420 5f5f 7665 7273  on import __vers
-00000380: 696f 6e5f 5f0a 6672 6f6d 206e 6562 6172  ion__.from nebar
-00000390: 692e 7363 6865 6d61 2069 6d70 6f72 7420  i.schema import 
-000003a0: 5072 6f76 6964 6572 456e 756d 2c20 6769  ProviderEnum, gi
-000003b0: 7468 7562 5f75 726c 5f72 6567 6578 0a0a  thub_url_regex..
-000003c0: 6c6f 6767 6572 203d 206c 6f67 6769 6e67  logger = logging
-000003d0: 2e67 6574 4c6f 6767 6572 285f 5f6e 616d  .getLogger(__nam
-000003e0: 655f 5f29 0a0a 5745 4c43 4f4d 455f 4845  e__)..WELCOME_HE
-000003f0: 4144 4552 5f54 4558 5420 3d20 2259 6f75  ADER_TEXT = "You
-00000400: 7220 6f70 656e 2073 6f75 7263 6520 6461  r open source da
-00000410: 7461 2073 6369 656e 6365 2070 6c61 7466  ta science platf
-00000420: 6f72 6d2c 2068 6f73 7465 6422 0a0a 0a64  orm, hosted"...d
-00000430: 6566 205f 6e6f 6465 5f67 726f 7570 735f  ef _node_groups_
-00000440: 746f 5f64 6963 7428 6e6f 6465 5f67 726f  to_dict(node_gro
-00000450: 7570 7329 3a0a 2020 2020 7265 7475 726e  ups):.    return
-00000460: 207b 6e67 5f6e 616d 653a 206e 672e 6469   {ng_name: ng.di
-00000470: 6374 2829 2066 6f72 206e 675f 6e61 6d65  ct() for ng_name
-00000480: 2c20 6e67 2069 6e20 6e6f 6465 5f67 726f  , ng in node_gro
-00000490: 7570 732e 6974 656d 7328 297d 0a0a 0a64  ups.items()}...d
-000004a0: 6566 2072 656e 6465 725f 636f 6e66 6967  ef render_config
-000004b0: 280a 2020 2020 7072 6f6a 6563 745f 6e61  (.    project_na
-000004c0: 6d65 3a20 7374 722c 0a20 2020 206e 6562  me: str,.    neb
-000004d0: 6172 695f 646f 6d61 696e 3a20 7374 7220  ari_domain: str 
-000004e0: 3d20 4e6f 6e65 2c0a 2020 2020 636c 6f75  = None,.    clou
-000004f0: 645f 7072 6f76 6964 6572 3a20 5072 6f76  d_provider: Prov
-00000500: 6964 6572 456e 756d 203d 2050 726f 7669  iderEnum = Provi
-00000510: 6465 7245 6e75 6d2e 6c6f 6361 6c2c 0a20  derEnum.local,. 
-00000520: 2020 2063 695f 7072 6f76 6964 6572 3a20     ci_provider: 
-00000530: 4369 456e 756d 203d 2043 6945 6e75 6d2e  CiEnum = CiEnum.
-00000540: 6e6f 6e65 2c0a 2020 2020 7265 706f 7369  none,.    reposi
-00000550: 746f 7279 3a20 7374 7220 3d20 4e6f 6e65  tory: str = None
-00000560: 2c0a 2020 2020 6175 7468 5f70 726f 7669  ,.    auth_provi
-00000570: 6465 723a 2041 7574 6865 6e74 6963 6174  der: Authenticat
-00000580: 696f 6e45 6e75 6d20 3d20 4175 7468 656e  ionEnum = Authen
-00000590: 7469 6361 7469 6f6e 456e 756d 2e70 6173  ticationEnum.pas
-000005a0: 7377 6f72 642c 0a20 2020 206e 616d 6573  sword,.    names
-000005b0: 7061 6365 3a20 7374 7220 3d20 2264 6576  pace: str = "dev
-000005c0: 222c 0a20 2020 2072 6570 6f73 6974 6f72  ",.    repositor
-000005d0: 795f 6175 746f 5f70 726f 7669 7369 6f6e  y_auto_provision
-000005e0: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-000005f0: 2020 2020 6175 7468 5f61 7574 6f5f 7072      auth_auto_pr
-00000600: 6f76 6973 696f 6e3a 2062 6f6f 6c20 3d20  ovision: bool = 
-00000610: 4661 6c73 652c 0a20 2020 2074 6572 7261  False,.    terra
-00000620: 666f 726d 5f73 7461 7465 3a20 5465 7272  form_state: Terr
-00000630: 6166 6f72 6d53 7461 7465 456e 756d 203d  aformStateEnum =
-00000640: 2054 6572 7261 666f 726d 5374 6174 6545   TerraformStateE
-00000650: 6e75 6d2e 7265 6d6f 7465 2c0a 2020 2020  num.remote,.    
-00000660: 6b75 6265 726e 6574 6573 5f76 6572 7369  kubernetes_versi
-00000670: 6f6e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  on: str = None,.
-00000680: 2020 2020 7265 6769 6f6e 3a20 7374 7220      region: str 
-00000690: 3d20 4e6f 6e65 2c0a 2020 2020 6469 7361  = None,.    disa
-000006a0: 626c 655f 7072 6f6d 7074 3a20 626f 6f6c  ble_prompt: bool
-000006b0: 203d 2046 616c 7365 2c0a 2020 2020 7373   = False,.    ss
-000006c0: 6c5f 6365 7274 5f65 6d61 696c 3a20 7374  l_cert_email: st
-000006d0: 7220 3d20 4e6f 6e65 2c0a 293a 0a20 2020  r = None,.):.   
-000006e0: 2063 6f6e 6669 6720 3d20 7b0a 2020 2020   config = {.    
-000006f0: 2020 2020 2270 726f 7669 6465 7222 3a20      "provider": 
-00000700: 636c 6f75 645f 7072 6f76 6964 6572 2c0a  cloud_provider,.
-00000710: 2020 2020 2020 2020 226e 616d 6573 7061          "namespa
-00000720: 6365 223a 206e 616d 6573 7061 6365 2c0a  ce": namespace,.
-00000730: 2020 2020 2020 2020 226e 6562 6172 695f          "nebari_
-00000740: 7665 7273 696f 6e22 3a20 5f5f 7665 7273  version": __vers
-00000750: 696f 6e5f 5f2c 0a20 2020 207d 0a0a 2020  ion__,.    }..  
-00000760: 2020 6966 2070 726f 6a65 6374 5f6e 616d    if project_nam
-00000770: 6520 6973 204e 6f6e 6520 616e 6420 6e6f  e is None and no
-00000780: 7420 6469 7361 626c 655f 7072 6f6d 7074  t disable_prompt
-00000790: 3a0a 2020 2020 2020 2020 7072 6f6a 6563  :.        projec
-000007a0: 745f 6e61 6d65 203d 2069 6e70 7574 2822  t_name = input("
-000007b0: 5072 6f76 6964 6520 7072 6f6a 6563 7420  Provide project 
-000007c0: 6e61 6d65 3a20 2229 0a20 2020 2063 6f6e  name: ").    con
-000007d0: 6669 675b 2270 726f 6a65 6374 5f6e 616d  fig["project_nam
-000007e0: 6522 5d20 3d20 7072 6f6a 6563 745f 6e61  e"] = project_na
-000007f0: 6d65 0a0a 2020 2020 6966 206e 6562 6172  me..    if nebar
-00000800: 695f 646f 6d61 696e 2069 7320 6e6f 7420  i_domain is not 
-00000810: 4e6f 6e65 3a0a 2020 2020 2020 2020 636f  None:.        co
-00000820: 6e66 6967 5b22 646f 6d61 696e 225d 203d  nfig["domain"] =
-00000830: 206e 6562 6172 695f 646f 6d61 696e 0a0a   nebari_domain..
-00000840: 2020 2020 636f 6e66 6967 5b22 6369 5f63      config["ci_c
-00000850: 6422 5d20 3d20 7b22 7479 7065 223a 2063  d"] = {"type": c
-00000860: 695f 7072 6f76 6964 6572 7d0a 2020 2020  i_provider}.    
-00000870: 636f 6e66 6967 5b22 7465 7272 6166 6f72  config["terrafor
-00000880: 6d5f 7374 6174 6522 5d20 3d20 7b22 7479  m_state"] = {"ty
-00000890: 7065 223a 2074 6572 7261 666f 726d 5f73  pe": terraform_s
-000008a0: 7461 7465 7d0a 0a20 2020 2023 2053 6176  tate}..    # Sav
-000008b0: 6520 6465 6661 756c 7420 7061 7373 776f  e default passwo
-000008c0: 7264 2074 6f20 6669 6c65 0a20 2020 2064  rd to file.    d
-000008d0: 6566 6175 6c74 5f70 6173 7377 6f72 645f  efault_password_
-000008e0: 6669 6c65 6e61 6d65 203d 2050 6174 6828  filename = Path(
-000008f0: 7465 6d70 6669 6c65 2e67 6574 7465 6d70  tempfile.gettemp
-00000900: 6469 7228 2929 202f 2022 4e45 4241 5249  dir()) / "NEBARI
-00000910: 5f44 4546 4155 4c54 5f50 4153 5357 4f52  _DEFAULT_PASSWOR
-00000920: 4422 0a20 2020 2063 6f6e 6669 675b 2273  D".    config["s
-00000930: 6563 7572 6974 7922 5d20 3d20 7b0a 2020  ecurity"] = {.  
-00000940: 2020 2020 2020 226b 6579 636c 6f61 6b22        "keycloak"
-00000950: 3a20 7b22 696e 6974 6961 6c5f 726f 6f74  : {"initial_root
-00000960: 5f70 6173 7377 6f72 6422 3a20 7261 6e64  _password": rand
-00000970: 6f6d 5f73 6563 7572 655f 7374 7269 6e67  om_secure_string
-00000980: 286c 656e 6774 683d 3332 297d 0a20 2020  (length=32)}.   
-00000990: 207d 0a20 2020 2077 6974 6820 6465 6661   }.    with defa
-000009a0: 756c 745f 7061 7373 776f 7264 5f66 696c  ult_password_fil
-000009b0: 656e 616d 652e 6f70 656e 2822 7722 2920  ename.open("w") 
-000009c0: 6173 2066 3a0a 2020 2020 2020 2020 662e  as f:.        f.
-000009d0: 7772 6974 6528 636f 6e66 6967 5b22 7365  write(config["se
-000009e0: 6375 7269 7479 225d 5b22 6b65 7963 6c6f  curity"]["keyclo
-000009f0: 616b 225d 5b22 696e 6974 6961 6c5f 726f  ak"]["initial_ro
-00000a00: 6f74 5f70 6173 7377 6f72 6422 5d29 0a20  ot_password"]). 
-00000a10: 2020 2064 6566 6175 6c74 5f70 6173 7377     default_passw
-00000a20: 6f72 645f 6669 6c65 6e61 6d65 2e63 686d  ord_filename.chm
-00000a30: 6f64 2830 6f37 3030 290a 0a20 2020 2063  od(0o700)..    c
-00000a40: 6f6e 6669 675b 2274 6865 6d65 225d 203d  onfig["theme"] =
-00000a50: 207b 226a 7570 7974 6572 6875 6222 3a20   {"jupyterhub": 
-00000a60: 7b22 6875 625f 7469 746c 6522 3a20 6622  {"hub_title": f"
-00000a70: 4e65 6261 7269 202d 207b 2070 726f 6a65  Nebari - { proje
-00000a80: 6374 5f6e 616d 6520 7d22 7d7d 0a20 2020  ct_name }"}}.   
-00000a90: 2063 6f6e 6669 675b 2274 6865 6d65 225d   config["theme"]
-00000aa0: 5b22 6a75 7079 7465 7268 7562 225d 5b0a  ["jupyterhub"][.
-00000ab0: 2020 2020 2020 2020 2277 656c 636f 6d65          "welcome
-00000ac0: 220a 2020 2020 5d20 3d20 2222 2257 656c  ".    ] = """Wel
-00000ad0: 636f 6d65 2120 4c65 6172 6e20 6162 6f75  come! Learn abou
-00000ae0: 7420 4e65 6261 7269 2773 2066 6561 7475  t Nebari's featu
-00000af0: 7265 7320 616e 6420 636f 6e66 6967 7572  res and configur
-00000b00: 6174 696f 6e73 2069 6e20 3c61 2068 7265  ations in <a hre
-00000b10: 663d 2268 7474 7073 3a2f 2f77 7777 2e6e  f="https://www.n
-00000b20: 6562 6172 692e 6465 762f 646f 6373 2f77  ebari.dev/docs/w
-00000b30: 656c 636f 6d65 223e 7468 6520 646f 6375  elcome">the docu
-00000b40: 6d65 6e74 6174 696f 6e3c 2f61 3e2e 2049  mentation</a>. I
-00000b50: 6620 796f 7520 6861 7665 2061 6e79 2071  f you have any q
-00000b60: 7565 7374 696f 6e73 206f 7220 6665 6564  uestions or feed
-00000b70: 6261 636b 2c20 7265 6163 6820 7468 6520  back, reach the 
-00000b80: 7465 616d 206f 6e20 3c61 2068 7265 663d  team on <a href=
-00000b90: 2268 7474 7073 3a2f 2f77 7777 2e6e 6562  "https://www.neb
-00000ba0: 6172 692e 6465 762f 646f 6373 2f63 6f6d  ari.dev/docs/com
-00000bb0: 6d75 6e69 7479 2367 6574 7469 6e67 2d73  munity#getting-s
-00000bc0: 7570 706f 7274 223e 4e65 6261 7269 2773  upport">Nebari's
-00000bd0: 2073 7570 706f 7274 2066 6f72 756d 733c   support forums<
-00000be0: 2f61 3e2e 2222 220a 0a20 2020 2063 6f6e  /a>."""..    con
-00000bf0: 6669 675b 2273 6563 7572 6974 7922 5d5b  fig["security"][
-00000c00: 2261 7574 6865 6e74 6963 6174 696f 6e22  "authentication"
-00000c10: 5d20 3d20 7b22 7479 7065 223a 2061 7574  ] = {"type": aut
-00000c20: 685f 7072 6f76 6964 6572 7d0a 0a20 2020  h_provider}..   
-00000c30: 2069 6620 6175 7468 5f70 726f 7669 6465   if auth_provide
-00000c40: 7220 3d3d 2041 7574 6865 6e74 6963 6174  r == Authenticat
-00000c50: 696f 6e45 6e75 6d2e 6769 7468 7562 3a0a  ionEnum.github:.
-00000c60: 2020 2020 2020 2020 636f 6e66 6967 5b22          config["
-00000c70: 7365 6375 7269 7479 225d 5b22 6175 7468  security"]["auth
-00000c80: 656e 7469 6361 7469 6f6e 225d 5b22 636f  entication"]["co
-00000c90: 6e66 6967 225d 203d 207b 0a20 2020 2020  nfig"] = {.     
-00000ca0: 2020 2020 2020 2022 636c 6965 6e74 5f69         "client_i
-00000cb0: 6422 3a20 6f73 2e65 6e76 6972 6f6e 2e67  d": os.environ.g
-00000cc0: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
-00000cd0: 2020 2020 2247 4954 4855 425f 434c 4945      "GITHUB_CLIE
-00000ce0: 4e54 5f49 4422 2c0a 2020 2020 2020 2020  NT_ID",.        
-00000cf0: 2020 2020 2020 2020 223c 656e 7465 7220          "<enter 
-00000d00: 636c 6965 6e74 2069 6420 6f72 2072 656d  client id or rem
-00000d10: 6f76 6520 746f 2075 7365 2047 4954 4855  ove to use GITHU
-00000d20: 425f 434c 4945 4e54 5f49 4420 656e 7669  B_CLIENT_ID envi
-00000d30: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00000d40: 2028 7072 6566 6572 7265 6429 3e22 2c0a   (preferred)>",.
-00000d50: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00000d60: 2020 2020 2020 2020 2020 2022 636c 6965             "clie
-00000d70: 6e74 5f73 6563 7265 7422 3a20 6f73 2e65  nt_secret": os.e
-00000d80: 6e76 6972 6f6e 2e67 6574 280a 2020 2020  nviron.get(.    
-00000d90: 2020 2020 2020 2020 2020 2020 2247 4954              "GIT
-00000da0: 4855 425f 434c 4945 4e54 5f53 4543 5245  HUB_CLIENT_SECRE
-00000db0: 5422 2c0a 2020 2020 2020 2020 2020 2020  T",.            
-00000dc0: 2020 2020 223c 656e 7465 7220 636c 6965      "<enter clie
-00000dd0: 6e74 2073 6563 7265 7420 6f72 2072 656d  nt secret or rem
-00000de0: 6f76 6520 746f 2075 7365 2047 4954 4855  ove to use GITHU
-00000df0: 425f 434c 4945 4e54 5f53 4543 5245 5420  B_CLIENT_SECRET 
-00000e00: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-00000e10: 6162 6c65 2028 7072 6566 6572 7265 6429  able (preferred)
-00000e20: 3e22 2c0a 2020 2020 2020 2020 2020 2020  >",.            
-00000e30: 292c 0a20 2020 2020 2020 207d 0a20 2020  ),.        }.   
-00000e40: 2065 6c69 6620 6175 7468 5f70 726f 7669   elif auth_provi
-00000e50: 6465 7220 3d3d 2041 7574 6865 6e74 6963  der == Authentic
-00000e60: 6174 696f 6e45 6e75 6d2e 6175 7468 303a  ationEnum.auth0:
-00000e70: 0a20 2020 2020 2020 2069 6620 6175 7468  .        if auth
-00000e80: 5f61 7574 6f5f 7072 6f76 6973 696f 6e3a  _auto_provision:
-00000e90: 0a20 2020 2020 2020 2020 2020 2061 7574  .            aut
-00000ea0: 6830 5f63 6f6e 6669 6720 3d20 6372 6561  h0_config = crea
-00000eb0: 7465 5f63 6c69 656e 7428 636f 6e66 6967  te_client(config
-00000ec0: 2e64 6f6d 6169 6e2c 2063 6f6e 6669 672e  .domain, config.
-00000ed0: 7072 6f6a 6563 745f 6e61 6d65 290a 2020  project_name).  
-00000ee0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-00000ef0: 5b22 7365 6375 7269 7479 225d 5b22 6175  ["security"]["au
-00000f00: 7468 656e 7469 6361 7469 6f6e 225d 5b22  thentication"]["
-00000f10: 636f 6e66 6967 225d 203d 2061 7574 6830  config"] = auth0
-00000f20: 5f63 6f6e 6669 670a 2020 2020 2020 2020  _config.        
-00000f30: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00000f40: 2020 636f 6e66 6967 5b22 7365 6375 7269    config["securi
-00000f50: 7479 225d 5b22 6175 7468 656e 7469 6361  ty"]["authentica
-00000f60: 7469 6f6e 225d 5b22 636f 6e66 6967 225d  tion"]["config"]
-00000f70: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-00000f80: 2020 2020 2022 636c 6965 6e74 5f69 6422       "client_id"
-00000f90: 3a20 6f73 2e65 6e76 6972 6f6e 2e67 6574  : os.environ.get
-00000fa0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00000fb0: 2020 2020 2020 2241 5554 4830 5f43 4c49        "AUTH0_CLI
-00000fc0: 454e 545f 4944 222c 0a20 2020 2020 2020  ENT_ID",.       
-00000fd0: 2020 2020 2020 2020 2020 2020 2022 3c65               "<e
-00000fe0: 6e74 6572 2063 6c69 656e 7420 6964 206f  nter client id o
-00000ff0: 7220 7265 6d6f 7665 2074 6f20 7573 6520  r remove to use 
-00001000: 4155 5448 305f 434c 4945 4e54 5f49 4420  AUTH0_CLIENT_ID 
-00001010: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-00001020: 6162 6c65 2028 7072 6566 6572 7265 6429  able (preferred)
-00001030: 3e22 2c0a 2020 2020 2020 2020 2020 2020  >",.            
-00001040: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-00001050: 2020 2020 2020 2022 636c 6965 6e74 5f73         "client_s
-00001060: 6563 7265 7422 3a20 6f73 2e65 6e76 6972  ecret": os.envir
-00001070: 6f6e 2e67 6574 280a 2020 2020 2020 2020  on.get(.        
-00001080: 2020 2020 2020 2020 2020 2020 2241 5554              "AUT
-00001090: 4830 5f43 4c49 454e 545f 5345 4352 4554  H0_CLIENT_SECRET
-000010a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000010b0: 2020 2020 2020 2022 3c65 6e74 6572 2063         "<enter c
-000010c0: 6c69 656e 7420 7365 6372 6574 206f 7220  lient secret or 
-000010d0: 7265 6d6f 7665 2074 6f20 7573 6520 4155  remove to use AU
-000010e0: 5448 305f 434c 4945 4e54 5f53 4543 5245  TH0_CLIENT_SECRE
-000010f0: 5420 656e 7669 726f 6e6d 656e 7420 7661  T environment va
-00001100: 7269 6162 6c65 2028 7072 6566 6572 7265  riable (preferre
-00001110: 6429 3e22 2c0a 2020 2020 2020 2020 2020  d)>",.          
-00001120: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-00001130: 2020 2020 2020 2020 2022 6175 7468 305f           "auth0_
-00001140: 7375 6264 6f6d 6169 6e22 3a20 6f73 2e65  subdomain": os.e
-00001150: 6e76 6972 6f6e 2e67 6574 280a 2020 2020  nviron.get(.    
-00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001170: 2241 5554 4830 5f44 4f4d 4149 4e22 2c0a  "AUTH0_DOMAIN",.
-00001180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001190: 2020 2020 223c 656e 7465 7220 7375 6264      "<enter subd
-000011a0: 6f6d 6169 6e20 2877 6974 686f 7574 202e  omain (without .
-000011b0: 6175 7468 302e 636f 6d29 206f 7220 7265  auth0.com) or re
-000011c0: 6d6f 7665 2074 6f20 7573 6520 4155 5448  move to use AUTH
-000011d0: 305f 444f 4d41 494e 2065 6e76 6972 6f6e  0_DOMAIN environ
-000011e0: 6d65 6e74 2076 6172 6961 626c 653e 222c  ment variable>",
-000011f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001200: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00001210: 7d0a 0a20 2020 2069 6620 636c 6f75 645f  }..    if cloud_
-00001220: 7072 6f76 6964 6572 203d 3d20 5072 6f76  provider == Prov
-00001230: 6964 6572 456e 756d 2e64 6f3a 0a20 2020  iderEnum.do:.   
-00001240: 2020 2020 2064 6f5f 7265 6769 6f6e 203d       do_region =
-00001250: 2072 6567 696f 6e20 6f72 2063 6f6e 7374   region or const
-00001260: 616e 7473 2e44 4f5f 4445 4641 554c 545f  ants.DO_DEFAULT_
-00001270: 5245 4749 4f4e 0a20 2020 2020 2020 2064  REGION.        d
-00001280: 6f5f 6b75 6265 726e 6574 6573 5f76 6572  o_kubernetes_ver
-00001290: 7369 6f6e 7320 3d20 6b75 6265 726e 6574  sions = kubernet
-000012a0: 6573 5f76 6572 7369 6f6e 206f 7220 6765  es_version or ge
-000012b0: 745f 6c61 7465 7374 5f6b 7562 6572 6e65  t_latest_kuberne
-000012c0: 7465 735f 7665 7273 696f 6e28 0a20 2020  tes_version(.   
-000012d0: 2020 2020 2020 2020 2064 6967 6974 616c           digital
-000012e0: 5f6f 6365 616e 2e6b 7562 6572 6e65 7465  _ocean.kubernete
-000012f0: 735f 7665 7273 696f 6e73 2864 6f5f 7265  s_versions(do_re
-00001300: 6769 6f6e 290a 2020 2020 2020 2020 290a  gion).        ).
-00001310: 2020 2020 2020 2020 636f 6e66 6967 5b22          config["
-00001320: 6469 6769 7461 6c5f 6f63 6561 6e22 5d20  digital_ocean"] 
-00001330: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00001340: 226b 7562 6572 6e65 7465 735f 7665 7273  "kubernetes_vers
-00001350: 696f 6e22 3a20 646f 5f6b 7562 6572 6e65  ion": do_kuberne
-00001360: 7465 735f 7665 7273 696f 6e73 2c0a 2020  tes_versions,.  
-00001370: 2020 2020 2020 2020 2020 2272 6567 696f            "regio
-00001380: 6e22 3a20 646f 5f72 6567 696f 6e2c 0a20  n": do_region,. 
-00001390: 2020 2020 2020 2020 2020 2022 6e6f 6465             "node
-000013a0: 5f67 726f 7570 7322 3a20 5f6e 6f64 655f  _groups": _node_
-000013b0: 6772 6f75 7073 5f74 6f5f 6469 6374 2844  groups_to_dict(D
-000013c0: 4546 4155 4c54 5f44 4f5f 4e4f 4445 5f47  EFAULT_DO_NODE_G
-000013d0: 524f 5550 5329 2c0a 2020 2020 2020 2020  ROUPS),.        
-000013e0: 7d0a 0a20 2020 2020 2020 2063 6f6e 6669  }..        confi
-000013f0: 675b 2274 6865 6d65 225d 5b22 6a75 7079  g["theme"]["jupy
-00001400: 7465 7268 7562 225d 5b0a 2020 2020 2020  terhub"][.      
-00001410: 2020 2020 2020 2268 7562 5f73 7562 7469        "hub_subti
-00001420: 746c 6522 0a20 2020 2020 2020 205d 203d  tle".        ] =
-00001430: 2066 227b 5745 4c43 4f4d 455f 4845 4144   f"{WELCOME_HEAD
-00001440: 4552 5f54 4558 547d 206f 6e20 4469 6769  ER_TEXT} on Digi
-00001450: 7461 6c20 4f63 6561 6e22 0a0a 2020 2020  tal Ocean"..    
-00001460: 656c 6966 2063 6c6f 7564 5f70 726f 7669  elif cloud_provi
-00001470: 6465 7220 3d3d 2050 726f 7669 6465 7245  der == ProviderE
-00001480: 6e75 6d2e 6763 703a 0a20 2020 2020 2020  num.gcp:.       
-00001490: 2067 6370 5f72 6567 696f 6e20 3d20 7265   gcp_region = re
-000014a0: 6769 6f6e 206f 7220 636f 6e73 7461 6e74  gion or constant
-000014b0: 732e 4743 505f 4445 4641 554c 545f 5245  s.GCP_DEFAULT_RE
-000014c0: 4749 4f4e 0a20 2020 2020 2020 2067 6370  GION.        gcp
-000014d0: 5f6b 7562 6572 6e65 7465 735f 7665 7273  _kubernetes_vers
-000014e0: 696f 6e20 3d20 6b75 6265 726e 6574 6573  ion = kubernetes
-000014f0: 5f76 6572 7369 6f6e 206f 7220 6765 745f  _version or get_
-00001500: 6c61 7465 7374 5f6b 7562 6572 6e65 7465  latest_kubernete
-00001510: 735f 7665 7273 696f 6e28 0a20 2020 2020  s_version(.     
-00001520: 2020 2020 2020 2067 6f6f 676c 655f 636c         google_cl
-00001530: 6f75 642e 6b75 6265 726e 6574 6573 5f76  oud.kubernetes_v
-00001540: 6572 7369 6f6e 7328 6763 705f 7265 6769  ersions(gcp_regi
-00001550: 6f6e 290a 2020 2020 2020 2020 290a 2020  on).        ).  
-00001560: 2020 2020 2020 636f 6e66 6967 5b22 676f        config["go
-00001570: 6f67 6c65 5f63 6c6f 7564 5f70 6c61 7466  ogle_cloud_platf
-00001580: 6f72 6d22 5d20 3d20 7b0a 2020 2020 2020  orm"] = {.      
-00001590: 2020 2020 2020 226b 7562 6572 6e65 7465        "kubernete
-000015a0: 735f 7665 7273 696f 6e22 3a20 6763 705f  s_version": gcp_
-000015b0: 6b75 6265 726e 6574 6573 5f76 6572 7369  kubernetes_versi
-000015c0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-000015d0: 2272 6567 696f 6e22 3a20 6763 705f 7265  "region": gcp_re
-000015e0: 6769 6f6e 2c0a 2020 2020 2020 2020 2020  gion,.          
-000015f0: 2020 226e 6f64 655f 6772 6f75 7073 223a    "node_groups":
-00001600: 205f 6e6f 6465 5f67 726f 7570 735f 746f   _node_groups_to
-00001610: 5f64 6963 7428 4445 4641 554c 545f 4743  _dict(DEFAULT_GC
-00001620: 505f 4e4f 4445 5f47 524f 5550 5329 2c0a  P_NODE_GROUPS),.
-00001630: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00001640: 2020 2063 6f6e 6669 675b 2274 6865 6d65     config["theme
-00001650: 225d 5b22 6a75 7079 7465 7268 7562 225d  "]["jupyterhub"]
-00001660: 5b0a 2020 2020 2020 2020 2020 2020 2268  [.            "h
-00001670: 7562 5f73 7562 7469 746c 6522 0a20 2020  ub_subtitle".   
-00001680: 2020 2020 205d 203d 2066 227b 5745 4c43       ] = f"{WELC
-00001690: 4f4d 455f 4845 4144 4552 5f54 4558 547d  OME_HEADER_TEXT}
-000016a0: 206f 6e20 476f 6f67 6c65 2043 6c6f 7564   on Google Cloud
-000016b0: 2050 6c61 7466 6f72 6d22 0a20 2020 2020   Platform".     
-000016c0: 2020 2069 6620 2250 524f 4a45 4354 5f49     if "PROJECT_I
-000016d0: 4422 2069 6e20 6f73 2e65 6e76 6972 6f6e  D" in os.environ
-000016e0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-000016f0: 6e66 6967 5b22 676f 6f67 6c65 5f63 6c6f  nfig["google_clo
-00001700: 7564 5f70 6c61 7466 6f72 6d22 5d5b 2270  ud_platform"]["p
-00001710: 726f 6a65 6374 225d 203d 206f 732e 656e  roject"] = os.en
-00001720: 7669 726f 6e5b 2250 524f 4a45 4354 5f49  viron["PROJECT_I
-00001730: 4422 5d0a 2020 2020 2020 2020 656c 6966  D"].        elif
-00001740: 206e 6f74 2064 6973 6162 6c65 5f70 726f   not disable_pro
-00001750: 6d70 743a 0a20 2020 2020 2020 2020 2020  mpt:.           
-00001760: 2063 6f6e 6669 675b 2267 6f6f 676c 655f   config["google_
-00001770: 636c 6f75 645f 706c 6174 666f 726d 225d  cloud_platform"]
-00001780: 5b22 7072 6f6a 6563 7422 5d20 3d20 696e  ["project"] = in
-00001790: 7075 7428 0a20 2020 2020 2020 2020 2020  put(.           
-000017a0: 2020 2020 2022 456e 7465 7220 476f 6f67       "Enter Goog
-000017b0: 6c65 2043 6c6f 7564 2050 6c61 7466 6f72  le Cloud Platfor
-000017c0: 6d20 5072 6f6a 6563 7420 4944 3a20 220a  m Project ID: ".
-000017d0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-000017e0: 2020 2065 6c69 6620 636c 6f75 645f 7072     elif cloud_pr
-000017f0: 6f76 6964 6572 203d 3d20 5072 6f76 6964  ovider == Provid
-00001800: 6572 456e 756d 2e61 7a75 7265 3a0a 2020  erEnum.azure:.  
-00001810: 2020 2020 2020 617a 7572 655f 7265 6769        azure_regi
-00001820: 6f6e 203d 2072 6567 696f 6e20 6f72 2063  on = region or c
-00001830: 6f6e 7374 616e 7473 2e41 5a55 5245 5f44  onstants.AZURE_D
-00001840: 4546 4155 4c54 5f52 4547 494f 4e0a 2020  EFAULT_REGION.  
-00001850: 2020 2020 2020 617a 7572 655f 6b75 6265        azure_kube
-00001860: 726e 6574 6573 5f76 6572 7369 6f6e 203d  rnetes_version =
-00001870: 206b 7562 6572 6e65 7465 735f 7665 7273   kubernetes_vers
-00001880: 696f 6e20 6f72 2067 6574 5f6c 6174 6573  ion or get_lates
-00001890: 745f 6b75 6265 726e 6574 6573 5f76 6572  t_kubernetes_ver
-000018a0: 7369 6f6e 280a 2020 2020 2020 2020 2020  sion(.          
-000018b0: 2020 617a 7572 655f 636c 6f75 642e 6b75    azure_cloud.ku
-000018c0: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
-000018d0: 7328 617a 7572 655f 7265 6769 6f6e 290a  s(azure_region).
-000018e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000018f0: 2020 636f 6e66 6967 5b22 617a 7572 6522    config["azure"
-00001900: 5d20 3d20 7b0a 2020 2020 2020 2020 2020  ] = {.          
-00001910: 2020 226b 7562 6572 6e65 7465 735f 7665    "kubernetes_ve
-00001920: 7273 696f 6e22 3a20 617a 7572 655f 6b75  rsion": azure_ku
-00001930: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
-00001940: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
-00001950: 6567 696f 6e22 3a20 617a 7572 655f 7265  egion": azure_re
-00001960: 6769 6f6e 2c0a 2020 2020 2020 2020 2020  gion,.          
-00001970: 2020 2273 746f 7261 6765 5f61 6363 6f75    "storage_accou
-00001980: 6e74 5f70 6f73 7466 6978 223a 2072 616e  nt_postfix": ran
-00001990: 646f 6d5f 7365 6375 7265 5f73 7472 696e  dom_secure_strin
-000019a0: 6728 6c65 6e67 7468 3d34 292c 0a20 2020  g(length=4),.   
-000019b0: 2020 2020 2020 2020 2022 6e6f 6465 5f67           "node_g
-000019c0: 726f 7570 7322 3a20 5f6e 6f64 655f 6772  roups": _node_gr
-000019d0: 6f75 7073 5f74 6f5f 6469 6374 2844 4546  oups_to_dict(DEF
-000019e0: 4155 4c54 5f41 5a55 5245 5f4e 4f44 455f  AULT_AZURE_NODE_
-000019f0: 4752 4f55 5053 292c 0a20 2020 2020 2020  GROUPS),.       
-00001a00: 207d 0a0a 2020 2020 2020 2020 636f 6e66   }..        conf
-00001a10: 6967 5b22 7468 656d 6522 5d5b 226a 7570  ig["theme"]["jup
-00001a20: 7974 6572 6875 6222 5d5b 0a20 2020 2020  yterhub"][.     
-00001a30: 2020 2020 2020 2022 6875 625f 7375 6274         "hub_subt
-00001a40: 6974 6c65 220a 2020 2020 2020 2020 5d20  itle".        ] 
-00001a50: 3d20 6622 7b57 454c 434f 4d45 5f48 4541  = f"{WELCOME_HEA
-00001a60: 4445 525f 5445 5854 7d20 6f6e 2041 7a75  DER_TEXT} on Azu
-00001a70: 7265 220a 0a20 2020 2065 6c69 6620 636c  re"..    elif cl
-00001a80: 6f75 645f 7072 6f76 6964 6572 203d 3d20  oud_provider == 
-00001a90: 5072 6f76 6964 6572 456e 756d 2e61 7773  ProviderEnum.aws
-00001aa0: 3a0a 2020 2020 2020 2020 6177 735f 7265  :.        aws_re
-00001ab0: 6769 6f6e 203d 2028 0a20 2020 2020 2020  gion = (.       
-00001ac0: 2020 2020 2072 6567 696f 6e0a 2020 2020       region.    
-00001ad0: 2020 2020 2020 2020 6f72 206f 732e 656e          or os.en
-00001ae0: 7669 726f 6e2e 6765 7428 2241 5753 5f44  viron.get("AWS_D
-00001af0: 4546 4155 4c54 5f52 4547 494f 4e22 290a  EFAULT_REGION").
-00001b00: 2020 2020 2020 2020 2020 2020 6f72 2063              or c
-00001b10: 6f6e 7374 616e 7473 2e41 5753 5f44 4546  onstants.AWS_DEF
-00001b20: 4155 4c54 5f52 4547 494f 4e0a 2020 2020  AULT_REGION.    
-00001b30: 2020 2020 290a 2020 2020 2020 2020 6177      ).        aw
-00001b40: 735f 6b75 6265 726e 6574 6573 5f76 6572  s_kubernetes_ver
-00001b50: 7369 6f6e 203d 206b 7562 6572 6e65 7465  sion = kubernete
-00001b60: 735f 7665 7273 696f 6e20 6f72 2067 6574  s_version or get
-00001b70: 5f6c 6174 6573 745f 6b75 6265 726e 6574  _latest_kubernet
-00001b80: 6573 5f76 6572 7369 6f6e 280a 2020 2020  es_version(.    
-00001b90: 2020 2020 2020 2020 616d 617a 6f6e 5f77          amazon_w
-00001ba0: 6562 5f73 6572 7669 6365 732e 6b75 6265  eb_services.kube
-00001bb0: 726e 6574 6573 5f76 6572 7369 6f6e 7328  rnetes_versions(
-00001bc0: 6177 735f 7265 6769 6f6e 290a 2020 2020  aws_region).    
-00001bd0: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
-00001be0: 6e66 6967 5b22 616d 617a 6f6e 5f77 6562  nfig["amazon_web
-00001bf0: 5f73 6572 7669 6365 7322 5d20 3d20 7b0a  _services"] = {.
-00001c00: 2020 2020 2020 2020 2020 2020 226b 7562              "kub
-00001c10: 6572 6e65 7465 735f 7665 7273 696f 6e22  ernetes_version"
-00001c20: 3a20 6177 735f 6b75 6265 726e 6574 6573  : aws_kubernetes
-00001c30: 5f76 6572 7369 6f6e 2c0a 2020 2020 2020  _version,.      
-00001c40: 2020 2020 2020 2272 6567 696f 6e22 3a20        "region": 
-00001c50: 6177 735f 7265 6769 6f6e 2c0a 2020 2020  aws_region,.    
-00001c60: 2020 2020 2020 2020 226e 6f64 655f 6772          "node_gr
-00001c70: 6f75 7073 223a 205f 6e6f 6465 5f67 726f  oups": _node_gro
-00001c80: 7570 735f 746f 5f64 6963 7428 4445 4641  ups_to_dict(DEFA
-00001c90: 554c 545f 4157 535f 4e4f 4445 5f47 524f  ULT_AWS_NODE_GRO
-00001ca0: 5550 5329 2c0a 2020 2020 2020 2020 7d0a  UPS),.        }.
-00001cb0: 2020 2020 2020 2020 636f 6e66 6967 5b22          config["
-00001cc0: 7468 656d 6522 5d5b 226a 7570 7974 6572  theme"]["jupyter
-00001cd0: 6875 6222 5d5b 0a20 2020 2020 2020 2020  hub"][.         
-00001ce0: 2020 2022 6875 625f 7375 6274 6974 6c65     "hub_subtitle
-00001cf0: 220a 2020 2020 2020 2020 5d20 3d20 6622  ".        ] = f"
-00001d00: 7b57 454c 434f 4d45 5f48 4541 4445 525f  {WELCOME_HEADER_
-00001d10: 5445 5854 7d20 6f6e 2041 6d61 7a6f 6e20  TEXT} on Amazon 
-00001d20: 5765 6220 5365 7276 6963 6573 220a 0a20  Web Services".. 
-00001d30: 2020 2065 6c69 6620 636c 6f75 645f 7072     elif cloud_pr
-00001d40: 6f76 6964 6572 203d 3d20 5072 6f76 6964  ovider == Provid
-00001d50: 6572 456e 756d 2e65 7869 7374 696e 673a  erEnum.existing:
-00001d60: 0a20 2020 2020 2020 2063 6f6e 6669 675b  .        config[
-00001d70: 2274 6865 6d65 225d 5b22 6a75 7079 7465  "theme"]["jupyte
-00001d80: 7268 7562 225d 5b22 6875 625f 7375 6274  rhub"]["hub_subt
-00001d90: 6974 6c65 225d 203d 2057 454c 434f 4d45  itle"] = WELCOME
-00001da0: 5f48 4541 4445 525f 5445 5854 0a0a 2020  _HEADER_TEXT..  
-00001db0: 2020 656c 6966 2063 6c6f 7564 5f70 726f    elif cloud_pro
-00001dc0: 7669 6465 7220 3d3d 2050 726f 7669 6465  vider == Provide
-00001dd0: 7245 6e75 6d2e 6c6f 6361 6c3a 0a20 2020  rEnum.local:.   
-00001de0: 2020 2020 2063 6f6e 6669 675b 2274 6865       config["the
-00001df0: 6d65 225d 5b22 6a75 7079 7465 7268 7562  me"]["jupyterhub
-00001e00: 225d 5b22 6875 625f 7375 6274 6974 6c65  "]["hub_subtitle
-00001e10: 225d 203d 2057 454c 434f 4d45 5f48 4541  "] = WELCOME_HEA
-00001e20: 4445 525f 5445 5854 0a0a 2020 2020 6966  DER_TEXT..    if
-00001e30: 2073 736c 5f63 6572 745f 656d 6169 6c3a   ssl_cert_email:
-00001e40: 0a20 2020 2020 2020 2063 6f6e 6669 675b  .        config[
-00001e50: 2263 6572 7469 6669 6361 7465 225d 203d  "certificate"] =
-00001e60: 207b 2274 7970 6522 3a20 4365 7274 6966   {"type": Certif
-00001e70: 6963 6174 6545 6e75 6d2e 6c65 7473 656e  icateEnum.letsen
-00001e80: 6372 7970 742e 7661 6c75 657d 0a20 2020  crypt.value}.   
-00001e90: 2020 2020 2063 6f6e 6669 675b 2263 6572       config["cer
-00001ea0: 7469 6669 6361 7465 225d 5b22 6163 6d65  tificate"]["acme
-00001eb0: 5f65 6d61 696c 225d 203d 2073 736c 5f63  _email"] = ssl_c
-00001ec0: 6572 745f 656d 6169 6c0a 0a20 2020 2023  ert_email..    #
-00001ed0: 2076 616c 6964 6174 6520 636f 6e66 6967   validate config
-00001ee0: 7572 6174 696f 6e20 616e 6420 636f 6e76  uration and conv
-00001ef0: 6572 7420 746f 206d 6f64 656c 0a20 2020  ert to model.   
-00001f00: 2066 726f 6d20 6e65 6261 7269 2e70 6c75   from nebari.plu
-00001f10: 6769 6e73 2069 6d70 6f72 7420 6e65 6261  gins import neba
-00001f20: 7269 5f70 6c75 6769 6e5f 6d61 6e61 6765  ri_plugin_manage
-00001f30: 720a 0a20 2020 2074 7279 3a0a 2020 2020  r..    try:.    
-00001f40: 2020 2020 636f 6e66 6967 5f6d 6f64 656c      config_model
-00001f50: 203d 206e 6562 6172 695f 706c 7567 696e   = nebari_plugin
-00001f60: 5f6d 616e 6167 6572 2e63 6f6e 6669 675f  _manager.config_
-00001f70: 7363 6865 6d61 2e70 6172 7365 5f6f 626a  schema.parse_obj
-00001f80: 2863 6f6e 6669 6729 0a20 2020 2065 7863  (config).    exc
-00001f90: 6570 7420 7079 6461 6e74 6963 2e56 616c  ept pydantic.Val
-00001fa0: 6964 6174 696f 6e45 7272 6f72 2061 7320  idationError as 
-00001fb0: 653a 0a20 2020 2020 2020 2070 7269 6e74  e:.        print
-00001fc0: 2873 7472 2865 2929 0a0a 2020 2020 6966  (str(e))..    if
-00001fd0: 2072 6570 6f73 6974 6f72 795f 6175 746f   repository_auto
-00001fe0: 5f70 726f 7669 7369 6f6e 3a0a 2020 2020  _provision:.    
-00001ff0: 2020 2020 6d61 7463 6820 3d20 7265 2e73      match = re.s
-00002000: 6561 7263 6828 6769 7468 7562 5f75 726c  earch(github_url
-00002010: 5f72 6567 6578 2c20 7265 706f 7369 746f  _regex, reposito
-00002020: 7279 290a 2020 2020 2020 2020 6966 206d  ry).        if m
-00002030: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
-00002040: 2020 6769 745f 7265 706f 7369 746f 7279    git_repository
-00002050: 203d 2067 6974 6875 625f 6175 746f 5f70   = github_auto_p
-00002060: 726f 7669 7369 6f6e 280a 2020 2020 2020  rovision(.      
-00002070: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-00002080: 5f6d 6f64 656c 2c20 6d61 7463 682e 6772  _model, match.gr
-00002090: 6f75 7028 3229 2c20 6d61 7463 682e 6772  oup(2), match.gr
-000020a0: 6f75 7028 3329 0a20 2020 2020 2020 2020  oup(3).         
-000020b0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000020c0: 2067 6974 5f72 6570 6f73 6974 6f72 795f   git_repository_
-000020d0: 696e 6974 6961 6c69 7a65 2867 6974 5f72  initialize(git_r
-000020e0: 6570 6f73 6974 6f72 7929 0a20 2020 2020  epository).     
-000020f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00002100: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00002110: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00002120: 2020 2020 2020 2066 2252 6570 6f73 6974         f"Reposit
-00002130: 6f72 7920 746f 2062 6520 6175 746f 2d70  ory to be auto-p
-00002140: 726f 7669 7369 6f6e 6564 2069 7320 6e6f  rovisioned is no
-00002150: 7420 7468 6520 6675 6c6c 2055 524c 206f  t the full URL o
-00002160: 6620 6120 4769 7448 7562 2072 6570 6f3a  f a GitHub repo:
-00002170: 207b 7265 706f 7369 746f 7279 7d22 0a20   {repository}". 
-00002180: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00002190: 2020 7265 7475 726e 2063 6f6e 6669 670a    return config.
-000021a0: 0a0a 6465 6620 6769 7468 7562 5f61 7574  ..def github_aut
-000021b0: 6f5f 7072 6f76 6973 696f 6e28 636f 6e66  o_provision(conf
-000021c0: 6967 3a20 7079 6461 6e74 6963 2e42 6173  ig: pydantic.Bas
-000021d0: 654d 6f64 656c 2c20 6f77 6e65 723a 2073  eModel, owner: s
-000021e0: 7472 2c20 7265 706f 3a20 7374 7229 3a0a  tr, repo: str):.
-000021f0: 2020 2020 616c 7265 6164 795f 6578 6973      already_exis
-00002200: 7473 203d 2054 7275 650a 2020 2020 7472  ts = True.    tr
-00002210: 793a 0a20 2020 2020 2020 2067 6974 6875  y:.        githu
-00002220: 622e 6765 745f 7265 706f 7369 746f 7279  b.get_repository
-00002230: 286f 776e 6572 2c20 7265 706f 290a 2020  (owner, repo).  
-00002240: 2020 6578 6365 7074 2072 6571 7565 7374    except request
-00002250: 732e 6578 6365 7074 696f 6e73 2e48 5454  s.exceptions.HTT
-00002260: 5045 7272 6f72 3a0a 2020 2020 2020 2020  PError:.        
-00002270: 2320 7265 706f 206e 6f74 2066 6f75 6e64  # repo not found
-00002280: 0a20 2020 2020 2020 2061 6c72 6561 6479  .        already
-00002290: 5f65 7869 7374 7320 3d20 4661 6c73 650a  _exists = False.
-000022a0: 0a20 2020 2069 6620 6e6f 7420 616c 7265  .    if not alre
-000022b0: 6164 795f 6578 6973 7473 3a0a 2020 2020  ady_exists:.    
-000022c0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-000022d0: 2020 2020 2067 6974 6875 622e 6372 6561       github.crea
-000022e0: 7465 5f72 6570 6f73 6974 6f72 7928 0a20  te_repository(. 
-000022f0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00002300: 776e 6572 2c0a 2020 2020 2020 2020 2020  wner,.          
-00002310: 2020 2020 2020 7265 706f 2c0a 2020 2020        repo,.    
-00002320: 2020 2020 2020 2020 2020 2020 6465 7363              desc
-00002330: 7269 7074 696f 6e3d 6622 4e65 6261 7269  ription=f"Nebari
-00002340: 207b 636f 6e66 6967 2e70 726f 6a65 6374   {config.project
-00002350: 5f6e 616d 657d 2d7b 636f 6e66 6967 2e70  _name}-{config.p
-00002360: 726f 7669 6465 727d 222c 0a20 2020 2020  rovider}",.     
-00002370: 2020 2020 2020 2020 2020 2068 6f6d 6570             homep
-00002380: 6167 653d 6622 6874 7470 733a 2f2f 7b63  age=f"https://{c
-00002390: 6f6e 6669 672e 646f 6d61 696e 7d22 2c0a  onfig.domain}",.
-000023a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000023b0: 2020 2020 2020 6578 6365 7074 2072 6571        except req
-000023c0: 7565 7374 732e 6578 6365 7074 696f 6e73  uests.exceptions
-000023d0: 2e48 5454 5045 7272 6f72 2061 7320 6865  .HTTPError as he
-000023e0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000023f0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002410: 6622 556e 6162 6c65 2074 6f20 6372 6561  f"Unable to crea
-00002420: 7465 2047 6974 4875 6220 7265 706f 2068  te GitHub repo h
-00002430: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002440: 6d2f 7b6f 776e 6572 7d2f 7b72 6570 6f7d  m/{owner}/{repo}
-00002450: 202d 2065 7272 6f72 206d 6573 7361 6765   - error message
-00002460: 2066 726f 6d20 4769 7448 7562 2069 733a   from GitHub is:
-00002470: 207b 6865 7d22 0a20 2020 2020 2020 2020   {he}".         
-00002480: 2020 2029 0a20 2020 2065 6c73 653a 0a20     ).    else:. 
-00002490: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
-000024a0: 726e 696e 6728 6622 4769 7448 7562 2072  rning(f"GitHub r
-000024b0: 6570 6f20 6874 7470 733a 2f2f 6769 7468  epo https://gith
-000024c0: 7562 2e63 6f6d 2f7b 6f77 6e65 727d 2f7b  ub.com/{owner}/{
-000024d0: 7265 706f 7d20 616c 7265 6164 7920 6578  repo} already ex
-000024e0: 6973 7473 2229 0a0a 2020 2020 7472 793a  ists")..    try:
-000024f0: 0a20 2020 2020 2020 2023 2053 6563 7265  .        # Secre
-00002500: 7473 0a20 2020 2020 2020 2069 6620 636f  ts.        if co
-00002510: 6e66 6967 2e70 726f 7669 6465 7220 3d3d  nfig.provider ==
-00002520: 2050 726f 7669 6465 7245 6e75 6d2e 646f   ProviderEnum.do
-00002530: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-00002540: 7220 6e61 6d65 2069 6e20 7b0a 2020 2020  r name in {.    
-00002550: 2020 2020 2020 2020 2020 2020 2241 5753              "AWS
-00002560: 5f41 4343 4553 535f 4b45 595f 4944 222c  _ACCESS_KEY_ID",
-00002570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002580: 2022 4157 535f 5345 4352 4554 5f41 4343   "AWS_SECRET_ACC
-00002590: 4553 535f 4b45 5922 2c0a 2020 2020 2020  ESS_KEY",.      
-000025a0: 2020 2020 2020 2020 2020 2253 5041 4345            "SPACE
-000025b0: 535f 4143 4345 5353 5f4b 4559 5f49 4422  S_ACCESS_KEY_ID"
-000025c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000025d0: 2020 2253 5041 4345 535f 5345 4352 4554    "SPACES_SECRET
-000025e0: 5f41 4343 4553 535f 4b45 5922 2c0a 2020  _ACCESS_KEY",.  
-000025f0: 2020 2020 2020 2020 2020 2020 2020 2244                "D
-00002600: 4947 4954 414c 4f43 4541 4e5f 544f 4b45  IGITALOCEAN_TOKE
-00002610: 4e22 2c0a 2020 2020 2020 2020 2020 2020  N",.            
-00002620: 7d3a 0a20 2020 2020 2020 2020 2020 2020  }:.             
-00002630: 2020 2067 6974 6875 622e 7570 6461 7465     github.update
-00002640: 5f73 6563 7265 7428 6f77 6e65 722c 2072  _secret(owner, r
-00002650: 6570 6f2c 206e 616d 652c 206f 732e 656e  epo, name, os.en
-00002660: 7669 726f 6e5b 6e61 6d65 5d29 0a20 2020  viron[name]).   
-00002670: 2020 2020 2065 6c69 6620 636f 6e66 6967       elif config
-00002680: 2e70 726f 7669 6465 7220 3d3d 2050 726f  .provider == Pro
-00002690: 7669 6465 7245 6e75 6d2e 6177 733a 0a20  viderEnum.aws:. 
-000026a0: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
-000026b0: 616d 6520 696e 207b 0a20 2020 2020 2020  ame in {.       
-000026c0: 2020 2020 2020 2020 2022 4157 535f 4143           "AWS_AC
-000026d0: 4345 5353 5f4b 4559 5f49 4422 2c0a 2020  CESS_KEY_ID",.  
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2241                "A
-000026f0: 5753 5f53 4543 5245 545f 4143 4345 5353  WS_SECRET_ACCESS
-00002700: 5f4b 4559 222c 0a20 2020 2020 2020 2020  _KEY",.         
-00002710: 2020 207d 3a0a 2020 2020 2020 2020 2020     }:.          
-00002720: 2020 2020 2020 6769 7468 7562 2e75 7064        github.upd
-00002730: 6174 655f 7365 6372 6574 286f 776e 6572  ate_secret(owner
-00002740: 2c20 7265 706f 2c20 6e61 6d65 2c20 6f73  , repo, name, os
-00002750: 2e65 6e76 6972 6f6e 5b6e 616d 655d 290a  .environ[name]).
-00002760: 2020 2020 2020 2020 656c 6966 2063 6f6e          elif con
-00002770: 6669 672e 7072 6f76 6964 6572 203d 3d20  fig.provider == 
-00002780: 5072 6f76 6964 6572 456e 756d 2e67 6370  ProviderEnum.gcp
-00002790: 3a0a 2020 2020 2020 2020 2020 2020 6769  :.            gi
-000027a0: 7468 7562 2e75 7064 6174 655f 7365 6372  thub.update_secr
-000027b0: 6574 286f 776e 6572 2c20 7265 706f 2c20  et(owner, repo, 
-000027c0: 2250 524f 4a45 4354 5f49 4422 2c20 6f73  "PROJECT_ID", os
-000027d0: 2e65 6e76 6972 6f6e 5b22 5052 4f4a 4543  .environ["PROJEC
-000027e0: 545f 4944 225d 290a 2020 2020 2020 2020  T_ID"]).        
-000027f0: 2020 2020 7769 7468 206f 7065 6e28 6f73      with open(os
-00002800: 2e65 6e76 6972 6f6e 5b22 474f 4f47 4c45  .environ["GOOGLE
-00002810: 5f43 5245 4445 4e54 4941 4c53 225d 2920  _CREDENTIALS"]) 
-00002820: 6173 2066 3a0a 2020 2020 2020 2020 2020  as f:.          
-00002830: 2020 2020 2020 6769 7468 7562 2e75 7064        github.upd
-00002840: 6174 655f 7365 6372 6574 286f 776e 6572  ate_secret(owner
-00002850: 2c20 7265 706f 2c20 2247 4f4f 474c 455f  , repo, "GOOGLE_
-00002860: 4352 4544 454e 5449 414c 5322 2c20 662e  CREDENTIALS", f.
-00002870: 7265 6164 2829 290a 2020 2020 2020 2020  read()).        
-00002880: 656c 6966 2063 6f6e 6669 672e 7072 6f76  elif config.prov
-00002890: 6964 6572 203d 3d20 5072 6f76 6964 6572  ider == Provider
-000028a0: 456e 756d 2e61 7a75 7265 3a0a 2020 2020  Enum.azure:.    
-000028b0: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
-000028c0: 2069 6e20 7b0a 2020 2020 2020 2020 2020   in {.          
-000028d0: 2020 2020 2020 2241 524d 5f43 4c49 454e        "ARM_CLIEN
-000028e0: 545f 4944 222c 0a20 2020 2020 2020 2020  T_ID",.         
-000028f0: 2020 2020 2020 2022 4152 4d5f 434c 4945         "ARM_CLIE
-00002900: 4e54 5f53 4543 5245 5422 2c0a 2020 2020  NT_SECRET",.    
-00002910: 2020 2020 2020 2020 2020 2020 2241 524d              "ARM
-00002920: 5f53 5542 5343 5249 5054 494f 4e5f 4944  _SUBSCRIPTION_ID
-00002930: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002940: 2020 2022 4152 4d5f 5445 4e41 4e54 5f49     "ARM_TENANT_I
-00002950: 4422 2c0a 2020 2020 2020 2020 2020 2020  D",.            
-00002960: 7d3a 0a20 2020 2020 2020 2020 2020 2020  }:.             
-00002970: 2020 2067 6974 6875 622e 7570 6461 7465     github.update
-00002980: 5f73 6563 7265 7428 6f77 6e65 722c 2072  _secret(owner, r
-00002990: 6570 6f2c 206e 616d 652c 206f 732e 656e  epo, name, os.en
-000029a0: 7669 726f 6e5b 6e61 6d65 5d29 0a20 2020  viron[name]).   
-000029b0: 2020 2020 2067 6974 6875 622e 7570 6461       github.upda
-000029c0: 7465 5f73 6563 7265 7428 0a20 2020 2020  te_secret(.     
-000029d0: 2020 2020 2020 206f 776e 6572 2c20 7265         owner, re
-000029e0: 706f 2c20 2252 4550 4f53 4954 4f52 595f  po, "REPOSITORY_
-000029f0: 4143 4345 5353 5f54 4f4b 454e 222c 206f  ACCESS_TOKEN", o
-00002a00: 732e 656e 7669 726f 6e5b 2247 4954 4855  s.environ["GITHU
-00002a10: 425f 544f 4b45 4e22 5d0a 2020 2020 2020  B_TOKEN"].      
-00002a20: 2020 290a 2020 2020 6578 6365 7074 2072    ).    except r
-00002a30: 6571 7565 7374 732e 6578 6365 7074 696f  equests.exceptio
-00002a40: 6e73 2e48 5454 5045 7272 6f72 2061 7320  ns.HTTPError as 
-00002a50: 6865 3a0a 2020 2020 2020 2020 7261 6973  he:.        rais
-00002a60: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
-00002a70: 2020 2020 2020 2020 2020 6622 556e 6162            f"Unab
-00002a80: 6c65 2074 6f20 7365 7420 5365 6372 6574  le to set Secret
-00002a90: 7320 6f6e 2047 6974 4875 6220 7265 706f  s on GitHub repo
-00002aa0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00002ab0: 636f 6d2f 7b6f 776e 6572 7d2f 7b72 6570  com/{owner}/{rep
-00002ac0: 6f7d 202d 2065 7272 6f72 206d 6573 7361  o} - error messa
-00002ad0: 6765 2066 726f 6d20 4769 7448 7562 2069  ge from GitHub i
-00002ae0: 733a 207b 6865 7d22 0a20 2020 2020 2020  s: {he}".       
-00002af0: 2029 0a0a 2020 2020 7265 7475 726e 2066   )..    return f
-00002b00: 2267 6974 4067 6974 6875 622e 636f 6d3a  "git@github.com:
-00002b10: 7b6f 776e 6572 7d2f 7b72 6570 6f7d 2e67  {owner}/{repo}.g
-00002b20: 6974 220a 0a0a 6465 6620 6769 745f 7265  it"...def git_re
-00002b30: 706f 7369 746f 7279 5f69 6e69 7469 616c  pository_initial
-00002b40: 697a 6528 6769 745f 7265 706f 7369 746f  ize(git_reposito
-00002b50: 7279 293a 0a20 2020 2069 6620 6e6f 7420  ry):.    if not 
-00002b60: 6769 742e 6973 5f67 6974 5f72 6570 6f28  git.is_git_repo(
-00002b70: 5061 7468 2e63 7764 2829 293a 0a20 2020  Path.cwd()):.   
-00002b80: 2020 2020 2067 6974 2e69 6e69 7469 616c       git.initial
-00002b90: 697a 655f 6769 7428 5061 7468 2e63 7764  ize_git(Path.cwd
-00002ba0: 2829 290a 2020 2020 6769 742e 6164 645f  ()).    git.add_
-00002bb0: 6769 745f 7265 6d6f 7465 2867 6974 5f72  git_remote(git_r
-00002bc0: 6570 6f73 6974 6f72 792c 2070 6174 683d  epository, path=
-00002bd0: 5061 7468 2e63 7764 2829 2c20 7265 6d6f  Path.cwd(), remo
-00002be0: 7465 5f6e 616d 653d 226f 7269 6769 6e22  te_name="origin"
-00002bf0: 290a                                     ).
+00000040: 696d 706f 7274 2050 6174 680a 6672 6f6d  import Path.from
+00000050: 2074 7970 696e 6720 696d 706f 7274 2041   typing import A
+00000060: 6e79 2c20 4469 6374 0a0a 696d 706f 7274  ny, Dict..import
+00000070: 2070 7964 616e 7469 630a 696d 706f 7274   pydantic.import
+00000080: 2072 6571 7565 7374 730a 0a66 726f 6d20   requests..from 
+00000090: 5f6e 6562 6172 6920 696d 706f 7274 2063  _nebari import c
+000000a0: 6f6e 7374 616e 7473 0a66 726f 6d20 5f6e  onstants.from _n
+000000b0: 6562 6172 692e 7072 6f76 6964 6572 2069  ebari.provider i
+000000c0: 6d70 6f72 7420 6769 740a 6672 6f6d 205f  mport git.from _
+000000d0: 6e65 6261 7269 2e70 726f 7669 6465 722e  nebari.provider.
+000000e0: 6369 6364 2069 6d70 6f72 7420 6769 7468  cicd import gith
+000000f0: 7562 0a66 726f 6d20 5f6e 6562 6172 692e  ub.from _nebari.
+00000100: 7072 6f76 6964 6572 2e63 6c6f 7564 2069  provider.cloud i
+00000110: 6d70 6f72 7420 280a 2020 2020 616d 617a  mport (.    amaz
+00000120: 6f6e 5f77 6562 5f73 6572 7669 6365 732c  on_web_services,
+00000130: 0a20 2020 2061 7a75 7265 5f63 6c6f 7564  .    azure_cloud
+00000140: 2c0a 2020 2020 6469 6769 7461 6c5f 6f63  ,.    digital_oc
+00000150: 6561 6e2c 0a20 2020 2067 6f6f 676c 655f  ean,.    google_
+00000160: 636c 6f75 642c 0a29 0a66 726f 6d20 5f6e  cloud,.).from _n
+00000170: 6562 6172 692e 7072 6f76 6964 6572 2e6f  ebari.provider.o
+00000180: 6175 7468 2e61 7574 6830 2069 6d70 6f72  auth.auth0 impor
+00000190: 7420 6372 6561 7465 5f63 6c69 656e 740a  t create_client.
+000001a0: 6672 6f6d 205f 6e65 6261 7269 2e73 7461  from _nebari.sta
+000001b0: 6765 732e 626f 6f74 7374 7261 7020 696d  ges.bootstrap im
+000001c0: 706f 7274 2043 6945 6e75 6d0a 6672 6f6d  port CiEnum.from
+000001d0: 205f 6e65 6261 7269 2e73 7461 6765 732e   _nebari.stages.
+000001e0: 696e 6672 6173 7472 7563 7475 7265 2069  infrastructure i
+000001f0: 6d70 6f72 7420 280a 2020 2020 4445 4641  mport (.    DEFA
+00000200: 554c 545f 4157 535f 4e4f 4445 5f47 524f  ULT_AWS_NODE_GRO
+00000210: 5550 532c 0a20 2020 2044 4546 4155 4c54  UPS,.    DEFAULT
+00000220: 5f41 5a55 5245 5f4e 4f44 455f 4752 4f55  _AZURE_NODE_GROU
+00000230: 5053 2c0a 2020 2020 4445 4641 554c 545f  PS,.    DEFAULT_
+00000240: 444f 5f4e 4f44 455f 4752 4f55 5053 2c0a  DO_NODE_GROUPS,.
+00000250: 2020 2020 4445 4641 554c 545f 4743 505f      DEFAULT_GCP_
+00000260: 4e4f 4445 5f47 524f 5550 532c 0a20 2020  NODE_GROUPS,.   
+00000270: 206e 6f64 655f 6772 6f75 7073 5f74 6f5f   node_groups_to_
+00000280: 6469 6374 2c0a 290a 6672 6f6d 205f 6e65  dict,.).from _ne
+00000290: 6261 7269 2e73 7461 6765 732e 6b75 6265  bari.stages.kube
+000002a0: 726e 6574 6573 5f69 6e67 7265 7373 2069  rnetes_ingress i
+000002b0: 6d70 6f72 7420 4365 7274 6966 6963 6174  mport Certificat
+000002c0: 6545 6e75 6d0a 6672 6f6d 205f 6e65 6261  eEnum.from _neba
+000002d0: 7269 2e73 7461 6765 732e 6b75 6265 726e  ri.stages.kubern
+000002e0: 6574 6573 5f6b 6579 636c 6f61 6b20 696d  etes_keycloak im
+000002f0: 706f 7274 2041 7574 6865 6e74 6963 6174  port Authenticat
+00000300: 696f 6e45 6e75 6d0a 6672 6f6d 205f 6e65  ionEnum.from _ne
+00000310: 6261 7269 2e73 7461 6765 732e 7465 7272  bari.stages.terr
+00000320: 6166 6f72 6d5f 7374 6174 6520 696d 706f  aform_state impo
+00000330: 7274 2054 6572 7261 666f 726d 5374 6174  rt TerraformStat
+00000340: 6545 6e75 6d0a 6672 6f6d 205f 6e65 6261  eEnum.from _neba
+00000350: 7269 2e75 7469 6c73 2069 6d70 6f72 7420  ri.utils import 
+00000360: 6765 745f 6c61 7465 7374 5f6b 7562 6572  get_latest_kuber
+00000370: 6e65 7465 735f 7665 7273 696f 6e2c 2072  netes_version, r
+00000380: 616e 646f 6d5f 7365 6375 7265 5f73 7472  andom_secure_str
+00000390: 696e 670a 6672 6f6d 205f 6e65 6261 7269  ing.from _nebari
+000003a0: 2e76 6572 7369 6f6e 2069 6d70 6f72 7420  .version import 
+000003b0: 5f5f 7665 7273 696f 6e5f 5f0a 6672 6f6d  __version__.from
+000003c0: 206e 6562 6172 692e 7363 6865 6d61 2069   nebari.schema i
+000003d0: 6d70 6f72 7420 5072 6f76 6964 6572 456e  mport ProviderEn
+000003e0: 756d 2c20 6769 7468 7562 5f75 726c 5f72  um, github_url_r
+000003f0: 6567 6578 0a0a 6c6f 6767 6572 203d 206c  egex..logger = l
+00000400: 6f67 6769 6e67 2e67 6574 4c6f 6767 6572  ogging.getLogger
+00000410: 285f 5f6e 616d 655f 5f29 0a0a 5745 4c43  (__name__)..WELC
+00000420: 4f4d 455f 4845 4144 4552 5f54 4558 5420  OME_HEADER_TEXT 
+00000430: 3d20 2259 6f75 7220 6f70 656e 2073 6f75  = "Your open sou
+00000440: 7263 6520 6461 7461 2073 6369 656e 6365  rce data science
+00000450: 2070 6c61 7466 6f72 6d2c 2068 6f73 7465   platform, hoste
+00000460: 6422 0a0a 0a64 6566 2072 656e 6465 725f  d"...def render_
+00000470: 636f 6e66 6967 280a 2020 2020 7072 6f6a  config(.    proj
+00000480: 6563 745f 6e61 6d65 3a20 7374 722c 0a20  ect_name: str,. 
+00000490: 2020 206e 6562 6172 695f 646f 6d61 696e     nebari_domain
+000004a0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000004b0: 2020 636c 6f75 645f 7072 6f76 6964 6572    cloud_provider
+000004c0: 3a20 5072 6f76 6964 6572 456e 756d 203d  : ProviderEnum =
+000004d0: 2050 726f 7669 6465 7245 6e75 6d2e 6c6f   ProviderEnum.lo
+000004e0: 6361 6c2c 0a20 2020 2063 695f 7072 6f76  cal,.    ci_prov
+000004f0: 6964 6572 3a20 4369 456e 756d 203d 2043  ider: CiEnum = C
+00000500: 6945 6e75 6d2e 6e6f 6e65 2c0a 2020 2020  iEnum.none,.    
+00000510: 7265 706f 7369 746f 7279 3a20 7374 7220  repository: str 
+00000520: 3d20 4e6f 6e65 2c0a 2020 2020 6175 7468  = None,.    auth
+00000530: 5f70 726f 7669 6465 723a 2041 7574 6865  _provider: Authe
+00000540: 6e74 6963 6174 696f 6e45 6e75 6d20 3d20  nticationEnum = 
+00000550: 4175 7468 656e 7469 6361 7469 6f6e 456e  AuthenticationEn
+00000560: 756d 2e70 6173 7377 6f72 642c 0a20 2020  um.password,.   
+00000570: 206e 616d 6573 7061 6365 3a20 7374 7220   namespace: str 
+00000580: 3d20 2264 6576 222c 0a20 2020 2072 6570  = "dev",.    rep
+00000590: 6f73 6974 6f72 795f 6175 746f 5f70 726f  ository_auto_pro
+000005a0: 7669 7369 6f6e 3a20 626f 6f6c 203d 2046  vision: bool = F
+000005b0: 616c 7365 2c0a 2020 2020 6175 7468 5f61  alse,.    auth_a
+000005c0: 7574 6f5f 7072 6f76 6973 696f 6e3a 2062  uto_provision: b
+000005d0: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+000005e0: 2074 6572 7261 666f 726d 5f73 7461 7465   terraform_state
+000005f0: 3a20 5465 7272 6166 6f72 6d53 7461 7465  : TerraformState
+00000600: 456e 756d 203d 2054 6572 7261 666f 726d  Enum = Terraform
+00000610: 5374 6174 6545 6e75 6d2e 7265 6d6f 7465  StateEnum.remote
+00000620: 2c0a 2020 2020 6b75 6265 726e 6574 6573  ,.    kubernetes
+00000630: 5f76 6572 7369 6f6e 3a20 7374 7220 3d20  _version: str = 
+00000640: 4e6f 6e65 2c0a 2020 2020 7265 6769 6f6e  None,.    region
+00000650: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00000660: 2020 6469 7361 626c 655f 7072 6f6d 7074    disable_prompt
+00000670: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+00000680: 2020 2020 7373 6c5f 6365 7274 5f65 6d61      ssl_cert_ema
+00000690: 696c 3a20 7374 7220 3d20 4e6f 6e65 2c0a  il: str = None,.
+000006a0: 2920 2d3e 2044 6963 745b 7374 722c 2041  ) -> Dict[str, A
+000006b0: 6e79 5d3a 0a20 2020 2063 6f6e 6669 6720  ny]:.    config 
+000006c0: 3d20 7b0a 2020 2020 2020 2020 2270 726f  = {.        "pro
+000006d0: 7669 6465 7222 3a20 636c 6f75 645f 7072  vider": cloud_pr
+000006e0: 6f76 6964 6572 2c0a 2020 2020 2020 2020  ovider,.        
+000006f0: 226e 616d 6573 7061 6365 223a 206e 616d  "namespace": nam
+00000700: 6573 7061 6365 2c0a 2020 2020 2020 2020  espace,.        
+00000710: 226e 6562 6172 695f 7665 7273 696f 6e22  "nebari_version"
+00000720: 3a20 5f5f 7665 7273 696f 6e5f 5f2c 0a20  : __version__,. 
+00000730: 2020 207d 0a0a 2020 2020 6966 2070 726f     }..    if pro
+00000740: 6a65 6374 5f6e 616d 6520 6973 204e 6f6e  ject_name is Non
+00000750: 6520 616e 6420 6e6f 7420 6469 7361 626c  e and not disabl
+00000760: 655f 7072 6f6d 7074 3a0a 2020 2020 2020  e_prompt:.      
+00000770: 2020 7072 6f6a 6563 745f 6e61 6d65 203d    project_name =
+00000780: 2069 6e70 7574 2822 5072 6f76 6964 6520   input("Provide 
+00000790: 7072 6f6a 6563 7420 6e61 6d65 3a20 2229  project name: ")
+000007a0: 0a20 2020 2063 6f6e 6669 675b 2270 726f  .    config["pro
+000007b0: 6a65 6374 5f6e 616d 6522 5d20 3d20 7072  ject_name"] = pr
+000007c0: 6f6a 6563 745f 6e61 6d65 0a0a 2020 2020  oject_name..    
+000007d0: 6966 206e 6562 6172 695f 646f 6d61 696e  if nebari_domain
+000007e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000007f0: 2020 2020 2020 636f 6e66 6967 5b22 646f        config["do
+00000800: 6d61 696e 225d 203d 206e 6562 6172 695f  main"] = nebari_
+00000810: 646f 6d61 696e 0a0a 2020 2020 636f 6e66  domain..    conf
+00000820: 6967 5b22 6369 5f63 6422 5d20 3d20 7b22  ig["ci_cd"] = {"
+00000830: 7479 7065 223a 2063 695f 7072 6f76 6964  type": ci_provid
+00000840: 6572 7d0a 2020 2020 636f 6e66 6967 5b22  er}.    config["
+00000850: 7465 7272 6166 6f72 6d5f 7374 6174 6522  terraform_state"
+00000860: 5d20 3d20 7b22 7479 7065 223a 2074 6572  ] = {"type": ter
+00000870: 7261 666f 726d 5f73 7461 7465 7d0a 0a20  raform_state}.. 
+00000880: 2020 2023 2053 6176 6520 6465 6661 756c     # Save defaul
+00000890: 7420 7061 7373 776f 7264 2074 6f20 6669  t password to fi
+000008a0: 6c65 0a20 2020 2064 6566 6175 6c74 5f70  le.    default_p
+000008b0: 6173 7377 6f72 645f 6669 6c65 6e61 6d65  assword_filename
+000008c0: 203d 2050 6174 6828 7465 6d70 6669 6c65   = Path(tempfile
+000008d0: 2e67 6574 7465 6d70 6469 7228 2929 202f  .gettempdir()) /
+000008e0: 2022 4e45 4241 5249 5f44 4546 4155 4c54   "NEBARI_DEFAULT
+000008f0: 5f50 4153 5357 4f52 4422 0a20 2020 2063  _PASSWORD".    c
+00000900: 6f6e 6669 675b 2273 6563 7572 6974 7922  onfig["security"
+00000910: 5d20 3d20 7b0a 2020 2020 2020 2020 226b  ] = {.        "k
+00000920: 6579 636c 6f61 6b22 3a20 7b22 696e 6974  eycloak": {"init
+00000930: 6961 6c5f 726f 6f74 5f70 6173 7377 6f72  ial_root_passwor
+00000940: 6422 3a20 7261 6e64 6f6d 5f73 6563 7572  d": random_secur
+00000950: 655f 7374 7269 6e67 286c 656e 6774 683d  e_string(length=
+00000960: 3332 297d 0a20 2020 207d 0a20 2020 2077  32)}.    }.    w
+00000970: 6974 6820 6465 6661 756c 745f 7061 7373  ith default_pass
+00000980: 776f 7264 5f66 696c 656e 616d 652e 6f70  word_filename.op
+00000990: 656e 2822 7722 2920 6173 2066 3a0a 2020  en("w") as f:.  
+000009a0: 2020 2020 2020 662e 7772 6974 6528 636f        f.write(co
+000009b0: 6e66 6967 5b22 7365 6375 7269 7479 225d  nfig["security"]
+000009c0: 5b22 6b65 7963 6c6f 616b 225d 5b22 696e  ["keycloak"]["in
+000009d0: 6974 6961 6c5f 726f 6f74 5f70 6173 7377  itial_root_passw
+000009e0: 6f72 6422 5d29 0a20 2020 2064 6566 6175  ord"]).    defau
+000009f0: 6c74 5f70 6173 7377 6f72 645f 6669 6c65  lt_password_file
+00000a00: 6e61 6d65 2e63 686d 6f64 2830 6f37 3030  name.chmod(0o700
+00000a10: 290a 0a20 2020 2063 6f6e 6669 675b 2274  )..    config["t
+00000a20: 6865 6d65 225d 203d 207b 226a 7570 7974  heme"] = {"jupyt
+00000a30: 6572 6875 6222 3a20 7b22 6875 625f 7469  erhub": {"hub_ti
+00000a40: 746c 6522 3a20 6622 4e65 6261 7269 202d  tle": f"Nebari -
+00000a50: 207b 2070 726f 6a65 6374 5f6e 616d 6520   { project_name 
+00000a60: 7d22 7d7d 0a20 2020 2063 6f6e 6669 675b  }"}}.    config[
+00000a70: 2274 6865 6d65 225d 5b22 6a75 7079 7465  "theme"]["jupyte
+00000a80: 7268 7562 225d 5b0a 2020 2020 2020 2020  rhub"][.        
+00000a90: 2277 656c 636f 6d65 220a 2020 2020 5d20  "welcome".    ] 
+00000aa0: 3d20 2222 2257 656c 636f 6d65 2120 4c65  = """Welcome! Le
+00000ab0: 6172 6e20 6162 6f75 7420 4e65 6261 7269  arn about Nebari
+00000ac0: 2773 2066 6561 7475 7265 7320 616e 6420  's features and 
+00000ad0: 636f 6e66 6967 7572 6174 696f 6e73 2069  configurations i
+00000ae0: 6e20 3c61 2068 7265 663d 2268 7474 7073  n <a href="https
+00000af0: 3a2f 2f77 7777 2e6e 6562 6172 692e 6465  ://www.nebari.de
+00000b00: 762f 646f 6373 2f77 656c 636f 6d65 223e  v/docs/welcome">
+00000b10: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
+00000b20: 6e3c 2f61 3e2e 2049 6620 796f 7520 6861  n</a>. If you ha
+00000b30: 7665 2061 6e79 2071 7565 7374 696f 6e73  ve any questions
+00000b40: 206f 7220 6665 6564 6261 636b 2c20 7265   or feedback, re
+00000b50: 6163 6820 7468 6520 7465 616d 206f 6e20  ach the team on 
+00000b60: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000b70: 2f77 7777 2e6e 6562 6172 692e 6465 762f  /www.nebari.dev/
+00000b80: 646f 6373 2f63 6f6d 6d75 6e69 7479 2367  docs/community#g
+00000b90: 6574 7469 6e67 2d73 7570 706f 7274 223e  etting-support">
+00000ba0: 4e65 6261 7269 2773 2073 7570 706f 7274  Nebari's support
+00000bb0: 2066 6f72 756d 733c 2f61 3e2e 2222 220a   forums</a>.""".
+00000bc0: 0a20 2020 2063 6f6e 6669 675b 2273 6563  .    config["sec
+00000bd0: 7572 6974 7922 5d5b 2261 7574 6865 6e74  urity"]["authent
+00000be0: 6963 6174 696f 6e22 5d20 3d20 7b22 7479  ication"] = {"ty
+00000bf0: 7065 223a 2061 7574 685f 7072 6f76 6964  pe": auth_provid
+00000c00: 6572 7d0a 0a20 2020 2069 6620 6175 7468  er}..    if auth
+00000c10: 5f70 726f 7669 6465 7220 3d3d 2041 7574  _provider == Aut
+00000c20: 6865 6e74 6963 6174 696f 6e45 6e75 6d2e  henticationEnum.
+00000c30: 6769 7468 7562 3a0a 2020 2020 2020 2020  github:.        
+00000c40: 636f 6e66 6967 5b22 7365 6375 7269 7479  config["security
+00000c50: 225d 5b22 6175 7468 656e 7469 6361 7469  "]["authenticati
+00000c60: 6f6e 225d 5b22 636f 6e66 6967 225d 203d  on"]["config"] =
+00000c70: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00000c80: 636c 6965 6e74 5f69 6422 3a20 6f73 2e65  client_id": os.e
+00000c90: 6e76 6972 6f6e 2e67 6574 280a 2020 2020  nviron.get(.    
+00000ca0: 2020 2020 2020 2020 2020 2020 2247 4954              "GIT
+00000cb0: 4855 425f 434c 4945 4e54 5f49 4422 2c0a  HUB_CLIENT_ID",.
+00000cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cd0: 223c 656e 7465 7220 636c 6965 6e74 2069  "<enter client i
+00000ce0: 6420 6f72 2072 656d 6f76 6520 746f 2075  d or remove to u
+00000cf0: 7365 2047 4954 4855 425f 434c 4945 4e54  se GITHUB_CLIENT
+00000d00: 5f49 4420 656e 7669 726f 6e6d 656e 7420  _ID environment 
+00000d10: 7661 7269 6162 6c65 2028 7072 6566 6572  variable (prefer
+00000d20: 7265 6429 3e22 2c0a 2020 2020 2020 2020  red)>",.        
+00000d30: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00000d40: 2020 2022 636c 6965 6e74 5f73 6563 7265     "client_secre
+00000d50: 7422 3a20 6f73 2e65 6e76 6972 6f6e 2e67  t": os.environ.g
+00000d60: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+00000d70: 2020 2020 2247 4954 4855 425f 434c 4945      "GITHUB_CLIE
+00000d80: 4e54 5f53 4543 5245 5422 2c0a 2020 2020  NT_SECRET",.    
+00000d90: 2020 2020 2020 2020 2020 2020 223c 656e              "<en
+00000da0: 7465 7220 636c 6965 6e74 2073 6563 7265  ter client secre
+00000db0: 7420 6f72 2072 656d 6f76 6520 746f 2075  t or remove to u
+00000dc0: 7365 2047 4954 4855 425f 434c 4945 4e54  se GITHUB_CLIENT
+00000dd0: 5f53 4543 5245 5420 656e 7669 726f 6e6d  _SECRET environm
+00000de0: 656e 7420 7661 7269 6162 6c65 2028 7072  ent variable (pr
+00000df0: 6566 6572 7265 6429 3e22 2c0a 2020 2020  eferred)>",.    
+00000e00: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00000e10: 2020 207d 0a20 2020 2065 6c69 6620 6175     }.    elif au
+00000e20: 7468 5f70 726f 7669 6465 7220 3d3d 2041  th_provider == A
+00000e30: 7574 6865 6e74 6963 6174 696f 6e45 6e75  uthenticationEnu
+00000e40: 6d2e 6175 7468 303a 0a20 2020 2020 2020  m.auth0:.       
+00000e50: 2069 6620 6175 7468 5f61 7574 6f5f 7072   if auth_auto_pr
+00000e60: 6f76 6973 696f 6e3a 0a20 2020 2020 2020  ovision:.       
+00000e70: 2020 2020 2061 7574 6830 5f63 6f6e 6669       auth0_confi
+00000e80: 6720 3d20 6372 6561 7465 5f63 6c69 656e  g = create_clien
+00000e90: 7428 636f 6e66 6967 2e64 6f6d 6169 6e2c  t(config.domain,
+00000ea0: 2063 6f6e 6669 672e 7072 6f6a 6563 745f   config.project_
+00000eb0: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
+00000ec0: 2020 636f 6e66 6967 5b22 7365 6375 7269    config["securi
+00000ed0: 7479 225d 5b22 6175 7468 656e 7469 6361  ty"]["authentica
+00000ee0: 7469 6f6e 225d 5b22 636f 6e66 6967 225d  tion"]["config"]
+00000ef0: 203d 2061 7574 6830 5f63 6f6e 6669 670a   = auth0_config.
+00000f00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00000f10: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00000f20: 5b22 7365 6375 7269 7479 225d 5b22 6175  ["security"]["au
+00000f30: 7468 656e 7469 6361 7469 6f6e 225d 5b22  thentication"]["
+00000f40: 636f 6e66 6967 225d 203d 207b 0a20 2020  config"] = {.   
+00000f50: 2020 2020 2020 2020 2020 2020 2022 636c               "cl
+00000f60: 6965 6e74 5f69 6422 3a20 6f73 2e65 6e76  ient_id": os.env
+00000f70: 6972 6f6e 2e67 6574 280a 2020 2020 2020  iron.get(.      
+00000f80: 2020 2020 2020 2020 2020 2020 2020 2241                "A
+00000f90: 5554 4830 5f43 4c49 454e 545f 4944 222c  UTH0_CLIENT_ID",
+00000fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000fb0: 2020 2020 2022 3c65 6e74 6572 2063 6c69       "<enter cli
+00000fc0: 656e 7420 6964 206f 7220 7265 6d6f 7665  ent id or remove
+00000fd0: 2074 6f20 7573 6520 4155 5448 305f 434c   to use AUTH0_CL
+00000fe0: 4945 4e54 5f49 4420 656e 7669 726f 6e6d  IENT_ID environm
+00000ff0: 656e 7420 7661 7269 6162 6c65 2028 7072  ent variable (pr
+00001000: 6566 6572 7265 6429 3e22 2c0a 2020 2020  eferred)>",.    
+00001010: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+00001020: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001030: 636c 6965 6e74 5f73 6563 7265 7422 3a20  client_secret": 
+00001040: 6f73 2e65 6e76 6972 6f6e 2e67 6574 280a  os.environ.get(.
+00001050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001060: 2020 2020 2241 5554 4830 5f43 4c49 454e      "AUTH0_CLIEN
+00001070: 545f 5345 4352 4554 222c 0a20 2020 2020  T_SECRET",.     
+00001080: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001090: 3c65 6e74 6572 2063 6c69 656e 7420 7365  <enter client se
+000010a0: 6372 6574 206f 7220 7265 6d6f 7665 2074  cret or remove t
+000010b0: 6f20 7573 6520 4155 5448 305f 434c 4945  o use AUTH0_CLIE
+000010c0: 4e54 5f53 4543 5245 5420 656e 7669 726f  NT_SECRET enviro
+000010d0: 6e6d 656e 7420 7661 7269 6162 6c65 2028  nment variable (
+000010e0: 7072 6566 6572 7265 6429 3e22 2c0a 2020  preferred)>",.  
+000010f0: 2020 2020 2020 2020 2020 2020 2020 292c                ),
+00001100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001110: 2022 6175 7468 305f 7375 6264 6f6d 6169   "auth0_subdomai
+00001120: 6e22 3a20 6f73 2e65 6e76 6972 6f6e 2e67  n": os.environ.g
+00001130: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+00001140: 2020 2020 2020 2020 2241 5554 4830 5f44          "AUTH0_D
+00001150: 4f4d 4149 4e22 2c0a 2020 2020 2020 2020  OMAIN",.        
+00001160: 2020 2020 2020 2020 2020 2020 223c 656e              "<en
+00001170: 7465 7220 7375 6264 6f6d 6169 6e20 2877  ter subdomain (w
+00001180: 6974 686f 7574 202e 6175 7468 302e 636f  ithout .auth0.co
+00001190: 6d29 206f 7220 7265 6d6f 7665 2074 6f20  m) or remove to 
+000011a0: 7573 6520 4155 5448 305f 444f 4d41 494e  use AUTH0_DOMAIN
+000011b0: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+000011c0: 6961 626c 653e 222c 0a20 2020 2020 2020  iable>",.       
+000011d0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+000011e0: 2020 2020 2020 2020 7d0a 0a20 2020 2069          }..    i
+000011f0: 6620 636c 6f75 645f 7072 6f76 6964 6572  f cloud_provider
+00001200: 203d 3d20 5072 6f76 6964 6572 456e 756d   == ProviderEnum
+00001210: 2e64 6f3a 0a20 2020 2020 2020 2064 6f5f  .do:.        do_
+00001220: 7265 6769 6f6e 203d 2072 6567 696f 6e20  region = region 
+00001230: 6f72 2063 6f6e 7374 616e 7473 2e44 4f5f  or constants.DO_
+00001240: 4445 4641 554c 545f 5245 4749 4f4e 0a20  DEFAULT_REGION. 
+00001250: 2020 2020 2020 2064 6f5f 6b75 6265 726e         do_kubern
+00001260: 6574 6573 5f76 6572 7369 6f6e 7320 3d20  etes_versions = 
+00001270: 6b75 6265 726e 6574 6573 5f76 6572 7369  kubernetes_versi
+00001280: 6f6e 206f 7220 6765 745f 6c61 7465 7374  on or get_latest
+00001290: 5f6b 7562 6572 6e65 7465 735f 7665 7273  _kubernetes_vers
+000012a0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+000012b0: 2064 6967 6974 616c 5f6f 6365 616e 2e6b   digital_ocean.k
+000012c0: 7562 6572 6e65 7465 735f 7665 7273 696f  ubernetes_versio
+000012d0: 6e73 2829 0a20 2020 2020 2020 2029 0a20  ns().        ). 
+000012e0: 2020 2020 2020 2063 6f6e 6669 675b 2264         config["d
+000012f0: 6967 6974 616c 5f6f 6365 616e 225d 203d  igital_ocean"] =
+00001300: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00001310: 6b75 6265 726e 6574 6573 5f76 6572 7369  kubernetes_versi
+00001320: 6f6e 223a 2064 6f5f 6b75 6265 726e 6574  on": do_kubernet
+00001330: 6573 5f76 6572 7369 6f6e 732c 0a20 2020  es_versions,.   
+00001340: 2020 2020 2020 2020 2022 7265 6769 6f6e           "region
+00001350: 223a 2064 6f5f 7265 6769 6f6e 2c0a 2020  ": do_region,.  
+00001360: 2020 2020 2020 2020 2020 226e 6f64 655f            "node_
+00001370: 6772 6f75 7073 223a 206e 6f64 655f 6772  groups": node_gr
+00001380: 6f75 7073 5f74 6f5f 6469 6374 2844 4546  oups_to_dict(DEF
+00001390: 4155 4c54 5f44 4f5f 4e4f 4445 5f47 524f  AULT_DO_NODE_GRO
+000013a0: 5550 5329 2c0a 2020 2020 2020 2020 7d0a  UPS),.        }.
+000013b0: 0a20 2020 2020 2020 2063 6f6e 6669 675b  .        config[
+000013c0: 2274 6865 6d65 225d 5b22 6a75 7079 7465  "theme"]["jupyte
+000013d0: 7268 7562 225d 5b0a 2020 2020 2020 2020  rhub"][.        
+000013e0: 2020 2020 2268 7562 5f73 7562 7469 746c      "hub_subtitl
+000013f0: 6522 0a20 2020 2020 2020 205d 203d 2066  e".        ] = f
+00001400: 227b 5745 4c43 4f4d 455f 4845 4144 4552  "{WELCOME_HEADER
+00001410: 5f54 4558 547d 206f 6e20 4469 6769 7461  _TEXT} on Digita
+00001420: 6c20 4f63 6561 6e22 0a0a 2020 2020 656c  l Ocean"..    el
+00001430: 6966 2063 6c6f 7564 5f70 726f 7669 6465  if cloud_provide
+00001440: 7220 3d3d 2050 726f 7669 6465 7245 6e75  r == ProviderEnu
+00001450: 6d2e 6763 703a 0a20 2020 2020 2020 2067  m.gcp:.        g
+00001460: 6370 5f72 6567 696f 6e20 3d20 7265 6769  cp_region = regi
+00001470: 6f6e 206f 7220 636f 6e73 7461 6e74 732e  on or constants.
+00001480: 4743 505f 4445 4641 554c 545f 5245 4749  GCP_DEFAULT_REGI
+00001490: 4f4e 0a20 2020 2020 2020 2067 6370 5f6b  ON.        gcp_k
+000014a0: 7562 6572 6e65 7465 735f 7665 7273 696f  ubernetes_versio
+000014b0: 6e20 3d20 6b75 6265 726e 6574 6573 5f76  n = kubernetes_v
+000014c0: 6572 7369 6f6e 206f 7220 6765 745f 6c61  ersion or get_la
+000014d0: 7465 7374 5f6b 7562 6572 6e65 7465 735f  test_kubernetes_
+000014e0: 7665 7273 696f 6e28 0a20 2020 2020 2020  version(.       
+000014f0: 2020 2020 2067 6f6f 676c 655f 636c 6f75       google_clou
+00001500: 642e 6b75 6265 726e 6574 6573 5f76 6572  d.kubernetes_ver
+00001510: 7369 6f6e 7328 6763 705f 7265 6769 6f6e  sions(gcp_region
+00001520: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+00001530: 2020 2020 636f 6e66 6967 5b22 676f 6f67      config["goog
+00001540: 6c65 5f63 6c6f 7564 5f70 6c61 7466 6f72  le_cloud_platfor
+00001550: 6d22 5d20 3d20 7b0a 2020 2020 2020 2020  m"] = {.        
+00001560: 2020 2020 226b 7562 6572 6e65 7465 735f      "kubernetes_
+00001570: 7665 7273 696f 6e22 3a20 6763 705f 6b75  version": gcp_ku
+00001580: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
+00001590: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
+000015a0: 6567 696f 6e22 3a20 6763 705f 7265 6769  egion": gcp_regi
+000015b0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+000015c0: 226e 6f64 655f 6772 6f75 7073 223a 206e  "node_groups": n
+000015d0: 6f64 655f 6772 6f75 7073 5f74 6f5f 6469  ode_groups_to_di
+000015e0: 6374 2844 4546 4155 4c54 5f47 4350 5f4e  ct(DEFAULT_GCP_N
+000015f0: 4f44 455f 4752 4f55 5053 292c 0a20 2020  ODE_GROUPS),.   
+00001600: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00001610: 636f 6e66 6967 5b22 7468 656d 6522 5d5b  config["theme"][
+00001620: 226a 7570 7974 6572 6875 6222 5d5b 0a20  "jupyterhub"][. 
+00001630: 2020 2020 2020 2020 2020 2022 6875 625f             "hub_
+00001640: 7375 6274 6974 6c65 220a 2020 2020 2020  subtitle".      
+00001650: 2020 5d20 3d20 6622 7b57 454c 434f 4d45    ] = f"{WELCOME
+00001660: 5f48 4541 4445 525f 5445 5854 7d20 6f6e  _HEADER_TEXT} on
+00001670: 2047 6f6f 676c 6520 436c 6f75 6420 506c   Google Cloud Pl
+00001680: 6174 666f 726d 220a 2020 2020 2020 2020  atform".        
+00001690: 6966 2022 5052 4f4a 4543 545f 4944 2220  if "PROJECT_ID" 
+000016a0: 696e 206f 732e 656e 7669 726f 6e3a 0a20  in os.environ:. 
+000016b0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+000016c0: 675b 2267 6f6f 676c 655f 636c 6f75 645f  g["google_cloud_
+000016d0: 706c 6174 666f 726d 225d 5b22 7072 6f6a  platform"]["proj
+000016e0: 6563 7422 5d20 3d20 6f73 2e65 6e76 6972  ect"] = os.envir
+000016f0: 6f6e 5b22 5052 4f4a 4543 545f 4944 225d  on["PROJECT_ID"]
+00001700: 0a20 2020 2020 2020 2065 6c69 6620 6e6f  .        elif no
+00001710: 7420 6469 7361 626c 655f 7072 6f6d 7074  t disable_prompt
+00001720: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+00001730: 6e66 6967 5b22 676f 6f67 6c65 5f63 6c6f  nfig["google_clo
+00001740: 7564 5f70 6c61 7466 6f72 6d22 5d5b 2270  ud_platform"]["p
+00001750: 726f 6a65 6374 225d 203d 2069 6e70 7574  roject"] = input
+00001760: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00001770: 2020 2245 6e74 6572 2047 6f6f 676c 6520    "Enter Google 
+00001780: 436c 6f75 6420 506c 6174 666f 726d 2050  Cloud Platform P
+00001790: 726f 6a65 6374 2049 443a 2022 0a20 2020  roject ID: ".   
+000017a0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+000017b0: 656c 6966 2063 6c6f 7564 5f70 726f 7669  elif cloud_provi
+000017c0: 6465 7220 3d3d 2050 726f 7669 6465 7245  der == ProviderE
+000017d0: 6e75 6d2e 617a 7572 653a 0a20 2020 2020  num.azure:.     
+000017e0: 2020 2061 7a75 7265 5f72 6567 696f 6e20     azure_region 
+000017f0: 3d20 7265 6769 6f6e 206f 7220 636f 6e73  = region or cons
+00001800: 7461 6e74 732e 415a 5552 455f 4445 4641  tants.AZURE_DEFA
+00001810: 554c 545f 5245 4749 4f4e 0a20 2020 2020  ULT_REGION.     
+00001820: 2020 2061 7a75 7265 5f6b 7562 6572 6e65     azure_kuberne
+00001830: 7465 735f 7665 7273 696f 6e20 3d20 6b75  tes_version = ku
+00001840: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
+00001850: 206f 7220 6765 745f 6c61 7465 7374 5f6b   or get_latest_k
+00001860: 7562 6572 6e65 7465 735f 7665 7273 696f  ubernetes_versio
+00001870: 6e28 0a20 2020 2020 2020 2020 2020 2061  n(.            a
+00001880: 7a75 7265 5f63 6c6f 7564 2e6b 7562 6572  zure_cloud.kuber
+00001890: 6e65 7465 735f 7665 7273 696f 6e73 2861  netes_versions(a
+000018a0: 7a75 7265 5f72 6567 696f 6e29 0a20 2020  zure_region).   
+000018b0: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
+000018c0: 6f6e 6669 675b 2261 7a75 7265 225d 203d  onfig["azure"] =
+000018d0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+000018e0: 6b75 6265 726e 6574 6573 5f76 6572 7369  kubernetes_versi
+000018f0: 6f6e 223a 2061 7a75 7265 5f6b 7562 6572  on": azure_kuber
+00001900: 6e65 7465 735f 7665 7273 696f 6e2c 0a20  netes_version,. 
+00001910: 2020 2020 2020 2020 2020 2022 7265 6769             "regi
+00001920: 6f6e 223a 2061 7a75 7265 5f72 6567 696f  on": azure_regio
+00001930: 6e2c 0a20 2020 2020 2020 2020 2020 2022  n,.            "
+00001940: 7374 6f72 6167 655f 6163 636f 756e 745f  storage_account_
+00001950: 706f 7374 6669 7822 3a20 7261 6e64 6f6d  postfix": random
+00001960: 5f73 6563 7572 655f 7374 7269 6e67 286c  _secure_string(l
+00001970: 656e 6774 683d 3429 2c0a 2020 2020 2020  ength=4),.      
+00001980: 2020 2020 2020 226e 6f64 655f 6772 6f75        "node_grou
+00001990: 7073 223a 206e 6f64 655f 6772 6f75 7073  ps": node_groups
+000019a0: 5f74 6f5f 6469 6374 2844 4546 4155 4c54  _to_dict(DEFAULT
+000019b0: 5f41 5a55 5245 5f4e 4f44 455f 4752 4f55  _AZURE_NODE_GROU
+000019c0: 5053 292c 0a20 2020 2020 2020 207d 0a0a  PS),.        }..
+000019d0: 2020 2020 2020 2020 636f 6e66 6967 5b22          config["
+000019e0: 7468 656d 6522 5d5b 226a 7570 7974 6572  theme"]["jupyter
+000019f0: 6875 6222 5d5b 0a20 2020 2020 2020 2020  hub"][.         
+00001a00: 2020 2022 6875 625f 7375 6274 6974 6c65     "hub_subtitle
+00001a10: 220a 2020 2020 2020 2020 5d20 3d20 6622  ".        ] = f"
+00001a20: 7b57 454c 434f 4d45 5f48 4541 4445 525f  {WELCOME_HEADER_
+00001a30: 5445 5854 7d20 6f6e 2041 7a75 7265 220a  TEXT} on Azure".
+00001a40: 0a20 2020 2065 6c69 6620 636c 6f75 645f  .    elif cloud_
+00001a50: 7072 6f76 6964 6572 203d 3d20 5072 6f76  provider == Prov
+00001a60: 6964 6572 456e 756d 2e61 7773 3a0a 2020  iderEnum.aws:.  
+00001a70: 2020 2020 2020 6177 735f 7265 6769 6f6e        aws_region
+00001a80: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00001a90: 2072 6567 696f 6e0a 2020 2020 2020 2020   region.        
+00001aa0: 2020 2020 6f72 206f 732e 656e 7669 726f      or os.enviro
+00001ab0: 6e2e 6765 7428 2241 5753 5f44 4546 4155  n.get("AWS_DEFAU
+00001ac0: 4c54 5f52 4547 494f 4e22 290a 2020 2020  LT_REGION").    
+00001ad0: 2020 2020 2020 2020 6f72 2063 6f6e 7374          or const
+00001ae0: 616e 7473 2e41 5753 5f44 4546 4155 4c54  ants.AWS_DEFAULT
+00001af0: 5f52 4547 494f 4e0a 2020 2020 2020 2020  _REGION.        
+00001b00: 290a 2020 2020 2020 2020 6177 735f 6b75  ).        aws_ku
+00001b10: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
+00001b20: 203d 206b 7562 6572 6e65 7465 735f 7665   = kubernetes_ve
+00001b30: 7273 696f 6e20 6f72 2067 6574 5f6c 6174  rsion or get_lat
+00001b40: 6573 745f 6b75 6265 726e 6574 6573 5f76  est_kubernetes_v
+00001b50: 6572 7369 6f6e 280a 2020 2020 2020 2020  ersion(.        
+00001b60: 2020 2020 616d 617a 6f6e 5f77 6562 5f73      amazon_web_s
+00001b70: 6572 7669 6365 732e 6b75 6265 726e 6574  ervices.kubernet
+00001b80: 6573 5f76 6572 7369 6f6e 7328 6177 735f  es_versions(aws_
+00001b90: 7265 6769 6f6e 290a 2020 2020 2020 2020  region).        
+00001ba0: 290a 2020 2020 2020 2020 636f 6e66 6967  ).        config
+00001bb0: 5b22 616d 617a 6f6e 5f77 6562 5f73 6572  ["amazon_web_ser
+00001bc0: 7669 6365 7322 5d20 3d20 7b0a 2020 2020  vices"] = {.    
+00001bd0: 2020 2020 2020 2020 226b 7562 6572 6e65          "kuberne
+00001be0: 7465 735f 7665 7273 696f 6e22 3a20 6177  tes_version": aw
+00001bf0: 735f 6b75 6265 726e 6574 6573 5f76 6572  s_kubernetes_ver
+00001c00: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
+00001c10: 2020 2272 6567 696f 6e22 3a20 6177 735f    "region": aws_
+00001c20: 7265 6769 6f6e 2c0a 2020 2020 2020 2020  region,.        
+00001c30: 2020 2020 226e 6f64 655f 6772 6f75 7073      "node_groups
+00001c40: 223a 206e 6f64 655f 6772 6f75 7073 5f74  ": node_groups_t
+00001c50: 6f5f 6469 6374 2844 4546 4155 4c54 5f41  o_dict(DEFAULT_A
+00001c60: 5753 5f4e 4f44 455f 4752 4f55 5053 292c  WS_NODE_GROUPS),
+00001c70: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00001c80: 2020 2063 6f6e 6669 675b 2274 6865 6d65     config["theme
+00001c90: 225d 5b22 6a75 7079 7465 7268 7562 225d  "]["jupyterhub"]
+00001ca0: 5b0a 2020 2020 2020 2020 2020 2020 2268  [.            "h
+00001cb0: 7562 5f73 7562 7469 746c 6522 0a20 2020  ub_subtitle".   
+00001cc0: 2020 2020 205d 203d 2066 227b 5745 4c43       ] = f"{WELC
+00001cd0: 4f4d 455f 4845 4144 4552 5f54 4558 547d  OME_HEADER_TEXT}
+00001ce0: 206f 6e20 416d 617a 6f6e 2057 6562 2053   on Amazon Web S
+00001cf0: 6572 7669 6365 7322 0a0a 2020 2020 656c  ervices"..    el
+00001d00: 6966 2063 6c6f 7564 5f70 726f 7669 6465  if cloud_provide
+00001d10: 7220 3d3d 2050 726f 7669 6465 7245 6e75  r == ProviderEnu
+00001d20: 6d2e 6578 6973 7469 6e67 3a0a 2020 2020  m.existing:.    
+00001d30: 2020 2020 636f 6e66 6967 5b22 7468 656d      config["them
+00001d40: 6522 5d5b 226a 7570 7974 6572 6875 6222  e"]["jupyterhub"
+00001d50: 5d5b 2268 7562 5f73 7562 7469 746c 6522  ]["hub_subtitle"
+00001d60: 5d20 3d20 5745 4c43 4f4d 455f 4845 4144  ] = WELCOME_HEAD
+00001d70: 4552 5f54 4558 540a 0a20 2020 2065 6c69  ER_TEXT..    eli
+00001d80: 6620 636c 6f75 645f 7072 6f76 6964 6572  f cloud_provider
+00001d90: 203d 3d20 5072 6f76 6964 6572 456e 756d   == ProviderEnum
+00001da0: 2e6c 6f63 616c 3a0a 2020 2020 2020 2020  .local:.        
+00001db0: 636f 6e66 6967 5b22 7468 656d 6522 5d5b  config["theme"][
+00001dc0: 226a 7570 7974 6572 6875 6222 5d5b 2268  "jupyterhub"]["h
+00001dd0: 7562 5f73 7562 7469 746c 6522 5d20 3d20  ub_subtitle"] = 
+00001de0: 5745 4c43 4f4d 455f 4845 4144 4552 5f54  WELCOME_HEADER_T
+00001df0: 4558 540a 0a20 2020 2069 6620 7373 6c5f  EXT..    if ssl_
+00001e00: 6365 7274 5f65 6d61 696c 3a0a 2020 2020  cert_email:.    
+00001e10: 2020 2020 636f 6e66 6967 5b22 6365 7274      config["cert
+00001e20: 6966 6963 6174 6522 5d20 3d20 7b22 7479  ificate"] = {"ty
+00001e30: 7065 223a 2043 6572 7469 6669 6361 7465  pe": Certificate
+00001e40: 456e 756d 2e6c 6574 7365 6e63 7279 7074  Enum.letsencrypt
+00001e50: 2e76 616c 7565 7d0a 2020 2020 2020 2020  .value}.        
+00001e60: 636f 6e66 6967 5b22 6365 7274 6966 6963  config["certific
+00001e70: 6174 6522 5d5b 2261 636d 655f 656d 6169  ate"]["acme_emai
+00001e80: 6c22 5d20 3d20 7373 6c5f 6365 7274 5f65  l"] = ssl_cert_e
+00001e90: 6d61 696c 0a0a 2020 2020 2320 7661 6c69  mail..    # vali
+00001ea0: 6461 7465 2063 6f6e 6669 6775 7261 7469  date configurati
+00001eb0: 6f6e 2061 6e64 2063 6f6e 7665 7274 2074  on and convert t
+00001ec0: 6f20 6d6f 6465 6c0a 2020 2020 6672 6f6d  o model.    from
+00001ed0: 206e 6562 6172 692e 706c 7567 696e 7320   nebari.plugins 
+00001ee0: 696d 706f 7274 206e 6562 6172 695f 706c  import nebari_pl
+00001ef0: 7567 696e 5f6d 616e 6167 6572 0a0a 2020  ugin_manager..  
+00001f00: 2020 7472 793a 0a20 2020 2020 2020 2063    try:.        c
+00001f10: 6f6e 6669 675f 6d6f 6465 6c20 3d20 6e65  onfig_model = ne
+00001f20: 6261 7269 5f70 6c75 6769 6e5f 6d61 6e61  bari_plugin_mana
+00001f30: 6765 722e 636f 6e66 6967 5f73 6368 656d  ger.config_schem
+00001f40: 612e 6d6f 6465 6c5f 7661 6c69 6461 7465  a.model_validate
+00001f50: 2863 6f6e 6669 6729 0a20 2020 2065 7863  (config).    exc
+00001f60: 6570 7420 7079 6461 6e74 6963 2e56 616c  ept pydantic.Val
+00001f70: 6964 6174 696f 6e45 7272 6f72 2061 7320  idationError as 
+00001f80: 653a 0a20 2020 2020 2020 2070 7269 6e74  e:.        print
+00001f90: 2873 7472 2865 2929 0a0a 2020 2020 6966  (str(e))..    if
+00001fa0: 2072 6570 6f73 6974 6f72 795f 6175 746f   repository_auto
+00001fb0: 5f70 726f 7669 7369 6f6e 3a0a 2020 2020  _provision:.    
+00001fc0: 2020 2020 6d61 7463 6820 3d20 7265 2e73      match = re.s
+00001fd0: 6561 7263 6828 6769 7468 7562 5f75 726c  earch(github_url
+00001fe0: 5f72 6567 6578 2c20 7265 706f 7369 746f  _regex, reposito
+00001ff0: 7279 290a 2020 2020 2020 2020 6966 206d  ry).        if m
+00002000: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
+00002010: 2020 6769 745f 7265 706f 7369 746f 7279    git_repository
+00002020: 203d 2067 6974 6875 625f 6175 746f 5f70   = github_auto_p
+00002030: 726f 7669 7369 6f6e 280a 2020 2020 2020  rovision(.      
+00002040: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00002050: 5f6d 6f64 656c 2c20 6d61 7463 682e 6772  _model, match.gr
+00002060: 6f75 7028 3229 2c20 6d61 7463 682e 6772  oup(2), match.gr
+00002070: 6f75 7028 3329 0a20 2020 2020 2020 2020  oup(3).         
+00002080: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00002090: 2067 6974 5f72 6570 6f73 6974 6f72 795f   git_repository_
+000020a0: 696e 6974 6961 6c69 7a65 2867 6974 5f72  initialize(git_r
+000020b0: 6570 6f73 6974 6f72 7929 0a20 2020 2020  epository).     
+000020c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000020d0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+000020e0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+000020f0: 2020 2020 2020 2066 2252 6570 6f73 6974         f"Reposit
+00002100: 6f72 7920 746f 2062 6520 6175 746f 2d70  ory to be auto-p
+00002110: 726f 7669 7369 6f6e 6564 2069 7320 6e6f  rovisioned is no
+00002120: 7420 7468 6520 6675 6c6c 2055 524c 206f  t the full URL o
+00002130: 6620 6120 4769 7448 7562 2072 6570 6f3a  f a GitHub repo:
+00002140: 207b 7265 706f 7369 746f 7279 7d22 0a20   {repository}". 
+00002150: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00002160: 2020 7265 7475 726e 2063 6f6e 6669 670a    return config.
+00002170: 0a0a 6465 6620 6769 7468 7562 5f61 7574  ..def github_aut
+00002180: 6f5f 7072 6f76 6973 696f 6e28 636f 6e66  o_provision(conf
+00002190: 6967 3a20 7079 6461 6e74 6963 2e42 6173  ig: pydantic.Bas
+000021a0: 654d 6f64 656c 2c20 6f77 6e65 723a 2073  eModel, owner: s
+000021b0: 7472 2c20 7265 706f 3a20 7374 7229 3a0a  tr, repo: str):.
+000021c0: 2020 2020 616c 7265 6164 795f 6578 6973      already_exis
+000021d0: 7473 203d 2054 7275 650a 2020 2020 7472  ts = True.    tr
+000021e0: 793a 0a20 2020 2020 2020 2067 6974 6875  y:.        githu
+000021f0: 622e 6765 745f 7265 706f 7369 746f 7279  b.get_repository
+00002200: 286f 776e 6572 2c20 7265 706f 290a 2020  (owner, repo).  
+00002210: 2020 6578 6365 7074 2072 6571 7565 7374    except request
+00002220: 732e 6578 6365 7074 696f 6e73 2e48 5454  s.exceptions.HTT
+00002230: 5045 7272 6f72 3a0a 2020 2020 2020 2020  PError:.        
+00002240: 2320 7265 706f 206e 6f74 2066 6f75 6e64  # repo not found
+00002250: 0a20 2020 2020 2020 2061 6c72 6561 6479  .        already
+00002260: 5f65 7869 7374 7320 3d20 4661 6c73 650a  _exists = False.
+00002270: 0a20 2020 2069 6620 6e6f 7420 616c 7265  .    if not alre
+00002280: 6164 795f 6578 6973 7473 3a0a 2020 2020  ady_exists:.    
+00002290: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+000022a0: 2020 2020 2067 6974 6875 622e 6372 6561       github.crea
+000022b0: 7465 5f72 6570 6f73 6974 6f72 7928 0a20  te_repository(. 
+000022c0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+000022d0: 776e 6572 2c0a 2020 2020 2020 2020 2020  wner,.          
+000022e0: 2020 2020 2020 7265 706f 2c0a 2020 2020        repo,.    
+000022f0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00002300: 7269 7074 696f 6e3d 6622 4e65 6261 7269  ription=f"Nebari
+00002310: 207b 636f 6e66 6967 2e70 726f 6a65 6374   {config.project
+00002320: 5f6e 616d 657d 2d7b 636f 6e66 6967 2e70  _name}-{config.p
+00002330: 726f 7669 6465 727d 222c 0a20 2020 2020  rovider}",.     
+00002340: 2020 2020 2020 2020 2020 2068 6f6d 6570             homep
+00002350: 6167 653d 6622 6874 7470 733a 2f2f 7b63  age=f"https://{c
+00002360: 6f6e 6669 672e 646f 6d61 696e 7d22 2c0a  onfig.domain}",.
+00002370: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00002380: 2020 2020 2020 6578 6365 7074 2072 6571        except req
+00002390: 7565 7374 732e 6578 6365 7074 696f 6e73  uests.exceptions
+000023a0: 2e48 5454 5045 7272 6f72 2061 7320 6865  .HTTPError as he
+000023b0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+000023c0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+000023d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023e0: 6622 556e 6162 6c65 2074 6f20 6372 6561  f"Unable to crea
+000023f0: 7465 2047 6974 4875 6220 7265 706f 2068  te GitHub repo h
+00002400: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002410: 6d2f 7b6f 776e 6572 7d2f 7b72 6570 6f7d  m/{owner}/{repo}
+00002420: 202d 2065 7272 6f72 206d 6573 7361 6765   - error message
+00002430: 2066 726f 6d20 4769 7448 7562 2069 733a   from GitHub is:
+00002440: 207b 6865 7d22 0a20 2020 2020 2020 2020   {he}".         
+00002450: 2020 2029 0a20 2020 2065 6c73 653a 0a20     ).    else:. 
+00002460: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
+00002470: 726e 696e 6728 6622 4769 7448 7562 2072  rning(f"GitHub r
+00002480: 6570 6f20 6874 7470 733a 2f2f 6769 7468  epo https://gith
+00002490: 7562 2e63 6f6d 2f7b 6f77 6e65 727d 2f7b  ub.com/{owner}/{
+000024a0: 7265 706f 7d20 616c 7265 6164 7920 6578  repo} already ex
+000024b0: 6973 7473 2229 0a0a 2020 2020 7472 793a  ists")..    try:
+000024c0: 0a20 2020 2020 2020 2023 2053 6563 7265  .        # Secre
+000024d0: 7473 0a20 2020 2020 2020 2069 6620 636f  ts.        if co
+000024e0: 6e66 6967 2e70 726f 7669 6465 7220 3d3d  nfig.provider ==
+000024f0: 2050 726f 7669 6465 7245 6e75 6d2e 646f   ProviderEnum.do
+00002500: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00002510: 7220 6e61 6d65 2069 6e20 7b0a 2020 2020  r name in {.    
+00002520: 2020 2020 2020 2020 2020 2020 2241 5753              "AWS
+00002530: 5f41 4343 4553 535f 4b45 595f 4944 222c  _ACCESS_KEY_ID",
+00002540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002550: 2022 4157 535f 5345 4352 4554 5f41 4343   "AWS_SECRET_ACC
+00002560: 4553 535f 4b45 5922 2c0a 2020 2020 2020  ESS_KEY",.      
+00002570: 2020 2020 2020 2020 2020 2253 5041 4345            "SPACE
+00002580: 535f 4143 4345 5353 5f4b 4559 5f49 4422  S_ACCESS_KEY_ID"
+00002590: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000025a0: 2020 2253 5041 4345 535f 5345 4352 4554    "SPACES_SECRET
+000025b0: 5f41 4343 4553 535f 4b45 5922 2c0a 2020  _ACCESS_KEY",.  
+000025c0: 2020 2020 2020 2020 2020 2020 2020 2244                "D
+000025d0: 4947 4954 414c 4f43 4541 4e5f 544f 4b45  IGITALOCEAN_TOKE
+000025e0: 4e22 2c0a 2020 2020 2020 2020 2020 2020  N",.            
+000025f0: 7d3a 0a20 2020 2020 2020 2020 2020 2020  }:.             
+00002600: 2020 2067 6974 6875 622e 7570 6461 7465     github.update
+00002610: 5f73 6563 7265 7428 6f77 6e65 722c 2072  _secret(owner, r
+00002620: 6570 6f2c 206e 616d 652c 206f 732e 656e  epo, name, os.en
+00002630: 7669 726f 6e5b 6e61 6d65 5d29 0a20 2020  viron[name]).   
+00002640: 2020 2020 2065 6c69 6620 636f 6e66 6967       elif config
+00002650: 2e70 726f 7669 6465 7220 3d3d 2050 726f  .provider == Pro
+00002660: 7669 6465 7245 6e75 6d2e 6177 733a 0a20  viderEnum.aws:. 
+00002670: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
+00002680: 616d 6520 696e 207b 0a20 2020 2020 2020  ame in {.       
+00002690: 2020 2020 2020 2020 2022 4157 535f 4143           "AWS_AC
+000026a0: 4345 5353 5f4b 4559 5f49 4422 2c0a 2020  CESS_KEY_ID",.  
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2241                "A
+000026c0: 5753 5f53 4543 5245 545f 4143 4345 5353  WS_SECRET_ACCESS
+000026d0: 5f4b 4559 222c 0a20 2020 2020 2020 2020  _KEY",.         
+000026e0: 2020 207d 3a0a 2020 2020 2020 2020 2020     }:.          
+000026f0: 2020 2020 2020 6769 7468 7562 2e75 7064        github.upd
+00002700: 6174 655f 7365 6372 6574 286f 776e 6572  ate_secret(owner
+00002710: 2c20 7265 706f 2c20 6e61 6d65 2c20 6f73  , repo, name, os
+00002720: 2e65 6e76 6972 6f6e 5b6e 616d 655d 290a  .environ[name]).
+00002730: 2020 2020 2020 2020 656c 6966 2063 6f6e          elif con
+00002740: 6669 672e 7072 6f76 6964 6572 203d 3d20  fig.provider == 
+00002750: 5072 6f76 6964 6572 456e 756d 2e67 6370  ProviderEnum.gcp
+00002760: 3a0a 2020 2020 2020 2020 2020 2020 6769  :.            gi
+00002770: 7468 7562 2e75 7064 6174 655f 7365 6372  thub.update_secr
+00002780: 6574 286f 776e 6572 2c20 7265 706f 2c20  et(owner, repo, 
+00002790: 2250 524f 4a45 4354 5f49 4422 2c20 6f73  "PROJECT_ID", os
+000027a0: 2e65 6e76 6972 6f6e 5b22 5052 4f4a 4543  .environ["PROJEC
+000027b0: 545f 4944 225d 290a 2020 2020 2020 2020  T_ID"]).        
+000027c0: 2020 2020 7769 7468 206f 7065 6e28 6f73      with open(os
+000027d0: 2e65 6e76 6972 6f6e 5b22 474f 4f47 4c45  .environ["GOOGLE
+000027e0: 5f43 5245 4445 4e54 4941 4c53 225d 2920  _CREDENTIALS"]) 
+000027f0: 6173 2066 3a0a 2020 2020 2020 2020 2020  as f:.          
+00002800: 2020 2020 2020 6769 7468 7562 2e75 7064        github.upd
+00002810: 6174 655f 7365 6372 6574 286f 776e 6572  ate_secret(owner
+00002820: 2c20 7265 706f 2c20 2247 4f4f 474c 455f  , repo, "GOOGLE_
+00002830: 4352 4544 454e 5449 414c 5322 2c20 662e  CREDENTIALS", f.
+00002840: 7265 6164 2829 290a 2020 2020 2020 2020  read()).        
+00002850: 656c 6966 2063 6f6e 6669 672e 7072 6f76  elif config.prov
+00002860: 6964 6572 203d 3d20 5072 6f76 6964 6572  ider == Provider
+00002870: 456e 756d 2e61 7a75 7265 3a0a 2020 2020  Enum.azure:.    
+00002880: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
+00002890: 2069 6e20 7b0a 2020 2020 2020 2020 2020   in {.          
+000028a0: 2020 2020 2020 2241 524d 5f43 4c49 454e        "ARM_CLIEN
+000028b0: 545f 4944 222c 0a20 2020 2020 2020 2020  T_ID",.         
+000028c0: 2020 2020 2020 2022 4152 4d5f 434c 4945         "ARM_CLIE
+000028d0: 4e54 5f53 4543 5245 5422 2c0a 2020 2020  NT_SECRET",.    
+000028e0: 2020 2020 2020 2020 2020 2020 2241 524d              "ARM
+000028f0: 5f53 5542 5343 5249 5054 494f 4e5f 4944  _SUBSCRIPTION_ID
+00002900: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002910: 2020 2022 4152 4d5f 5445 4e41 4e54 5f49     "ARM_TENANT_I
+00002920: 4422 2c0a 2020 2020 2020 2020 2020 2020  D",.            
+00002930: 7d3a 0a20 2020 2020 2020 2020 2020 2020  }:.             
+00002940: 2020 2067 6974 6875 622e 7570 6461 7465     github.update
+00002950: 5f73 6563 7265 7428 6f77 6e65 722c 2072  _secret(owner, r
+00002960: 6570 6f2c 206e 616d 652c 206f 732e 656e  epo, name, os.en
+00002970: 7669 726f 6e5b 6e61 6d65 5d29 0a20 2020  viron[name]).   
+00002980: 2020 2020 2067 6974 6875 622e 7570 6461       github.upda
+00002990: 7465 5f73 6563 7265 7428 0a20 2020 2020  te_secret(.     
+000029a0: 2020 2020 2020 206f 776e 6572 2c20 7265         owner, re
+000029b0: 706f 2c20 2252 4550 4f53 4954 4f52 595f  po, "REPOSITORY_
+000029c0: 4143 4345 5353 5f54 4f4b 454e 222c 206f  ACCESS_TOKEN", o
+000029d0: 732e 656e 7669 726f 6e5b 2247 4954 4855  s.environ["GITHU
+000029e0: 425f 544f 4b45 4e22 5d0a 2020 2020 2020  B_TOKEN"].      
+000029f0: 2020 290a 2020 2020 6578 6365 7074 2072    ).    except r
+00002a00: 6571 7565 7374 732e 6578 6365 7074 696f  equests.exceptio
+00002a10: 6e73 2e48 5454 5045 7272 6f72 2061 7320  ns.HTTPError as 
+00002a20: 6865 3a0a 2020 2020 2020 2020 7261 6973  he:.        rais
+00002a30: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+00002a40: 2020 2020 2020 2020 2020 6622 556e 6162            f"Unab
+00002a50: 6c65 2074 6f20 7365 7420 5365 6372 6574  le to set Secret
+00002a60: 7320 6f6e 2047 6974 4875 6220 7265 706f  s on GitHub repo
+00002a70: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00002a80: 636f 6d2f 7b6f 776e 6572 7d2f 7b72 6570  com/{owner}/{rep
+00002a90: 6f7d 202d 2065 7272 6f72 206d 6573 7361  o} - error messa
+00002aa0: 6765 2066 726f 6d20 4769 7448 7562 2069  ge from GitHub i
+00002ab0: 733a 207b 6865 7d22 0a20 2020 2020 2020  s: {he}".       
+00002ac0: 2029 0a0a 2020 2020 7265 7475 726e 2066   )..    return f
+00002ad0: 2267 6974 4067 6974 6875 622e 636f 6d3a  "git@github.com:
+00002ae0: 7b6f 776e 6572 7d2f 7b72 6570 6f7d 2e67  {owner}/{repo}.g
+00002af0: 6974 220a 0a0a 6465 6620 6769 745f 7265  it"...def git_re
+00002b00: 706f 7369 746f 7279 5f69 6e69 7469 616c  pository_initial
+00002b10: 697a 6528 6769 745f 7265 706f 7369 746f  ize(git_reposito
+00002b20: 7279 293a 0a20 2020 2069 6620 6e6f 7420  ry):.    if not 
+00002b30: 6769 742e 6973 5f67 6974 5f72 6570 6f28  git.is_git_repo(
+00002b40: 5061 7468 2e63 7764 2829 293a 0a20 2020  Path.cwd()):.   
+00002b50: 2020 2020 2067 6974 2e69 6e69 7469 616c       git.initial
+00002b60: 697a 655f 6769 7428 5061 7468 2e63 7764  ize_git(Path.cwd
+00002b70: 2829 290a 2020 2020 6769 742e 6164 645f  ()).    git.add_
+00002b80: 6769 745f 7265 6d6f 7465 2867 6974 5f72  git_remote(git_r
+00002b90: 6570 6f73 6974 6f72 792c 2070 6174 683d  epository, path=
+00002ba0: 5061 7468 2e63 7764 2829 2c20 7265 6d6f  Path.cwd(), remo
+00002bb0: 7465 5f6e 616d 653d 226f 7269 6769 6e22  te_name="origin"
+00002bc0: 290a                                     ).
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/keycloak.py` & `nebari-2024.5.1rc1/src/_nebari/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/render.py` & `nebari-2024.5.1rc1/src/_nebari/render.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/upgrade.py` & `nebari-2024.5.1rc1/src/_nebari/upgrade.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 import string
 from abc import ABC
 from pathlib import Path
 from typing import Any, ClassVar, Dict
 
 import rich
 from packaging.version import Version
-from pydantic.error_wrappers import ValidationError
+from pydantic import ValidationError
 from rich.prompt import Prompt
 
 from _nebari.config import backup_configuration
+from _nebari.stages.infrastructure import (
+    provider_enum_default_node_groups_map,
+    provider_enum_name_map,
+)
 from _nebari.utils import (
     get_k8s_version_prefix,
     get_provider_config_block_name,
     load_yaml,
     yaml,
 )
 from _nebari.version import __version__, rounded_ver_parse
@@ -734,14 +738,45 @@
         self, config, start_version, config_filename: Path, *args, **kwargs
     ):
         rich.print("Ready to upgrade to Nebari version [green]2024.3.3[/green].")
 
         return config
 
 
+class Upgrade_2024_4_1(UpgradeStep):
+    version = "2024.4.1"
+
+    def _version_specific_upgrade(
+        self, config, start_version, config_filename: Path, *args, **kwargs
+    ):
+        # Default configuration for the node groups was added in this version. Therefore,
+        # users upgrading who don't have any specific node groups defined on their config
+        # file already, will be prompted and asked whether they want to include the default
+        if provider := config.get("provider", ""):
+            provider_full_name = provider_enum_name_map[provider]
+            if provider_full_name in config and "node_groups" not in config.get(
+                provider_full_name, {}
+            ):
+                try:
+                    default_node_groups = provider_enum_default_node_groups_map[
+                        provider
+                    ]
+                    continue_ = Prompt.ask(
+                        f"Would you like to include the default configuration for the node groups in [purple]{config_filename}[/purple]?",
+                        choices=["y", "N"],
+                        default="N",
+                    )
+                    if continue_ == "y":
+                        config[provider_full_name]["node_groups"] = default_node_groups
+                except KeyError:
+                    pass
+
+        return config
+
+
 __rounded_version__ = str(rounded_ver_parse(__version__))
 
 # Manually-added upgrade steps must go above this line
 if not UpgradeStep.has_step(__rounded_version__):
     # Always have a way to upgrade to the latest full version number, even if no customizations
     # Don't let dev/prerelease versions cloud things
     class UpgradeLatest(UpgradeStep):
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/utils.py` & `nebari-2024.5.1rc1/src/_nebari/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import string
 import subprocess
 import sys
 import threading
 import time
 import warnings
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Set
 
 from ruamel.yaml import YAML
 
 from _nebari import constants
 
 # environment variable overrides
 NEBARI_GH_BRANCH = os.getenv("NEBARI_GH_BRANCH", None)
@@ -334,7 +334,22 @@
         "gcp": "google_cloud_platform",
     }
 
     if provider in PROVIDER_CONFIG_NAMES.keys():
         return PROVIDER_CONFIG_NAMES[provider]
     else:
         return provider
+
+
+def check_environment_variables(variables: Set[str], reference: str) -> None:
+    """Check that environment variables are set."""
+    required_variables = {
+        variable: os.environ.get(variable, None) for variable in variables
+    }
+    missing_variables = {
+        variable for variable, value in required_variables.items() if value is None
+    }
+    if missing_variables:
+        raise ValueError(
+            f"""Missing the following required environment variables: {required_variables}\n
+            Please see the documentation for more information: {reference}"""
+        )
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/version.py` & `nebari-2024.5.1rc1/src/_nebari/version.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/provider/git.py` & `nebari-2024.5.1rc1/src/_nebari/provider/git.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/provider/terraform.py` & `nebari-2024.5.1rc1/src/_nebari/provider/terraform.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/provider/cicd/github.py` & `nebari-2024.5.1rc1/src/_nebari/provider/cicd/github.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import os
 from typing import Dict, List, Optional, Union
 
 import requests
 from nacl import encoding, public
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field, RootModel
 
 from _nebari.constants import LATEST_SUPPORTED_PYTHON_VERSION
 from _nebari.provider.cicd.common import pip_install_nebari
 from nebari import schema
 
 GITHUB_BASE_URL = "https://api.github.com/"
 
@@ -139,57 +139,42 @@
 
 
 class GHA_on_extras(BaseModel):
     branches: List[str]
     paths: List[str]
 
 
-class GHA_on(BaseModel):
-    # to allow for dynamic key names
-    __root__: Dict[str, GHA_on_extras]
-
-    # TODO: validate __root__ values
-    # `push`, `pull_request`, etc.
-
-
-class GHA_job_steps_extras(BaseModel):
-    # to allow for dynamic key names
-    __root__: Union[str, float, int]
+GHA_on = RootModel[Dict[str, GHA_on_extras]]
+GHA_job_steps_extras = RootModel[Union[str, float, int]]
 
 
 class GHA_job_step(BaseModel):
     name: str
-    uses: Optional[str]
-    with_: Optional[Dict[str, GHA_job_steps_extras]] = Field(alias="with")
-    run: Optional[str]
-    env: Optional[Dict[str, GHA_job_steps_extras]]
-
-    class Config:
-        allow_population_by_field_name = True
+    uses: Optional[str] = None
+    with_: Optional[Dict[str, GHA_job_steps_extras]] = Field(alias="with", default=None)
+    run: Optional[str] = None
+    env: Optional[Dict[str, GHA_job_steps_extras]] = None
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class GHA_job_id(BaseModel):
     name: str
     runs_on_: str = Field(alias="runs-on")
-    permissions: Optional[Dict[str, str]]
+    permissions: Optional[Dict[str, str]] = None
     steps: List[GHA_job_step]
-
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
 
 
-class GHA_jobs(BaseModel):
-    # to allow for dynamic key names
-    __root__: Dict[str, GHA_job_id]
+GHA_jobs = RootModel[Dict[str, GHA_job_id]]
 
 
 class GHA(BaseModel):
     name: str
     on: GHA_on
-    env: Optional[Dict[str, str]]
+    env: Optional[Dict[str, str]] = None
     jobs: GHA_jobs
 
 
 class NebariOps(GHA):
     pass
 
 
@@ -200,31 +185,23 @@
 ### GITHUB ACTION WORKFLOWS ###
 
 
 def checkout_image_step():
     return GHA_job_step(
         name="Checkout Image",
         uses="actions/checkout@v3",
-        with_={
-            "token": GHA_job_steps_extras(
-                __root__="${{ secrets.REPOSITORY_ACCESS_TOKEN }}"
-            )
-        },
+        with_={"token": GHA_job_steps_extras("${{ secrets.REPOSITORY_ACCESS_TOKEN }}")},
     )
 
 
 def setup_python_step():
     return GHA_job_step(
         name="Set up Python",
         uses="actions/setup-python@v4",
-        with_={
-            "python-version": GHA_job_steps_extras(
-                __root__=LATEST_SUPPORTED_PYTHON_VERSION
-            )
-        },
+        with_={"python-version": GHA_job_steps_extras(LATEST_SUPPORTED_PYTHON_VERSION)},
     )
 
 
 def setup_gcloud():
     return GHA_job_step(
         name="Setup gcloud",
         uses="google-github-actions/auth@v1",
@@ -238,15 +215,15 @@
     return GHA_job_step(name="Install Nebari", run=pip_install_nebari(nebari_version))
 
 
 def gen_nebari_ops(config):
     env_vars = gha_env_vars(config)
 
     push = GHA_on_extras(branches=[config.ci_cd.branch], paths=["nebari-config.yaml"])
-    on = GHA_on(__root__={"push": push})
+    on = GHA_on({"push": push})
 
     step1 = checkout_image_step()
     step2 = setup_python_step()
     step3 = install_nebari_step(config.nebari_version)
     gha_steps = [step1, step2, step3]
 
     if config.provider == schema.ProviderEnum.gcp:
@@ -268,15 +245,15 @@
             "git config user.name 'github action' ; "
             "git add ./.gitignore ./.github ./stages; "
             "git diff --quiet && git diff --staged --quiet || (git commit -m '${{ env.COMMIT_MSG }}') ; "
             f"git push origin {config.ci_cd.branch}"
         ),
         env={
             "COMMIT_MSG": GHA_job_steps_extras(
-                __root__="nebari-config.yaml automated commit: ${{ github.sha }}"
+                "nebari-config.yaml automated commit: ${{ github.sha }}"
             )
         },
     )
     if config.ci_cd.commit_render:
         gha_steps.append(step5)
 
     for step in config.ci_cd.after_script:
@@ -287,15 +264,15 @@
         runs_on_="ubuntu-latest",
         permissions={
             "id-token": "write",
             "contents": "read",
         },
         steps=gha_steps,
     )
-    jobs = GHA_jobs(__root__={"build": job1})
+    jobs = GHA_jobs({"build": job1})
 
     return NebariOps(
         name="nebari auto update",
         on=on,
         env=env_vars,
         jobs=jobs,
     )
@@ -308,39 +285,37 @@
         env_vars["NEBARI_GH_BRANCH"] = "${{ secrets.NEBARI_GH_BRANCH }}"
     else:
         env_vars = None
 
     pull_request = GHA_on_extras(
         branches=[config.ci_cd.branch], paths=["nebari-config.yaml"]
     )
-    on = GHA_on(__root__={"pull_request": pull_request})
+    on = GHA_on({"pull_request": pull_request})
 
     step1 = checkout_image_step()
     step2 = setup_python_step()
     step3 = install_nebari_step(config.nebari_version)
 
     step4_envs = {
-        "PR_NUMBER": GHA_job_steps_extras(__root__="${{ github.event.number }}"),
-        "REPO_NAME": GHA_job_steps_extras(__root__="${{ github.repository }}"),
-        "GITHUB_TOKEN": GHA_job_steps_extras(
-            __root__="${{ secrets.REPOSITORY_ACCESS_TOKEN }}"
-        ),
+        "PR_NUMBER": GHA_job_steps_extras("${{ github.event.number }}"),
+        "REPO_NAME": GHA_job_steps_extras("${{ github.repository }}"),
+        "GITHUB_TOKEN": GHA_job_steps_extras("${{ secrets.REPOSITORY_ACCESS_TOKEN }}"),
     }
 
     step4 = GHA_job_step(
         name="Nebari Lintify",
         run="nebari validate --config nebari-config.yaml --enable-commenting",
         env=step4_envs,
     )
 
     job1 = GHA_job_id(
         name="nebari", runs_on_="ubuntu-latest", steps=[step1, step2, step3, step4]
     )
     jobs = GHA_jobs(
-        __root__={
+        {
             "nebari-validate": job1,
         }
     )
 
     return NebariLinter(
         name="nebari linter",
         on=on,
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/provider/cicd/gitlab.py` & `nebari-2024.5.1rc1/src/_nebari/provider/cicd/gitlab.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 from typing import Dict, List, Optional, Union
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field, RootModel
 
 from _nebari.constants import LATEST_SUPPORTED_PYTHON_VERSION
 from _nebari.provider.cicd.common import pip_install_nebari
 
-
-class GLCI_extras(BaseModel):
-    # to allow for dynamic key names
-    __root__: Union[str, float, int]
+GLCI_extras = RootModel[Union[str, float, int]]
 
 
 class GLCI_image(BaseModel):
     name: str
-    entrypoint: Optional[str]
+    entrypoint: Optional[str] = None
 
 
 class GLCI_rules(BaseModel):
     if_: Optional[str] = Field(alias="if")
-    changes: Optional[List[str]]
-
-    class Config:
-        allow_population_by_field_name = True
+    changes: Optional[List[str]] = None
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class GLCI_job(BaseModel):
-    image: Optional[Union[str, GLCI_image]]
-    variables: Optional[Dict[str, str]]
-    before_script: Optional[List[str]]
-    after_script: Optional[List[str]]
+    image: Optional[Union[str, GLCI_image]] = None
+    variables: Optional[Dict[str, str]] = None
+    before_script: Optional[List[str]] = None
+    after_script: Optional[List[str]] = None
     script: List[str]
-    rules: Optional[List[GLCI_rules]]
+    rules: Optional[List[GLCI_rules]] = None
 
 
-class GLCI(BaseModel):
-    __root__: Dict[str, GLCI_job]
+GLCI = RootModel[Dict[str, GLCI_job]]
 
 
 def gen_gitlab_ci(config):
     render_vars = {
         "COMMIT_MSG": "nebari-config.yaml automated commit: {{ '$CI_COMMIT_SHA' }}",
     }
 
@@ -72,11 +66,11 @@
         before_script=config.ci_cd.before_script,
         after_script=config.ci_cd.after_script,
         script=script,
         rules=rules,
     )
 
     return GLCI(
-        __root__={
+        {
             "render-nebari": render_nebari,
         }
     )
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/provider/cicd/linter.py` & `nebari-2024.5.1rc1/src/_nebari/provider/cicd/linter.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/provider/cloud/amazon_web_services.py` & `nebari-2024.5.1rc1/src/_nebari/provider/cloud/amazon_web_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,33 +3,26 @@
 import re
 import time
 from typing import Dict, List, Optional
 
 import boto3
 from botocore.exceptions import ClientError, EndpointConnectionError
 
-from _nebari import constants
+from _nebari.constants import AWS_ENV_DOCS
 from _nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
+from _nebari.utils import check_environment_variables
 from nebari import schema
 
 MAX_RETRIES = 5
 DELAY = 5
 
 
-def check_credentials():
-    """Check for AWS credentials are set in the environment."""
-    for variable in {
-        "AWS_ACCESS_KEY_ID",
-        "AWS_SECRET_ACCESS_KEY",
-    }:
-        if variable not in os.environ:
-            raise ValueError(
-                f"""Missing the following required environment variable: {variable}\n
-                Please see the documentation for more information: {constants.AWS_ENV_DOCS}"""
-            )
+def check_credentials() -> None:
+    required_variables = {"AWS_ACCESS_KEY_ID", "AWS_SECRET_ACCESS_KEY"}
+    check_environment_variables(required_variables, AWS_ENV_DOCS)
 
 
 @functools.lru_cache()
 def aws_session(
     region: Optional[str] = None, digitalocean_region: Optional[str] = None
 ) -> boto3.Session:
     """Create a boto3 session."""
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/provider/cloud/azure_cloud.py` & `nebari-2024.5.1rc1/src/_nebari/provider/cloud/azure_cloud.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,52 +5,42 @@
 from typing import Dict
 
 from azure.core.exceptions import ResourceNotFoundError
 from azure.identity import DefaultAzureCredential
 from azure.mgmt.containerservice import ContainerServiceClient
 from azure.mgmt.resource import ResourceManagementClient
 
-from _nebari import constants
+from _nebari.constants import AZURE_ENV_DOCS
 from _nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
 from _nebari.utils import (
     AZURE_TF_STATE_RESOURCE_GROUP_SUFFIX,
+    check_environment_variables,
     construct_azure_resource_group_name,
 )
 from nebari import schema
 
 logger = logging.getLogger("azure")
 logger.setLevel(logging.ERROR)
 
 DURATION = 10
 RETRIES = 10
 
 
-def check_credentials():
-    """Check if credentials are valid."""
-
-    required_variables = {
-        "ARM_CLIENT_ID": os.environ.get("ARM_CLIENT_ID", None),
-        "ARM_SUBSCRIPTION_ID": os.environ.get("ARM_SUBSCRIPTION_ID", None),
-        "ARM_TENANT_ID": os.environ.get("ARM_TENANT_ID", None),
-    }
-    arm_client_secret = os.environ.get("ARM_CLIENT_SECRET", None)
-
-    if not all(required_variables.values()):
-        raise ValueError(
-            f"""Missing the following required environment variables: {required_variables}\n
-            Please see the documentation for more information: {constants.AZURE_ENV_DOCS}"""
-        )
+def check_credentials() -> DefaultAzureCredential:
+    required_variables = {"ARM_CLIENT_ID", "ARM_SUBSCRIPTION_ID", "ARM_TENANT_ID"}
+    check_environment_variables(required_variables, AZURE_ENV_DOCS)
 
+    optional_variable = "ARM_CLIENT_SECRET"
+    arm_client_secret = os.environ.get(optional_variable, None)
     if arm_client_secret:
         logger.info("Authenticating as a service principal.")
-        return DefaultAzureCredential()
     else:
-        logger.info("No ARM_CLIENT_SECRET environment variable found.")
+        logger.info(f"No {optional_variable} environment variable found.")
         logger.info("Allowing Azure SDK to authenticate using OIDC or other methods.")
-        return DefaultAzureCredential()
+    return DefaultAzureCredential()
 
 
 @functools.lru_cache()
 def initiate_container_service_client():
     subscription_id = os.environ.get("ARM_SUBSCRIPTION_ID", None)
     credentials = check_credentials()
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/provider/cloud/digital_ocean.py` & `nebari-2024.5.1rc1/src/_nebari/provider/cloud/digital_ocean.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,32 +3,28 @@
 import tempfile
 import typing
 
 import kubernetes.client
 import kubernetes.config
 import requests
 
-from _nebari import constants
+from _nebari.constants import DO_ENV_DOCS
 from _nebari.provider.cloud.amazon_web_services import aws_delete_s3_bucket
 from _nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
-from _nebari.utils import set_do_environment
+from _nebari.utils import check_environment_variables, set_do_environment
 from nebari import schema
 
 
-def check_credentials():
-    for variable in {
+def check_credentials() -> None:
+    required_variables = {
+        "DIGITALOCEAN_TOKEN",
         "SPACES_ACCESS_KEY_ID",
         "SPACES_SECRET_ACCESS_KEY",
-        "DIGITALOCEAN_TOKEN",
-    }:
-        if variable not in os.environ:
-            raise ValueError(
-                f"""Missing the following required environment variable: {variable}\n
-                Please see the documentation for more information: {constants.DO_ENV_DOCS}"""
-            )
+    }
+    check_environment_variables(required_variables, DO_ENV_DOCS)
 
 
 def digital_ocean_request(url, method="GET", json=None):
     BASE_DIGITALOCEAN_URL = "https://api.digitalocean.com/v2/"
 
     for name in {"DIGITALOCEAN_TOKEN"}:
         if name not in os.environ:
@@ -59,15 +55,15 @@
     return _kubernetes_options()["options"]["sizes"]
 
 
 def regions():
     return _kubernetes_options()["options"]["regions"]
 
 
-def kubernetes_versions(region) -> typing.List[str]:
+def kubernetes_versions() -> typing.List[str]:
     """Return list of available kubernetes supported by cloud provider. Sorted from oldest to latest."""
     supported_kubernetes_versions = sorted(
         [_["slug"].split("-")[0] for _ in _kubernetes_options()["options"]["versions"]]
     )
     filtered_versions = filter_by_highest_supported_k8s_version(
         supported_kubernetes_versions
     )
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/provider/cloud/google_cloud.py` & `nebari-2024.5.1rc1/src/_nebari/provider/cloud/google_cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 import functools
 import json
-import os
 import subprocess
 from typing import Dict, List, Set
 
-from _nebari import constants
+from _nebari.constants import GCP_ENV_DOCS
 from _nebari.provider.cloud.commons import filter_by_highest_supported_k8s_version
+from _nebari.utils import check_environment_variables
 from nebari import schema
 
 
-def check_credentials():
-    for variable in {"GOOGLE_CREDENTIALS", "PROJECT_ID"}:
-        if variable not in os.environ:
-            raise ValueError(
-                f"""Missing the following required environment variable: {variable}\n
-                Please see the documentation for more information: {constants.GCP_ENV_DOCS}"""
-            )
+def check_credentials() -> None:
+    required_variables = {"GOOGLE_CREDENTIALS", "PROJECT_ID"}
+    check_environment_variables(required_variables, GCP_ENV_DOCS)
 
 
 @functools.lru_cache()
 def projects() -> Dict[str, str]:
     """Return a dict of available projects."""
     check_credentials()
     output = subprocess.check_output(
@@ -278,15 +274,15 @@
     }
     activated = activated_services()
     common = required.intersection(activated)
     missing = required.difference(common)
     if missing:
         raise ValueError(
             f"""Missing required services: {missing}\n
-            Please see the documentation for more information: {constants.GCP_ENV_DOCS}"""
+            Please see the documentation for more information: {GCP_ENV_DOCS}"""
         )
 
 
 # Getting pricing data could come from here
 # https://cloudpricingcalculator.appspot.com/static/data/pricelist.json
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/provider/dns/cloudflare.py` & `nebari-2024.5.1rc1/src/_nebari/provider/dns/cloudflare.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/provider/oauth/auth0.py` & `nebari-2024.5.1rc1/src/_nebari/provider/oauth/auth0.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/base.py` & `nebari-2024.5.1rc1/src/_nebari/stages/base.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/tf_objects.py` & `nebari-2024.5.1rc1/src/_nebari/stages/tf_objects.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/bootstrap/__init__.py` & `nebari-2024.5.1rc1/src/_nebari/stages/bootstrap/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     def render(self) -> Dict[str, str]:
         contents = {}
         if self.config.ci_cd.type != CiEnum.none:
             for fn, workflow in gen_cicd(self.config).items():
                 stream = io.StringIO()
                 schema.yaml.dump(
-                    workflow.dict(
+                    workflow.model_dump(
                         by_alias=True, exclude_unset=True, exclude_defaults=True
                     ),
                     stream,
                 )
                 contents.update({fn: stream.getvalue()})
 
         contents.update(gen_gitignore())
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/__init__.py` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import contextlib
 import inspect
 import os
 import pathlib
 import re
 import sys
 import tempfile
-from typing import Any, Dict, List, Optional, Tuple, Type, Union
+from typing import Annotated, Any, Dict, List, Optional, Tuple, Type, Union
 
-import pydantic
+from pydantic import Field, field_validator, model_validator
 
 from _nebari import constants
 from _nebari.provider import terraform
 from _nebari.provider.cloud import (
     amazon_web_services,
     azure_cloud,
     digital_ocean,
@@ -30,15 +30,15 @@
 
 def get_kubeconfig_filename():
     return str(pathlib.Path(tempfile.gettempdir()) / "NEBARI_KUBECONFIG")
 
 
 class LocalInputVars(schema.Base):
     kubeconfig_filename: str = get_kubeconfig_filename()
-    kube_context: Optional[str]
+    kube_context: Optional[str] = None
 
 
 class ExistingInputVars(schema.Base):
     kube_context: str
 
 
 class DigitalOceanNodeGroup(schema.Base):
@@ -53,27 +53,22 @@
     region: str
     tags: List[str]
     kubernetes_version: str
     node_groups: Dict[str, DigitalOceanNodeGroup]
     kubeconfig_filename: str = get_kubeconfig_filename()
 
 
-class GCPGuestAccelerators(schema.Base):
-    name: str
-    count: int
-
-
 class GCPNodeGroupInputVars(schema.Base):
     name: str
     instance_type: str
     min_size: int
     max_size: int
     labels: Dict[str, str]
     preemptible: bool
-    guest_accelerators: List[GCPGuestAccelerators]
+    guest_accelerators: List["GCPGuestAccelerator"]
 
 
 class GCPPrivateClusterConfig(schema.Base):
     enable_private_nodes: bool
     enable_private_endpoint: bool
     master_ipv4_cidr_block: str
 
@@ -87,18 +82,18 @@
     node_groups: List[GCPNodeGroupInputVars]
     kubeconfig_filename: str = get_kubeconfig_filename()
     tags: List[str]
     kubernetes_version: str
     release_channel: str
     networking_mode: str
     network: str
-    subnetwork: str = None
-    ip_allocation_policy: Dict[str, str] = None
-    master_authorized_networks_config: Dict[str, str] = None
-    private_cluster_config: GCPPrivateClusterConfig = None
+    subnetwork: Optional[str] = None
+    ip_allocation_policy: Optional[Dict[str, str]] = None
+    master_authorized_networks_config: Optional[Dict[str, str]] = None
+    private_cluster_config: Optional[GCPPrivateClusterConfig] = None
 
 
 class AzureNodeGroupInputVars(schema.Base):
     instance: str
     min_nodes: int
     max_nodes: int
 
@@ -108,19 +103,19 @@
     environment: str
     region: str
     kubeconfig_filename: str = get_kubeconfig_filename()
     kubernetes_version: str
     node_groups: Dict[str, AzureNodeGroupInputVars]
     resource_group_name: str
     node_resource_group_name: str
-    vnet_subnet_id: str = None
+    vnet_subnet_id: Optional[str] = None
     private_cluster_enabled: bool
     tags: Dict[str, str] = {}
-    max_pods: int = None
-    network_profile: Dict[str, str] = None
+    max_pods: Optional[int] = None
+    network_profile: Optional[Dict[str, str]] = None
 
 
 class AWSNodeGroupInputVars(schema.Base):
     name: str
     instance_type: str
     gpu: bool = False
     min_size: int
@@ -129,16 +124,16 @@
     single_subnet: bool
     permissions_boundary: Optional[str] = None
 
 
 class AWSInputVars(schema.Base):
     name: str
     environment: str
-    existing_security_group_id: str = None
-    existing_subnet_ids: List[str] = None
+    existing_security_group_id: Optional[str] = None
+    existing_subnet_ids: Optional[List[str]] = None
     region: str
     kubernetes_version: str
     node_groups: List[AWSNodeGroupInputVars]
     availability_zones: List[str]
     vpc_cidr_block: str
     permissions_boundary: Optional[str] = None
     kubeconfig_filename: str = get_kubeconfig_filename()
@@ -176,15 +171,19 @@
         return {
             group: {"key": "doks.digitalocean.com/node-pool", "value": group}
             for group in ["general", "user", "worker"]
         }
     elif config.provider == schema.ProviderEnum.existing:
         return config.existing.node_selectors
     else:
-        return config.local.dict()["node_selectors"]
+        return config.local.model_dump()["node_selectors"]
+
+
+def node_groups_to_dict(node_groups):
+    return {ng_name: ng.model_dump() for ng_name, ng in node_groups.items()}
 
 
 @contextlib.contextmanager
 def kubernetes_provider_context(kubernetes_credentials: Dict[str, str]):
     credential_mapping = {
         "config_path": "KUBE_CONFIG_PATH",
         "config_context": "KUBE_CTX",
@@ -215,77 +214,65 @@
     """Representation of a node group with Digital Ocean
 
     - Kubernetes limits: https://docs.digitalocean.com/products/kubernetes/details/limits/
     - Available instance types: https://slugs.do-api.dev/
     """
 
     instance: str
-    min_nodes: pydantic.conint(ge=1) = 1
-    max_nodes: pydantic.conint(ge=1) = 1
+    min_nodes: Annotated[int, Field(ge=1)] = 1
+    max_nodes: Annotated[int, Field(ge=1)] = 1
 
 
 DEFAULT_DO_NODE_GROUPS = {
     "general": DigitalOceanNodeGroup(instance="g-8vcpu-32gb", min_nodes=1, max_nodes=1),
     "user": DigitalOceanNodeGroup(instance="g-4vcpu-16gb", min_nodes=1, max_nodes=5),
     "worker": DigitalOceanNodeGroup(instance="g-4vcpu-16gb", min_nodes=1, max_nodes=5),
 }
 
 
 class DigitalOceanProvider(schema.Base):
     region: str
-    kubernetes_version: str
+    kubernetes_version: Optional[str] = None
     # Digital Ocean image slugs are listed here https://slugs.do-api.dev/
     node_groups: Dict[str, DigitalOceanNodeGroup] = DEFAULT_DO_NODE_GROUPS
     tags: Optional[List[str]] = []
 
-    @pydantic.validator("region")
-    def _validate_region(cls, value):
+    @model_validator(mode="before")
+    @classmethod
+    def _check_input(cls, data: Any) -> Any:
         digital_ocean.check_credentials()
 
+        # check if region is valid
         available_regions = set(_["slug"] for _ in digital_ocean.regions())
-        if value not in available_regions:
+        if data["region"] not in available_regions:
             raise ValueError(
-                f"Digital Ocean region={value} is not one of {available_regions}"
+                f"Digital Ocean region={data['region']} is not one of {available_regions}"
             )
-        return value
-
-    @pydantic.validator("node_groups")
-    def _validate_node_group(cls, value):
-        digital_ocean.check_credentials()
 
-        available_instances = {_["slug"] for _ in digital_ocean.instances()}
-        for name, node_group in value.items():
-            if node_group.instance not in available_instances:
-                raise ValueError(
-                    f"Digital Ocean instance {node_group.instance} not one of available instance types={available_instances}"
-                )
-
-        return value
-
-    @pydantic.root_validator
-    def _validate_kubernetes_version(cls, values):
-        digital_ocean.check_credentials()
-
-        if "region" not in values:
-            raise ValueError("Region required in order to set kubernetes_version")
-
-        available_kubernetes_versions = digital_ocean.kubernetes_versions(
-            values["region"]
-        )
-        assert available_kubernetes_versions
-        if (
-            values["kubernetes_version"] is not None
-            and values["kubernetes_version"] not in available_kubernetes_versions
-        ):
+        # check if kubernetes version is valid
+        available_kubernetes_versions = digital_ocean.kubernetes_versions()
+        if len(available_kubernetes_versions) == 0:
             raise ValueError(
-                f"\nInvalid `kubernetes-version` provided: {values['kubernetes_version']}.\nPlease select from one of the following supported Kubernetes versions: {available_kubernetes_versions} or omit flag to use latest Kubernetes version available."
+                "Request to Digital Ocean for available Kubernetes versions failed."
             )
-        else:
-            values["kubernetes_version"] = available_kubernetes_versions[-1]
-        return values
+        if data["kubernetes_version"] is None:
+            data["kubernetes_version"] = available_kubernetes_versions[-1]
+        elif data["kubernetes_version"] not in available_kubernetes_versions:
+            raise ValueError(
+                f"\nInvalid `kubernetes-version` provided: {data['kubernetes_version']}.\nPlease select from one of the following supported Kubernetes versions: {available_kubernetes_versions} or omit flag to use latest Kubernetes version available."
+            )
+
+        available_instances = {_["slug"] for _ in digital_ocean.instances()}
+        if "node_groups" in data:
+            for _, node_group in data["node_groups"].items():
+                if node_group["instance"] not in available_instances:
+                    raise ValueError(
+                        f"Digital Ocean instance {node_group.instance} not one of available instance types={available_instances}"
+                    )
+        return data
 
 
 class GCPIPAllocationPolicy(schema.Base):
     cluster_secondary_range_name: str
     services_secondary_range_name: str
     cluster_ipv4_cidr_block: str
     services_ipv4_cidr_block: str
@@ -310,21 +297,21 @@
     """
     See general information regarding GPU support at:
     # TODO: replace with nebari.dev new URL
     https://docs.nebari.dev/en/stable/source/admin_guide/gpu.html?#add-gpu-node-group
     """
 
     name: str
-    count: pydantic.conint(ge=1) = 1
+    count: Annotated[int, Field(ge=1)] = 1
 
 
 class GCPNodeGroup(schema.Base):
     instance: str
-    min_nodes: pydantic.conint(ge=0) = 0
-    max_nodes: pydantic.conint(ge=1) = 1
+    min_nodes: Annotated[int, Field(ge=0)] = 0
+    max_nodes: Annotated[int, Field(ge=1)] = 1
     preemptible: bool = False
     labels: Dict[str, str] = {}
     guest_accelerators: List[GCPGuestAccelerator] = []
 
 
 DEFAULT_GCP_NODE_GROUPS = {
     "general": GCPNodeGroup(instance="n1-standard-8", min_nodes=1, max_nodes=1),
@@ -344,39 +331,31 @@
     networking_mode: str = "ROUTE"
     network: str = "default"
     subnetwork: Optional[Union[str, None]] = None
     ip_allocation_policy: Optional[Union[GCPIPAllocationPolicy, None]] = None
     master_authorized_networks_config: Optional[Union[GCPCIDRBlock, None]] = None
     private_cluster_config: Optional[Union[GCPPrivateClusterConfig, None]] = None
 
-    @pydantic.root_validator
-    def validate_all(cls, values):
-        region = values.get("region")
-        project_id = values.get("project")
-
-        if project_id is None:
-            raise ValueError("The `google_cloud_platform.project` field is required.")
-
-        if region is None:
-            raise ValueError("The `google_cloud_platform.region` field is required.")
-
-        # validate region
-        google_cloud.validate_region(region)
-
-        # validate kubernetes version
-        kubernetes_version = values.get("kubernetes_version")
-        available_kubernetes_versions = google_cloud.kubernetes_versions(region)
-        if kubernetes_version is None:
-            values["kubernetes_version"] = available_kubernetes_versions[-1]
-        elif kubernetes_version not in available_kubernetes_versions:
+    @model_validator(mode="before")
+    @classmethod
+    def _check_input(cls, data: Any) -> Any:
+        google_cloud.check_credentials()
+        avaliable_regions = google_cloud.regions()
+        if data["region"] not in avaliable_regions:
             raise ValueError(
-                f"\nInvalid `kubernetes-version` provided: {values['kubernetes_version']}.\nPlease select from one of the following supported Kubernetes versions: {available_kubernetes_versions} or omit flag to use latest Kubernetes version available."
+                f"Google Cloud region={data['region']} is not one of {avaliable_regions}"
             )
 
-        return values
+        available_kubernetes_versions = google_cloud.kubernetes_versions(data["region"])
+        print(available_kubernetes_versions)
+        if data["kubernetes_version"] not in available_kubernetes_versions:
+            raise ValueError(
+                f"\nInvalid `kubernetes-version` provided: {data['kubernetes_version']}.\nPlease select from one of the following supported Kubernetes versions: {available_kubernetes_versions} or omit flag to use latest Kubernetes version available."
+            )
+        return data
 
 
 class AzureNodeGroup(schema.Base):
     instance: str
     min_nodes: int
     max_nodes: int
 
@@ -386,38 +365,46 @@
     "user": AzureNodeGroup(instance="Standard_D4_v3", min_nodes=0, max_nodes=5),
     "worker": AzureNodeGroup(instance="Standard_D4_v3", min_nodes=0, max_nodes=5),
 }
 
 
 class AzureProvider(schema.Base):
     region: str
-    kubernetes_version: str
+    kubernetes_version: Optional[str] = None
     storage_account_postfix: str
-    resource_group_name: str = None
+    resource_group_name: Optional[str] = None
     node_groups: Dict[str, AzureNodeGroup] = DEFAULT_AZURE_NODE_GROUPS
     storage_account_postfix: str
-    vnet_subnet_id: Optional[Union[str, None]] = None
+    vnet_subnet_id: Optional[str] = None
     private_cluster_enabled: bool = False
     resource_group_name: Optional[str] = None
     tags: Optional[Dict[str, str]] = {}
     network_profile: Optional[Dict[str, str]] = None
     max_pods: Optional[int] = None
 
-    @pydantic.validator("kubernetes_version")
-    def _validate_kubernetes_version(cls, value):
+    @model_validator(mode="before")
+    @classmethod
+    def _check_credentials(cls, data: Any) -> Any:
+        azure_cloud.check_credentials()
+        return data
+
+    @field_validator("kubernetes_version")
+    @classmethod
+    def _validate_kubernetes_version(cls, value: Optional[str]) -> str:
         available_kubernetes_versions = azure_cloud.kubernetes_versions()
         if value is None:
             value = available_kubernetes_versions[-1]
         elif value not in available_kubernetes_versions:
             raise ValueError(
                 f"\nInvalid `kubernetes-version` provided: {value}.\nPlease select from one of the following supported Kubernetes versions: {available_kubernetes_versions} or omit flag to use latest Kubernetes version available."
             )
         return value
 
-    @pydantic.validator("resource_group_name")
+    @field_validator("resource_group_name")
+    @classmethod
     def _validate_resource_group_name(cls, value):
         if value is None:
             return value
         length = len(value) + len(AZURE_NODE_RESOURCE_GROUP_SUFFIX)
         if length < 1 or length > 90:
             raise ValueError(
                 f"Azure Resource Group name must be between 1 and 90 characters long, when combined with the suffix `{AZURE_NODE_RESOURCE_GROUP_SUFFIX}`."
@@ -427,17 +414,18 @@
                 "Azure Resource Group name can only contain alphanumerics, underscores, parentheses, hyphens, and periods."
             )
         if value[-1] == ".":
             raise ValueError("Azure Resource Group name can't end with a period.")
 
         return value
 
-    @pydantic.validator("tags")
-    def _validate_tags(cls, tags):
-        return azure_cloud.validate_tags(tags)
+    @field_validator("tags")
+    @classmethod
+    def _validate_tags(cls, value: Optional[Dict[str, str]]) -> Dict[str, str]:
+        return value if value is None else azure_cloud.validate_tags(value)
 
 
 class AWSNodeGroup(schema.Base):
     instance: str
     min_nodes: int = 0
     max_nodes: int
     gpu: bool = False
@@ -457,66 +445,83 @@
 
 
 class AmazonWebServicesProvider(schema.Base):
     region: str
     kubernetes_version: str
     availability_zones: Optional[List[str]]
     node_groups: Dict[str, AWSNodeGroup] = DEFAULT_AWS_NODE_GROUPS
-    existing_subnet_ids: List[str] = None
-    existing_security_group_id: str = None
+    existing_subnet_ids: Optional[List[str]] = None
+    existing_security_group_id: Optional[str] = None
     vpc_cidr_block: str = "10.10.0.0/16"
     permissions_boundary: Optional[str] = None
     tags: Optional[Dict[str, str]] = {}
 
-    @pydantic.root_validator
-    def validate_all(cls, values):
-        region = values.get("region")
-        if region is None:
-            raise ValueError("The `amazon_web_services.region` field is required.")
-
-        # validate region
-        amazon_web_services.validate_region(region)
-
-        # validate kubernetes version
-        kubernetes_version = values.get("kubernetes_version")
-        available_kubernetes_versions = amazon_web_services.kubernetes_versions(region)
-        if kubernetes_version is None:
-            values["kubernetes_version"] = available_kubernetes_versions[-1]
-        elif kubernetes_version not in available_kubernetes_versions:
+    @model_validator(mode="before")
+    @classmethod
+    def _check_input(cls, data: Any) -> Any:
+        amazon_web_services.check_credentials()
+
+        # check if region is valid
+        available_regions = amazon_web_services.regions(data["region"])
+        if data["region"] not in available_regions:
             raise ValueError(
-                f"\nInvalid `kubernetes-version` provided: {values['kubernetes_version']}.\nPlease select from one of the following supported Kubernetes versions: {available_kubernetes_versions} or omit flag to use latest Kubernetes version available."
+                f"Amazon Web Services region={data['region']} is not one of {available_regions}"
             )
 
-        # validate node groups
-        node_groups = values["node_groups"]
-        available_instances = amazon_web_services.instances(region)
-        for name, node_group in node_groups.items():
-            if node_group.instance not in available_instances:
-                raise ValueError(
-                    f"Instance {node_group.instance} not available out of available instances {available_instances.keys()}"
-                )
+        # check if kubernetes version is valid
+        available_kubernetes_versions = amazon_web_services.kubernetes_versions(
+            data["region"]
+        )
+        if len(available_kubernetes_versions) == 0:
+            raise ValueError("Request to AWS for available Kubernetes versions failed.")
+        if data["kubernetes_version"] is None:
+            data["kubernetes_version"] = available_kubernetes_versions[-1]
+        elif data["kubernetes_version"] not in available_kubernetes_versions:
+            raise ValueError(
+                f"\nInvalid `kubernetes-version` provided: {data['kubernetes_version']}.\nPlease select from one of the following supported Kubernetes versions: {available_kubernetes_versions} or omit flag to use latest Kubernetes version available."
+            )
 
-        if values["availability_zones"] is None:
-            zones = amazon_web_services.zones(region)
-            values["availability_zones"] = list(sorted(zones))[:2]
+        # check if availability zones are valid
+        available_zones = amazon_web_services.zones(data["region"])
+        if "availability_zones" not in data:
+            data["availability_zones"] = list(sorted(available_zones))[:2]
+        else:
+            for zone in data["availability_zones"]:
+                if zone not in available_zones:
+                    raise ValueError(
+                        f"Amazon Web Services availability zone={zone} is not one of {available_zones}"
+                    )
 
-        return values
+        # check if instances are valid
+        available_instances = amazon_web_services.instances(data["region"])
+        if "node_groups" in data:
+            for _, node_group in data["node_groups"].items():
+                instance = (
+                    node_group["instance"]
+                    if hasattr(node_group, "__getitem__")
+                    else node_group.instance
+                )
+                if instance not in available_instances:
+                    raise ValueError(
+                        f"Amazon Web Services instance {node_group.instance} not one of available instance types={available_instances}"
+                    )
+        return data
 
 
 class LocalProvider(schema.Base):
-    kube_context: Optional[str]
+    kube_context: Optional[str] = None
     node_selectors: Dict[str, KeyValueDict] = {
         "general": KeyValueDict(key="kubernetes.io/os", value="linux"),
         "user": KeyValueDict(key="kubernetes.io/os", value="linux"),
         "worker": KeyValueDict(key="kubernetes.io/os", value="linux"),
     }
 
 
 class ExistingProvider(schema.Base):
-    kube_context: Optional[str]
+    kube_context: Optional[str] = None
     node_selectors: Dict[str, KeyValueDict] = {
         "general": KeyValueDict(key="kubernetes.io/os", value="linux"),
         "user": KeyValueDict(key="kubernetes.io/os", value="linux"),
         "worker": KeyValueDict(key="kubernetes.io/os", value="linux"),
     }
 
 
@@ -538,78 +543,86 @@
     schema.ProviderEnum.do: "digital_ocean",
 }
 
 provider_name_abbreviation_map: Dict[str, str] = {
     value: key.value for key, value in provider_enum_name_map.items()
 }
 
+provider_enum_default_node_groups_map: Dict[schema.ProviderEnum, Any] = {
+    schema.ProviderEnum.gcp: node_groups_to_dict(DEFAULT_GCP_NODE_GROUPS),
+    schema.ProviderEnum.aws: node_groups_to_dict(DEFAULT_AWS_NODE_GROUPS),
+    schema.ProviderEnum.azure: node_groups_to_dict(DEFAULT_AZURE_NODE_GROUPS),
+    schema.ProviderEnum.do: node_groups_to_dict(DEFAULT_DO_NODE_GROUPS),
+}
+
 
 class InputSchema(schema.Base):
-    local: Optional[LocalProvider]
-    existing: Optional[ExistingProvider]
-    google_cloud_platform: Optional[GoogleCloudPlatformProvider]
-    amazon_web_services: Optional[AmazonWebServicesProvider]
-    azure: Optional[AzureProvider]
-    digital_ocean: Optional[DigitalOceanProvider]
-
-    @pydantic.root_validator(pre=True)
-    def check_provider(cls, values):
-        if "provider" in values:
-            provider: str = values["provider"]
+    local: Optional[LocalProvider] = None
+    existing: Optional[ExistingProvider] = None
+    google_cloud_platform: Optional[GoogleCloudPlatformProvider] = None
+    amazon_web_services: Optional[AmazonWebServicesProvider] = None
+    azure: Optional[AzureProvider] = None
+    digital_ocean: Optional[DigitalOceanProvider] = None
+
+    @model_validator(mode="before")
+    @classmethod
+    def check_provider(cls, data: Any) -> Any:
+        if "provider" in data:
+            provider: str = data["provider"]
             if hasattr(schema.ProviderEnum, provider):
                 # TODO: all cloud providers has required fields, but local and existing don't.
                 #  And there is no way to initialize a model without user input here.
                 #  We preserve the original behavior here, but we should find a better way to do this.
-                if provider in ["local", "existing"] and provider not in values:
-                    values[provider] = provider_enum_model_map[provider]()
+                if provider in ["local", "existing"] and provider not in data:
+                    data[provider] = provider_enum_model_map[provider]()
             else:
                 # if the provider field is invalid, it won't be set when this validator is called
                 # so we need to check for it explicitly here, and set the `pre` to True
                 # TODO: this is a workaround, check if there is a better way to do this in Pydantic v2
                 raise ValueError(
                     f"'{provider}' is not a valid enumeration member; permitted: local, existing, do, aws, gcp, azure"
                 )
         else:
             setted_providers = [
                 provider
                 for provider in provider_name_abbreviation_map.keys()
-                if provider in values
+                if provider in data
             ]
             num_providers = len(setted_providers)
             if num_providers > 1:
                 raise ValueError(f"Multiple providers set: {setted_providers}")
             elif num_providers == 1:
-                values["provider"] = provider_name_abbreviation_map[setted_providers[0]]
+                data["provider"] = provider_name_abbreviation_map[setted_providers[0]]
             elif num_providers == 0:
-                values["provider"] = schema.ProviderEnum.local.value
-        return values
+                data["provider"] = schema.ProviderEnum.local.value
+        return data
 
 
 class NodeSelectorKeyValue(schema.Base):
     key: str
     value: str
 
 
 class KubernetesCredentials(schema.Base):
     host: str
     cluster_ca_certifiate: str
-    token: Optional[str]
-    username: Optional[str]
-    password: Optional[str]
-    client_certificate: Optional[str]
-    client_key: Optional[str]
-    config_path: Optional[str]
-    config_context: Optional[str]
+    token: Optional[str] = None
+    username: Optional[str] = None
+    password: Optional[str] = None
+    client_certificate: Optional[str] = None
+    client_key: Optional[str] = None
+    config_path: Optional[str] = None
+    config_context: Optional[str] = None
 
 
 class OutputSchema(schema.Base):
     node_selectors: Dict[str, NodeSelectorKeyValue]
     kubernetes_credentials: KubernetesCredentials
     kubeconfig_filename: str
-    nfs_endpoint: Optional[str]
+    nfs_endpoint: Optional[str] = None
 
 
 class KubernetesInfrastructureStage(NebariTerraformStage):
     """Generalized method to provision infrastructure.
 
     After successful deployment the following properties are set on
     `stage_outputs[directory]`.
@@ -689,28 +702,30 @@
                 NebariTerraformState(self.name, self.config),
             ]
         else:
             return []
 
     def input_vars(self, stage_outputs: Dict[str, Dict[str, Any]]):
         if self.config.provider == schema.ProviderEnum.local:
-            return LocalInputVars(kube_context=self.config.local.kube_context).dict()
+            return LocalInputVars(
+                kube_context=self.config.local.kube_context
+            ).model_dump()
         elif self.config.provider == schema.ProviderEnum.existing:
             return ExistingInputVars(
                 kube_context=self.config.existing.kube_context
-            ).dict()
+            ).model_dump()
         elif self.config.provider == schema.ProviderEnum.do:
             return DigitalOceanInputVars(
                 name=self.config.escaped_project_name,
                 environment=self.config.namespace,
                 region=self.config.digital_ocean.region,
                 tags=self.config.digital_ocean.tags,
                 kubernetes_version=self.config.digital_ocean.kubernetes_version,
                 node_groups=self.config.digital_ocean.node_groups,
-            ).dict()
+            ).model_dump()
         elif self.config.provider == schema.ProviderEnum.gcp:
             return GCPInputVars(
                 name=self.config.escaped_project_name,
                 environment=self.config.namespace,
                 region=self.config.google_cloud_platform.region,
                 project_id=self.config.google_cloud_platform.project,
                 availability_zones=self.config.google_cloud_platform.availability_zones,
@@ -731,15 +746,15 @@
                 release_channel=self.config.google_cloud_platform.release_channel,
                 networking_mode=self.config.google_cloud_platform.networking_mode,
                 network=self.config.google_cloud_platform.network,
                 subnetwork=self.config.google_cloud_platform.subnetwork,
                 ip_allocation_policy=self.config.google_cloud_platform.ip_allocation_policy,
                 master_authorized_networks_config=self.config.google_cloud_platform.master_authorized_networks_config,
                 private_cluster_config=self.config.google_cloud_platform.private_cluster_config,
-            ).dict()
+            ).model_dump()
         elif self.config.provider == schema.ProviderEnum.azure:
             return AzureInputVars(
                 name=self.config.escaped_project_name,
                 environment=self.config.namespace,
                 region=self.config.azure.region,
                 kubernetes_version=self.config.azure.kubernetes_version,
                 node_groups={
@@ -762,15 +777,15 @@
                     suffix=AZURE_NODE_RESOURCE_GROUP_SUFFIX,
                 ),
                 vnet_subnet_id=self.config.azure.vnet_subnet_id,
                 private_cluster_enabled=self.config.azure.private_cluster_enabled,
                 tags=self.config.azure.tags,
                 network_profile=self.config.azure.network_profile,
                 max_pods=self.config.azure.max_pods,
-            ).dict()
+            ).model_dump()
         elif self.config.provider == schema.ProviderEnum.aws:
             return AWSInputVars(
                 name=self.config.escaped_project_name,
                 environment=self.config.namespace,
                 existing_subnet_ids=self.config.amazon_web_services.existing_subnet_ids,
                 existing_security_group_id=self.config.amazon_web_services.existing_security_group_id,
                 region=self.config.amazon_web_services.region,
@@ -788,15 +803,15 @@
                     )
                     for name, node_group in self.config.amazon_web_services.node_groups.items()
                 ],
                 availability_zones=self.config.amazon_web_services.availability_zones,
                 vpc_cidr_block=self.config.amazon_web_services.vpc_cidr_block,
                 permissions_boundary=self.config.amazon_web_services.permissions_boundary,
                 tags=self.config.amazon_web_services.tags,
-            ).dict()
+            ).model_dump()
         else:
             raise ValueError(f"Unknown provider: {self.config.provider}")
 
     def check(
         self, stage_outputs: Dict[str, Dict[str, Any]], disable_prompt: bool = False
     ):
         from kubernetes import client, config
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/outputs.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/__init__.py` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import enum
 import logging
 import socket
 import sys
 import time
-import typing
-from typing import Any, Dict, List, Type
+from typing import Any, Dict, List, Optional, Type
 
 from _nebari import constants
 from _nebari.provider.dns.cloudflare import update_record
 from _nebari.stages.base import NebariTerraformStage
 from _nebari.stages.tf_objects import (
     NebariHelmProvider,
     NebariKubernetesProvider,
@@ -124,43 +123,43 @@
     def to_yaml(cls, representer, node):
         return representer.represent_str(node.value)
 
 
 class Certificate(schema.Base):
     type: CertificateEnum = CertificateEnum.selfsigned
     # existing
-    secret_name: typing.Optional[str]
+    secret_name: Optional[str] = None
     # lets-encrypt
-    acme_email: typing.Optional[str]
+    acme_email: Optional[str] = None
     acme_server: str = "https://acme-v02.api.letsencrypt.org/directory"
 
 
 class DnsProvider(schema.Base):
-    provider: typing.Optional[str]
-    auto_provision: typing.Optional[bool] = False
+    provider: Optional[str] = None
+    auto_provision: Optional[bool] = False
 
 
 class Ingress(schema.Base):
-    terraform_overrides: typing.Dict = {}
+    terraform_overrides: Dict = {}
 
 
 class InputSchema(schema.Base):
-    domain: typing.Optional[str]
+    domain: Optional[str] = None
     certificate: Certificate = Certificate()
     ingress: Ingress = Ingress()
     dns: DnsProvider = DnsProvider()
 
 
 class IngressEndpoint(schema.Base):
     ip: str
     hostname: str
 
 
 class OutputSchema(schema.Base):
-    load_balancer_address: typing.List[IngressEndpoint]
+    load_balancer_address: List[IngressEndpoint]
     domain: str
 
 
 class KubernetesIngressStage(NebariTerraformStage):
     name = "04-kubernetes-ingress"
     priority = 40
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/__init__.py` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 import sys
-import typing
-from typing import Any, Dict, List, Type, Union
+from typing import Any, Dict, List, Optional, Type
 
-import pydantic
+from pydantic import model_validator
 
 from _nebari.stages.base import NebariTerraformStage
 from _nebari.stages.tf_objects import (
     NebariHelmProvider,
     NebariKubernetesProvider,
     NebariTerraformState,
 )
 from nebari import schema
 from nebari.hookspecs import NebariStage, hookimpl
 
 
 class ExtContainerReg(schema.Base):
     enabled: bool = False
-    access_key_id: typing.Optional[str]
-    secret_access_key: typing.Optional[str]
-    extcr_account: typing.Optional[str]
-    extcr_region: typing.Optional[str]
-
-    @pydantic.root_validator
-    def enabled_must_have_fields(cls, values):
-        if values["enabled"]:
+    access_key_id: Optional[str] = None
+    secret_access_key: Optional[str] = None
+    extcr_account: Optional[str] = None
+    extcr_region: Optional[str] = None
+
+    @model_validator(mode="after")
+    def enabled_must_have_fields(self):
+        if self.enabled:
             for fldname in (
                 "access_key_id",
                 "secret_access_key",
                 "extcr_account",
                 "extcr_region",
             ):
-                if (
-                    fldname not in values
-                    or values[fldname] is None
-                    or values[fldname].strip() == ""
-                ):
+                value = getattr(self, fldname)
+                if value is None or value.strip() == "":
                     raise ValueError(
                         f"external_container_reg must contain a non-blank {fldname} when enabled is true"
                     )
-        return values
+        return self
 
 
 class InputVars(schema.Base):
     name: str
     environment: str
     cloud_provider: str
-    aws_region: Union[str, None] = None
-    external_container_reg: Union[ExtContainerReg, None] = None
+    aws_region: Optional[str] = None
+    external_container_reg: Optional[ExtContainerReg] = None
     gpu_enabled: bool = False
     gpu_node_group_names: List[str] = []
 
 
 class InputSchema(schema.Base):
     external_container_reg: ExtContainerReg = ExtContainerReg()
 
@@ -74,15 +70,15 @@
         ]
 
     def input_vars(self, stage_outputs: Dict[str, Dict[str, Any]]):
         input_vars = InputVars(
             name=self.config.project_name,
             environment=self.config.namespace,
             cloud_provider=self.config.provider.value,
-            external_container_reg=self.config.external_container_reg.dict(),
+            external_container_reg=self.config.external_container_reg.model_dump(),
         )
 
         if self.config.provider == schema.ProviderEnum.gcp:
             input_vars.gpu_enabled = any(
                 node_group.guest_accelerators
                 for node_group in self.config.google_cloud_platform.node_groups.values()
             )
@@ -93,15 +89,15 @@
                 for node_group in self.config.amazon_web_services.node_groups.values()
             )
             input_vars.gpu_node_group_names = [
                 group for group in self.config.amazon_web_services.node_groups.keys()
             ]
             input_vars.aws_region = self.config.amazon_web_services.region
 
-        return input_vars.dict()
+        return input_vars.model_dump()
 
     def check(
         self, stage_outputs: Dict[str, Dict[str, Any]], disable_prompt: bool = False
     ):
         from kubernetes import client, config
         from kubernetes.client.rest import ApiException
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 import enum
 import json
 import os
 import secrets
 import string
 import sys
 import time
-import typing
-from abc import ABC
-from typing import Any, Dict, List, Type
+from typing import Any, Dict, List, Optional, Type, Union
 
-import pydantic
+from pydantic import Field, ValidationInfo, field_validator
 
 from _nebari.stages.base import NebariTerraformStage
 from _nebari.stages.tf_objects import (
     NebariHelmProvider,
     NebariKubernetesProvider,
     NebariTerraformState,
 )
@@ -58,136 +56,145 @@
 
     @classmethod
     def to_yaml(cls, representer, node):
         return representer.represent_str(node.value)
 
 
 class GitHubConfig(schema.Base):
-    client_id: str = pydantic.Field(
-        default_factory=lambda: os.environ.get("GITHUB_CLIENT_ID")
+    client_id: str = Field(
+        default_factory=lambda: os.environ.get("GITHUB_CLIENT_ID"),
+        validate_default=True,
     )
-    client_secret: str = pydantic.Field(
-        default_factory=lambda: os.environ.get("GITHUB_CLIENT_SECRET")
+    client_secret: str = Field(
+        default_factory=lambda: os.environ.get("GITHUB_CLIENT_SECRET"),
+        validate_default=True,
     )
 
-    @pydantic.root_validator(allow_reuse=True)
-    def validate_required(cls, values):
-        missing = []
-        for k, v in {
+    @field_validator("client_id", "client_secret", mode="before")
+    @classmethod
+    def validate_credentials(cls, value: Optional[str], info: ValidationInfo) -> str:
+        variable_mapping = {
             "client_id": "GITHUB_CLIENT_ID",
             "client_secret": "GITHUB_CLIENT_SECRET",
-        }.items():
-            if not values.get(k):
-                missing.append(v)
-
-        if len(missing) > 0:
+        }
+        if value is None:
             raise ValueError(
-                f"Missing the following required environment variable(s): {', '.join(missing)}"
+                f"Missing the following required environment variable: {variable_mapping[info.field_name]}"
             )
-
-        return values
+        return value
 
 
 class Auth0Config(schema.Base):
-    client_id: str = pydantic.Field(
-        default_factory=lambda: os.environ.get("AUTH0_CLIENT_ID")
+    client_id: str = Field(
+        default_factory=lambda: os.environ.get("AUTH0_CLIENT_ID"),
+        validate_default=True,
     )
-    client_secret: str = pydantic.Field(
-        default_factory=lambda: os.environ.get("AUTH0_CLIENT_SECRET")
+    client_secret: str = Field(
+        default_factory=lambda: os.environ.get("AUTH0_CLIENT_SECRET"),
+        validate_default=True,
     )
-    auth0_subdomain: str = pydantic.Field(
-        default_factory=lambda: os.environ.get("AUTH0_DOMAIN")
+    auth0_subdomain: str = Field(
+        default_factory=lambda: os.environ.get("AUTH0_DOMAIN"),
+        validate_default=True,
     )
 
-    @pydantic.root_validator(allow_reuse=True)
-    def validate_required(cls, values):
-        missing = []
-        for k, v in {
+    @field_validator("client_id", "client_secret", "auth0_subdomain", mode="before")
+    @classmethod
+    def validate_credentials(cls, value: Optional[str], info: ValidationInfo) -> str:
+        variable_mapping = {
             "client_id": "AUTH0_CLIENT_ID",
             "client_secret": "AUTH0_CLIENT_SECRET",
             "auth0_subdomain": "AUTH0_DOMAIN",
-        }.items():
-            if not values.get(k):
-                missing.append(v)
-
-        if len(missing) > 0:
+        }
+        if value is None:
             raise ValueError(
-                f"Missing the following required environment variable(s): {', '.join(missing)}"
+                f"Missing the following required environment variable: {variable_mapping[info.field_name]} "
             )
+        return value
 
-        return values
-
-
-class Authentication(schema.Base, ABC):
-    _types: typing.Dict[str, type] = {}
 
+class BaseAuthentication(schema.Base):
     type: AuthenticationEnum
 
-    # Based on https://github.com/samuelcolvin/pydantic/issues/2177#issuecomment-739578307
 
-    # This allows type field to determine which subclass of Authentication should be used for validation.
+class PasswordAuthentication(BaseAuthentication):
+    type: AuthenticationEnum = AuthenticationEnum.password
 
-    # Used to register automatically all the submodels in `_types`.
-    def __init_subclass__(cls):
-        cls._types[cls._typ.value] = cls
 
-    @classmethod
-    def __get_validators__(cls):
-        yield cls.validate
+class Auth0Authentication(BaseAuthentication):
+    type: AuthenticationEnum = AuthenticationEnum.auth0
+    config: Auth0Config = Field(default_factory=lambda: Auth0Config())
 
-    @classmethod
-    def validate(cls, value: typing.Dict[str, typing.Any]) -> "Authentication":
-        if "type" not in value:
-            raise ValueError("type field is missing from security.authentication")
 
-        specified_type = value.get("type")
-        sub_class = cls._types.get(specified_type, None)
+class GitHubAuthentication(BaseAuthentication):
+    type: AuthenticationEnum = AuthenticationEnum.github
+    config: GitHubConfig = Field(default_factory=lambda: GitHubConfig())
 
-        if not sub_class:
-            raise ValueError(
-                f"No registered Authentication type called {specified_type}"
-            )
 
-        # init with right submodel
-        return sub_class(**value)
+Authentication = Union[
+    PasswordAuthentication, Auth0Authentication, GitHubAuthentication
+]
 
 
 def random_secure_string(
     length: int = 16, chars: str = string.ascii_lowercase + string.digits
 ):
     return "".join(secrets.choice(chars) for i in range(length))
 
 
-class PasswordAuthentication(Authentication):
-    _typ = AuthenticationEnum.password
-
-
-class Auth0Authentication(Authentication):
-    _typ = AuthenticationEnum.auth0
-    config: Auth0Config = pydantic.Field(default_factory=lambda: Auth0Config())
-
-
-class GitHubAuthentication(Authentication):
-    _typ = AuthenticationEnum.github
-    config: GitHubConfig = pydantic.Field(default_factory=lambda: GitHubConfig())
-
-
 class Keycloak(schema.Base):
-    initial_root_password: str = pydantic.Field(default_factory=random_secure_string)
-    overrides: typing.Dict = {}
+    initial_root_password: str = Field(default_factory=random_secure_string)
+    overrides: Dict = {}
     realm_display_name: str = "Nebari"
 
 
+auth_enum_to_model = {
+    AuthenticationEnum.password: PasswordAuthentication,
+    AuthenticationEnum.auth0: Auth0Authentication,
+    AuthenticationEnum.github: GitHubAuthentication,
+}
+
+auth_enum_to_config = {
+    AuthenticationEnum.auth0: Auth0Config,
+    AuthenticationEnum.github: GitHubConfig,
+}
+
+
 class Security(schema.Base):
-    authentication: Authentication = PasswordAuthentication(
-        type=AuthenticationEnum.password
-    )
+    authentication: Authentication = PasswordAuthentication()
     shared_users_group: bool = True
     keycloak: Keycloak = Keycloak()
 
+    @field_validator("authentication", mode="before")
+    @classmethod
+    def validate_authentication(cls, value: Optional[Dict]) -> Authentication:
+        if value is None:
+            return PasswordAuthentication()
+        if "type" not in value:
+            raise ValueError(
+                "Authentication type must be specified if authentication is set"
+            )
+        auth_type = value["type"] if hasattr(value, "__getitem__") else value.type
+        if auth_type in auth_enum_to_model:
+            if auth_type == AuthenticationEnum.password:
+                return auth_enum_to_model[auth_type]()
+            else:
+                if "config" in value:
+                    config_dict = (
+                        value["config"]
+                        if hasattr(value, "__getitem__")
+                        else value.config
+                    )
+                    config = auth_enum_to_config[auth_type](**config_dict)
+                else:
+                    config = auth_enum_to_config[auth_type]()
+                return auth_enum_to_model[auth_type](config=config)
+        else:
+            raise ValueError(f"Unsupported authentication type {auth_type}")
+
 
 class InputSchema(schema.Base):
     security: Security = Security()
 
 
 class KeycloakCredentials(schema.Base):
     url: str
@@ -222,15 +229,15 @@
             environment=self.config.namespace,
             endpoint=stage_outputs["stages/04-kubernetes-ingress"]["domain"],
             initial_root_password=self.config.security.keycloak.initial_root_password,
             overrides=[json.dumps(self.config.security.keycloak.overrides)],
             node_group=stage_outputs["stages/02-infrastructure"]["node_selectors"][
                 "general"
             ],
-        ).dict()
+        ).model_dump()
 
     def check(
         self, stage_outputs: Dict[str, Dict[str, Any]], disable_check: bool = False
     ):
         from keycloak import KeycloakAdmin
         from keycloak.exceptions import KeycloakError
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import sys
 import time
 from typing import Any, Dict, List, Type
 
 from _nebari.stages.base import NebariTerraformStage
+from _nebari.stages.kubernetes_keycloak import Authentication
 from _nebari.stages.tf_objects import NebariTerraformState
 from nebari import schema
 from nebari.hookspecs import NebariStage, hookimpl
 
 NUM_ATTEMPTS = 10
 TIMEOUT = 10
 
 
 class InputVars(schema.Base):
     realm: str = "nebari"
     realm_display_name: str
-    authentication: Dict[str, Any]
+    authentication: Authentication
     keycloak_groups: List[str] = ["superadmin", "admin", "developer", "analyst"]
     default_groups: List[str] = ["analyst"]
 
 
 class KubernetesKeycloakConfigurationStage(NebariTerraformStage):
     name = "06-kubernetes-keycloak-configuration"
     priority = 60
@@ -35,15 +36,15 @@
         )
 
         users_group = ["users"] if self.config.security.shared_users_group else []
 
         input_vars.keycloak_groups += users_group
         input_vars.default_groups += users_group
 
-        return input_vars.dict()
+        return input_vars.model_dump()
 
     def check(
         self, stage_outputs: Dict[str, Dict[str, Any]], disable_prompt: bool = False
     ):
         directory = "stages/05-kubernetes-keycloak"
 
         from keycloak import KeycloakAdmin
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/__init__.py` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import enum
 import json
 import sys
 import time
-import typing
-from typing import Any, Dict, List, Type
+from typing import Any, Dict, List, Optional, Type, Union
 from urllib.parse import urlencode
 
-import pydantic
-from pydantic import Field
+from pydantic import ConfigDict, Field, field_validator, model_validator
 
 from _nebari import constants
 from _nebari.stages.base import NebariTerraformStage
 from _nebari.stages.tf_objects import (
     NebariHelmProvider,
     NebariKubernetesProvider,
     NebariTerraformState,
@@ -77,58 +75,51 @@
 
 
 class Theme(schema.Base):
     jupyterhub: JupyterHubTheme = JupyterHubTheme()
 
 
 class KubeSpawner(schema.Base):
-    cpu_limit: int
-    cpu_guarantee: int
+    cpu_limit: float
+    cpu_guarantee: float
     mem_limit: str
     mem_guarantee: str
-
-    class Config:
-        extra = "allow"
+    model_config = ConfigDict(extra="allow")
 
 
 class JupyterLabProfile(schema.Base):
     access: AccessEnum = AccessEnum.all
     display_name: str
     description: str
     default: bool = False
-    users: typing.Optional[typing.List[str]]
-    groups: typing.Optional[typing.List[str]]
-    kubespawner_override: typing.Optional[KubeSpawner]
-
-    @pydantic.root_validator
-    def only_yaml_can_have_groups_and_users(cls, values):
-        if values["access"] != AccessEnum.yaml:
-            if (
-                values.get("users", None) is not None
-                or values.get("groups", None) is not None
-            ):
+    users: Optional[List[str]] = None
+    groups: Optional[List[str]] = None
+    kubespawner_override: Optional[KubeSpawner] = None
+
+    @model_validator(mode="after")
+    def only_yaml_can_have_groups_and_users(self):
+        if self.access != AccessEnum.yaml:
+            if self.users is not None or self.groups is not None:
                 raise ValueError(
                     "Profile must not contain groups or users fields unless access = yaml"
                 )
-        return values
+        return self
 
 
 class DaskWorkerProfile(schema.Base):
-    worker_cores_limit: int
-    worker_cores: int
+    worker_cores_limit: float
+    worker_cores: float
     worker_memory_limit: str
     worker_memory: str
     worker_threads: int = 1
-
-    class Config:
-        extra = "allow"
+    model_config = ConfigDict(extra="allow")
 
 
 class Profiles(schema.Base):
-    jupyterlab: typing.List[JupyterLabProfile] = [
+    jupyterlab: List[JupyterLabProfile] = [
         JupyterLabProfile(
             display_name="Small Instance",
             description="Stable environment with 2 cpu / 8 GB ram",
             default=True,
             kubespawner_override=KubeSpawner(
                 cpu_limit=2,
                 cpu_guarantee=1.5,
@@ -143,15 +134,15 @@
                 cpu_limit=4,
                 cpu_guarantee=3,
                 mem_limit="16G",
                 mem_guarantee="10G",
             ),
         ),
     ]
-    dask_worker: typing.Dict[str, DaskWorkerProfile] = {
+    dask_worker: Dict[str, DaskWorkerProfile] = {
         "Small Worker": DaskWorkerProfile(
             worker_cores_limit=2,
             worker_cores=1.5,
             worker_memory_limit="8G",
             worker_memory="5G",
             worker_threads=2,
         ),
@@ -160,103 +151,104 @@
             worker_cores=3,
             worker_memory_limit="16G",
             worker_memory="10G",
             worker_threads=4,
         ),
     }
 
-    @pydantic.validator("jupyterlab")
-    def check_default(cls, v, values):
+    @field_validator("jupyterlab")
+    @classmethod
+    def check_default(cls, value):
         """Check if only one default value is present."""
-        default = [attrs["default"] for attrs in v if "default" in attrs]
+        default = [attrs["default"] for attrs in value if "default" in attrs]
         if default.count(True) > 1:
             raise TypeError(
                 "Multiple default Jupyterlab profiles may cause unexpected problems."
             )
-        return v
+        return value
 
 
 class CondaEnvironment(schema.Base):
     name: str
-    channels: typing.Optional[typing.List[str]]
-    dependencies: typing.List[typing.Union[str, typing.Dict[str, typing.List[str]]]]
+    channels: Optional[List[str]] = None
+    dependencies: List[Union[str, Dict[str, List[str]]]]
 
 
 class CondaStore(schema.Base):
-    extra_settings: typing.Dict[str, typing.Any] = {}
+    extra_settings: Dict[str, Any] = {}
     extra_config: str = ""
     image: str = "quansight/conda-store-server"
     image_tag: str = constants.DEFAULT_CONDA_STORE_IMAGE_TAG
     default_namespace: str = "nebari-git"
     object_storage: str = "200Gi"
 
 
 class NebariWorkflowController(schema.Base):
     enabled: bool = True
     image_tag: str = constants.DEFAULT_NEBARI_WORKFLOW_CONTROLLER_IMAGE_TAG
 
 
 class ArgoWorkflows(schema.Base):
     enabled: bool = True
-    overrides: typing.Dict = {}
+    overrides: Dict = {}
     nebari_workflow_controller: NebariWorkflowController = NebariWorkflowController()
 
 
 class JHubApps(schema.Base):
     enabled: bool = False
 
 
 class MonitoringOverrides(schema.Base):
-    loki: typing.Dict = {}
-    promtail: typing.Dict = {}
-    minio: typing.Dict = {}
+    loki: Dict = {}
+    promtail: Dict = {}
+    minio: Dict = {}
 
 
 class Monitoring(schema.Base):
     enabled: bool = True
     overrides: MonitoringOverrides = MonitoringOverrides()
     minio_enabled: bool = True
 
 
 class JupyterLabPioneer(schema.Base):
     enabled: bool = False
-    log_format: typing.Optional[str] = None
+    log_format: Optional[str] = None
 
 
 class Telemetry(schema.Base):
     jupyterlab_pioneer: JupyterLabPioneer = JupyterLabPioneer()
 
 
 class JupyterHub(schema.Base):
-    overrides: typing.Dict = {}
+    overrides: Dict = {}
 
 
 class IdleCuller(schema.Base):
     terminal_cull_inactive_timeout: int = 15
     terminal_cull_interval: int = 5
     kernel_cull_idle_timeout: int = 15
     kernel_cull_interval: int = 5
     kernel_cull_connected: bool = True
     kernel_cull_busy: bool = False
     server_shutdown_no_activity_timeout: int = 15
 
 
 class JupyterLab(schema.Base):
-    default_settings: typing.Dict[str, typing.Any] = {}
+    default_settings: Dict[str, Any] = {}
     idle_culler: IdleCuller = IdleCuller()
-    initial_repositories: typing.List[typing.Dict[str, str]] = []
-    preferred_dir: typing.Optional[str] = None
+    initial_repositories: List[Dict[str, str]] = []
+    preferred_dir: Optional[str] = None
 
 
 class InputSchema(schema.Base):
     default_images: DefaultImages = DefaultImages()
     storage: Storage = Storage()
     theme: Theme = Theme()
     profiles: Profiles = Profiles()
-    environments: typing.Dict[str, CondaEnvironment] = {
+    environments: Dict[str, CondaEnvironment] = {
         "environment-dask.yaml": CondaEnvironment(
             name="dask",
             channels=["conda-forge"],
             dependencies=[
                 "python==3.11.6",
                 "ipykernel==6.26.0",
                 "ipywidgets==8.1.1",
@@ -370,25 +362,25 @@
     jupyterlab_image: ImageNameTag = Field(alias="jupyterlab-image")
     jupyterlab_default_settings: Dict[str, Any] = Field(
         alias="jupyterlab-default-settings"
     )
     initial_repositories: str = Field(alias="initial-repositories")
     jupyterhub_overrides: List[str] = Field(alias="jupyterhub-overrides")
     jupyterhub_stared_storage: str = Field(alias="jupyterhub-shared-storage")
-    jupyterhub_shared_endpoint: str = Field(None, alias="jupyterhub-shared-endpoint")
+    jupyterhub_shared_endpoint: Optional[str] = Field(
+        alias="jupyterhub-shared-endpoint", default=None
+    )
     jupyterhub_profiles: List[JupyterLabProfile] = Field(alias="jupyterlab-profiles")
     jupyterhub_image: ImageNameTag = Field(alias="jupyterhub-image")
     jupyterhub_hub_extraEnv: str = Field(alias="jupyterhub-hub-extraEnv")
     idle_culler_settings: Dict[str, Any] = Field(alias="idle-culler-settings")
     argo_workflows_enabled: bool = Field(alias="argo-workflows-enabled")
     jhub_apps_enabled: bool = Field(alias="jhub-apps-enabled")
     cloud_provider: str = Field(alias="cloud-provider")
-    jupyterlab_preferred_dir: typing.Optional[str] = Field(
-        alias="jupyterlab-preferred-dir"
-    )
+    jupyterlab_preferred_dir: Optional[str] = Field(alias="jupyterlab-preferred-dir")
 
 
 class DaskGatewayInputVars(schema.Base):
     dask_worker_image: ImageNameTag = Field(alias="dask-worker-image")
     dask_gateway_profiles: Dict[str, Any] = Field(alias="dask-gateway-profiles")
     cloud_provider: str = Field(alias="cloud-provider")
 
@@ -401,15 +393,15 @@
     grafana_loki_minio_overrides: List[str] = Field(
         alias="grafana-loki-minio-overrides"
     )
 
 
 class TelemetryInputVars(schema.Base):
     jupyterlab_pioneer_enabled: bool = Field(alias="jupyterlab-pioneer-enabled")
-    jupyterlab_pioneer_log_format: typing.Optional[str] = Field(
+    jupyterlab_pioneer_log_format: Optional[str] = Field(
         alias="jupyterlab-pioneer-log-format"
     )
 
 
 class ArgoWorkflowsInputVars(schema.Base):
     argo_workflows_enabled: bool = Field(alias="argo-workflows-enabled")
     argo_workflows_overrides: List[str] = Field(alias="argo-workflows-overrides")
@@ -494,55 +486,55 @@
             realm_id=realm_id,
             node_groups=stage_outputs["stages/02-infrastructure"]["node_selectors"],
             jupyterhub_logout_redirect_url=final_logout_uri,
         )
 
         conda_store_vars = CondaStoreInputVars(
             conda_store_environments={
-                k: v.dict() for k, v in self.config.environments.items()
+                k: v.model_dump() for k, v in self.config.environments.items()
             },
             conda_store_default_namespace=self.config.conda_store.default_namespace,
             conda_store_filesystem_storage=self.config.storage.conda_store,
             conda_store_object_storage=self.config.storage.conda_store,
             conda_store_service_token_scopes=conda_store_token_scopes,
             conda_store_extra_settings=self.config.conda_store.extra_settings,
             conda_store_extra_config=self.config.conda_store.extra_config,
             conda_store_image=self.config.conda_store.image,
             conda_store_image_tag=self.config.conda_store.image_tag,
         )
 
         jupyterhub_vars = JupyterhubInputVars(
-            jupyterhub_theme=jupyterhub_theme.dict(),
+            jupyterhub_theme=jupyterhub_theme.model_dump(),
             jupyterlab_image=_split_docker_image_name(
                 self.config.default_images.jupyterlab
             ),
             jupyterhub_stared_storage=self.config.storage.shared_filesystem,
             jupyterhub_shared_endpoint=jupyterhub_shared_endpoint,
             cloud_provider=cloud_provider,
-            jupyterhub_profiles=self.config.profiles.dict()["jupyterlab"],
+            jupyterhub_profiles=self.config.profiles.model_dump()["jupyterlab"],
             jupyterhub_image=_split_docker_image_name(
                 self.config.default_images.jupyterhub
             ),
             jupyterhub_overrides=[json.dumps(self.config.jupyterhub.overrides)],
             jupyterhub_hub_extraEnv=json.dumps(
                 self.config.jupyterhub.overrides.get("hub", {}).get("extraEnv", [])
             ),
-            idle_culler_settings=self.config.jupyterlab.idle_culler.dict(),
+            idle_culler_settings=self.config.jupyterlab.idle_culler.model_dump(),
             argo_workflows_enabled=self.config.argo_workflows.enabled,
             jhub_apps_enabled=self.config.jhub_apps.enabled,
             initial_repositories=str(self.config.jupyterlab.initial_repositories),
             jupyterlab_default_settings=self.config.jupyterlab.default_settings,
             jupyterlab_preferred_dir=self.config.jupyterlab.preferred_dir,
         )
 
         dask_gateway_vars = DaskGatewayInputVars(
             dask_worker_image=_split_docker_image_name(
                 self.config.default_images.dask_worker
             ),
-            dask_gateway_profiles=self.config.profiles.dict()["dask_worker"],
+            dask_gateway_profiles=self.config.profiles.model_dump()["dask_worker"],
             cloud_provider=cloud_provider,
         )
 
         monitoring_vars = MonitoringInputVars(
             monitoring_enabled=self.config.monitoring.enabled,
             minio_enabled=self.config.monitoring.minio_enabled,
             grafana_loki_overrides=[json.dumps(self.config.monitoring.overrides.loki)],
@@ -564,21 +556,21 @@
             argo_workflows_overrides=[json.dumps(self.config.argo_workflows.overrides)],
             nebari_workflow_controller=self.config.argo_workflows.nebari_workflow_controller.enabled,
             workflow_controller_image_tag=self.config.argo_workflows.nebari_workflow_controller.image_tag,
             keycloak_read_only_user_credentials=keycloak_read_only_user_credentials,
         )
 
         return {
-            **kubernetes_services_vars.dict(by_alias=True),
-            **conda_store_vars.dict(by_alias=True),
-            **jupyterhub_vars.dict(by_alias=True),
-            **dask_gateway_vars.dict(by_alias=True),
-            **monitoring_vars.dict(by_alias=True),
-            **argo_workflows_vars.dict(by_alias=True),
-            **telemetry_vars.dict(by_alias=True),
+            **kubernetes_services_vars.model_dump(by_alias=True),
+            **conda_store_vars.model_dump(by_alias=True),
+            **jupyterhub_vars.model_dump(by_alias=True),
+            **dask_gateway_vars.model_dump(by_alias=True),
+            **monitoring_vars.model_dump(by_alias=True),
+            **argo_workflows_vars.model_dump(by_alias=True),
+            **telemetry_vars.model_dump(by_alias=True),
         }
 
     def check(
         self, stage_outputs: Dict[str, Dict[str, Any]], disable_prompt: bool = False
     ):
         directory = "stages/07-kubernetes-services"
         import requests
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
   special = false
 }
 
 locals {
   jhub_apps_secrets_name           = "jhub-apps-secrets"
   jhub_apps_env_var_name           = "JHUB_APP_JWT_SECRET_KEY"
   singleuser_nodeselector_key      = var.cloud-provider == "aws" ? "dedicated" : var.user-node-group.key
-  userscheduler_nodeselector_key   = var.cloud-provider == "aws" ? "dedicated" : var.user-node-group.key
-  userscheduler_nodeselector_value = var.cloud-provider == "aws" ? var.general-node-group.value : var.user-node-group.value
+  userscheduler_nodeselector_key   = var.cloud-provider == "aws" ? "dedicated" : var.general-node-group.key
+  userscheduler_nodeselector_value = var.general-node-group.value
 }
 
 resource "kubernetes_secret" "jhub_apps_secrets" {
   metadata {
     name      = local.jhub_apps_secrets_name
     namespace = var.namespace
   }
@@ -155,16 +155,16 @@
             oauth_callback_url   = "https://${var.external-url}/hub/oauth_callback"
             authorize_url        = module.jupyterhub-openid-client.config.authentication_url
             token_url            = module.jupyterhub-openid-client.config.token_url
             userdata_url         = module.jupyterhub-openid-client.config.userinfo_url
             login_service        = "Keycloak"
             username_claim       = "preferred_username"
             claim_groups_key     = "groups"
-            allowed_groups       = ["/analyst", "/developer", "/admin"]
-            admin_groups         = ["/admin"]
+            allowed_groups       = ["/analyst", "/developer", "/admin", "jupyterhub_admin", "jupyterhub_developer"]
+            admin_groups         = ["/admin", "jupyterhub_admin"]
             manage_groups        = true
             refresh_pre_spawn    = true
             validate_server_cert = false
 
             # deprecated, to be removed (replaced by validate_server_cert)
             tls_verify = false
             # deprecated, to be removed (replaced by username_claim)
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/middleware.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/middleware.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,15 +422,18 @@
     if not argo_sa:
         return {}
 
     return {
         "ARGO_BASE_HREF": "/argo",
         "ARGO_SERVER": f"{domain}:443",
         "ARGO_NAMESPACE": namespace,
-        "ARGO_TOKEN": {
+        "ARGO_TOKEN": "Bearer $(HERA_TOKEN)",
+        "ARGO_HTTP1": "true",  # Maybe due to traefik config, but `argo list` returns 404 without this set.  Try removing after upgrading argo past v3.4.4.
+        # Hera token is needed for versions of hera released before https://github.com/argoproj-labs/hera/pull/1053 is merged
+        "HERA_TOKEN": {
             "valueFrom": {
                 "secretKeyRef": {
                     "name": f"{argo_sa}.service-account-token",
                     "key": "token",
                 }
             }
         },
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py` & `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import typing
-from typing import Any, Dict, List, Type
+from typing import Any, Dict, List, Optional, Type
 
 from _nebari.stages.base import NebariTerraformStage
 from _nebari.stages.tf_objects import (
     NebariHelmProvider,
     NebariKubernetesProvider,
     NebariTerraformState,
 )
@@ -21,29 +20,29 @@
     image: str
     urlslug: str
     private: bool = False
     oauth2client: bool = False
     keycloakadmin: bool = False
     jwt: bool = False
     nebariconfigyaml: bool = False
-    logout: typing.Optional[str]
-    envs: typing.Optional[typing.List[NebariExtensionEnv]]
+    logout: Optional[str] = None
+    envs: Optional[List[NebariExtensionEnv]] = None
 
 
 class HelmExtension(schema.Base):
     name: str
     repository: str
     chart: str
     version: str
-    overrides: typing.Dict = {}
+    overrides: Dict = {}
 
 
 class InputSchema(schema.Base):
-    helm_extensions: typing.List[HelmExtension] = []
-    tf_extensions: typing.List[NebariExtension] = []
+    helm_extensions: List[HelmExtension] = []
+    tf_extensions: List[NebariExtension] = []
 
 
 class OutputSchema(schema.Base):
     pass
 
 
 class NebariTFExtensionsStage(NebariTerraformStage):
@@ -63,19 +62,19 @@
     def input_vars(self, stage_outputs: Dict[str, Dict[str, Any]]):
         return {
             "environment": self.config.namespace,
             "endpoint": self.config.domain,
             "realm_id": stage_outputs["stages/06-kubernetes-keycloak-configuration"][
                 "realm_id"
             ]["value"],
-            "tf_extensions": [_.dict() for _ in self.config.tf_extensions],
-            "nebari_config_yaml": self.config.dict(),
+            "tf_extensions": [_.model_dump() for _ in self.config.tf_extensions],
+            "nebari_config_yaml": self.config.model_dump(),
             "keycloak_nebari_bot_password": stage_outputs[
                 "stages/05-kubernetes-keycloak"
             ]["keycloak_nebari_bot_password"]["value"],
-            "helm_extensions": [_.dict() for _ in self.config.helm_extensions],
+            "helm_extensions": [_.model_dump() for _ in self.config.helm_extensions],
         }
 
 
 @hookimpl
 def nebari_stage() -> List[Type[NebariStage]]:
     return [NebariTFExtensionsStage]
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/__init__.py` & `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import contextlib
 import enum
 import inspect
 import os
 import pathlib
 import re
-import typing
-from typing import Any, Dict, List, Tuple, Type
+from typing import Any, Dict, List, Optional, Tuple, Type
 
-import pydantic
+from pydantic import field_validator
 
 from _nebari.provider import terraform
 from _nebari.provider.cloud import azure_cloud
 from _nebari.stages.base import NebariTerraformStage
 from _nebari.utils import (
     AZURE_TF_STATE_RESOURCE_GROUP_SUFFIX,
     construct_azure_resource_group_name,
@@ -35,18 +34,19 @@
 
 class AzureInputVars(schema.Base):
     name: str
     namespace: str
     region: str
     storage_account_postfix: str
     state_resource_group_name: str
-    tags: Dict[str, str] = {}
+    tags: Dict[str, str]
 
-    @pydantic.validator("state_resource_group_name")
-    def _validate_resource_group_name(cls, value):
+    @field_validator("state_resource_group_name")
+    @classmethod
+    def _validate_resource_group_name(cls, value: str) -> str:
         if value is None:
             return value
         length = len(value) + len(AZURE_TF_STATE_RESOURCE_GROUP_SUFFIX)
         if length < 1 or length > 90:
             raise ValueError(
                 f"Azure Resource Group name must be between 1 and 90 characters long, when combined with the suffix `{AZURE_TF_STATE_RESOURCE_GROUP_SUFFIX}`."
             )
@@ -55,17 +55,18 @@
                 "Azure Resource Group name can only contain alphanumerics, underscores, parentheses, hyphens, and periods."
             )
         if value[-1] == ".":
             raise ValueError("Azure Resource Group name can't end with a period.")
 
         return value
 
-    @pydantic.validator("tags")
-    def _validate_tags(cls, tags):
-        return azure_cloud.validate_tags(tags)
+    @field_validator("tags")
+    @classmethod
+    def _validate_tags(cls, value: Dict[str, str]) -> Dict[str, str]:
+        return azure_cloud.validate_tags(value)
 
 
 class AWSInputVars(schema.Base):
     name: str
     namespace: str
 
 
@@ -78,16 +79,16 @@
     @classmethod
     def to_yaml(cls, representer, node):
         return representer.represent_str(node.value)
 
 
 class TerraformState(schema.Base):
     type: TerraformStateEnum = TerraformStateEnum.remote
-    backend: typing.Optional[str]
-    config: typing.Dict[str, str] = {}
+    backend: Optional[str] = None
+    config: Dict[str, str] = {}
 
 
 class InputSchema(schema.Base):
     terraform_state: TerraformState = TerraformState()
 
 
 class OutputSchema(schema.Base):
@@ -188,40 +189,40 @@
 
     def input_vars(self, stage_outputs: Dict[str, Dict[str, Any]]):
         if self.config.provider == schema.ProviderEnum.do:
             return DigitalOceanInputVars(
                 name=self.config.project_name,
                 namespace=self.config.namespace,
                 region=self.config.digital_ocean.region,
-            ).dict()
+            ).model_dump()
         elif self.config.provider == schema.ProviderEnum.gcp:
             return GCPInputVars(
                 name=self.config.project_name,
                 namespace=self.config.namespace,
                 region=self.config.google_cloud_platform.region,
-            ).dict()
+            ).model_dump()
         elif self.config.provider == schema.ProviderEnum.aws:
             return AWSInputVars(
                 name=self.config.project_name,
                 namespace=self.config.namespace,
-            ).dict()
+            ).model_dump()
         elif self.config.provider == schema.ProviderEnum.azure:
             return AzureInputVars(
                 name=self.config.project_name,
                 namespace=self.config.namespace,
                 region=self.config.azure.region,
                 storage_account_postfix=self.config.azure.storage_account_postfix,
                 state_resource_group_name=construct_azure_resource_group_name(
                     project_name=self.config.project_name,
                     namespace=self.config.namespace,
                     base_resource_group_name=self.config.azure.resource_group_name,
                     suffix=AZURE_TF_STATE_RESOURCE_GROUP_SUFFIX,
                 ),
                 tags=self.config.azure.tags,
-            ).dict()
+            ).model_dump()
         elif (
             self.config.provider == schema.ProviderEnum.local
             or self.config.provider == schema.ProviderEnum.existing
         ):
             return {}
         else:
             ValueError(f"Unknown provider: {self.config.provider}")
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf` & `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/subcommands/deploy.py` & `nebari-2024.5.1rc1/src/_nebari/subcommands/deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/subcommands/destroy.py` & `nebari-2024.5.1rc1/src/_nebari/subcommands/destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/subcommands/dev.py` & `nebari-2024.5.1rc1/src/_nebari/subcommands/dev.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/subcommands/info.py` & `nebari-2024.5.1rc1/src/_nebari/subcommands/info.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/subcommands/init.py` & `nebari-2024.5.1rc1/src/_nebari/subcommands/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,15 +415,15 @@
                 )
             )
         if kubernetes_version not in versions:
             raise ValueError(
                 f"Invalid Kubernetes version `{kubernetes_version}`. Please refer to the GCP docs for a list of valid versions: {versions}"
             )
     elif cloud_provider == ProviderEnum.do.value.lower():
-        versions = digital_ocean.kubernetes_versions(region)
+        versions = digital_ocean.kubernetes_versions()
 
         if not kubernetes_version or kubernetes_version == LATEST:
             kubernetes_version = get_latest_kubernetes_version(versions)
             rich.print(
                 DEFAULT_KUBERNETES_VERSION_MSG.format(
                     kubernetes_version=kubernetes_version
                 )
@@ -917,15 +917,19 @@
                 value = getattr(model, key)
                 if isinstance(value, str) and (value != "" or value is not None):
                     return b.format(key=key, value=value).replace("_", "-")
                 if isinstance(value, bool) and value:
                     return b.format(key=key, value=value).replace("_", "-")
 
         cmds = " ".join(
-            [_ for _ in [if_used(_) for _ in inputs.dict().keys()] if _ is not None]
+            [
+                _
+                for _ in [if_used(_) for _ in inputs.model_dump().keys()]
+                if _ is not None
+            ]
         )
 
         rich.print(
             (
                 "For reference, if the previous Guided Init answers were converted into a direct [green]nebari init[/green] command, it would be:\n\n"
                 f"\t[green]{base_cmd} {cmds}[/green]\n\n"
             )
```

### Comparing `nebari-2024.4.1rc1/src/_nebari/subcommands/keycloak.py` & `nebari-2024.5.1rc1/src/_nebari/subcommands/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/subcommands/render.py` & `nebari-2024.5.1rc1/src/_nebari/subcommands/render.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/subcommands/support.py` & `nebari-2024.5.1rc1/src/_nebari/subcommands/support.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/subcommands/upgrade.py` & `nebari-2024.5.1rc1/src/_nebari/subcommands/upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/_nebari/subcommands/validate.py` & `nebari-2024.5.1rc1/src/_nebari/subcommands/validate.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/nebari/hookspecs.py` & `nebari-2024.5.1rc1/src/nebari/hookspecs.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/nebari/plugins.py` & `nebari-2024.5.1rc1/src/nebari/plugins.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/src/nebari/schema.py` & `nebari-2024.5.1rc1/src/nebari/schema.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import enum
+from typing import Annotated
 
 import pydantic
+from pydantic import ConfigDict, Field, StringConstraints, field_validator
 from ruamel.yaml import yaml_object
 
 from _nebari.utils import escape_string, yaml
 from _nebari.version import __version__, rounded_ver_parse
 
 # Regex for suitable project names
 project_name_regex = r"^[A-Za-z][A-Za-z0-9\-_]{1,14}[A-Za-z0-9]$"
-project_name_pydantic = pydantic.constr(regex=project_name_regex)
+project_name_pydantic = Annotated[str, StringConstraints(pattern=project_name_regex)]
 
 # Regex for suitable namespaces
 namespace_regex = r"^[A-Za-z][A-Za-z\-_]*[A-Za-z]$"
-namespace_pydantic = pydantic.constr(regex=namespace_regex)
+namespace_pydantic = Annotated[str, StringConstraints(pattern=namespace_regex)]
 
 email_regex = "^[^ @]+@[^ @]+\\.[^ @]+$"
-email_pydantic = pydantic.constr(regex=email_regex)
+email_pydantic = Annotated[str, StringConstraints(pattern=email_regex)]
 
 github_url_regex = "^(https://)?github.com/([^/]+)/([^/]+)/?$"
-github_url_pydantic = pydantic.constr(regex=github_url_regex)
+github_url_pydantic = Annotated[str, StringConstraints(pattern=github_url_regex)]
 
 
 class Base(pydantic.BaseModel):
-    ...
-
-    class Config:
-        extra = "forbid"
-        validate_assignment = True
-        allow_population_by_field_name = True
+    model_config = ConfigDict(
+        extra="forbid", validate_assignment=True, populate_by_name=True
+    )
 
 
 @yaml_object(yaml)
 class ProviderEnum(str, enum.Enum):
     local = "local"
     existing = "existing"
     do = "do"
@@ -45,35 +44,29 @@
 
 
 class Main(Base):
     project_name: project_name_pydantic
     namespace: namespace_pydantic = "dev"
     provider: ProviderEnum = ProviderEnum.local
     # In nebari_version only use major.minor.patch version - drop any pre/post/dev suffixes
-    nebari_version: str = __version__
+    nebari_version: Annotated[str, Field(validate_default=True)] = __version__
 
     prevent_deploy: bool = (
         False  # Optional, but will be given default value if not present
     )
 
     # If the nebari_version in the schema is old
     # we must tell the user to first run nebari upgrade
-    @pydantic.validator("nebari_version", pre=True, always=True)
-    def check_default(cls, v):
-        """
-        Always called even if nebari_version is not supplied at all (so defaults to ''). That way we can give a more helpful error message.
-        """
-        if not cls.is_version_accepted(v):
-            if v == "":
-                v = "not supplied"
-            raise ValueError(
-                f"nebari_version in the config file must be equivalent to {__version__} to be processed by this version of nebari (your config file version is {v})."
-                " Install a different version of nebari or run nebari upgrade to ensure your config file is compatible."
-            )
-        return v
+    @field_validator("nebari_version")
+    @classmethod
+    def check_default(cls, value):
+        assert cls.is_version_accepted(
+            value
+        ), f"nebari_version={value} is not an accepted version, it must be equivalent to {__version__}.\nInstall a different version of nebari or run nebari upgrade to ensure your config file is compatible."
+        return value
 
     @classmethod
     def is_version_accepted(cls, v):
         return v != "" and rounded_ver_parse(v) == rounded_ver_parse(__version__)
 
     @property
     def escaped_project_name(self):
```

### Comparing `nebari-2024.4.1rc1/tests/utils.py` & `nebari-2024.5.1rc1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/common/config_mod_utils.py` & `nebari-2024.5.1rc1/tests/common/config_mod_utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/common/kube_api.py` & `nebari-2024.5.1rc1/tests/common/kube_api.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/common/navigator.py` & `nebari-2024.5.1rc1/tests/common/navigator.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/common/playwright_fixtures.py` & `nebari-2024.5.1rc1/tests/common/playwright_fixtures.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/common/run_notebook.py` & `nebari-2024.5.1rc1/tests/common/run_notebook.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/common/notebooks/test_notebook_output.ipynb` & `nebari-2024.5.1rc1/tests/common/notebooks/test_notebook_output.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/common/tests/test_notebook.py` & `nebari-2024.5.1rc1/tests/common/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_deployment/test_dask_gateway.py` & `nebari-2024.5.1rc1/tests/tests_deployment/test_dask_gateway.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_deployment/test_grafana_api.py` & `nebari-2024.5.1rc1/tests/tests_deployment/test_grafana_api.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_deployment/test_jupyterhub_ssh.py` & `nebari-2024.5.1rc1/tests/tests_deployment/test_jupyterhub_ssh.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_deployment/test_loki_deployment.py` & `nebari-2024.5.1rc1/tests/tests_deployment/test_loki_deployment.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_deployment/utils.py` & `nebari-2024.5.1rc1/tests/tests_deployment/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_deployment/assets/notebook/simple.ipynb` & `nebari-2024.5.1rc1/tests/tests_deployment/assets/notebook/simple.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_e2e/package-lock.json` & `nebari-2024.5.1rc1/tests/tests_e2e/package-lock.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_e2e/cypress/integration/main.js` & `nebari-2024.5.1rc1/tests/tests_e2e/cypress/integration/main.js`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb` & `nebari-2024.5.1rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_e2e/cypress/plugins/index.js` & `nebari-2024.5.1rc1/tests/tests_e2e/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_e2e/cypress/support/index.js` & `nebari-2024.5.1rc1/tests/tests_e2e/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_e2e/playwright/README.md` & `nebari-2024.5.1rc1/tests/tests_e2e/playwright/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_e2e/playwright/test_playwright.py` & `nebari-2024.5.1rc1/tests/tests_e2e/playwright/test_playwright.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_integration/README.md` & `nebari-2024.5.1rc1/tests/tests_integration/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_integration/deployment_fixtures.py` & `nebari-2024.5.1rc1/tests/tests_integration/deployment_fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     )
 
     if cloud in ["aws"]:
         config = add_gpu_config(config, cloud=cloud)
         config = add_preemptible_node_group(config, cloud=cloud)
 
     print("*" * 100)
-    pprint.pprint(config.dict())
+    pprint.pprint(config.model_dump())
     print("*" * 100)
 
     # render
     render_template(deployment_dir_abs, config, stages)
 
     failed = False
```

### Comparing `nebari-2024.4.1rc1/tests/tests_integration/test_all_clouds.py` & `nebari-2024.5.1rc1/tests/tests_integration/test_all_clouds.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_integration/test_gpu.py` & `nebari-2024.5.1rc1/tests/tests_integration/test_gpu.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_integration/test_preemptible.py` & `nebari-2024.5.1rc1/tests/tests_integration/test_preemptible.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/conftest.py` & `nebari-2024.5.1rc1/tests/tests_unit/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         terraform_state=DEFAULT_TERRAFORM_STATE,
         disable_prompt=True,
     )
 
 
 @pytest.fixture
 def nebari_config(nebari_config_options):
-    return nebari_plugin_manager.config_schema.parse_obj(
+    return nebari_plugin_manager.config_schema.model_validate(
         render_config(**nebari_config_options)
     )
 
 
 @pytest.fixture
 def nebari_stages():
     return nebari_plugin_manager.ordered_stages
```

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_cli.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_cli_deploy.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_cli_deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_cli_dev.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_cli_dev.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_cli_init.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_cli_init.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_cli_init_repository.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_cli_init_repository.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_cli_keycloak.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_cli_keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_cli_support.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_cli_support.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_cli_upgrade.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_cli_upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_cli_validate.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_cli_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,21 @@
         assert "Invalid `kubernetes-version`" in invalid_result.stdout
 
 
 @pytest.mark.parametrize(
     "key, value, provider, expected_message, addl_config",
     [
         ("NEBARI_SECRET__project_name", "123invalid", "local", "validation error", {}),
-        ("NEBARI_SECRET__this_is_an_error", "true", "local", "object has no field", {}),
+        (
+            "NEBARI_SECRET__this_is_an_error",
+            "true",
+            "local",
+            "Object has no attribute",
+            {},
+        ),
         (
             "NEBARI_SECRET__amazon_web_services__kubernetes_version",
             "1.0",
             "aws",
             "validation error",
             {
                 "amazon_web_services": {
```

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_commons.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_commons.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_config.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     with pytest.raises(ValueError, match="does not exist"):
         read_configuration(non_existent_file, nebari_config.__class__)
 
 
 def test_write_configuration_with_dict(nebari_config, tmp_path):
     config_file = tmp_path / "nebari-config-dict.yaml"
-    config_dict = nebari_config.dict()
+    config_dict = nebari_config.model_dump()
 
     write_configuration(config_file, config_dict)
     read_config = read_configuration(config_file, nebari_config.__class__)
 
     # TODO: determine a way to compare the two objects directly
     assert nebari_config.namespace == read_config.namespace
     assert (
```

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_dependencies.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_init.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_init.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_provider.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_provider.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_render.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_render.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_schema.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from contextlib import nullcontext
 
 import pytest
-from pydantic.error_wrappers import ValidationError
+from pydantic import ValidationError
 
 from nebari import schema
 from nebari.plugins import nebari_plugin_manager
 
 
 def test_minimal_schema():
     config = nebari_plugin_manager.config_schema(project_name="test")
@@ -121,15 +121,15 @@
 def test_no_provider(config_schema, provider, full_name, default_fields):
     config_dict = {
         "project_name": "test",
         f"{full_name}": default_fields,
     }
     config = config_schema(**config_dict)
     assert config.provider == provider
-    assert full_name in config.dict()
+    assert full_name in config.model_dump()
 
 
 def test_multiple_providers(config_schema):
     config_dict = {
         "project_name": "test",
         "local": {},
         "existing": {},
@@ -160,10 +160,10 @@
     config_dict = {
         "project_name": "test",
         "provider": provider,
         f"{provider}": {"kube_context": "some_context"},
     }
     config = config_schema(**config_dict)
     assert config.provider == provider
-    result_config_dict = config.dict()
+    result_config_dict = config.model_dump()
     assert provider in result_config_dict
     assert result_config_dict[provider]["kube_context"] == "some_context"
```

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/test_upgrade.py` & `nebari-2024.5.1rc1/tests/tests_unit/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/utils.py` & `nebari-2024.5.1rc1/tests/tests_unit/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/aws.happy.yaml` & `nebari-2024.5.1rc1/tests/tests_unit/cli_validate/aws.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/azure.happy.yaml` & `nebari-2024.5.1rc1/tests/tests_unit/cli_validate/azure.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/do.happy.yaml` & `nebari-2024.5.1rc1/tests/tests_unit/cli_validate/do.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/gcp.happy.yaml` & `nebari-2024.5.1rc1/tests/tests_unit/cli_validate/gcp.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.yaml` & `nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml` & `nebari-2024.5.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml` & `nebari-2024.5.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/.gitignore` & `nebari-2024.5.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/LICENSE` & `nebari-2024.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/README.md` & `nebari-2024.5.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.4.1rc1/pyproject.toml` & `nebari-2024.5.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,17 @@
     "azure-mgmt-resource==23.0.1",
     "bcrypt==4.0.1",
     "boto3==1.34.63",
     "cloudflare==2.11.7",
     "kubernetes==27.2.0",
     "pluggy==1.3.0",
     "prompt-toolkit==3.0.36",
-    "pydantic==1.10.12",
+    "pydantic==2.4.2",
     "pynacl==1.5.0",
-    "python-keycloak>=3.9.0",
+    "python-keycloak>=3.9.0,<4.0.0",
     "questionary==2.0.0",
     "requests-toolbelt==1.0.0",
     "rich==13.5.1",
     "ruamel.yaml==0.18.6",
     "typer==0.9.0",
     "packaging==23.2",
 ]
@@ -97,15 +97,15 @@
 ]
 docs = [
     "sphinx",
     "sphinx_click",
 ]
 
 [project.urls]
-Documentation = "https://www.nebari.dev/docs"
+Documentation = "https://www.nebari.dev/docs/welcome"
 Source = "https://github.com/nebari-dev/nebari"
 
 [project.scripts]
 nebari = "nebari.__main__:main"
 
 [tool.mypy]
 warn_return_any = true
```

### Comparing `nebari-2024.4.1rc1/PKG-INFO` & `nebari-2024.5.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.3
 Name: nebari
-Version: 2024.4.1rc1
+Version: 2024.5.1rc1
 Summary: A Jupyter and Dask-powered open source data science platform.
-Project-URL: Documentation, https://www.nebari.dev/docs
+Project-URL: Documentation, https://www.nebari.dev/docs/welcome
 Project-URL: Source, https://github.com/nebari-dev/nebari
 Author-email: Nebari development team <internal-it@quansight.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: aws,azure,dask,do,gcp,jupyter,nebari
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Jupyter :: JupyterLab
@@ -27,17 +27,17 @@
 Requires-Dist: bcrypt==4.0.1
 Requires-Dist: boto3==1.34.63
 Requires-Dist: cloudflare==2.11.7
 Requires-Dist: kubernetes==27.2.0
 Requires-Dist: packaging==23.2
 Requires-Dist: pluggy==1.3.0
 Requires-Dist: prompt-toolkit==3.0.36
-Requires-Dist: pydantic==1.10.12
+Requires-Dist: pydantic==2.4.2
 Requires-Dist: pynacl==1.5.0
-Requires-Dist: python-keycloak>=3.9.0
+Requires-Dist: python-keycloak<4.0.0,>=3.9.0
 Requires-Dist: questionary==2.0.0
 Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: rich==13.5.1
 Requires-Dist: ruamel-yaml==0.18.6
 Requires-Dist: typer==0.9.0
 Provides-Extra: dev
 Requires-Dist: black==22.3.0; extra == 'dev'
```

