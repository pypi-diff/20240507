# Comparing `tmp/ansible-risk-insight-0.2.5.tar.gz` & `tmp/ansible-risk-insight-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-risk-insight-0.2.5.tar", last modified: Thu Apr 25 12:40:09 2024, max compression
+gzip compressed data, was "ansible-risk-insight-0.2.6.tar", last modified: Tue May  7 06:48:34 2024, max compression
```

## Comparing `ansible-risk-insight-0.2.5.tar` & `ansible-risk-insight-0.2.6.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.449210 ansible-risk-insight-0.2.5/
--rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.5/.flake8
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.403555 ansible-risk-insight-0.2.5/.github/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.407896 ansible-risk-insight-0.2.5/.github/workflows/
--rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.5/.github/workflows/lint.yml
--rw-r--r--   0 hiro       (501) staff       (20)      793 2023-08-22 04:18:04.000000 ansible-risk-insight-0.2.5/.github/workflows/test.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.2.5/.gitignore
--rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/CONTRIBUTING.md
--rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.5/LICENSE
--rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.5/Makefile
--rw-r--r--   0 hiro       (501) staff       (20)      272 2024-04-25 12:40:09.449064 ansible-risk-insight-0.2.5/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.5/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.415675 ansible-risk-insight-0.2.5/ansible_risk_insight/
--rw-r--r--   0 hiro       (501) staff       (20)     1907 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)      659 2024-04-25 12:37:00.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/_version.py
--rw-r--r--   0 hiro       (501) staff       (20)     3519 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/analyzer.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.418436 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/
--rw-r--r--   0 hiro       (501) staff       (20)      636 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1408 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/annotator_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.422058 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/
--rw-r--r--   0 hiro       (501) staff       (20)     1393 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/apt.py
--rw-r--r--   0 hiro       (501) staff       (20)     1587 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1446 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/assemble.py
--rw-r--r--   0 hiro       (501) staff       (20)     1460 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1388 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/command.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/dnf.py
--rw-r--r--   0 hiro       (501) staff       (20)     1447 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/expect.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/file.py
--rw-r--r--   0 hiro       (501) staff       (20)     1320 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/get_url.py
--rw-r--r--   0 hiro       (501) staff       (20)     1317 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/git.py
--rw-r--r--   0 hiro       (501) staff       (20)     1511 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1339 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/pip.py
--rw-r--r--   0 hiro       (501) staff       (20)     1380 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/raw.py
--rw-r--r--   0 hiro       (501) staff       (20)     1448 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/replace.py
--rw-r--r--   0 hiro       (501) staff       (20)     1371 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1386 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/script.py
--rw-r--r--   0 hiro       (501) staff       (20)     1384 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/shell.py
--rw-r--r--   0 hiro       (501) staff       (20)     1327 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/subversion.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/template.py
--rw-r--r--   0 hiro       (501) staff       (20)     2221 2024-04-25 12:09:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/uri.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/yum.py
--rw-r--r--   0 hiro       (501) staff       (20)     1230 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible_builtin.py
--rw-r--r--   0 hiro       (501) staff       (20)    46432 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible_builtin.py.bak
--rw-r--r--   0 hiro       (501) staff       (20)     1113 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/module_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2846 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/risk_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2381 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/sample_custom_annotator.py
--rw-r--r--   0 hiro       (501) staff       (20)     9222 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/variable_resolver.py
--rw-r--r--   0 hiro       (501) staff       (20)   846979 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/ansible_builtin_modules.json
--rw-r--r--   0 hiro       (501) staff       (20)     2306 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/ansible_variables.txt
--rw-r--r--   0 hiro       (501) staff       (20)     3211 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/awx_utils.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      678 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/batch.sh
--rw-r--r--   0 hiro       (501) staff       (20)     1049 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/builtin-modules.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.422228 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/
--rw-r--r--   0 hiro       (501) staff       (20)     7770 2024-04-25 11:59:38.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.423358 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/
--rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-09-26 03:55:49.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1705 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/diff.py
--rw-r--r--   0 hiro       (501) staff       (20)     3085 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/generate.py
--rw-r--r--   0 hiro       (501) staff       (20)     1486 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/list.py
--rw-r--r--   0 hiro       (501) staff       (20)     1690 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/release.py
--rw-r--r--   0 hiro       (501) staff       (20)     1720 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/search.py
--rw-r--r--   0 hiro       (501) staff       (20)     2033 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/update.py
--rw-r--r--   0 hiro       (501) staff       (20)    31923 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/context.py
--rw-r--r--   0 hiro       (501) staff       (20)    48633 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/dependency_dir_preparator.py
--rw-r--r--   0 hiro       (501) staff       (20)    14850 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/dependency_finder.py
--rw-r--r--   0 hiro       (501) staff       (20)    20780 2024-01-05 07:03:36.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/finder.py
--rw-r--r--   0 hiro       (501) staff       (20)     2683 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/findings.py
--rw-r--r--   0 hiro       (501) staff       (20)     1291 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/key_test.py
--rw-r--r--   0 hiro       (501) staff       (20)     8582 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/keyutil.py
--rw-r--r--   0 hiro       (501) staff       (20)     8728 2024-04-25 12:13:13.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/loader.py
--rw-r--r--   0 hiro       (501) staff       (20)     1615 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/logger.py
--rw-r--r--   0 hiro       (501) staff       (20)    73469 2024-04-25 12:06:34.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/model_loader.py
--rw-r--r--   0 hiro       (501) staff       (20)    82614 2024-04-25 12:09:28.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/models.py
--rw-r--r--   0 hiro       (501) staff       (20)    26942 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/parser.py
--rw-r--r--   0 hiro       (501) staff       (20)     5955 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/ram_generator.py
--rw-r--r--   0 hiro       (501) staff       (20)      105 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/requirements.txt
--rw-r--r--   0 hiro       (501) staff       (20)    45276 2024-03-26 08:07:23.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/risk_assessment_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     8376 2024-01-18 10:18:59.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/risk_detector.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.436027 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     4292 2024-04-25 11:59:38.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P001_module_name_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     6677 2024-01-18 10:18:42.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P002_module_argument_key_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     7106 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P003_module_argument_value_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     3418 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P004_variable_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     1801 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R101_command_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)     1684 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R102_command_instead_of_shell.py
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     2703 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R103_download_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)     2370 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R104_unauthorized_download_src.py
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1846 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R105_outbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1947 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R106_inbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)     2066 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)     1536 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R108_privilege_escalation.py
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     1756 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R109_key_config_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1642 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R110_non_builtin_use.py
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)     1729 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R111_parameterized_import_role.py
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)     1952 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)     1875 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     2088 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R114_file_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)     1871 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R115_file_deletion.py
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)     1649 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R116_insecure_file_permission.py
--rw-r--r--   0 hiro       (501) staff       (20)     1661 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R117_external_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1927 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R201_changed_data_dependence.py
--rw-r--r--   0 hiro       (501) staff       (20)     2123 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R202_unconditional_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2181 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R203_unused_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2180 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
--rw-r--r--   0 hiro       (501) staff       (20)     1707 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R301_non_fqcn_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1827 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R301_non_fqcn_use.py
--rw-r--r--   0 hiro       (501) staff       (20)     1430 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R302_role_without_metadata.py
--rw-r--r--   0 hiro       (501) staff       (20)     1416 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R303_task_without_name.py
--rw-r--r--   0 hiro       (501) staff       (20)     1607 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R304_unresolved_module.py
--rw-r--r--   0 hiro       (501) staff       (20)     1712 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R305_unresolved_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1787 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R306_undefined_variable.py
--rw-r--r--   0 hiro       (501) staff       (20)     1925 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R401_list_all_inbound_src.py
--rw-r--r--   0 hiro       (501) staff       (20)     1609 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R402_list_all_used_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1939 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R404_show_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1974 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R501_dependency_suggestion.py
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/rule_versions.json
--rw-r--r--   0 hiro       (501) staff       (20)     1521 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     4224 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/safe_glob.py
--rw-r--r--   0 hiro       (501) staff       (20)    49966 2024-01-26 00:47:50.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/scanner.py
--rw-r--r--   0 hiro       (501) staff       (20)      401 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/task_keywords.txt
--rw-r--r--   0 hiro       (501) staff       (20)    43475 2024-04-25 12:17:59.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/tree.py
--rw-r--r--   0 hiro       (501) staff       (20)    24692 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/utils.py
--rw-r--r--   0 hiro       (501) staff       (20)     2251 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/ansible_risk_insight/yaml.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.416578 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)      272 2024-04-25 12:40:09.000000 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     8106 2024-04-25 12:40:09.000000 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2024-04-25 12:40:09.000000 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       99 2024-04-25 12:40:09.000000 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       99 2024-04-25 12:40:09.000000 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)       21 2024-04-25 12:40:09.000000 ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.5/data-struct.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.404338 ansible-risk-insight-0.2.5/doc/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.437271 ansible-risk-insight-0.2.5/doc/images/
--rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.5/doc/images/ari-apply-rules.png
--rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.5/doc/images/ari-arch.png
--rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.5/doc/images/ari-overview.png
--rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.5/doc/images/ari-ram-list.png
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.438197 ansible-risk-insight-0.2.5/docs/
--rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.2.5/docs/annotation.md
--rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.2.5/docs/customize_rules.md
--rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.2.5/docs/index.md
--rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.2.5/docs/installing.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.440672 ansible-risk-insight-0.2.5/docs/rules/
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.5/docs/rules/R301_non_fqcn_use.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.440995 ansible-risk-insight-0.2.5/example/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.441158 ansible-risk-insight-0.2.5/example/playbooks/
--rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.2.5/example/playbooks/sample_playbook.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.2.5/example/readme.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.441312 ansible-risk-insight-0.2.5/example/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     1366 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.5/example/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     1728 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/example/sample.py
--rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.2.5/mkdocs.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1001 2024-04-25 11:59:15.000000 ansible-risk-insight-0.2.5/pyproject.toml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.441673 ansible-risk-insight-0.2.5/scripts/
--rw-r--r--   0 hiro       (501) staff       (20)     5105 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/scripts/gen_ram_slim.py
--rw-r--r--   0 hiro       (501) staff       (20)     5964 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/scripts/gen_ram_subset.py
--rw-r--r--   0 hiro       (501) staff       (20)       38 2024-04-25 12:40:09.449255 ansible-risk-insight-0.2.5/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.5/setup.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.441842 ansible-risk-insight-0.2.5/test/
--rw-r--r--   0 hiro       (501) staff       (20)     2668 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.5/test/test_scanner.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.405486 ansible-risk-insight-0.2.5/test/testdata/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.405068 ansible-risk-insight-0.2.5/test/testdata/projects/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.442204 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/
--rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/MANIFEST.json
--rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/galaxy.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.405205 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.405409 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.446147 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.446473 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.446639 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.405542 ansible-risk-insight-0.2.5/test/testdata/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.405751 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.447645 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.448667 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-04-25 12:40:09.448842 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.5/test/testdata/roles/test_role/tasks/main.yml
--rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.2.5/tox.ini
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.102702 ansible-risk-insight-0.2.6/
+-rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.6/.flake8
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.037731 ansible-risk-insight-0.2.6/.github/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.044084 ansible-risk-insight-0.2.6/.github/workflows/
+-rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.6/.github/workflows/lint.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      793 2023-08-22 04:18:04.000000 ansible-risk-insight-0.2.6/.github/workflows/test.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.2.6/.gitignore
+-rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.6/CONTRIBUTING.md
+-rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.6/LICENSE
+-rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.6/Makefile
+-rw-r--r--   0 hiro       (501) staff       (20)      272 2024-05-07 06:48:34.102514 ansible-risk-insight-0.2.6/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.6/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.052300 ansible-risk-insight-0.2.6/ansible_risk_insight/
+-rw-r--r--   0 hiro       (501) staff       (20)     1907 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)      659 2024-05-07 06:43:33.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/_version.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3519 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/analyzer.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.055102 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1408 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/annotator_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.058177 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/
+-rw-r--r--   0 hiro       (501) staff       (20)     1393 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/apt.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1587 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1446 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/assemble.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1460 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1388 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/command.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/dnf.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1447 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/expect.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/file.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1320 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/get_url.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1317 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/git.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1511 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1339 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/pip.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1380 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/raw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1448 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/replace.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1371 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1386 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/script.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1384 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1327 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/subversion.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/template.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2215 2024-05-07 06:21:39.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/uri.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/yum.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1230 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible_builtin.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46432 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible_builtin.py.bak
+-rw-r--r--   0 hiro       (501) staff       (20)     1113 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/module_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2846 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/risk_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2381 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/sample_custom_annotator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9222 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/variable_resolver.py
+-rw-r--r--   0 hiro       (501) staff       (20)   846979 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/ansible_builtin_modules.json
+-rw-r--r--   0 hiro       (501) staff       (20)     2306 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/ansible_variables.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     3211 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/awx_utils.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      678 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/batch.sh
+-rw-r--r--   0 hiro       (501) staff       (20)     1049 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/builtin-modules.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.058324 ansible-risk-insight-0.2.6/ansible_risk_insight/cli/
+-rw-r--r--   0 hiro       (501) staff       (20)     7770 2024-04-25 11:59:38.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/cli/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.060335 ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/
+-rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-09-26 03:55:49.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1705 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/diff.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3085 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/generate.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1486 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/list.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1690 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/release.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1720 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/search.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2033 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/update.py
+-rw-r--r--   0 hiro       (501) staff       (20)    31923 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/context.py
+-rw-r--r--   0 hiro       (501) staff       (20)    48633 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/dependency_dir_preparator.py
+-rw-r--r--   0 hiro       (501) staff       (20)    14868 2024-05-07 06:21:39.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/dependency_finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)    20780 2024-01-05 07:03:36.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2683 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/findings.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1291 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/key_test.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8582 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/keyutil.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8728 2024-04-25 12:41:17.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1615 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/logger.py
+-rw-r--r--   0 hiro       (501) staff       (20)    73460 2024-05-07 06:21:39.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/model_loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)    82605 2024-05-07 06:21:39.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/models.py
+-rw-r--r--   0 hiro       (501) staff       (20)    26942 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/parser.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5955 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/ram_generator.py
+-rw-r--r--   0 hiro       (501) staff       (20)      105 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/requirements.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    45276 2024-03-26 08:07:23.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/risk_assessment_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8376 2024-05-06 10:04:18.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/risk_detector.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.082096 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     4292 2024-04-25 11:59:38.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/P001_module_name_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6677 2024-01-18 10:18:42.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/P002_module_argument_key_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     7106 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/P003_module_argument_value_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3418 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/P004_variable_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1801 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R101_command_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1684 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R102_command_instead_of_shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2703 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R103_download_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2370 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R104_unauthorized_download_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1846 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R105_outbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1947 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R106_inbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2066 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1536 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R108_privilege_escalation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1756 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R109_key_config_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1642 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R110_non_builtin_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1729 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R111_parameterized_import_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1952 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1875 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2088 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R114_file_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1871 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R115_file_deletion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1649 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R116_insecure_file_permission.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1661 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R117_external_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1927 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R201_changed_data_dependence.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2123 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R202_unconditional_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2181 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R203_unused_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2180 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1707 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R301_non_fqcn_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1827 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R301_non_fqcn_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1430 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R302_role_without_metadata.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1416 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R303_task_without_name.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1607 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R304_unresolved_module.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1712 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R305_unresolved_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1787 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R306_undefined_variable.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1925 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R401_list_all_inbound_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1609 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R402_list_all_used_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1939 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R404_show_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1974 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R501_dependency_suggestion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/rule_versions.json
+-rw-r--r--   0 hiro       (501) staff       (20)     1521 2024-01-18 08:23:31.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4224 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/safe_glob.py
+-rw-r--r--   0 hiro       (501) staff       (20)    50084 2024-04-30 04:35:16.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/scanner.py
+-rw-r--r--   0 hiro       (501) staff       (20)      401 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/task_keywords.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    43475 2024-04-25 12:41:17.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/tree.py
+-rw-r--r--   0 hiro       (501) staff       (20)    25900 2024-05-07 06:21:39.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/utils.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2251 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/ansible_risk_insight/yaml.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.053308 ansible-risk-insight-0.2.6/ansible_risk_insight.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)      272 2024-05-07 06:48:33.000000 ansible-risk-insight-0.2.6/ansible_risk_insight.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     8106 2024-05-07 06:48:33.000000 ansible-risk-insight-0.2.6/ansible_risk_insight.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2024-05-07 06:48:33.000000 ansible-risk-insight-0.2.6/ansible_risk_insight.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       99 2024-05-07 06:48:33.000000 ansible-risk-insight-0.2.6/ansible_risk_insight.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       86 2024-05-07 06:48:33.000000 ansible-risk-insight-0.2.6/ansible_risk_insight.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       21 2024-05-07 06:48:33.000000 ansible-risk-insight-0.2.6/ansible_risk_insight.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.2.6/data-struct.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.038466 ansible-risk-insight-0.2.6/doc/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.087842 ansible-risk-insight-0.2.6/doc/images/
+-rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.6/doc/images/ari-apply-rules.png
+-rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.6/doc/images/ari-arch.png
+-rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.6/doc/images/ari-overview.png
+-rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.2.6/doc/images/ari-ram-list.png
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.091177 ansible-risk-insight-0.2.6/docs/
+-rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.2.6/docs/annotation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.2.6/docs/customize_rules.md
+-rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.2.6/docs/index.md
+-rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.2.6/docs/installing.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.097138 ansible-risk-insight-0.2.6/docs/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.2.6/docs/rules/R301_non_fqcn_use.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.097810 ansible-risk-insight-0.2.6/example/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.097967 ansible-risk-insight-0.2.6/example/playbooks/
+-rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.2.6/example/playbooks/sample_playbook.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.2.6/example/readme.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.098313 ansible-risk-insight-0.2.6/example/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     1366 2024-01-18 08:23:32.000000 ansible-risk-insight-0.2.6/example/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1728 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/example/sample.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.2.6/mkdocs.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      981 2024-05-07 06:21:39.000000 ansible-risk-insight-0.2.6/pyproject.toml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.098781 ansible-risk-insight-0.2.6/scripts/
+-rw-r--r--   0 hiro       (501) staff       (20)     5105 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/scripts/gen_ram_slim.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5964 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/scripts/gen_ram_subset.py
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2024-05-07 06:48:34.102764 ansible-risk-insight-0.2.6/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.2.6/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.099076 ansible-risk-insight-0.2.6/test/
+-rw-r--r--   0 hiro       (501) staff       (20)     2668 2024-01-04 02:55:15.000000 ansible-risk-insight-0.2.6/test/test_scanner.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.039743 ansible-risk-insight-0.2.6/test/testdata/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.039240 ansible-risk-insight-0.2.6/test/testdata/projects/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.099667 ansible-risk-insight-0.2.6/test/testdata/projects/my.collection/
+-rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.6/test/testdata/projects/my.collection/MANIFEST.json
+-rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.6/test/testdata/projects/my.collection/galaxy.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.039429 ansible-risk-insight-0.2.6/test/testdata/projects/my.collection/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.039662 ansible-risk-insight-0.2.6/test/testdata/projects/my.collection/roles/sample-role-1/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.099971 ansible-risk-insight-0.2.6/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.6/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.100355 ansible-risk-insight-0.2.6/test/testdata/projects/my.collection/roles/sample-role-1/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.6/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.100866 ansible-risk-insight-0.2.6/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.6/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.039801 ansible-risk-insight-0.2.6/test/testdata/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.040030 ansible-risk-insight-0.2.6/test/testdata/roles/test_role/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.101405 ansible-risk-insight-0.2.6/test/testdata/roles/test_role/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.6/test/testdata/roles/test_role/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.101694 ansible-risk-insight-0.2.6/test/testdata/roles/test_role/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.6/test/testdata/roles/test_role/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2024-05-07 06:48:34.101996 ansible-risk-insight-0.2.6/test/testdata/roles/test_role/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.2.6/test/testdata/roles/test_role/tasks/main.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.2.6/tox.ini
```

### Comparing `ansible-risk-insight-0.2.5/.github/workflows/lint.yml` & `ansible-risk-insight-0.2.6/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/.github/workflows/test.yml` & `ansible-risk-insight-0.2.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/.gitignore` & `ansible-risk-insight-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/CONTRIBUTING.md` & `ansible-risk-insight-0.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/LICENSE` & `ansible-risk-insight-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/README.md` & `ansible-risk-insight-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/__init__.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/_version.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
```

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/analyzer.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/analyzer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/__init__.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/annotator_base.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/apt.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/apt.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/apt_key.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/apt_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/assemble.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/assemble.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/command.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/command.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/dnf.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/dnf.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/expect.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/expect.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/file.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/file.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/get_url.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/get_url.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/git.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/git.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/pip.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/pip.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/raw.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/raw.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/replace.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/replace.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/script.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/script.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/shell.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/subversion.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/subversion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/template.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/template.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/unarchive.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/unarchive.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List
 from ansible_risk_insight.models import Annotation, RiskAnnotation, TaskCall, DefaultRiskType, InboundTransferDetail
+from ansible_risk_insight.utils import parse_bool
 from ansible_risk_insight.annotators.module_annotator_base import ModuleAnnotator, ModuleAnnotatorResult
-from ansible.module_utils.parsing.convert_bool import boolean
 
 
 class UnarchiveAnnotator(ModuleAnnotator):
     fqcn: str = "ansible.builtin.unarchive"
     enabled: bool = True
 
     def run(self, task: TaskCall) -> List[Annotation]:
@@ -30,20 +30,20 @@
         remote_src = task.args.get("remote_src")
 
         is_remote_src = False
         if remote_src:
 
             if isinstance(remote_src.raw, str) or isinstance(remote_src.raw, bool):
                 try:
-                    is_remote_src = boolean(remote_src.raw)
+                    is_remote_src = parse_bool(remote_src.raw)
                 except Exception:
                     pass
             if not is_remote_src and (isinstance(remote_src.templated, str) or isinstance(remote_src.templated, bool)):
                 try:
-                    is_remote_src = boolean(remote_src.templated)
+                    is_remote_src = parse_bool(remote_src.templated)
                 except Exception:
                     pass
 
         url_sep = "://"
         is_download = False
         if is_remote_src and (url_sep in src.raw or url_sep in src.templated):
             is_download = True
```

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/uri.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/uri.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible.builtin/yum.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible.builtin/yum.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible_builtin.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible_builtin.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/ansible_builtin.py.bak` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/ansible_builtin.py.bak`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/module_annotator_base.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/module_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/risk_annotator_base.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/risk_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/sample_custom_annotator.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/sample_custom_annotator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/annotators/variable_resolver.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/annotators/variable_resolver.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/ansible_builtin_modules.json` & `ansible-risk-insight-0.2.6/ansible_risk_insight/ansible_builtin_modules.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/ansible_variables.txt` & `ansible-risk-insight-0.2.6/ansible_risk_insight/ansible_variables.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/awx_utils.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/awx_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/batch.sh` & `ansible-risk-insight-0.2.6/ansible_risk_insight/batch.sh`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/builtin-modules.txt` & `ansible-risk-insight-0.2.6/ansible_risk_insight/builtin-modules.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/__init__.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/__init__.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/diff.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/diff.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/generate.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/generate.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/list.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/list.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/release.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/release.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/search.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/search.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/cli/ram/update.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/cli/ram/update.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/context.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/context.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/dependency_dir_preparator.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/dependency_dir_preparator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/dependency_finder.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/dependency_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # limitations under the License.
 
 import os
 import yaml
 import json
 import subprocess
 from pathlib import Path
-from ansible import constants as C
 
 import ansible_risk_insight.logger as logger
 from .safe_glob import safe_glob
 
 from .models import (
     LoadType,
 )
@@ -31,14 +30,15 @@
 collection_manifest_json = "MANIFEST.json"
 role_meta_main_yml = "meta/main.yml"
 role_meta_main_yaml = "meta/main.yaml"
 requirements_yml = "requirements.yml"
 galaxy_yml = "galaxy.yml"
 GALAXY_yml = "GALAXY.yml"
 github_workflows_dir = ".github/workflows"
+ansible_home = os.getenv("ANSIBLE_HOME", "~/.ansible")
 
 
 def find_dependency(type, target, dependency_dir, use_ansible_path=False):
     dependencies = {"dependencies": {}, "type": "", "file": ""}
     logger.debug("search dependency")
     if dependency_dir:
         requirements, paths, metadata = load_existing_dependency_dir(dependency_dir)
@@ -64,15 +64,15 @@
             logger.debug("search collection dependency")
             requirements, manifestjson = find_collection_dependency(target)
             dependencies["dependencies"] = requirements
             dependencies["type"] = LoadType.COLLECTION
             dependencies["file"] = manifestjson
 
     if use_ansible_path and dependencies["dependencies"]:
-        ansible_dir = Path(C.ANSIBLE_HOME).expanduser()
+        ansible_dir = Path(ansible_home).expanduser()
         paths, metadata = search_ansible_dir(dependencies["dependencies"], str(ansible_dir))
         if paths:
             dependencies["paths"] = paths
         if metadata:
             dependencies["metadata"] = metadata
 
     return dependencies
```

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/finder.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/findings.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/findings.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/key_test.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/key_test.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/keyutil.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/keyutil.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/loader.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/loader.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/logger.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/model_loader.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/model_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 try:
     # if `libyaml` is available, use C based loader for performance
     import _yaml  # noqa: F401
     from yaml import CSafeLoader as Loader
 except Exception:
     # otherwise, use Python based loader
     from yaml import SafeLoader as Loader
