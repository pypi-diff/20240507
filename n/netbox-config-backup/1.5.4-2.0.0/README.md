# Comparing `tmp/netbox_config_backup-1.5.4.tar.gz` & `tmp/netbox_config_backup-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_config_backup-1.5.4.tar", last modified: Tue Jan 23 20:25:03 2024, max compression
+gzip compressed data, was "netbox_config_backup-2.0.0.tar", last modified: Tue May  7 18:56:21 2024, max compression
```

## Comparing `netbox_config_backup-1.5.4.tar` & `netbox_config_backup-2.0.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.055966 netbox_config_backup-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-01-23 20:25:03.055966 netbox_config_backup-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.047967 netbox_config_backup-1.5.4/netbox_config_backup/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.047967 netbox_config_backup-1.5.4/netbox_config_backup/api/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.047967 netbox_config_backup-1.5.4/netbox_config_backup/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.051967 netbox_config_backup-1.5.4/netbox_config_backup/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/management/commands/enqueue_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/management/commands/fix_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/management/commands/listbackups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/management/commands/rebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/management/commands/runbackup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.051967 netbox_config_backup-1.5.4/netbox_config_backup/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/0002_git_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/0003_primary_model_to_bigid.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/0004_custom_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/0005_commit_add_time_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/0008_backupjob_scheduled_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/0010_backup_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/0011_alter_backup_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/0012_backup_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/0013_backup__to_netboxmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.055966 netbox_config_backup-1.5.4/netbox_config_backup/models/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/models/backups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/models/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/models/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.055966 netbox_config_backup-1.5.4/netbox_config_backup/querysets/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/querysets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.043967 netbox_config_backup-1.5.4/netbox_config_backup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.055966 netbox_config_backup-1.5.4/netbox_config_backup/templates/netbox_config_backup/
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/templates/netbox_config_backup/backup.html
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/templates/netbox_config_backup/backups.html
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/templates/netbox_config_backup/config.html
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/templates/netbox_config_backup/diff.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.055966 netbox_config_backup-1.5.4/netbox_config_backup/templates/netbox_config_backup/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/templates/netbox_config_backup/inc/backup_tables.html
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/templates/netbox_config_backup/repository.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.055966 netbox_config_backup-1.5.4/netbox_config_backup/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/templatetags/ncb_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.055966 netbox_config_backup-1.5.4/netbox_config_backup/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/utils/backups.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/utils/rq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/netbox_config_backup/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:25:03.055966 netbox_config_backup-1.5.4/netbox_config_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-01-23 20:25:03.000000 netbox_config_backup-1.5.4/netbox_config_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-01-23 20:25:03.000000 netbox_config_backup-1.5.4/netbox_config_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 20:25:03.000000 netbox_config_backup-1.5.4/netbox_config_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 20:25:03.000000 netbox_config_backup-1.5.4/netbox_config_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-23 20:25:03.000000 netbox_config_backup-1.5.4/netbox_config_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-23 20:25:03.000000 netbox_config_backup-1.5.4/netbox_config_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 20:25:03.055966 netbox_config_backup-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-01-23 20:24:52.000000 netbox_config_backup-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.212715 netbox_config_backup-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-07 18:56:21.208715 netbox_config_backup-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.200715 netbox_config_backup-2.0.0/netbox_config_backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.200715 netbox_config_backup-2.0.0/netbox_config_backup/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.200715 netbox_config_backup-2.0.0/netbox_config_backup/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.204715 netbox_config_backup-2.0.0/netbox_config_backup/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/management/commands/enqueue_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/management/commands/fix_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/management/commands/listbackups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/management/commands/rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/management/commands/runbackup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.204715 netbox_config_backup-2.0.0/netbox_config_backup/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/0002_git_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/0003_primary_model_to_bigid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/0004_custom_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/0005_commit_add_time_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/0008_backupjob_scheduled_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/0010_backup_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/0011_alter_backup_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/0012_backup_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/0013_backup__to_netboxmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.208715 netbox_config_backup-2.0.0/netbox_config_backup/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/models/backups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/models/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/models/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.208715 netbox_config_backup-2.0.0/netbox_config_backup/querysets/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/querysets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.196715 netbox_config_backup-2.0.0/netbox_config_backup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.208715 netbox_config_backup-2.0.0/netbox_config_backup/templates/netbox_config_backup/
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/templates/netbox_config_backup/backup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/templates/netbox_config_backup/backups.html
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/templates/netbox_config_backup/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/templates/netbox_config_backup/diff.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.208715 netbox_config_backup-2.0.0/netbox_config_backup/templates/netbox_config_backup/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/templates/netbox_config_backup/inc/backup_tables.html
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/templates/netbox_config_backup/repository.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.208715 netbox_config_backup-2.0.0/netbox_config_backup/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/templatetags/ncb_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.208715 netbox_config_backup-2.0.0/netbox_config_backup/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/utils/backups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/utils/rq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/netbox_config_backup/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:56:21.208715 netbox_config_backup-2.0.0/netbox_config_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-07 18:56:21.000000 netbox_config_backup-2.0.0/netbox_config_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-07 18:56:21.000000 netbox_config_backup-2.0.0/netbox_config_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:56:21.000000 netbox_config_backup-2.0.0/netbox_config_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:56:21.000000 netbox_config_backup-2.0.0/netbox_config_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 18:56:21.000000 netbox_config_backup-2.0.0/netbox_config_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 18:56:21.000000 netbox_config_backup-2.0.0/netbox_config_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 18:56:21.212715 netbox_config_backup-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-07 18:56:16.000000 netbox_config_backup-2.0.0/setup.py
```

### Comparing `netbox_config_backup-1.5.4/LICENSE` & `netbox_config_backup-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/PKG-INFO` & `netbox_config_backup-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox_config_backup
-Version: 1.5.4
+Version: 2.0.0
 Summary: NetBox Configuration Backup
 Home-page: https://github.com/dansheps/netbox-config-backup/
 Download-URL: https://github.com/dansheps/netbox-config-backup/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox_config_backup-1.5.4/README.md` & `netbox_config_backup-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/__init__.py` & `netbox_config_backup-2.0.0/netbox_config_backup/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from extras.plugins import PluginConfig
 from importlib.metadata import metadata
 
