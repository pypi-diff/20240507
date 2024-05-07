# Comparing `tmp/gsapme-0.1.0.tar.gz` & `tmp/gsapme-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsapme-0.1.0.tar", max compression
+gzip compressed data, was "gsapme-0.1.1.tar", max compression
```

## Comparing `gsapme-0.1.0.tar` & `gsapme-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-16 18:31:32.275422 gsapme-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-16 18:31:32.275309 gsapme-0.1.0/gsapme/__init__.py
--rw-r--r--   0        0        0     3819 2024-04-16 18:32:39.573728 gsapme-0.1.0/gsapme/gsatools.py
--rw-r--r--   0        0        0      283 2024-04-16 18:31:50.785048 gsapme-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 gsapme-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      602 2024-04-25 19:23:14.417182 gsapme-0.1.1/README.md
+-rw-r--r--   0        0        0      274 2024-05-07 18:31:10.358195 gsapme-0.1.1/gsapme/__init__.py
+-rw-r--r--   0        0        0     3952 2024-05-07 18:29:01.335000 gsapme-0.1.1/gsapme/analysis.py
+-rw-r--r--   0        0        0      897 2024-05-07 18:30:15.119156 gsapme-0.1.1/gsapme/covariance.py
+-rw-r--r--   0        0        0      788 2024-05-07 18:29:33.413899 gsapme-0.1.1/gsapme/models.py
+-rw-r--r--   0        0        0     2658 2024-05-07 18:29:16.024598 gsapme-0.1.1/gsapme/simulation.py
+-rw-r--r--   0        0        0      378 2024-05-07 18:53:05.131511 gsapme-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 gsapme-0.1.1/PKG-INFO
```

