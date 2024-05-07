# Comparing `tmp/rattail-fabric2-0.3.3.tar.gz` & `tmp/rattail-fabric2-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rattail-fabric2-0.3.3.tar", last modified: Mon Sep 25 23:09:46 2023, max compression
+gzip compressed data, was "rattail-fabric2-0.3.4.tar", last modified: Tue May  7 19:14:48 2024, max compression
```

## Comparing `rattail-fabric2-0.3.3.tar` & `rattail-fabric2-0.3.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-25 23:09:46.949470 rattail-fabric2-0.3.3/
--rw-r--r--   0 lance     (1000) lance     (1000)     1483 2023-09-25 23:09:16.000000 rattail-fabric2-0.3.3/CHANGES.rst
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      105 2020-09-08 21:13:35.000000 rattail-fabric2-0.3.3/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     1188 2023-09-25 23:09:46.949470 rattail-fabric2-0.3.3/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      341 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/README.rst
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-25 23:09:46.945470 rattail-fabric2-0.3.3/rattail_fabric2/
--rw-r--r--   0 lance     (1000) lance     (1000)     1389 2023-05-17 12:21:22.000000 rattail-fabric2-0.3.3/rattail_fabric2/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-09-25 23:09:29.000000 rattail-fabric2-0.3.3/rattail_fabric2/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4672 2020-10-17 15:21:16.000000 rattail-fabric2-0.3.3/rattail_fabric2/apache.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3622 2020-09-29 01:17:27.000000 rattail-fabric2-0.3.3/rattail_fabric2/apt.py
--rw-r--r--   0 lance     (1000) lance     (1000)    10658 2023-02-23 19:05:47.000000 rattail-fabric2-0.3.3/rattail_fabric2/backup.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1304 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/borg.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1583 2023-01-05 13:40:50.000000 rattail-fabric2-0.3.3/rattail_fabric2/byjove.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2898 2020-12-15 18:31:03.000000 rattail-fabric2-0.3.3/rattail_fabric2/certbot.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2039 2023-02-19 17:19:37.000000 rattail-fabric2-0.3.3/rattail_fabric2/collectd.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1570 2022-08-27 03:27:45.000000 rattail-fabric2-0.3.3/rattail_fabric2/composer.py
--rw-r--r--   0 lance     (1000) lance     (1000)    13953 2023-08-09 00:14:24.000000 rattail-fabric2-0.3.3/rattail_fabric2/core.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6425 2023-06-10 22:48:33.000000 rattail-fabric2-0.3.3/rattail_fabric2/corepos.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-25 23:09:46.945470 rattail-fabric2-0.3.3/rattail_fabric2/deploy/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-25 23:09:46.945470 rattail-fabric2-0.3.3/rattail_fabric2/deploy/apt/
--rw-r--r--   0 lance     (1000) lance     (1000)       98 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/apt/listchanges.conf
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-25 23:09:46.945470 rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/
--rwxr-xr-x   0 lance     (1000) lance     (1000)      637 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/backup-everything.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      213 2023-02-23 19:03:28.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/crontab.mako
--rw-r--r--   0 lance     (1000) lance     (1000)       16 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/git-exclude
--rw-r--r--   0 lance     (1000) lance     (1000)      157 2019-02-06 20:44:14.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/logrotate.conf
--rw-r--r--   0 lance     (1000) lance     (1000)      790 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/luigi-logging.conf.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2030 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/luigi-overnight.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1029 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/luigi.cfg.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      599 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/overnight-backups.sh.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      467 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/rattail-backup.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      234 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/restart-overnight-backups.sh.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      318 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/supervisor.conf.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      656 2022-03-19 02:45:53.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/upgrade.sh.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)     1945 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/check-rattail-daemon
--rwxr-xr-x   0 lance     (1000) lance     (1000)     1848 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/check-supervisor-process
--rwxr-xr-x   0 lance     (1000) lance     (1000)     1598 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/check-systemd-service
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-25 23:09:46.945470 rattail-fabric2-0.3.3/rattail_fabric2/deploy/collectd/
--rw-r--r--   0 lance     (1000) lance     (1000)     1544 2022-08-22 03:36:50.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/collectd/check-mountpoints.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-25 23:09:46.945470 rattail-fabric2-0.3.3/rattail_fabric2/deploy/composer/
--rwxr-xr-x   0 lance     (1000) lance     (1000)      463 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/composer/install-composer.sh
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-25 23:09:46.945470 rattail-fabric2-0.3.3/rattail_fabric2/deploy/corepos/
--rw-r--r--   0 lance     (1000) lance     (1000)      386 2023-02-18 02:47:33.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/corepos/fannie-config.php.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-25 23:09:46.945470 rattail-fabric2-0.3.3/rattail_fabric2/deploy/luigi/
--rwxr-xr-x   0 lance     (1000) lance     (1000)      364 2022-11-27 18:22:06.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/luigi/cron-overnight.sh.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      191 2023-01-08 18:52:51.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/luigi/crontab.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      791 2022-01-28 20:25:09.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/luigi/logging.conf.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      414 2022-01-28 20:31:34.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/luigi/luigi-logrotate.conf.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     1468 2023-01-09 14:58:43.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/luigi/luigi.cfg.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      600 2022-01-28 21:02:15.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/luigi/overnight.sh.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      364 2022-11-27 18:22:37.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/luigi/restart-overnight.sh.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      359 2022-01-28 20:35:54.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/luigi/rotate-logs.sh.mako
--rw-r--r--   0 lance     (1000) lance     (1000)      335 2022-01-28 21:00:23.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/luigi/supervisor.conf.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-25 23:09:46.945470 rattail-fabric2-0.3.3/rattail_fabric2/deploy/python/
--rwxr-xr-x   0 lance     (1000) lance     (1000)      327 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/python/premkvirtualenv
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-25 23:09:46.945470 rattail-fabric2-0.3.3/rattail_fabric2/deploy/rattail/
--rwxr-xr-x   0 lance     (1000) lance     (1000)      620 2021-11-11 17:40:00.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/rattail/check-datasync-queue.mako
--rwxr-xr-x   0 lance     (1000) lance     (1000)      664 2021-11-11 17:40:07.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/rattail/check-datasync-watchers.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     2042 2023-06-02 19:34:23.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/rattail/rattail.conf.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     3849 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/deploy/soffice
--rw-r--r--   0 lance     (1000) lance     (1000)     2199 2023-01-05 17:41:25.000000 rattail-fabric2-0.3.3/rattail_fabric2/docker.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1292 2020-12-14 16:19:32.000000 rattail-fabric2-0.3.3/rattail_fabric2/ejabberd.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2099 2021-07-28 13:21:34.000000 rattail-fabric2-0.3.3/rattail_fabric2/freetds.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6791 2023-03-09 21:28:38.000000 rattail-fabric2-0.3.3/rattail_fabric2/luigi.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1283 2022-02-11 03:26:16.000000 rattail-fabric2-0.3.3/rattail_fabric2/mariadb.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1680 2023-06-09 03:48:53.000000 rattail-fabric2-0.3.3/rattail_fabric2/mssql.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7621 2023-08-04 20:35:24.000000 rattail-fabric2-0.3.3/rattail_fabric2/mysql.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2101 2023-08-03 15:53:50.000000 rattail-fabric2-0.3.3/rattail_fabric2/nodejs.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1702 2020-10-14 14:21:40.000000 rattail-fabric2-0.3.3/rattail_fabric2/pod.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3022 2023-01-09 18:03:43.000000 rattail-fabric2-0.3.3/rattail_fabric2/postfix.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9687 2023-09-17 16:10:31.000000 rattail-fabric2-0.3.3/rattail_fabric2/postgresql.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11414 2023-08-04 02:26:47.000000 rattail-fabric2-0.3.3/rattail_fabric2/python.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5088 2023-01-07 21:45:54.000000 rattail-fabric2-0.3.3/rattail_fabric2/rattail.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1271 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.3/rattail_fabric2/soffice.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3636 2020-10-09 21:38:14.000000 rattail-fabric2-0.3.3/rattail_fabric2/ssh.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11266 2023-01-07 23:20:19.000000 rattail-fabric2-0.3.3/rattail_fabric2/util.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-09-25 23:09:46.945470 rattail-fabric2-0.3.3/rattail_fabric2.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1188 2023-09-25 23:09:46.000000 rattail-fabric2-0.3.3/rattail_fabric2.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)     2650 2023-09-25 23:09:46.000000 rattail-fabric2-0.3.3/rattail_fabric2.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-09-25 23:09:46.000000 rattail-fabric2-0.3.3/rattail_fabric2.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-09-25 23:09:46.000000 rattail-fabric2-0.3.3/rattail_fabric2.egg-info/not-zip-safe
--rw-r--r--   0 lance     (1000) lance     (1000)       27 2023-09-25 23:09:46.000000 rattail-fabric2-0.3.3/rattail_fabric2.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       16 2023-09-25 23:09:46.000000 rattail-fabric2-0.3.3/rattail_fabric2.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      859 2023-09-25 23:09:46.949470 rattail-fabric2-0.3.3/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)      974 2023-05-16 18:47:04.000000 rattail-fabric2-0.3.3/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-07 19:14:48.879480 rattail-fabric2-0.3.4/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1597 2024-05-07 19:14:26.000000 rattail-fabric2-0.3.4/CHANGES.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      105 2020-09-08 21:13:35.000000 rattail-fabric2-0.3.4/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     1188 2024-05-07 19:14:48.879480 rattail-fabric2-0.3.4/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      341 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-07 19:14:48.875479 rattail-fabric2-0.3.4/rattail_fabric2/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1389 2023-05-17 12:21:22.000000 rattail-fabric2-0.3.4/rattail_fabric2/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2024-05-07 19:14:30.000000 rattail-fabric2-0.3.4/rattail_fabric2/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4672 2020-10-17 15:21:16.000000 rattail-fabric2-0.3.4/rattail_fabric2/apache.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3622 2020-09-29 01:17:27.000000 rattail-fabric2-0.3.4/rattail_fabric2/apt.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    10658 2023-02-23 19:05:47.000000 rattail-fabric2-0.3.4/rattail_fabric2/backup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1304 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/borg.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1583 2023-01-05 13:40:50.000000 rattail-fabric2-0.3.4/rattail_fabric2/byjove.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2898 2020-12-15 18:31:03.000000 rattail-fabric2-0.3.4/rattail_fabric2/certbot.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2039 2023-02-19 17:19:37.000000 rattail-fabric2-0.3.4/rattail_fabric2/collectd.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1570 2022-08-27 03:27:45.000000 rattail-fabric2-0.3.4/rattail_fabric2/composer.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    14153 2024-05-07 19:10:39.000000 rattail-fabric2-0.3.4/rattail_fabric2/core.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6425 2023-06-10 22:48:33.000000 rattail-fabric2-0.3.4/rattail_fabric2/corepos.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-07 19:14:48.875479 rattail-fabric2-0.3.4/rattail_fabric2/deploy/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-07 19:14:48.875479 rattail-fabric2-0.3.4/rattail_fabric2/deploy/apt/
+-rw-r--r--   0 lance     (1000) lance     (1000)       98 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/apt/listchanges.conf
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-07 19:14:48.875479 rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      637 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/backup-everything.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      213 2023-02-23 19:03:28.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/crontab.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)       16 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/git-exclude
+-rw-r--r--   0 lance     (1000) lance     (1000)      157 2019-02-06 20:44:14.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/logrotate.conf
+-rw-r--r--   0 lance     (1000) lance     (1000)      790 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/luigi-logging.conf.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2030 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/luigi-overnight.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1029 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/luigi.cfg.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      599 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/overnight-backups.sh.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      467 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/rattail-backup.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      234 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/restart-overnight-backups.sh.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      318 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/supervisor.conf.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      656 2022-03-19 02:45:53.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/upgrade.sh.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)     1945 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/check-rattail-daemon
+-rwxr-xr-x   0 lance     (1000) lance     (1000)     1848 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/check-supervisor-process
+-rwxr-xr-x   0 lance     (1000) lance     (1000)     1598 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/check-systemd-service
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-07 19:14:48.875479 rattail-fabric2-0.3.4/rattail_fabric2/deploy/collectd/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1544 2022-08-22 03:36:50.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/collectd/check-mountpoints.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-07 19:14:48.875479 rattail-fabric2-0.3.4/rattail_fabric2/deploy/composer/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      463 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/composer/install-composer.sh
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-07 19:14:48.875479 rattail-fabric2-0.3.4/rattail_fabric2/deploy/corepos/
+-rw-r--r--   0 lance     (1000) lance     (1000)      386 2023-02-18 02:47:33.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/corepos/fannie-config.php.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-07 19:14:48.875479 rattail-fabric2-0.3.4/rattail_fabric2/deploy/luigi/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      364 2022-11-27 18:22:06.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/luigi/cron-overnight.sh.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      191 2023-01-08 18:52:51.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/luigi/crontab.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      791 2022-01-28 20:25:09.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/luigi/logging.conf.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      414 2022-01-28 20:31:34.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/luigi/luigi-logrotate.conf.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     1468 2023-01-09 14:58:43.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/luigi/luigi.cfg.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      600 2022-01-28 21:02:15.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/luigi/overnight.sh.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      364 2022-11-27 18:22:37.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/luigi/restart-overnight.sh.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      359 2022-01-28 20:35:54.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/luigi/rotate-logs.sh.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      335 2022-01-28 21:00:23.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/luigi/supervisor.conf.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-07 19:14:48.875479 rattail-fabric2-0.3.4/rattail_fabric2/deploy/python/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      327 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/python/premkvirtualenv
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-07 19:14:48.879480 rattail-fabric2-0.3.4/rattail_fabric2/deploy/rattail/
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      620 2021-11-11 17:40:00.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/rattail/check-datasync-queue.mako
+-rwxr-xr-x   0 lance     (1000) lance     (1000)      664 2021-11-11 17:40:07.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/rattail/check-datasync-watchers.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     2042 2023-06-02 19:34:23.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/rattail/rattail.conf.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     3849 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/deploy/soffice
+-rw-r--r--   0 lance     (1000) lance     (1000)     2199 2023-01-05 17:41:25.000000 rattail-fabric2-0.3.4/rattail_fabric2/docker.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1292 2020-12-14 16:19:32.000000 rattail-fabric2-0.3.4/rattail_fabric2/ejabberd.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2099 2024-04-18 18:22:15.000000 rattail-fabric2-0.3.4/rattail_fabric2/freetds.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6791 2023-03-09 21:28:38.000000 rattail-fabric2-0.3.4/rattail_fabric2/luigi.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1283 2022-02-11 03:26:16.000000 rattail-fabric2-0.3.4/rattail_fabric2/mariadb.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1680 2023-06-09 03:48:53.000000 rattail-fabric2-0.3.4/rattail_fabric2/mssql.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7621 2023-11-18 16:27:18.000000 rattail-fabric2-0.3.4/rattail_fabric2/mysql.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2101 2023-08-03 15:53:50.000000 rattail-fabric2-0.3.4/rattail_fabric2/nodejs.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1702 2020-10-14 14:21:40.000000 rattail-fabric2-0.3.4/rattail_fabric2/pod.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3022 2023-01-09 18:03:43.000000 rattail-fabric2-0.3.4/rattail_fabric2/postfix.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9687 2023-09-17 16:10:31.000000 rattail-fabric2-0.3.4/rattail_fabric2/postgresql.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11414 2023-08-04 02:26:47.000000 rattail-fabric2-0.3.4/rattail_fabric2/python.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5088 2023-01-07 21:45:54.000000 rattail-fabric2-0.3.4/rattail_fabric2/rattail.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1271 2020-09-08 21:10:55.000000 rattail-fabric2-0.3.4/rattail_fabric2/soffice.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3636 2020-10-09 21:38:14.000000 rattail-fabric2-0.3.4/rattail_fabric2/ssh.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11266 2023-01-07 23:20:19.000000 rattail-fabric2-0.3.4/rattail_fabric2/util.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-07 19:14:48.879480 rattail-fabric2-0.3.4/rattail_fabric2.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1188 2024-05-07 19:14:48.000000 rattail-fabric2-0.3.4/rattail_fabric2.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)     2650 2024-05-07 19:14:48.000000 rattail-fabric2-0.3.4/rattail_fabric2.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-05-07 19:14:48.000000 rattail-fabric2-0.3.4/rattail_fabric2.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-05-07 19:14:48.000000 rattail-fabric2-0.3.4/rattail_fabric2.egg-info/not-zip-safe
+-rw-r--r--   0 lance     (1000) lance     (1000)       27 2024-05-07 19:14:48.000000 rattail-fabric2-0.3.4/rattail_fabric2.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       16 2024-05-07 19:14:48.000000 rattail-fabric2-0.3.4/rattail_fabric2.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      859 2024-05-07 19:14:48.879480 rattail-fabric2-0.3.4/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)      974 2023-05-16 18:47:04.000000 rattail-fabric2-0.3.4/setup.py
```

### Comparing `rattail-fabric2-0.3.3/CHANGES.rst` & `rattail-fabric2-0.3.4/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 
 CHANGELOG
 =========
 