+from netbox.plugins import PluginConfig
+
 metadata = metadata('netbox_config_backup')
 
 
 class NetboxConfigBackup(PluginConfig):
     name = metadata.get('Name').replace('-', '_')
     verbose_name = metadata.get('Summary')
     description = metadata.get('Description')
     version = metadata.get('Version')
     author = metadata.get('Author')
     author_email = metadata.get('Author-email')
     base_url = 'configbackup'
-    min_version = '3.5.8'
-    max_version = '3.7.99'
+    min_version = '4.0.0-dev'
+    max_version = '4.0.99'
     required_settings = [
         'repository',
         'committer',
         'author',
     ]
     default_settings = {
         # Frequency in seconds
```

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/api/serializers.py` & `netbox_config_backup-2.0.0/netbox_config_backup/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/choices.py` & `netbox_config_backup-2.0.0/netbox_config_backup/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/filtersets.py` & `netbox_config_backup-2.0.0/netbox_config_backup/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/forms.py` & `netbox_config_backup-2.0.0/netbox_config_backup/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/git.py` & `netbox_config_backup-2.0.0/netbox_config_backup/git.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/management/commands/fix_missing.py` & `netbox_config_backup-2.0.0/netbox_config_backup/management/commands/fix_missing.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/management/commands/listbackups.py` & `netbox_config_backup-2.0.0/netbox_config_backup/management/commands/listbackups.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/management/commands/rebuild.py` & `netbox_config_backup-2.0.0/netbox_config_backup/management/commands/rebuild.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/management/commands/runbackup.py` & `netbox_config_backup-2.0.0/netbox_config_backup/management/commands/runbackup.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/migrations/0001_initial.py` & `netbox_config_backup-2.0.0/netbox_config_backup/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/migrations/0002_git_models.py` & `netbox_config_backup-2.0.0/netbox_config_backup/migrations/0002_git_models.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/migrations/0003_primary_model_to_bigid.py` & `netbox_config_backup-2.0.0/netbox_config_backup/migrations/0003_primary_model_to_bigid.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py` & `netbox_config_backup-2.0.0/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py` & `netbox_config_backup-2.0.0/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py` & `netbox_config_backup-2.0.0/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/migrations/0010_backup_ip.py` & `netbox_config_backup-2.0.0/netbox_config_backup/migrations/0010_backup_ip.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/migrations/0013_backup__to_netboxmodel.py` & `netbox_config_backup-2.0.0/netbox_config_backup/migrations/0013_backup__to_netboxmodel.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/models/backups.py` & `netbox_config_backup-2.0.0/netbox_config_backup/models/backups.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/models/jobs.py` & `netbox_config_backup-2.0.0/netbox_config_backup/models/jobs.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/models/repository.py` & `netbox_config_backup-2.0.0/netbox_config_backup/models/repository.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/navigation.py` & `netbox_config_backup-2.0.0/netbox_config_backup/navigation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from extras.plugins import PluginMenuItem, PluginMenuButton, PluginMenu
+from netbox.plugins import PluginMenuItem, PluginMenuButton, PluginMenu
 from utilities.choices import ButtonColorChoices
 
 assigned = PluginMenuItem(
     link='plugins:netbox_config_backup:backup_list',
     link_text='Devices',
     permissions=['netbox_config_backup.view_backups'],
     buttons=[
```

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/querysets/__init__.py` & `netbox_config_backup-2.0.0/netbox_config_backup/querysets/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/tables.py` & `netbox_config_backup-2.0.0/netbox_config_backup/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/tasks.py` & `netbox_config_backup-2.0.0/netbox_config_backup/tasks.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/template_content.py` & `netbox_config_backup-2.0.0/netbox_config_backup/template_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from extras.plugins import PluginTemplateExtension
+from netbox.plugins import PluginTemplateExtension
 
 from netbox_config_backup.models import Backup, BackupJob, BackupCommitTreeChange
 from netbox_config_backup.tables import BackupsTable
 from netbox_config_backup.utils.backups import get_backup_tables
 from utilities.htmx import is_htmx
 
 logger = logging.getLogger(f"netbox_config_backup")
```

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/templates/netbox_config_backup/backup.html` & `netbox_config_backup-2.0.0/netbox_config_backup/templates/netbox_config_backup/backup.html`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/templates/netbox_config_backup/backups.html` & `netbox_config_backup-2.0.0/netbox_config_backup/templates/netbox_config_backup/backups.html`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/templates/netbox_config_backup/diff.html` & `netbox_config_backup-2.0.0/netbox_config_backup/templates/netbox_config_backup/diff.html`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/urls.py` & `netbox_config_backup-2.0.0/netbox_config_backup/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/utils/backups.py` & `netbox_config_backup-2.0.0/netbox_config_backup/utils/backups.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/utils/git.py` & `netbox_config_backup-2.0.0/netbox_config_backup/utils/git.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/utils/rq.py` & `netbox_config_backup-2.0.0/netbox_config_backup/utils/rq.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup/views.py` & `netbox_config_backup-2.0.0/netbox_config_backup/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,19 +77,18 @@
 class BackupBackupsView(ObjectChildrenView):
     queryset = Backup.objects.all().default_annotate()
 
     template_name = 'netbox_config_backup/backups.html'
     child_model = BackupCommitTreeChange
     table = BackupsTable
     filterset = BackupsFilterSet
-    actions = ['config', 'diff', 'bulk_diff']
-    action_perms = {
+    actions = {
         'config': {'view'},
         'diff': {'view'},
-        'bulk_diff': {'view'},
+        'bulk_diff': {'view'}
     }
     tab = ViewTab(
         label='View Backups',
         badge=lambda obj: BackupCommitTreeChange.objects.filter(backup=obj, file__isnull=False).count(),
     )
 
     def get_children(self, request, parent):
```

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup.egg-info/PKG-INFO` & `netbox_config_backup-2.0.0/netbox_config_backup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox_config_backup
-Version: 1.5.4
+Version: 2.0.0
 Summary: NetBox Configuration Backup
 Home-page: https://github.com/dansheps/netbox-config-backup/
 Download-URL: https://github.com/dansheps/netbox-config-backup/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox_config_backup-1.5.4/netbox_config_backup.egg-info/SOURCES.txt` & `netbox_config_backup-2.0.0/netbox_config_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.5.4/setup.py` & `netbox_config_backup-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox_config_backup',
-    version='1.5.4',
+    version='2.0.0',
     description='NetBox Configuration Backup',
     long_description='Plugin to backup device configuration',
     url='https://github.com/dansheps/netbox-config-backup/',
     download_url='https://github.com/dansheps/netbox-config-backup/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     maintainer='Daniel Sheppard',
```