-from ansible.module_utils.parsing.convert_bool import boolean
 
 import ansible_risk_insight.logger as logger
+from ansible_risk_insight.utils import parse_bool
 from .safe_glob import safe_glob
 from .models import (
     ExecutableType,
     Inventory,
     InventoryType,
     File,
     LoadType,
@@ -1356,15 +1356,15 @@
 
                 arg_elements_type = get_class_by_arg_type(arg_spec.get("elements", None))
                 arg_elements_type_str = ""
                 if arg_elements_type:
                     arg_elements_type_str = arg_elements_type.__name__
                 required = None
                 try:
-                    required = boolean(arg_spec.get("required", "false"))
+                    required = parse_bool(arg_spec.get("required", "false"))
                 except Exception:
                     pass
                 arg = ModuleArgument(
                     name=arg_name,
                     type=arg_value_type_str,
                     elements=arg_elements_type_str,
                     required=required,
```

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/models.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from ruamel.yaml.scalarstring import DoubleQuotedScalarString
 
 from copy import deepcopy
 import json
 import jsonpickle
 from rapidfuzz.distance import Levenshtein
 import ansible_risk_insight.yaml as ariyaml
-from ansible.module_utils.parsing.convert_bool import boolean
+from ansible_risk_insight.utils import parse_bool
 from .keyutil import (
     set_collection_key,
     set_module_key,
     set_play_key,
     set_playbook_key,
     set_repository_key,
     set_role_key,
@@ -1060,15 +1060,15 @@
 
     @staticmethod
     def from_options(options: dict):
         if "become" in options:
             become = options.get("become", "")
             enabled = False
             try:
-                enabled = boolean(become)
+                enabled = parse_bool(become)
             except Exception:
                 pass
             user = options.get("become_user", "")
             method = options.get("become_method", "")
             flags = options.get("become_flags", "")
             return BecomeInfo(enabled=enabled, user=user, method=method, flags=flags)
         return None
```

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/parser.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/ram_generator.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/ram_generator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/risk_assessment_model.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/risk_assessment_model.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/risk_detector.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/risk_detector.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P001_module_name_validation.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/P001_module_name_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P002_module_argument_key_validation.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/P002_module_argument_key_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P003_module_argument_value_validation.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/P003_module_argument_value_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/P004_variable_validation.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/P004_variable_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R101_command_exec.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R101_command_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R102_command_instead_of_shell.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R102_command_instead_of_shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R103_download_exec.md` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R103_download_exec.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R103_download_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R104_unauthorized_download_src.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R104_unauthorized_download_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R105_outbound_transfer.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R105_outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R106_inbound_transfer.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R106_inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R108_privilege_escalation.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R108_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R109_key_config_change.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R109_key_config_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R110_non_builtin_use.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R110_non_builtin_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R111_parameterized_import_role.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R111_parameterized_import_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R113_parameterized_pkg_install.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R113_parameterized_pkg_install.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R114_file_change.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R114_file_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R115_file_deletion.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R115_file_deletion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R116_insecure_file_permission.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R116_insecure_file_permission.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R117_external_role.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R117_external_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R201_changed_data_dependence.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R201_changed_data_dependence.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R202_unconditional_override.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R202_unconditional_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R203_unused_override.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R203_unused_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R204_unnecessary_set_fact.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R204_unnecessary_set_fact.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R205_unnecessary_include_vars.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R205_unnecessary_include_vars.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R301_non_fqcn_use.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R301_non_fqcn_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R302_role_without_metadata.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R302_role_without_metadata.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R303_task_without_name.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R303_task_without_name.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R304_unresolved_module.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R304_unresolved_module.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R305_unresolved_role.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R305_unresolved_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R306_undefined_variable.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R306_undefined_variable.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R401_list_all_inbound_src.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R401_list_all_inbound_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R402_list_all_used_variables.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R402_list_all_used_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R404_show_variables.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R404_show_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/R501_dependency_suggestion.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/R501_dependency_suggestion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/__init__.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/rule_versions.json` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/rule_versions.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/rules/sample_rule.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/safe_glob.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/safe_glob.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/scanner.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,19 @@
     summarize_findings,
     summarize_findings_data,
     split_target_playbook_fullpath,
     split_target_taskfile_fullpath,
     equal,
 )
 
-
-default_config_path = os.path.expanduser("~/.ari/config")
+ARI_CONFIG_PATH = os.getenv("ARI_CONFIG_PATH")
+if ARI_CONFIG_PATH:
+    default_config_path = ARI_CONFIG_PATH
+else:
+    default_config_path = os.path.expanduser("~/.ari/config")
 default_data_dir = os.path.join("/tmp", "ari-data")
 default_rules_dir = os.path.join(os.path.dirname(__file__), "rules")
 default_log_level = "info"
 default_rules = []
 default_disable_default_rules = False
 default_logger_key = "ari"
```

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/tree.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/tree.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/utils.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,23 +17,29 @@
 import os
 import traceback
 import subprocess
 import requests
 import hashlib
 import yaml
 import json
+import codecs
 from filelock import FileLock
 from copy import deepcopy
 from tabulate import tabulate
 from inspect import isclass
 from importlib.util import spec_from_file_location, module_from_spec
 
 import ansible_risk_insight.logger as logger
 
 
+bool_values_true = frozenset(("y", "yes", "on", "1", "true", "t", 1, 1.0, True))
+bool_values_false = frozenset(("n", "no", "off", "0", "false", "f", 0, 0.0, False))
+bool_values = bool_values_true.union(bool_values_false)
+
+
 def lock_file(fpath, timeout=10):
     if not fpath:
         return
     lockfile = get_lock_file_name(fpath)
     lock = FileLock(lockfile, timeout=timeout)
     lock.acquire()
     return lock
@@ -735,7 +741,39 @@
         else:
             dst[k] = deepcopy(sv)
     return
 
 
 def is_test_object(path: str):
     return path.startswith("tests/integration/") or path.startswith("molecule/")
+
+
+def parse_bool(value: any):
+    value_str = None
+    use_value_str = False
+    if isinstance(value, bool):
+        return value
+    elif isinstance(value, str):
+        value_str = value
+        use_value_str = True
+    elif isinstance(value, bytes):
+        surrogateescape_enabled = False
+        try:
+            codecs.lookup_error("surrogateescape")
+            surrogateescape_enabled = True
+        except Exception:
+            pass
+        errors = "surrogateescape" if surrogateescape_enabled else "strict"
+        value_str = value.decode("utf-8", errors)
+        use_value_str = True
+
+    if use_value_str and isinstance(value_str, str):
+        value_str = value_str.lower().strip()
+
+    target_value = value_str if use_value_str else value
+
+    if target_value in bool_values_true:
+        return True
+    elif target_value in bool_values_false:
+        return False
+    else:
+        raise TypeError(f'failed to parse the value "{value}" as a boolean.')
```

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight/yaml.py` & `ansible-risk-insight-0.2.6/ansible_risk_insight/yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/ansible_risk_insight.egg-info/SOURCES.txt` & `ansible-risk-insight-0.2.6/ansible_risk_insight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/data-struct.txt` & `ansible-risk-insight-0.2.6/data-struct.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/doc/images/ari-apply-rules.png` & `ansible-risk-insight-0.2.6/doc/images/ari-apply-rules.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/doc/images/ari-arch.png` & `ansible-risk-insight-0.2.6/doc/images/ari-arch.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/doc/images/ari-overview.png` & `ansible-risk-insight-0.2.6/doc/images/ari-overview.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/doc/images/ari-ram-list.png` & `ansible-risk-insight-0.2.6/doc/images/ari-ram-list.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/docs/annotation.md` & `ansible-risk-insight-0.2.6/docs/annotation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/docs/customize_rules.md` & `ansible-risk-insight-0.2.6/docs/customize_rules.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/docs/rules/R103_download_exec.md` & `ansible-risk-insight-0.2.6/docs/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/docs/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.2.6/docs/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/docs/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.2.6/docs/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/docs/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.2.6/docs/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/example/readme.md` & `ansible-risk-insight-0.2.6/example/readme.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/example/rules/sample_rule.py` & `ansible-risk-insight-0.2.6/example/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/example/sample.py` & `ansible-risk-insight-0.2.6/example/sample.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/mkdocs.yml` & `ansible-risk-insight-0.2.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/pyproject.toml` & `ansible-risk-insight-0.2.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     "gitdb",
     "joblib",
     "jsonpickle",
     "PyYAML",
     "smmap",
     "tabulate",
     "requests",
-    "ansible-core",
     "ruamel.yaml",
     "filelock",
     "rapidfuzz",
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
```

### Comparing `ansible-risk-insight-0.2.5/scripts/gen_ram_slim.py` & `ansible-risk-insight-0.2.6/scripts/gen_ram_slim.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/scripts/gen_ram_subset.py` & `ansible-risk-insight-0.2.6/scripts/gen_ram_subset.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/test/test_scanner.py` & `ansible-risk-insight-0.2.6/test/test_scanner.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/test/testdata/projects/my.collection/MANIFEST.json` & `ansible-risk-insight-0.2.6/test/testdata/projects/my.collection/MANIFEST.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.2.5/tox.ini` & `ansible-risk-insight-0.2.6/tox.ini`

 * *Files identical despite different names*