+Unreleased
+----------
+
+0.3.4 (2024-05-07)
+------------------
+
+* Fix shell when creating new linux user account.
+
+
 0.3.3 (2023-09-25)
 ------------------
 
 * Add separate functions for dump, restore of mysql DB.
 
 * Preserve correct owner for ``.bashrc`` when configuring node.js.
```

### Comparing `rattail-fabric2-0.3.3/COPYING.txt` & `rattail-fabric2-0.3.4/COPYING.txt`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/PKG-INFO` & `rattail-fabric2-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-fabric2
-Version: 0.3.3
+Version: 0.3.4
 Summary: Fabric (v2) Utilities for Rattail
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/__init__.py` & `rattail-fabric2-0.3.4/rattail_fabric2/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/apache.py` & `rattail-fabric2-0.3.4/rattail_fabric2/apache.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/apt.py` & `rattail-fabric2-0.3.4/rattail_fabric2/apt.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/backup.py` & `rattail-fabric2-0.3.4/rattail_fabric2/backup.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/borg.py` & `rattail-fabric2-0.3.4/rattail_fabric2/borg.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/byjove.py` & `rattail-fabric2-0.3.4/rattail_fabric2/byjove.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/certbot.py` & `rattail-fabric2-0.3.4/rattail_fabric2/certbot.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/collectd.py` & `rattail-fabric2-0.3.4/rattail_fabric2/collectd.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/composer.py` & `rattail-fabric2-0.3.4/rattail_fabric2/composer.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/core.py` & `rattail-fabric2-0.3.4/rattail_fabric2/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,29 +125,37 @@
         func('chown {} {}'.format(owner, ' '.join(paths)))
     if mode is not None:
         func = c.sudo if use_sudo else c.run
         func('chmod {} {}'.format(mode, ' '.join(paths)))
 
 
 def make_normal_user(c, username, full_name=None,
-                     # TODO: ugh why is this true by default..should change that
-                     disabled_login=True,
-                     password=None):
+                     shell='/bin/bash',
+                     password=None,
+                     disabled_login=False):
     """
     Make a new "normal" user account.
+
+    :param disabled_login: If true, will leave the account in a
+       non-usable state, i.e. with invalid shell.
     """
-    if not c.run('getent passwd {}'.format(username), warn=True).failed:
+    # do not bother if user exists
+    missing = c.run(f'getent passwd {username}', warn=True).failed
+    if not missing:
         return
 
-    if password:
-        disabled_login = True
-    disabled_login = '--disabled-login' if disabled_login else ''
-    c.sudo("adduser --gecos '{}' {} {}".format(full_name or username,
-                                               disabled_login,
-                                               username))
+    # nb. specify --disabled-login to avoid being prompted for password
+    c.sudo("adduser --gecos '{}' --disabled-login {}".format(full_name or username,
+                                                             username))
+
+    # then fix the shell unless we shouldn't
+    if not disabled_login:
+        c.sudo(f'usermod -s {shell} {username}')
+
+    # and maybe set password
     if password:
         c.sudo(f"bash -c 'echo {username}:{password} | chpasswd'",
                echo=False)
 
 
 def make_system_user(c, name, home=None, uid=None, shell=None,
                      disabled_password=None):
```

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/corepos.py` & `rattail-fabric2-0.3.4/rattail_fabric2/corepos.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/backup-everything.mako` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/backup-everything.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/luigi-logging.conf.mako` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/luigi-logging.conf.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/luigi-overnight.py` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/luigi-overnight.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/luigi.cfg.mako` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/luigi.cfg.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/overnight-backups.sh.mako` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/overnight-backups.sh.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/backup/upgrade.sh.mako` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/backup/upgrade.sh.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/check-rattail-daemon` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/check-rattail-daemon`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/check-supervisor-process` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/check-supervisor-process`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/check-systemd-service` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/check-systemd-service`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/collectd/check-mountpoints.py` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/collectd/check-mountpoints.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/luigi/logging.conf.mako` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/luigi/logging.conf.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/luigi/luigi.cfg.mako` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/luigi/luigi.cfg.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/luigi/overnight.sh.mako` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/luigi/overnight.sh.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/rattail/check-datasync-queue.mako` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/rattail/check-datasync-queue.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/rattail/check-datasync-watchers.mako` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/rattail/check-datasync-watchers.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/rattail/rattail.conf.mako` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/rattail/rattail.conf.mako`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/deploy/soffice` & `rattail-fabric2-0.3.4/rattail_fabric2/deploy/soffice`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/docker.py` & `rattail-fabric2-0.3.4/rattail_fabric2/docker.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/ejabberd.py` & `rattail-fabric2-0.3.4/rattail_fabric2/ejabberd.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/freetds.py` & `rattail-fabric2-0.3.4/rattail_fabric2/freetds.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/luigi.py` & `rattail-fabric2-0.3.4/rattail_fabric2/luigi.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/mariadb.py` & `rattail-fabric2-0.3.4/rattail_fabric2/mariadb.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/mssql.py` & `rattail-fabric2-0.3.4/rattail_fabric2/mssql.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/mysql.py` & `rattail-fabric2-0.3.4/rattail_fabric2/mysql.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/nodejs.py` & `rattail-fabric2-0.3.4/rattail_fabric2/nodejs.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/pod.py` & `rattail-fabric2-0.3.4/rattail_fabric2/pod.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/postfix.py` & `rattail-fabric2-0.3.4/rattail_fabric2/postfix.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/postgresql.py` & `rattail-fabric2-0.3.4/rattail_fabric2/postgresql.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/python.py` & `rattail-fabric2-0.3.4/rattail_fabric2/python.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/rattail.py` & `rattail-fabric2-0.3.4/rattail_fabric2/rattail.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/soffice.py` & `rattail-fabric2-0.3.4/rattail_fabric2/soffice.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/ssh.py` & `rattail-fabric2-0.3.4/rattail_fabric2/ssh.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2/util.py` & `rattail-fabric2-0.3.4/rattail_fabric2/util.py`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2.egg-info/PKG-INFO` & `rattail-fabric2-0.3.4/rattail_fabric2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-fabric2
-Version: 0.3.3
+Version: 0.3.4
 Summary: Fabric (v2) Utilities for Rattail
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `rattail-fabric2-0.3.3/rattail_fabric2.egg-info/SOURCES.txt` & `rattail-fabric2-0.3.4/rattail_fabric2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/setup.cfg` & `rattail-fabric2-0.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `rattail-fabric2-0.3.3/setup.py` & `rattail-fabric2-0.3.4/setup.py`

 * *Files identical despite different names*

