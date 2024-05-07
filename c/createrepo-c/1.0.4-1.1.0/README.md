# Comparing `tmp/createrepo_c-1.0.4.tar.gz` & `tmp/createrepo_c-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "createrepo_c-1.0.4.tar", last modified: Wed Feb  7 14:30:26 2024, max compression
+gzip compressed data, was "createrepo_c-1.1.0.tar", last modified: Mon Mar 11 07:20:20 2024, max compression
```

## Comparing `createrepo_c-1.0.4.tar` & `createrepo_c-1.1.0.tar`

### file list

```diff
@@ -1,510 +1,511 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.515258 createrepo_c-1.0.4/
--rw-rw-r--   0 root         (0) root         (0)      499 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/AUTHORS
--rw-rw-r--   0 root         (0) root         (0)     5817 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)    18092 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/COPYING
--rw-rw-r--   0 root         (0) root         (0)      198 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      886 2024-02-07 14:30:26.515258 createrepo_c-1.0.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    11449 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/README.md
--rw-rw-r--   0 root         (0) root         (0)       54 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/VERSION.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.423258 createrepo_c-1.0.4/doc/
--rw-rw-r--   0 root         (0) root         (0)      637 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/doc/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)   114986 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/doc/Doxyfile.in.in
--rw-rw-r--   0 root         (0) root         (0)     8915 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/doc/createrepo_c.8
--rw-rw-r--   0 root         (0) root         (0)     1523 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/doc/logo.png
--rw-rw-r--   0 root         (0) root         (0)    80453 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/doc/logo.xcf
--rw-rw-r--   0 root         (0) root         (0)     3476 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/doc/mergerepo_c.8
--rw-rw-r--   0 root         (0) root         (0)     2164 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/doc/modifyrepo_c.8
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.423258 createrepo_c-1.0.4/doc/python/
--rw-rw-r--   0 root         (0) root         (0)      255 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/doc/python/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     8128 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/doc/python/conf.py
--rw-rw-r--   0 root         (0) root         (0)      307 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/doc/python/index.rst
--rw-rw-r--   0 root         (0) root         (0)      550 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/doc/python/lib.rst
--rw-rw-r--   0 root         (0) root         (0)     1772 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/doc/sqliterepo_c.8
--rw-rw-r--   0 root         (0) root         (0)      140 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       30 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-07 14:30:26.515258 createrepo_c-1.0.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2143 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.439258 createrepo_c-1.0.4/src/
--rw-rw-r--   0 root         (0) root         (0)     5252 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     8242 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/checksum.c
--rw-rw-r--   0 root         (0) root         (0)     3660 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/checksum.h
--rw-rw-r--   0 root         (0) root         (0)     4014 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/cleanup.h
--rw-rw-r--   0 root         (0) root         (0)    30663 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/cmd_parser.c
--rw-rw-r--   0 root         (0) root         (0)     9165 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/cmd_parser.h
--rw-rw-r--   0 root         (0) root         (0)    61067 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/compression_wrapper.c
--rw-rw-r--   0 root         (0) root         (0)     8273 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/compression_wrapper.h
--rw-rw-r--   0 root         (0) root         (0)     1138 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/constants.h
--rw-rw-r--   0 root         (0) root         (0)   105051 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/createrepo_c.c
--rw-rw-r--   0 root         (0) root         (0)     1654 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/createrepo_c.h
--rw-rw-r--   0 root         (0) root         (0)      345 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/createrepo_c.pc.cmake
--rw-rw-r--   0 root         (0) root         (0)     9307 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/createrepo_shared.c
--rw-rw-r--   0 root         (0) root         (0)     4331 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/createrepo_shared.h
--rw-rw-r--   0 root         (0) root         (0)    27830 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/deltarpms.c
--rw-rw-r--   0 root         (0) root         (0)     3729 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/deltarpms.h.in
--rw-rw-r--   0 root         (0) root         (0)    27612 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/dumper_thread.c
--rw-rw-r--   0 root         (0) root         (0)     6182 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/dumper_thread.h
--rw-rw-r--   0 root         (0) root         (0)     3422 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/error.c
--rw-rw-r--   0 root         (0) root         (0)     4018 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/error.h
--rw-rw-r--   0 root         (0) root         (0)    15382 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/helpers.c
--rw-rw-r--   0 root         (0) root         (0)     2751 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/helpers.h
--rw-rw-r--   0 root         (0) root         (0)    11353 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/koji.c
--rw-rw-r--   0 root         (0) root         (0)     3679 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/koji.h
--rw-rw-r--   0 root         (0) root         (0)    23784 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/load_metadata.c
--rw-rw-r--   0 root         (0) root         (0)     5524 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/load_metadata.h
--rw-rw-r--   0 root         (0) root         (0)    13005 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/locate_metadata.c
--rw-rw-r--   0 root         (0) root         (0)     5817 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/locate_metadata.h
--rw-rw-r--   0 root         (0) root         (0)    85295 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/mergerepo_c.c
--rw-rw-r--   0 root         (0) root         (0)     2547 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/mergerepo_c.h
--rw-rw-r--   0 root         (0) root         (0)     2356 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/metadata_internal.h
--rw-rw-r--   0 root         (0) root         (0)    45291 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/misc.c
--rw-rw-r--   0 root         (0) root         (0)    20338 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/misc.h
--rw-rw-r--   0 root         (0) root         (0)    11612 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/modifyrepo_c.c
--rw-rw-r--   0 root         (0) root         (0)    18914 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/modifyrepo_shared.c
--rw-rw-r--   0 root         (0) root         (0)     2240 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/modifyrepo_shared.h
--rw-rw-r--   0 root         (0) root         (0)     8081 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/package.c
--rw-rw-r--   0 root         (0) root         (0)     7680 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/package.h
--rw-rw-r--   0 root         (0) root         (0)     1303 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/package_internal.h
--rw-rw-r--   0 root         (0) root         (0)    26867 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/parsehdr.c
--rw-rw-r--   0 root         (0) root         (0)     2020 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/parsehdr.h
--rw-rw-r--   0 root         (0) root         (0)     8518 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/parsepkg.c
--rw-rw-r--   0 root         (0) root         (0)     5467 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/parsepkg.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.447258 createrepo_c-1.0.4/src/python/
--rw-rw-r--   0 root         (0) root         (0)     2730 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     1473 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/checksum-py.c
--rw-rw-r--   0 root         (0) root         (0)     1298 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/checksum-py.h
--rw-rw-r--   0 root         (0) root         (0)     6450 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/compression_wrapper-py.c
--rw-rw-r--   0 root         (0) root         (0)     1622 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/compression_wrapper-py.h
--rw-rw-r--   0 root         (0) root         (0)     6696 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/contentstat-py.c
--rw-rw-r--   0 root         (0) root         (0)     1104 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/contentstat-py.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.447258 createrepo_c-1.0.4/src/python/createrepo_c/
--rw-rw-r--   0 root         (0) root         (0)    14798 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/createrepo_c/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.447258 createrepo_c-1.0.4/src/python/createrepo_c.egg-info/
--rw-r--r--   0 root         (0) root         (0)      886 2024-02-07 14:30:26.000000 createrepo_c-1.0.4/src/python/createrepo_c.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20644 2024-02-07 14:30:26.000000 createrepo_c-1.0.4/src/python/createrepo_c.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-07 14:30:26.000000 createrepo_c-1.0.4/src/python/createrepo_c.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      180 2024-02-07 14:30:26.000000 createrepo_c-1.0.4/src/python/createrepo_c.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-02-07 14:30:26.000000 createrepo_c-1.0.4/src/python/createrepo_c.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)    12098 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/createrepo_cmodule.c
--rw-rw-r--   0 root         (0) root         (0)     2517 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/exception-py.c
--rw-rw-r--   0 root         (0) root         (0)     1307 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/exception-py.h
--rw-rw-r--   0 root         (0) root         (0)    10077 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/load_metadata-py.c
--rw-rw-r--   0 root         (0) root         (0)     1043 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/load_metadata-py.h
--rw-rw-r--   0 root         (0) root         (0)     7280 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/locate_metadata-py.c
--rw-rw-r--   0 root         (0) root         (0)     1143 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/locate_metadata-py.h
--rw-rw-r--   0 root         (0) root         (0)     2573 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/misc-py.c
--rw-rw-r--   0 root         (0) root         (0)     1495 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/misc-py.h
--rw-rw-r--   0 root         (0) root         (0)    19974 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/package-py.c
--rw-rw-r--   0 root         (0) root         (0)     1242 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/package-py.h
--rw-rw-r--   0 root         (0) root         (0)     4047 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/parsepkg-py.c
--rw-rw-r--   0 root         (0) root         (0)     1444 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/parsepkg-py.h
--rw-rw-r--   0 root         (0) root         (0)    13961 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/repomd-py.c
--rw-rw-r--   0 root         (0) root         (0)     1069 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/repomd-py.h
--rw-rw-r--   0 root         (0) root         (0)    13674 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/repomdrecord-py.c
--rw-rw-r--   0 root         (0) root         (0)     1168 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/repomdrecord-py.h
--rw-rw-r--   0 root         (0) root         (0)     5675 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/sqlite-py.c
--rw-rw-r--   0 root         (0) root         (0)     1023 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/sqlite-py.h
--rw-rw-r--   0 root         (0) root         (0)     7844 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/typeconversion.c
--rw-rw-r--   0 root         (0) root         (0)     1849 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/typeconversion.h
--rw-rw-r--   0 root         (0) root         (0)    10308 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/updatecollection-py.c
--rw-rw-r--   0 root         (0) root         (0)     1216 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/updatecollection-py.h
--rw-rw-r--   0 root         (0) root         (0)     7595 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/updatecollectionmodule-py.c
--rw-rw-r--   0 root         (0) root         (0)     1270 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/updatecollectionmodule-py.h
--rw-rw-r--   0 root         (0) root         (0)     8365 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/updatecollectionpackage-py.c
--rw-rw-r--   0 root         (0) root         (0)     1279 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/updatecollectionpackage-py.h
--rw-rw-r--   0 root         (0) root         (0)     7867 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/updateinfo-py.c
--rw-rw-r--   0 root         (0) root         (0)     1097 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/updateinfo-py.h
--rw-rw-r--   0 root         (0) root         (0)    15281 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/updaterecord-py.c
--rw-rw-r--   0 root         (0) root         (0)     1168 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/updaterecord-py.h
--rw-rw-r--   0 root         (0) root         (0)     6257 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/updatereference-py.c
--rw-rw-r--   0 root         (0) root         (0)     1195 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/updatereference-py.h
--rw-rw-r--   0 root         (0) root         (0)     4938 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/xml_dump-py.c
--rw-rw-r--   0 root         (0) root         (0)     2121 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/xml_dump-py.h
--rw-rw-r--   0 root         (0) root         (0)     7503 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/xml_file-py.c
--rw-rw-r--   0 root         (0) root         (0)     1030 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/xml_file-py.h
--rw-rw-r--   0 root         (0) root         (0)    27454 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/xml_parser-py.c
--rw-rw-r--   0 root         (0) root         (0)     3318 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/python/xml_parser-py.h
--rw-rw-r--   0 root         (0) root         (0)    36316 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/repomd.c
--rw-rw-r--   0 root         (0) root         (0)    11634 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/repomd.h
--rw-rw-r--   0 root         (0) root         (0)     1359 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/repomd_internal.h
--rw-rw-r--   0 root         (0) root         (0)    48204 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/sqlite.c
--rw-rw-r--   0 root         (0) root         (0)     5768 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/sqlite.h
--rw-rw-r--   0 root         (0) root         (0)    34375 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/sqliterepo_c.c
--rw-rw-r--   0 root         (0) root         (0)     5190 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/threads.c
--rw-rw-r--   0 root         (0) root         (0)     5854 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/threads.h
--rw-rw-r--   0 root         (0) root         (0)     9476 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/updateinfo.c
--rw-rw-r--   0 root         (0) root         (0)     5407 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/updateinfo.h
--rw-rw-r--   0 root         (0) root         (0)     1312 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/version.h.in
--rw-rw-r--   0 root         (0) root         (0)    11665 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_dump.c
--rw-rw-r--   0 root         (0) root         (0)     7618 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_dump.h
--rw-rw-r--   0 root         (0) root         (0)     4545 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_dump_deltapackage.c
--rw-rw-r--   0 root         (0) root         (0)     3911 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_dump_filelists.c
--rw-rw-r--   0 root         (0) root         (0)     3145 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_dump_internal.h
--rw-rw-r--   0 root         (0) root         (0)     4414 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_dump_other.c
--rw-rw-r--   0 root         (0) root         (0)    12665 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_dump_primary.c
--rw-rw-r--   0 root         (0) root         (0)     8750 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_dump_repomd.c
--rw-rw-r--   0 root         (0) root         (0)     9530 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_dump_updateinfo.c
--rw-rw-r--   0 root         (0) root         (0)    15944 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_file.c
--rw-rw-r--   0 root         (0) root         (0)    10285 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_file.h
--rw-rw-r--   0 root         (0) root         (0)     9177 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_parser.c
--rw-rw-r--   0 root         (0) root         (0)    13838 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_parser.h
--rw-rw-r--   0 root         (0) root         (0)    14997 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_parser_filelists.c
--rw-rw-r--   0 root         (0) root         (0)     9269 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_parser_internal.h
--rw-rw-r--   0 root         (0) root         (0)    17385 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_parser_main_metadata_together.c
--rw-rw-r--   0 root         (0) root         (0)    13200 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_parser_other.c
--rw-rw-r--   0 root         (0) root         (0)    27752 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_parser_primary.c
--rw-rw-r--   0 root         (0) root         (0)    14399 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_parser_repomd.c
--rw-rw-r--   0 root         (0) root         (0)    20016 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/src/xml_parser_updateinfo.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.451258 createrepo_c-1.0.4/tests/
--rw-rw-r--   0 root         (0) root         (0)     2887 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.467258 createrepo_c-1.0.4/tests/createrepo/
--rw-rw-r--   0 root         (0) root         (0)     5252 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     8242 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/checksum.c
--rw-rw-r--   0 root         (0) root         (0)     3660 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/checksum.h
--rw-rw-r--   0 root         (0) root         (0)     4014 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/cleanup.h
--rw-rw-r--   0 root         (0) root         (0)    30663 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/cmd_parser.c
--rw-rw-r--   0 root         (0) root         (0)     9165 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/cmd_parser.h
--rw-rw-r--   0 root         (0) root         (0)    61067 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/compression_wrapper.c
--rw-rw-r--   0 root         (0) root         (0)     8273 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/compression_wrapper.h
--rw-rw-r--   0 root         (0) root         (0)     1138 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/constants.h
--rw-rw-r--   0 root         (0) root         (0)   105051 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/createrepo_c.c
--rw-rw-r--   0 root         (0) root         (0)     1654 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/createrepo_c.h
--rw-rw-r--   0 root         (0) root         (0)      345 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/createrepo_c.pc.cmake
--rw-rw-r--   0 root         (0) root         (0)     9307 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/createrepo_shared.c
--rw-rw-r--   0 root         (0) root         (0)     4331 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/createrepo_shared.h
--rw-rw-r--   0 root         (0) root         (0)    27830 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/deltarpms.c
--rw-rw-r--   0 root         (0) root         (0)     3729 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/deltarpms.h.in
--rw-rw-r--   0 root         (0) root         (0)    27612 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/dumper_thread.c
--rw-rw-r--   0 root         (0) root         (0)     6182 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/dumper_thread.h
--rw-rw-r--   0 root         (0) root         (0)     3422 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/error.c
--rw-rw-r--   0 root         (0) root         (0)     4018 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/error.h
--rw-rw-r--   0 root         (0) root         (0)    15382 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/helpers.c
--rw-rw-r--   0 root         (0) root         (0)     2751 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/helpers.h
--rw-rw-r--   0 root         (0) root         (0)    11353 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/koji.c
--rw-rw-r--   0 root         (0) root         (0)     3679 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/koji.h
--rw-rw-r--   0 root         (0) root         (0)    23784 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/load_metadata.c
--rw-rw-r--   0 root         (0) root         (0)     5524 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/load_metadata.h
--rw-rw-r--   0 root         (0) root         (0)    13005 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/locate_metadata.c
--rw-rw-r--   0 root         (0) root         (0)     5817 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/locate_metadata.h
--rw-rw-r--   0 root         (0) root         (0)    85295 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/mergerepo_c.c
--rw-rw-r--   0 root         (0) root         (0)     2547 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/mergerepo_c.h
--rw-rw-r--   0 root         (0) root         (0)     2356 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/metadata_internal.h
--rw-rw-r--   0 root         (0) root         (0)    45291 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/misc.c
--rw-rw-r--   0 root         (0) root         (0)    20338 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/misc.h
--rw-rw-r--   0 root         (0) root         (0)    11612 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/modifyrepo_c.c
--rw-rw-r--   0 root         (0) root         (0)    18914 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/modifyrepo_shared.c
--rw-rw-r--   0 root         (0) root         (0)     2240 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/modifyrepo_shared.h
--rw-rw-r--   0 root         (0) root         (0)     8081 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/package.c
--rw-rw-r--   0 root         (0) root         (0)     7680 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/package.h
--rw-rw-r--   0 root         (0) root         (0)     1303 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/package_internal.h
--rw-rw-r--   0 root         (0) root         (0)    26867 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/parsehdr.c
--rw-rw-r--   0 root         (0) root         (0)     2020 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/parsehdr.h
--rw-rw-r--   0 root         (0) root         (0)     8518 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/parsepkg.c
--rw-rw-r--   0 root         (0) root         (0)     5467 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/parsepkg.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.479258 createrepo_c-1.0.4/tests/createrepo/python/
--rw-rw-r--   0 root         (0) root         (0)     2730 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     1473 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/checksum-py.c
--rw-rw-r--   0 root         (0) root         (0)     1298 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/checksum-py.h
--rw-rw-r--   0 root         (0) root         (0)     6450 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/compression_wrapper-py.c
--rw-rw-r--   0 root         (0) root         (0)     1622 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/compression_wrapper-py.h
--rw-rw-r--   0 root         (0) root         (0)     6696 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/contentstat-py.c
--rw-rw-r--   0 root         (0) root         (0)     1104 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/contentstat-py.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.479258 createrepo_c-1.0.4/tests/createrepo/python/createrepo_c/
--rw-rw-r--   0 root         (0) root         (0)    14798 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/createrepo_c/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.479258 createrepo_c-1.0.4/tests/createrepo/python/createrepo_c.egg-info/
--rw-r--r--   0 root         (0) root         (0)      886 2024-02-07 14:30:26.000000 createrepo_c-1.0.4/tests/createrepo/python/createrepo_c.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20644 2024-02-07 14:30:26.000000 createrepo_c-1.0.4/tests/createrepo/python/createrepo_c.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-07 14:30:26.000000 createrepo_c-1.0.4/tests/createrepo/python/createrepo_c.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      180 2024-02-07 14:30:26.000000 createrepo_c-1.0.4/tests/createrepo/python/createrepo_c.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-02-07 14:30:26.000000 createrepo_c-1.0.4/tests/createrepo/python/createrepo_c.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)    12098 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/createrepo_cmodule.c
--rw-rw-r--   0 root         (0) root         (0)     2517 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/exception-py.c
--rw-rw-r--   0 root         (0) root         (0)     1307 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/exception-py.h
--rw-rw-r--   0 root         (0) root         (0)    10077 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/load_metadata-py.c
--rw-rw-r--   0 root         (0) root         (0)     1043 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/load_metadata-py.h
--rw-rw-r--   0 root         (0) root         (0)     7280 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/locate_metadata-py.c
--rw-rw-r--   0 root         (0) root         (0)     1143 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/locate_metadata-py.h
--rw-rw-r--   0 root         (0) root         (0)     2573 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/misc-py.c
--rw-rw-r--   0 root         (0) root         (0)     1495 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/misc-py.h
--rw-rw-r--   0 root         (0) root         (0)    19974 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/package-py.c
--rw-rw-r--   0 root         (0) root         (0)     1242 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/package-py.h
--rw-rw-r--   0 root         (0) root         (0)     4047 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/parsepkg-py.c
--rw-rw-r--   0 root         (0) root         (0)     1444 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/parsepkg-py.h
--rw-rw-r--   0 root         (0) root         (0)    13961 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/repomd-py.c
--rw-rw-r--   0 root         (0) root         (0)     1069 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/repomd-py.h
--rw-rw-r--   0 root         (0) root         (0)    13674 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/repomdrecord-py.c
--rw-rw-r--   0 root         (0) root         (0)     1168 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/repomdrecord-py.h
--rw-rw-r--   0 root         (0) root         (0)     5675 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/sqlite-py.c
--rw-rw-r--   0 root         (0) root         (0)     1023 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/sqlite-py.h
--rw-rw-r--   0 root         (0) root         (0)     7844 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/typeconversion.c
--rw-rw-r--   0 root         (0) root         (0)     1849 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/typeconversion.h
--rw-rw-r--   0 root         (0) root         (0)    10308 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/updatecollection-py.c
--rw-rw-r--   0 root         (0) root         (0)     1216 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/updatecollection-py.h
--rw-rw-r--   0 root         (0) root         (0)     7595 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/updatecollectionmodule-py.c
--rw-rw-r--   0 root         (0) root         (0)     1270 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/updatecollectionmodule-py.h
--rw-rw-r--   0 root         (0) root         (0)     8365 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/updatecollectionpackage-py.c
--rw-rw-r--   0 root         (0) root         (0)     1279 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/updatecollectionpackage-py.h
--rw-rw-r--   0 root         (0) root         (0)     7867 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/updateinfo-py.c
--rw-rw-r--   0 root         (0) root         (0)     1097 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/updateinfo-py.h
--rw-rw-r--   0 root         (0) root         (0)    15281 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/updaterecord-py.c
--rw-rw-r--   0 root         (0) root         (0)     1168 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/updaterecord-py.h
--rw-rw-r--   0 root         (0) root         (0)     6257 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/updatereference-py.c
--rw-rw-r--   0 root         (0) root         (0)     1195 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/updatereference-py.h
--rw-rw-r--   0 root         (0) root         (0)     4938 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/xml_dump-py.c
--rw-rw-r--   0 root         (0) root         (0)     2121 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/xml_dump-py.h
--rw-rw-r--   0 root         (0) root         (0)     7503 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/xml_file-py.c
--rw-rw-r--   0 root         (0) root         (0)     1030 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/xml_file-py.h
--rw-rw-r--   0 root         (0) root         (0)    27454 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/xml_parser-py.c
--rw-rw-r--   0 root         (0) root         (0)     3318 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/python/xml_parser-py.h
--rw-rw-r--   0 root         (0) root         (0)    36316 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/repomd.c
--rw-rw-r--   0 root         (0) root         (0)    11634 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/repomd.h
--rw-rw-r--   0 root         (0) root         (0)     1359 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/repomd_internal.h
--rw-rw-r--   0 root         (0) root         (0)    48204 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/sqlite.c
--rw-rw-r--   0 root         (0) root         (0)     5768 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/sqlite.h
--rw-rw-r--   0 root         (0) root         (0)    34375 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/sqliterepo_c.c
--rw-rw-r--   0 root         (0) root         (0)     5190 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/threads.c
--rw-rw-r--   0 root         (0) root         (0)     5854 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/threads.h
--rw-rw-r--   0 root         (0) root         (0)     9476 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/updateinfo.c
--rw-rw-r--   0 root         (0) root         (0)     5407 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/updateinfo.h
--rw-rw-r--   0 root         (0) root         (0)     1312 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/version.h.in
--rw-rw-r--   0 root         (0) root         (0)    11665 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_dump.c
--rw-rw-r--   0 root         (0) root         (0)     7618 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_dump.h
--rw-rw-r--   0 root         (0) root         (0)     4545 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_dump_deltapackage.c
--rw-rw-r--   0 root         (0) root         (0)     3911 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_dump_filelists.c
--rw-rw-r--   0 root         (0) root         (0)     3145 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_dump_internal.h
--rw-rw-r--   0 root         (0) root         (0)     4414 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_dump_other.c
--rw-rw-r--   0 root         (0) root         (0)    12665 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_dump_primary.c
--rw-rw-r--   0 root         (0) root         (0)     8750 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_dump_repomd.c
--rw-rw-r--   0 root         (0) root         (0)     9530 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_dump_updateinfo.c
--rw-rw-r--   0 root         (0) root         (0)    15944 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_file.c
--rw-rw-r--   0 root         (0) root         (0)    10285 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_file.h
--rw-rw-r--   0 root         (0) root         (0)     9177 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_parser.c
--rw-rw-r--   0 root         (0) root         (0)    13838 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_parser.h
--rw-rw-r--   0 root         (0) root         (0)    14997 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_parser_filelists.c
--rw-rw-r--   0 root         (0) root         (0)     9269 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_parser_internal.h
--rw-rw-r--   0 root         (0) root         (0)    17385 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_parser_main_metadata_together.c
--rw-rw-r--   0 root         (0) root         (0)    13200 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_parser_other.c
--rw-rw-r--   0 root         (0) root         (0)    27752 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_parser_primary.c
--rw-rw-r--   0 root         (0) root         (0)    14399 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_parser_repomd.c
--rw-rw-r--   0 root         (0) root         (0)    20016 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/createrepo/xml_parser_updateinfo.c
--rw-rw-r--   0 root         (0) root         (0)    11645 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/fixtures.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.479258 createrepo_c-1.0.4/tests/python/
--rw-rw-r--   0 root         (0) root         (0)       25 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.483258 createrepo_c-1.0.4/tests/python/tests/
--rw-rw-r--   0 root         (0) root         (0)      167 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7555 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/fixtures.py
--rwxrwxr-x   0 root         (0) root         (0)      199 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/run_unittests.sh.in
--rw-rw-r--   0 root         (0) root         (0)     1212 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_checksum.py
--rw-rw-r--   0 root         (0) root         (0)     3564 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_compression_wrapper.py
--rw-rw-r--   0 root         (0) root         (0)     2514 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_contentstat.py
--rw-rw-r--   0 root         (0) root         (0)     4166 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_crfile.py
--rw-rw-r--   0 root         (0) root         (0)     3414 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_load_metadata.py
--rw-rw-r--   0 root         (0) root         (0)     4235 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_locate_metadata.py
--rw-rw-r--   0 root         (0) root         (0)     3249 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_misc.py
--rw-rw-r--   0 root         (0) root         (0)    10895 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_package.py
--rw-rw-r--   0 root         (0) root         (0)     2433 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_parsepkg.py
--rw-rw-r--   0 root         (0) root         (0)     4875 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_repomd.py
--rw-rw-r--   0 root         (0) root         (0)     7982 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_repomdrecord.py
--rw-rw-r--   0 root         (0) root         (0)    10544 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_sqlite.py
--rw-rw-r--   0 root         (0) root         (0)     3063 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_updatecollection.py
--rw-rw-r--   0 root         (0) root         (0)      938 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_updatecollectionmodule.py
--rw-rw-r--   0 root         (0) root         (0)     1760 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_updatecollectionpackage.py
--rw-rw-r--   0 root         (0) root         (0)    13055 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_updateinfo.py
--rw-rw-r--   0 root         (0) root         (0)     6315 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_updaterecord.py
--rw-rw-r--   0 root         (0) root         (0)      710 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_updatereference.py
--rw-rw-r--   0 root         (0) root         (0)      317 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_version.py
--rw-rw-r--   0 root         (0) root         (0)    14610 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_xml_file.py
--rw-rw-r--   0 root         (0) root         (0)    56717 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/python/tests/test_xml_parser.py
--rwxrwxr-x   0 root         (0) root         (0)      688 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/run_tests.sh.in
--rw-rw-r--   0 root         (0) root         (0)     5518 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_checksum.c
--rw-rw-r--   0 root         (0) root         (0)    32047 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_compression_wrapper.c
--rw-rw-r--   0 root         (0) root         (0)    14240 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_koji.c
--rw-rw-r--   0 root         (0) root         (0)     8130 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_load_metadata.c
--rw-rw-r--   0 root         (0) root         (0)    10128 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_locate_metadata.c
--rw-rw-r--   0 root         (0) root         (0)    43471 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_misc.c
--rw-rw-r--   0 root         (0) root         (0)     4673 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_modifyrepo_shared.c
--rw-rw-r--   0 root         (0) root         (0)     6327 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_sqlite.c
--rw-rw-r--   0 root         (0) root         (0)     4116 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_xml_dump.c
--rw-rw-r--   0 root         (0) root         (0)    15388 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_xml_dump_primary.c
--rw-rw-r--   0 root         (0) root         (0)     4565 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_xml_file.c
--rw-rw-r--   0 root         (0) root         (0)    17435 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_xml_parser_filelists.c
--rw-rw-r--   0 root         (0) root         (0)    11263 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_xml_parser_main_metadata_together.c
--rw-rw-r--   0 root         (0) root         (0)     4156 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_xml_parser_repomd.c
--rw-rw-r--   0 root         (0) root         (0)    10261 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/test_xml_parser_updateinfo.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.419258 createrepo_c-1.0.4/tests/testdata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.491258 createrepo_c-1.0.4/tests/testdata/compressed_files/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/00_plain.foo0
--rw-rw-r--   0 root         (0) root         (0)       33 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/00_plain.foo1
--rw-rw-r--   0 root         (0) root         (0)       14 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/00_plain.foo2
--rw-rw-r--   0 root         (0) root         (0)       32 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/00_plain.foo3
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/00_plain.foo4
--rw-rw-r--   0 root         (0) root         (0)       13 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/00_plain.foo5
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/00_plain.txt
--rw-rw-r--   0 root         (0) root         (0)       14 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/00_plain.txt.bz2
--rw-rw-r--   0 root         (0) root         (0)       33 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/00_plain.txt.gz
--rw-rw-r--   0 root         (0) root         (0)       32 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/00_plain.txt.xz
--rw-rw-r--   0 root         (0) root         (0)       95 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/00_plain.txt.zck
--rw-rw-r--   0 root         (0) root         (0)       13 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/00_plain.txt.zst
--rw-rw-r--   0 root         (0) root         (0)       56 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/01_plain.foo0
--rw-rw-r--   0 root         (0) root         (0)       64 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/01_plain.foo1
--rw-rw-r--   0 root         (0) root         (0)       69 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/01_plain.foo2
--rw-rw-r--   0 root         (0) root         (0)       96 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/01_plain.foo3
--rw-rw-r--   0 root         (0) root         (0)      169 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/01_plain.foo4
--rw-rw-r--   0 root         (0) root         (0)       51 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/01_plain.foo5
--rw-rw-r--   0 root         (0) root         (0)       56 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/01_plain.txt
--rw-rw-r--   0 root         (0) root         (0)       69 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/01_plain.txt.bz2
--rw-rw-r--   0 root         (0) root         (0)       64 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/01_plain.txt.gz
--rw-rw-r--   0 root         (0) root         (0)       96 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/01_plain.txt.xz
--rw-rw-r--   0 root         (0) root         (0)      158 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/01_plain.txt.zck
--rw-rw-r--   0 root         (0) root         (0)       51 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/compressed_files/01_plain.txt.zst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.491258 createrepo_c-1.0.4/tests/testdata/comps_files/
--rw-rw-r--   0 root         (0) root         (0)      638 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/comps_files/comps_00.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.495258 createrepo_c-1.0.4/tests/testdata/modified_repo_files/
--rw-rw-r--   0 root         (0) root         (0)      633 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/bad_file_type-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      570 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/error_00-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      802 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/error_00-other.xml
--rw-rw-r--   0 root         (0) root         (0)     3174 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/error_00-primary.xml
--rw-rw-r--   0 root         (0) root         (0)    68135 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/long_primary.xml
--rw-rw-r--   0 root         (0) root         (0)     1528 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/missing_type-repomd.xml
--rw-rw-r--   0 root         (0) root         (0)      764 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/multiple_warnings_00-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      985 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/multiple_warnings_00-other.xml
--rw-rw-r--   0 root         (0) root         (0)     3588 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/multiple_warnings_00-primary.xml
--rw-rw-r--   0 root         (0) root         (0)      510 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/no_pkgid-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      767 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/no_pkgid-other.xml
--rw-rw-r--   0 root         (0) root         (0)      405 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/repo_01_ampersand-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      551 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/repo_01_ampersand-other.xml
--rw-rw-r--   0 root         (0) root         (0)     2239 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/repo_01_ampersand-primary.xml
--rw-rw-r--   0 root         (0) root         (0)      598 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/repo_02_different_order_filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      608 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_00-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      840 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_00-other.xml
--rw-rw-r--   0 root         (0) root         (0)     3277 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_00-primary.xml
--rw-rw-r--   0 root         (0) root         (0)      606 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_01-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      838 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_01-other.xml
--rw-rw-r--   0 root         (0) root         (0)     3353 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_01-primary.xml
--rw-rw-r--   0 root         (0) root         (0)      657 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_02-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      889 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_02-other.xml
--rw-rw-r--   0 root         (0) root         (0)     3342 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_02-primary.xml
--rw-rw-r--   0 root         (0) root         (0)     1277 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/modified_repo_files/updateinfo_ampersand.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.495258 createrepo_c-1.0.4/tests/testdata/other_metadata/
--rw-rw-r--   0 root         (0) root         (0)      894 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/other_metadata/0402e012013246e7e2f2f638c8a6046efdfd71ae1cbeff9c391d9c1ae5d7d431-comps-f19.xml.bz2
--rw-rw-r--   0 root         (0) root         (0)     2364 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/other_metadata/36c4f2d6dda3b015b4a7da59552c7c76eff99a59979178513cb51341f6eead44-comps-f19.xml
--rw-rw-r--   0 root         (0) root         (0)      760 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/other_metadata/71d988ca33b31a18b0d775478d6f59b40583c794ae76393284850ee97bfba4dc-comps-f19.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      804 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/other_metadata/c941e2c77a27cdca324c0e0bc3190e134fddddb36a03fb5517e55d156b955205-comps-f19.xml.xz
--rw-rw-r--   0 root         (0) root         (0)     2364 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/other_metadata/comps-f19.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.499258 createrepo_c-1.0.4/tests/testdata/packages/
--rw-rw-r--   0 root         (0) root         (0)     3101 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/packages/Archer-3.4.5-6.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     3096 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/packages/Rimmer-1.0.2-2.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     1717 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/packages/balicek-iso88591-1.1.1-1.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     1741 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/packages/balicek-iso88592-1.1.1-1.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     1789 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/packages/balicek-utf8-1.1.1-1.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     1488 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/packages/empty-0-0.src.rpm
--rw-rw-r--   0 root         (0) root         (0)     1401 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/packages/empty-0-0.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     2237 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/packages/fake_bash-1.1.1-1.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     2845 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/packages/super_kernel-6.0.1-2.x86_64.rpm
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.415258 createrepo_c-1.0.4/tests/testdata/repo_00/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.499258 createrepo_c-1.0.4/tests/testdata/repo_00/repodata/
--rw-rw-r--   0 root         (0) root         (0)      134 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_00/repodata/1cb61ea996355add02b1426ed4c1780ea75ce0c04c5d1107c025c3fbd7d8bcae-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      262 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_00/repodata/2e7db4492173b6c437fd1299dc335e63d09f24cbdadeac5175a61b787c2f7a44-filelists.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      123 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_00/repodata/95a4415d859d7120efb6b3cf964c07bebbff9a5275ca673e6e74a97bcbfb2a5f-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      263 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_00/repodata/a939c4765106655c3f7a13fb41d0f239824efa66bcd6c1e6c044a854012bda75-other.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      269 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_00/repodata/e0ac03cd77e95e724dbf90ded0dba664e233315a8940051dd8882c56b9878595-primary.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      123 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_00/repodata/ef3e20691954c3d1318ec3071a982da339f4ed76967ded668b795c9e070aaab6-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     3381 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_00/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.415258 createrepo_c-1.0.4/tests/testdata/repo_01/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.499258 createrepo_c-1.0.4/tests/testdata/repo_01/repodata/
--rw-rw-r--   0 root         (0) root         (0)      783 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_01/repodata/6c662d665c24de9a0f62c17d8fa50622307739d7376f0d19097ca96c6d7f5e3e-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      332 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_01/repodata/b752a73d9efd4006d740f943db5fb7c2dd77a8324bd99da92e86bd55a2c126ef-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      273 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_01/repodata/c7db035d0e6f1b2e883a7fa3229e2d2be70c05a8b8d2b57dbb5f9c1a67483b6c-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1497 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_01/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.415258 createrepo_c-1.0.4/tests/testdata/repo_02/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.503258 createrepo_c-1.0.4/tests/testdata/repo_02/repodata/
--rw-rw-r--   0 root         (0) root         (0)      341 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_02/repodata/3b7e6ecd01af9cb674aff6458186911d7081bb5676d5562a21a963afc8a8bcc7-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      403 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_02/repodata/ab5d3edeea50f9b4ec5ee13e4d25c147e318e3a433dbabc94d3461f58ac28255-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      973 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_02/repodata/bcde64b04916a2a72fdc257d61bc922c70b3d58e953499180585f7a360ce86cf-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1497 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_02/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.415258 createrepo_c-1.0.4/tests/testdata/repo_03/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.503258 createrepo_c-1.0.4/tests/testdata/repo_03/repodata/
--rw-rw-r--   0 root         (0) root         (0)      134 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_03/repodata/1cb61ea996355add02b1426ed4c1780ea75ce0c04c5d1107c025c3fbd7d8bcae-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      262 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_03/repodata/2e7db4492173b6c437fd1299dc335e63d09f24cbdadeac5175a61b787c2f7a44-filelists.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      123 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_03/repodata/95a4415d859d7120efb6b3cf964c07bebbff9a5275ca673e6e74a97bcbfb2a5f-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1044 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_03/repodata/a850093e240506c728d6ce26a6fc51d6a7fe10730c67988d13afa7dd82df82d5-modules.yaml.xz
--rw-rw-r--   0 root         (0) root         (0)      263 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_03/repodata/a939c4765106655c3f7a13fb41d0f239824efa66bcd6c1e6c044a854012bda75-other.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      269 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_03/repodata/e0ac03cd77e95e724dbf90ded0dba664e233315a8940051dd8882c56b9878595-primary.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      123 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_03/repodata/ef3e20691954c3d1318ec3071a982da339f4ed76967ded668b795c9e070aaab6-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     3838 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_03/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.415258 createrepo_c-1.0.4/tests/testdata/repo_04/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.503258 createrepo_c-1.0.4/tests/testdata/repo_04/repodata/
--rw-rw-r--   0 root         (0) root         (0)      987 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_04/repodata/6a5f64dd82a126a161657764fe8f4b4092c0a3b61b9a34bde2af89dc1df112a1-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      397 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_04/repodata/6d0101044d9b4683e4ddc76491b3eb2228cddaace9e1d148c5eb138de9f71c17-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      429 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_04/repodata/d1c632d489f1c72b68b5c0d5de38ed1cb5c7a521380a88bed86771d39fb19538-filelists-ext.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      336 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_04/repodata/d7b8b1b6caa124aa17e4c6a1867e50e6893791ade0ebe212ab6f536695b5ce84-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     2012 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_04/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.415258 createrepo_c-1.0.4/tests/testdata/repo_koji_01/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.503258 createrepo_c-1.0.4/tests/testdata/repo_koji_01/repodata/
--rw-rw-r--   0 root         (0) root         (0)      816 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_koji_01/repodata/5d039d9ec332d158c69d083f04ac88a187c6b68444472b802eaf0249aec83294-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1007 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_koji_01/repodata/b153f86915d1dacbb89b244da26e50adb204195262fd3562290de26725daa21d-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      487 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_koji_01/repodata/c0e88e9a81f76341e91cd06f8ded80d4c289bdb4977e7624068802654b6da506-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1549 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_koji_01/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.415258 createrepo_c-1.0.4/tests/testdata/repo_koji_02/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.507258 createrepo_c-1.0.4/tests/testdata/repo_koji_02/repodata/
--rw-rw-r--   0 root         (0) root         (0)      338 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_koji_02/repodata/118e790330a62cfb167ce670478b25f4bfc58d7fc671096e4fd294fe40cee201-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      913 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_koji_02/repodata/ee9261d1d2916d841cf24bb01743198ec63ed596f410784602eca2350e430e17-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      687 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_koji_02/repodata/feb0b5fdcb0ee1cf981b041f0749ec381145cd9f6b4397991ef5dafcb6807bba-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1547 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_koji_02/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.415258 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.511258 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/
--rw-rw-r--   0 root         (0) root         (0)      656 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/0219a2f1f9f32af6b7873905269ac1bc27b03e0caf3968c929a49e5a939e8935-updateinfo_01.xml.gz.zck
--rw-rw-r--   0 root         (0) root         (0)     2366 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/04460bfaf6cb5af6b0925d8c99401a44e5192d287796aed4cced5f7ce881761f-comps.f20.xml
--rw-rw-r--   0 root         (0) root         (0)     3775 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/1e12239bf5cb07ec73c74482c35e80dabe30dbe2fdd57bd9e557d987cbacc8c2-primary.sqlite.bz2
--rw-rw-r--   0 root         (0) root         (0)      864 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.gz.zck
--rw-rw-r--   0 root         (0) root         (0)      864 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      932 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/3d6eaa7c77ef92586470dd6a542478e42cc421a85f12e0db93aa783077704cd0-filelists.xml.zck
--rw-rw-r--   0 root         (0) root         (0)     1287 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/490a2a494a3827b8a356f728ac36bc02fb009b0eaea173c890e727bb54219037-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1519 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/4f4de7d3254a033b84626f330bc6adb8a3c1a4a20f0ddbe30a5692a041318c81-filelists.sqlite.bz2
--rw-rw-r--   0 root         (0) root         (0)    88281 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/4fbad65c641f4f8fb3cec9b1672fcec2357443e1ea6e93541a0bb559c7dc9238-modules.yaml.gz
--rw-rw-r--   0 root         (0) root         (0)      533 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/88514679cb03d8f51e850ad3639c089f899e83407a2380ef9e62873a8eb1db13-updateinfo_01.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1301 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/8b13cba732c1a02b841f43d6791ca68788d45f376787d9f3ccf68e75f01af499-other.sqlite.bz2
--rw-rw-r--   0 root         (0) root         (0)      749 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/ba5a4fdbb20e7b9b70d9a9abd974bcab1065b1e81d711f80e06ad8cae30c4183-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      850 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/c5582e660ed9a2d3c10ba44f0aeb02f2bb70e85dc3c8cda4266183d4e5235aa7-other.xml.zck
--rw-rw-r--   0 root         (0) root         (0)    86680 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/cb0f4b5df8268f248158e50d66ee1565591bca23ee2dbd84ae9c457962fa3122-modules.yaml.gz.zck
--rw-rw-r--   0 root         (0) root         (0)     1482 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/e9e6ca4765de75cc3b2bf05e6cf631703c6557edd642300748d7747000547365-primary.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      748 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/f9d860ddcb64fbdc88a9b71a14ddb9f5670968d5dd3430412565c13d42b6804d-comps.f20.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      687 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/fd458a424a3f3e0dadc95b806674b79055c24e73637e47ad5a6e57926aa1b9d1-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     8640 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.419258 createrepo_c-1.0.4/tests/testdata/repo_with_duplicate_packages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.511258 createrepo_c-1.0.4/tests/testdata/repo_with_duplicate_packages/repodata/
--rw-rw-r--   0 root         (0) root         (0)      341 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_duplicate_packages/repodata/filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      405 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_duplicate_packages/repodata/other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1017 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_duplicate_packages/repodata/primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1354 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repo_with_duplicate_packages/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.511258 createrepo_c-1.0.4/tests/testdata/repodata_snippets/
--rw-rw-r--   0 root         (0) root         (0)      436 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repodata_snippets/filelists_ext_snippet_01.xml
--rw-rw-r--   0 root         (0) root         (0)      745 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repodata_snippets/filelists_ext_snippet_02.xml
--rw-rw-r--   0 root         (0) root         (0)      263 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repodata_snippets/filelists_snippet_01.xml
--rw-rw-r--   0 root         (0) root         (0)      471 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repodata_snippets/filelists_snippet_02.xml
--rw-rw-r--   0 root         (0) root         (0)      408 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repodata_snippets/other_snippet_01.xml
--rw-rw-r--   0 root         (0) root         (0)      697 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repodata_snippets/other_snippet_02.xml
--rw-rw-r--   0 root         (0) root         (0)     1918 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repodata_snippets/primary_snippet_01.xml
--rw-rw-r--   0 root         (0) root         (0)     3085 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/repodata_snippets/primary_snippet_02.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.515258 createrepo_c-1.0.4/tests/testdata/specs/
--rwxrwxr-x   0 root         (0) root         (0)       67 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/specs/build.sh
--rw-rw-r--   0 root         (0) root         (0)     1369 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/specs/fake-Archer.spec
--rw-rw-r--   0 root         (0) root         (0)     1023 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/specs/fake-Rimmer.spec
--rw-rw-r--   0 root         (0) root         (0)      571 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/specs/fake-balicek-iso88591.spec
--rw-rw-r--   0 root         (0) root         (0)      594 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/specs/fake-balicek-iso88592.spec
--rw-rw-r--   0 root         (0) root         (0)      653 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/specs/fake-balicek-utf8.spec
--rw-rw-r--   0 root         (0) root         (0)      176 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/specs/fake-empty.spec
--rw-rw-r--   0 root         (0) root         (0)      632 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/specs/fake-fake_bash.spec
--rw-rw-r--   0 root         (0) root         (0)     1236 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/specs/fake-super_kernel.spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.515258 createrepo_c-1.0.4/tests/testdata/test_files/
--rw-rw-r--   0 root         (0) root         (0)     1523 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/test_files/binary_file
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/test_files/empty_file
--rw-rw-r--   0 root         (0) root         (0)    24576 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/test_files/sqlite_file.sqlite
--rw-rw-r--   0 root         (0) root         (0)      910 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/test_files/text_file
--rw-rw-r--   0 root         (0) root         (0)      522 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/test_files/text_file.gz
--rw-rw-r--   0 root         (0) root         (0)      628 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/test_files/text_file.xz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 14:30:26.515258 createrepo_c-1.0.4/tests/testdata/updateinfo_files/
--rw-rw-r--   0 root         (0) root         (0)       60 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/updateinfo_files/updateinfo_00.xml
--rw-rw-r--   0 root         (0) root         (0)     1222 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/updateinfo_files/updateinfo_01.xml
--rw-rw-r--   0 root         (0) root         (0)      188 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/updateinfo_files/updateinfo_02.xml.xz
--rw-rw-r--   0 root         (0) root         (0)     4805 2024-02-07 14:25:15.000000 createrepo_c-1.0.4/tests/testdata/updateinfo_files/updateinfo_03.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.319782 createrepo_c-1.1.0/
+-rw-rw-r--   0 root         (0) root         (0)      499 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/AUTHORS
+-rw-rw-r--   0 root         (0) root         (0)     5817 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)    18092 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/COPYING
+-rw-rw-r--   0 root         (0) root         (0)      198 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      886 2024-03-11 07:20:20.319782 createrepo_c-1.1.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    11449 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)       54 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/VERSION.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.223782 createrepo_c-1.1.0/doc/
+-rw-rw-r--   0 root         (0) root         (0)      637 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/doc/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)   114986 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/doc/Doxyfile.in.in
+-rw-rw-r--   0 root         (0) root         (0)     8915 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/doc/createrepo_c.8
+-rw-rw-r--   0 root         (0) root         (0)     1523 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/doc/logo.png
+-rw-rw-r--   0 root         (0) root         (0)    80453 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/doc/logo.xcf
+-rw-rw-r--   0 root         (0) root         (0)     3476 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/doc/mergerepo_c.8
+-rw-rw-r--   0 root         (0) root         (0)     2164 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/doc/modifyrepo_c.8
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.223782 createrepo_c-1.1.0/doc/python/
+-rw-rw-r--   0 root         (0) root         (0)      255 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/doc/python/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     8128 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/doc/python/conf.py
+-rw-rw-r--   0 root         (0) root         (0)      307 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/doc/python/index.rst
+-rw-rw-r--   0 root         (0) root         (0)      550 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/doc/python/lib.rst
+-rw-rw-r--   0 root         (0) root         (0)     1772 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/doc/sqliterepo_c.8
+-rw-rw-r--   0 root         (0) root         (0)      140 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       30 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-11 07:20:20.319782 createrepo_c-1.1.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2143 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.239782 createrepo_c-1.1.0/src/
+-rw-rw-r--   0 root         (0) root         (0)     5252 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     8242 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/checksum.c
+-rw-rw-r--   0 root         (0) root         (0)     3660 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/checksum.h
+-rw-rw-r--   0 root         (0) root         (0)     4014 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/cleanup.h
+-rw-rw-r--   0 root         (0) root         (0)    30663 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/cmd_parser.c
+-rw-rw-r--   0 root         (0) root         (0)     9165 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/cmd_parser.h
+-rw-rw-r--   0 root         (0) root         (0)    61067 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/compression_wrapper.c
+-rw-rw-r--   0 root         (0) root         (0)     8271 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/compression_wrapper.h
+-rw-rw-r--   0 root         (0) root         (0)     1138 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/constants.h
+-rw-rw-r--   0 root         (0) root         (0)   105052 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/createrepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)     1654 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/createrepo_c.h
+-rw-rw-r--   0 root         (0) root         (0)      345 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/createrepo_c.pc.cmake
+-rw-rw-r--   0 root         (0) root         (0)     9307 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/createrepo_shared.c
+-rw-rw-r--   0 root         (0) root         (0)     4331 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/createrepo_shared.h
+-rw-rw-r--   0 root         (0) root         (0)    27830 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/deltarpms.c
+-rw-rw-r--   0 root         (0) root         (0)     3729 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/deltarpms.h.in
+-rw-rw-r--   0 root         (0) root         (0)    27612 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/dumper_thread.c
+-rw-rw-r--   0 root         (0) root         (0)     6182 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/dumper_thread.h
+-rw-rw-r--   0 root         (0) root         (0)     3422 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/error.c
+-rw-rw-r--   0 root         (0) root         (0)     4018 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/error.h
+-rw-rw-r--   0 root         (0) root         (0)    15382 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/helpers.c
+-rw-rw-r--   0 root         (0) root         (0)     2751 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/helpers.h
+-rw-rw-r--   0 root         (0) root         (0)    11353 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/koji.c
+-rw-rw-r--   0 root         (0) root         (0)     3679 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/koji.h
+-rw-rw-r--   0 root         (0) root         (0)    23784 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/load_metadata.c
+-rw-rw-r--   0 root         (0) root         (0)     5524 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/load_metadata.h
+-rw-rw-r--   0 root         (0) root         (0)    13005 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/locate_metadata.c
+-rw-rw-r--   0 root         (0) root         (0)     5817 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/locate_metadata.h
+-rw-rw-r--   0 root         (0) root         (0)    85295 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/mergerepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)     2547 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/mergerepo_c.h
+-rw-rw-r--   0 root         (0) root         (0)     2356 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/metadata_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    45291 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/misc.c
+-rw-rw-r--   0 root         (0) root         (0)    20338 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/misc.h
+-rw-rw-r--   0 root         (0) root         (0)    11612 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/modifyrepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)    18914 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/modifyrepo_shared.c
+-rw-rw-r--   0 root         (0) root         (0)     2240 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/modifyrepo_shared.h
+-rw-rw-r--   0 root         (0) root         (0)     8081 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/package.c
+-rw-rw-r--   0 root         (0) root         (0)     7680 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/package.h
+-rw-rw-r--   0 root         (0) root         (0)     1303 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/package_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    26867 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/parsehdr.c
+-rw-rw-r--   0 root         (0) root         (0)     2020 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/parsehdr.h
+-rw-rw-r--   0 root         (0) root         (0)     8518 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/parsepkg.c
+-rw-rw-r--   0 root         (0) root         (0)     5467 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/parsepkg.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.247782 createrepo_c-1.1.0/src/python/
+-rw-rw-r--   0 root         (0) root         (0)     2730 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     1473 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/checksum-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1298 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/checksum-py.h
+-rw-rw-r--   0 root         (0) root         (0)     6450 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/compression_wrapper-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1622 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/compression_wrapper-py.h
+-rw-rw-r--   0 root         (0) root         (0)     6696 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/contentstat-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1104 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/contentstat-py.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.247782 createrepo_c-1.1.0/src/python/createrepo_c/
+-rw-rw-r--   0 root         (0) root         (0)    29092 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/createrepo_c/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.247782 createrepo_c-1.1.0/src/python/createrepo_c.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      886 2024-03-11 07:20:20.000000 createrepo_c-1.1.0/src/python/createrepo_c.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20682 2024-03-11 07:20:20.000000 createrepo_c-1.1.0/src/python/createrepo_c.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 07:20:20.000000 createrepo_c-1.1.0/src/python/createrepo_c.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2024-03-11 07:20:20.000000 createrepo_c-1.1.0/src/python/createrepo_c.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-03-11 07:20:20.000000 createrepo_c-1.1.0/src/python/createrepo_c.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)    12098 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/createrepo_cmodule.c
+-rw-rw-r--   0 root         (0) root         (0)     2517 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/exception-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1307 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/exception-py.h
+-rw-rw-r--   0 root         (0) root         (0)    10077 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/load_metadata-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1043 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/load_metadata-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7280 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/locate_metadata-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1143 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/locate_metadata-py.h
+-rw-rw-r--   0 root         (0) root         (0)     2573 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/misc-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1495 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/misc-py.h
+-rw-rw-r--   0 root         (0) root         (0)    19974 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/package-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1242 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/package-py.h
+-rw-rw-r--   0 root         (0) root         (0)     4047 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/parsepkg-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1444 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/parsepkg-py.h
+-rw-rw-r--   0 root         (0) root         (0)    13961 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/repomd-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1069 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/repomd-py.h
+-rw-rw-r--   0 root         (0) root         (0)    13674 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/repomdrecord-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1168 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/repomdrecord-py.h
+-rw-rw-r--   0 root         (0) root         (0)     5675 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/sqlite-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1023 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/sqlite-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7844 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/typeconversion.c
+-rw-rw-r--   0 root         (0) root         (0)     1849 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/typeconversion.h
+-rw-rw-r--   0 root         (0) root         (0)    10308 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/updatecollection-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1216 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/updatecollection-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7595 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/updatecollectionmodule-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1270 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/updatecollectionmodule-py.h
+-rw-rw-r--   0 root         (0) root         (0)     8365 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/updatecollectionpackage-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1279 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/updatecollectionpackage-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7867 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/updateinfo-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1097 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/updateinfo-py.h
+-rw-rw-r--   0 root         (0) root         (0)    15281 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/updaterecord-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1168 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/updaterecord-py.h
+-rw-rw-r--   0 root         (0) root         (0)     6257 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/updatereference-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1195 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/updatereference-py.h
+-rw-rw-r--   0 root         (0) root         (0)     4938 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/xml_dump-py.c
+-rw-rw-r--   0 root         (0) root         (0)     2121 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/xml_dump-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7503 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/xml_file-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1030 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/xml_file-py.h
+-rw-rw-r--   0 root         (0) root         (0)    27454 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/xml_parser-py.c
+-rw-rw-r--   0 root         (0) root         (0)     3318 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/python/xml_parser-py.h
+-rw-rw-r--   0 root         (0) root         (0)    36316 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/repomd.c
+-rw-rw-r--   0 root         (0) root         (0)    11634 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/repomd.h
+-rw-rw-r--   0 root         (0) root         (0)     1359 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/repomd_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    48204 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/sqlite.c
+-rw-rw-r--   0 root         (0) root         (0)     5768 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/sqlite.h
+-rw-rw-r--   0 root         (0) root         (0)    34375 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/sqliterepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)     5190 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/threads.c
+-rw-rw-r--   0 root         (0) root         (0)     5854 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/threads.h
+-rw-rw-r--   0 root         (0) root         (0)     9476 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/updateinfo.c
+-rw-rw-r--   0 root         (0) root         (0)     5407 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/updateinfo.h
+-rw-rw-r--   0 root         (0) root         (0)     1312 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/version.h.in
+-rw-rw-r--   0 root         (0) root         (0)    16489 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_dump.c
+-rw-rw-r--   0 root         (0) root         (0)     7618 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_dump.h
+-rw-rw-r--   0 root         (0) root         (0)     4545 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_dump_deltapackage.c
+-rw-rw-r--   0 root         (0) root         (0)     3911 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_dump_filelists.c
+-rw-rw-r--   0 root         (0) root         (0)     3145 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_dump_internal.h
+-rw-rw-r--   0 root         (0) root         (0)     4414 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_dump_other.c
+-rw-rw-r--   0 root         (0) root         (0)    12665 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_dump_primary.c
+-rw-rw-r--   0 root         (0) root         (0)     8750 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_dump_repomd.c
+-rw-rw-r--   0 root         (0) root         (0)     9530 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_dump_updateinfo.c
+-rw-rw-r--   0 root         (0) root         (0)    15944 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_file.c
+-rw-rw-r--   0 root         (0) root         (0)    10285 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_file.h
+-rw-rw-r--   0 root         (0) root         (0)     9177 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_parser.c
+-rw-rw-r--   0 root         (0) root         (0)    13838 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_parser.h
+-rw-rw-r--   0 root         (0) root         (0)    14997 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_parser_filelists.c
+-rw-rw-r--   0 root         (0) root         (0)     9269 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_parser_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    17385 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_parser_main_metadata_together.c
+-rw-rw-r--   0 root         (0) root         (0)    13200 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_parser_other.c
+-rw-rw-r--   0 root         (0) root         (0)    27752 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_parser_primary.c
+-rw-rw-r--   0 root         (0) root         (0)    14399 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_parser_repomd.c
+-rw-rw-r--   0 root         (0) root         (0)    20016 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/src/xml_parser_updateinfo.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.251782 createrepo_c-1.1.0/tests/
+-rw-rw-r--   0 root         (0) root         (0)     2887 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.271782 createrepo_c-1.1.0/tests/createrepo/
+-rw-rw-r--   0 root         (0) root         (0)     5252 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     8242 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/checksum.c
+-rw-rw-r--   0 root         (0) root         (0)     3660 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/checksum.h
+-rw-rw-r--   0 root         (0) root         (0)     4014 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/cleanup.h
+-rw-rw-r--   0 root         (0) root         (0)    30663 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/cmd_parser.c
+-rw-rw-r--   0 root         (0) root         (0)     9165 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/cmd_parser.h
+-rw-rw-r--   0 root         (0) root         (0)    61067 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/compression_wrapper.c
+-rw-rw-r--   0 root         (0) root         (0)     8271 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/compression_wrapper.h
+-rw-rw-r--   0 root         (0) root         (0)     1138 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/constants.h
+-rw-rw-r--   0 root         (0) root         (0)   105052 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/createrepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)     1654 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/createrepo_c.h
+-rw-rw-r--   0 root         (0) root         (0)      345 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/createrepo_c.pc.cmake
+-rw-rw-r--   0 root         (0) root         (0)     9307 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/createrepo_shared.c
+-rw-rw-r--   0 root         (0) root         (0)     4331 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/createrepo_shared.h
+-rw-rw-r--   0 root         (0) root         (0)    27830 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/deltarpms.c
+-rw-rw-r--   0 root         (0) root         (0)     3729 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/deltarpms.h.in
+-rw-rw-r--   0 root         (0) root         (0)    27612 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/dumper_thread.c
+-rw-rw-r--   0 root         (0) root         (0)     6182 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/dumper_thread.h
+-rw-rw-r--   0 root         (0) root         (0)     3422 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/error.c
+-rw-rw-r--   0 root         (0) root         (0)     4018 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/error.h
+-rw-rw-r--   0 root         (0) root         (0)    15382 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/helpers.c
+-rw-rw-r--   0 root         (0) root         (0)     2751 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/helpers.h
+-rw-rw-r--   0 root         (0) root         (0)    11353 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/koji.c
+-rw-rw-r--   0 root         (0) root         (0)     3679 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/koji.h
+-rw-rw-r--   0 root         (0) root         (0)    23784 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/load_metadata.c
+-rw-rw-r--   0 root         (0) root         (0)     5524 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/load_metadata.h
+-rw-rw-r--   0 root         (0) root         (0)    13005 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/locate_metadata.c
+-rw-rw-r--   0 root         (0) root         (0)     5817 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/locate_metadata.h
+-rw-rw-r--   0 root         (0) root         (0)    85295 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/mergerepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)     2547 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/mergerepo_c.h
+-rw-rw-r--   0 root         (0) root         (0)     2356 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/metadata_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    45291 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/misc.c
+-rw-rw-r--   0 root         (0) root         (0)    20338 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/misc.h
+-rw-rw-r--   0 root         (0) root         (0)    11612 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/modifyrepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)    18914 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/modifyrepo_shared.c
+-rw-rw-r--   0 root         (0) root         (0)     2240 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/modifyrepo_shared.h
+-rw-rw-r--   0 root         (0) root         (0)     8081 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/package.c
+-rw-rw-r--   0 root         (0) root         (0)     7680 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/package.h
+-rw-rw-r--   0 root         (0) root         (0)     1303 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/package_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    26867 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/parsehdr.c
+-rw-rw-r--   0 root         (0) root         (0)     2020 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/parsehdr.h
+-rw-rw-r--   0 root         (0) root         (0)     8518 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/parsepkg.c
+-rw-rw-r--   0 root         (0) root         (0)     5467 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/parsepkg.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.279782 createrepo_c-1.1.0/tests/createrepo/python/
+-rw-rw-r--   0 root         (0) root         (0)     2730 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     1473 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/checksum-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1298 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/checksum-py.h
+-rw-rw-r--   0 root         (0) root         (0)     6450 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/compression_wrapper-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1622 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/compression_wrapper-py.h
+-rw-rw-r--   0 root         (0) root         (0)     6696 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/contentstat-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1104 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/contentstat-py.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.279782 createrepo_c-1.1.0/tests/createrepo/python/createrepo_c/
+-rw-rw-r--   0 root         (0) root         (0)    29092 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/createrepo_c/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.279782 createrepo_c-1.1.0/tests/createrepo/python/createrepo_c.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      886 2024-03-11 07:20:20.000000 createrepo_c-1.1.0/tests/createrepo/python/createrepo_c.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20682 2024-03-11 07:20:20.000000 createrepo_c-1.1.0/tests/createrepo/python/createrepo_c.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 07:20:20.000000 createrepo_c-1.1.0/tests/createrepo/python/createrepo_c.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2024-03-11 07:20:20.000000 createrepo_c-1.1.0/tests/createrepo/python/createrepo_c.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-03-11 07:20:20.000000 createrepo_c-1.1.0/tests/createrepo/python/createrepo_c.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)    12098 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/createrepo_cmodule.c
+-rw-rw-r--   0 root         (0) root         (0)     2517 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/exception-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1307 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/exception-py.h
+-rw-rw-r--   0 root         (0) root         (0)    10077 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/load_metadata-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1043 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/load_metadata-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7280 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/locate_metadata-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1143 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/locate_metadata-py.h
+-rw-rw-r--   0 root         (0) root         (0)     2573 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/misc-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1495 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/misc-py.h
+-rw-rw-r--   0 root         (0) root         (0)    19974 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/package-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1242 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/package-py.h
+-rw-rw-r--   0 root         (0) root         (0)     4047 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/parsepkg-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1444 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/parsepkg-py.h
+-rw-rw-r--   0 root         (0) root         (0)    13961 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/repomd-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1069 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/repomd-py.h
+-rw-rw-r--   0 root         (0) root         (0)    13674 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/repomdrecord-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1168 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/repomdrecord-py.h
+-rw-rw-r--   0 root         (0) root         (0)     5675 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/sqlite-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1023 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/sqlite-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7844 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/typeconversion.c
+-rw-rw-r--   0 root         (0) root         (0)     1849 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/typeconversion.h
+-rw-rw-r--   0 root         (0) root         (0)    10308 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/updatecollection-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1216 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/updatecollection-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7595 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/updatecollectionmodule-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1270 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/updatecollectionmodule-py.h
+-rw-rw-r--   0 root         (0) root         (0)     8365 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/updatecollectionpackage-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1279 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/updatecollectionpackage-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7867 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/updateinfo-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1097 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/updateinfo-py.h
+-rw-rw-r--   0 root         (0) root         (0)    15281 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/updaterecord-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1168 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/updaterecord-py.h
+-rw-rw-r--   0 root         (0) root         (0)     6257 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/updatereference-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1195 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/updatereference-py.h
+-rw-rw-r--   0 root         (0) root         (0)     4938 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/xml_dump-py.c
+-rw-rw-r--   0 root         (0) root         (0)     2121 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/xml_dump-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7503 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/xml_file-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1030 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/xml_file-py.h
+-rw-rw-r--   0 root         (0) root         (0)    27454 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/xml_parser-py.c
+-rw-rw-r--   0 root         (0) root         (0)     3318 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/python/xml_parser-py.h
+-rw-rw-r--   0 root         (0) root         (0)    36316 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/repomd.c
+-rw-rw-r--   0 root         (0) root         (0)    11634 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/repomd.h
+-rw-rw-r--   0 root         (0) root         (0)     1359 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/repomd_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    48204 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/sqlite.c
+-rw-rw-r--   0 root         (0) root         (0)     5768 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/sqlite.h
+-rw-rw-r--   0 root         (0) root         (0)    34375 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/sqliterepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)     5190 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/threads.c
+-rw-rw-r--   0 root         (0) root         (0)     5854 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/threads.h
+-rw-rw-r--   0 root         (0) root         (0)     9476 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/updateinfo.c
+-rw-rw-r--   0 root         (0) root         (0)     5407 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/updateinfo.h
+-rw-rw-r--   0 root         (0) root         (0)     1312 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/version.h.in
+-rw-rw-r--   0 root         (0) root         (0)    16489 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_dump.c
+-rw-rw-r--   0 root         (0) root         (0)     7618 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_dump.h
+-rw-rw-r--   0 root         (0) root         (0)     4545 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_dump_deltapackage.c
+-rw-rw-r--   0 root         (0) root         (0)     3911 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_dump_filelists.c
+-rw-rw-r--   0 root         (0) root         (0)     3145 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_dump_internal.h
+-rw-rw-r--   0 root         (0) root         (0)     4414 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_dump_other.c
+-rw-rw-r--   0 root         (0) root         (0)    12665 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_dump_primary.c
+-rw-rw-r--   0 root         (0) root         (0)     8750 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_dump_repomd.c
+-rw-rw-r--   0 root         (0) root         (0)     9530 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_dump_updateinfo.c
+-rw-rw-r--   0 root         (0) root         (0)    15944 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_file.c
+-rw-rw-r--   0 root         (0) root         (0)    10285 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_file.h
+-rw-rw-r--   0 root         (0) root         (0)     9177 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_parser.c
+-rw-rw-r--   0 root         (0) root         (0)    13838 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_parser.h
+-rw-rw-r--   0 root         (0) root         (0)    14997 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_parser_filelists.c
+-rw-rw-r--   0 root         (0) root         (0)     9269 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_parser_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    17385 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_parser_main_metadata_together.c
+-rw-rw-r--   0 root         (0) root         (0)    13200 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_parser_other.c
+-rw-rw-r--   0 root         (0) root         (0)    27752 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_parser_primary.c
+-rw-rw-r--   0 root         (0) root         (0)    14399 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_parser_repomd.c
+-rw-rw-r--   0 root         (0) root         (0)    20016 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/createrepo/xml_parser_updateinfo.c
+-rw-rw-r--   0 root         (0) root         (0)    11645 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/fixtures.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.279782 createrepo_c-1.1.0/tests/python/
+-rw-rw-r--   0 root         (0) root         (0)       25 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.287782 createrepo_c-1.1.0/tests/python/tests/
+-rw-rw-r--   0 root         (0) root         (0)      167 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9182 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/fixtures.py
+-rwxrwxr-x   0 root         (0) root         (0)      199 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/run_unittests.sh.in
+-rw-rw-r--   0 root         (0) root         (0)     1212 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_checksum.py
+-rw-rw-r--   0 root         (0) root         (0)     3564 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_compression_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     2514 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_contentstat.py
+-rw-rw-r--   0 root         (0) root         (0)     4166 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_crfile.py
+-rw-rw-r--   0 root         (0) root         (0)     3414 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_load_metadata.py
+-rw-rw-r--   0 root         (0) root         (0)     4235 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_locate_metadata.py
+-rw-rw-r--   0 root         (0) root         (0)     3249 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_misc.py
+-rw-rw-r--   0 root         (0) root         (0)    10895 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_package.py
+-rw-rw-r--   0 root         (0) root         (0)     2433 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_parsepkg.py
+-rw-rw-r--   0 root         (0) root         (0)     4875 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_repomd.py
+-rw-rw-r--   0 root         (0) root         (0)     7982 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_repomdrecord.py
+-rw-rw-r--   0 root         (0) root         (0)    10782 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_repository.py
+-rw-rw-r--   0 root         (0) root         (0)    10544 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_sqlite.py
+-rw-rw-r--   0 root         (0) root         (0)     3063 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_updatecollection.py
+-rw-rw-r--   0 root         (0) root         (0)      938 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_updatecollectionmodule.py
+-rw-rw-r--   0 root         (0) root         (0)     1760 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_updatecollectionpackage.py
+-rw-rw-r--   0 root         (0) root         (0)    13055 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_updateinfo.py
+-rw-rw-r--   0 root         (0) root         (0)     6315 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_updaterecord.py
+-rw-rw-r--   0 root         (0) root         (0)      710 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_updatereference.py
+-rw-rw-r--   0 root         (0) root         (0)      317 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_version.py
+-rw-rw-r--   0 root         (0) root         (0)    14610 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_xml_file.py
+-rw-rw-r--   0 root         (0) root         (0)    56717 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/python/tests/test_xml_parser.py
+-rwxrwxr-x   0 root         (0) root         (0)      688 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/run_tests.sh.in
+-rw-rw-r--   0 root         (0) root         (0)     5518 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_checksum.c
+-rw-rw-r--   0 root         (0) root         (0)    32047 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_compression_wrapper.c
+-rw-rw-r--   0 root         (0) root         (0)    14240 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_koji.c
+-rw-rw-r--   0 root         (0) root         (0)     8130 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_load_metadata.c
+-rw-rw-r--   0 root         (0) root         (0)    10128 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_locate_metadata.c
+-rw-rw-r--   0 root         (0) root         (0)    43471 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_misc.c
+-rw-rw-r--   0 root         (0) root         (0)     4673 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_modifyrepo_shared.c
+-rw-rw-r--   0 root         (0) root         (0)     6327 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_sqlite.c
+-rw-rw-r--   0 root         (0) root         (0)     4116 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_xml_dump.c
+-rw-rw-r--   0 root         (0) root         (0)    15388 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_xml_dump_primary.c
+-rw-rw-r--   0 root         (0) root         (0)     4565 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_xml_file.c
+-rw-rw-r--   0 root         (0) root         (0)    17435 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_xml_parser_filelists.c
+-rw-rw-r--   0 root         (0) root         (0)    11263 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_xml_parser_main_metadata_together.c
+-rw-rw-r--   0 root         (0) root         (0)     4156 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_xml_parser_repomd.c
+-rw-rw-r--   0 root         (0) root         (0)    10261 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/test_xml_parser_updateinfo.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.219782 createrepo_c-1.1.0/tests/testdata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.291782 createrepo_c-1.1.0/tests/testdata/compressed_files/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/00_plain.foo0
+-rw-rw-r--   0 root         (0) root         (0)       33 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/00_plain.foo1
+-rw-rw-r--   0 root         (0) root         (0)       14 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/00_plain.foo2
+-rw-rw-r--   0 root         (0) root         (0)       32 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/00_plain.foo3
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/00_plain.foo4
+-rw-rw-r--   0 root         (0) root         (0)       13 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/00_plain.foo5
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/00_plain.txt
+-rw-rw-r--   0 root         (0) root         (0)       14 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/00_plain.txt.bz2
+-rw-rw-r--   0 root         (0) root         (0)       33 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/00_plain.txt.gz
+-rw-rw-r--   0 root         (0) root         (0)       32 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/00_plain.txt.xz
+-rw-rw-r--   0 root         (0) root         (0)       95 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/00_plain.txt.zck
+-rw-rw-r--   0 root         (0) root         (0)       13 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/00_plain.txt.zst
+-rw-rw-r--   0 root         (0) root         (0)       56 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/01_plain.foo0
+-rw-rw-r--   0 root         (0) root         (0)       64 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/01_plain.foo1
+-rw-rw-r--   0 root         (0) root         (0)       69 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/01_plain.foo2
+-rw-rw-r--   0 root         (0) root         (0)       96 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/01_plain.foo3
+-rw-rw-r--   0 root         (0) root         (0)      169 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/01_plain.foo4
+-rw-rw-r--   0 root         (0) root         (0)       51 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/01_plain.foo5
+-rw-rw-r--   0 root         (0) root         (0)       56 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/01_plain.txt
+-rw-rw-r--   0 root         (0) root         (0)       69 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/01_plain.txt.bz2
+-rw-rw-r--   0 root         (0) root         (0)       64 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/01_plain.txt.gz
+-rw-rw-r--   0 root         (0) root         (0)       96 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/01_plain.txt.xz
+-rw-rw-r--   0 root         (0) root         (0)      158 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/01_plain.txt.zck
+-rw-rw-r--   0 root         (0) root         (0)       51 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/compressed_files/01_plain.txt.zst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.291782 createrepo_c-1.1.0/tests/testdata/comps_files/
+-rw-rw-r--   0 root         (0) root         (0)      638 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/comps_files/comps_00.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.299782 createrepo_c-1.1.0/tests/testdata/modified_repo_files/
+-rw-rw-r--   0 root         (0) root         (0)      633 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/bad_file_type-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      570 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/error_00-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      802 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/error_00-other.xml
+-rw-rw-r--   0 root         (0) root         (0)     3174 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/error_00-primary.xml
+-rw-rw-r--   0 root         (0) root         (0)    68135 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/long_primary.xml
+-rw-rw-r--   0 root         (0) root         (0)     1528 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/missing_type-repomd.xml
+-rw-rw-r--   0 root         (0) root         (0)      764 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/multiple_warnings_00-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      985 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/multiple_warnings_00-other.xml
+-rw-rw-r--   0 root         (0) root         (0)     3588 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/multiple_warnings_00-primary.xml
+-rw-rw-r--   0 root         (0) root         (0)      510 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/no_pkgid-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      767 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/no_pkgid-other.xml
+-rw-rw-r--   0 root         (0) root         (0)      405 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/repo_01_ampersand-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      551 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/repo_01_ampersand-other.xml
+-rw-rw-r--   0 root         (0) root         (0)     2239 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/repo_01_ampersand-primary.xml
+-rw-rw-r--   0 root         (0) root         (0)      598 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/repo_02_different_order_filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      608 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_00-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      840 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_00-other.xml
+-rw-rw-r--   0 root         (0) root         (0)     3277 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_00-primary.xml
+-rw-rw-r--   0 root         (0) root         (0)      606 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_01-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      838 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_01-other.xml
+-rw-rw-r--   0 root         (0) root         (0)     3353 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_01-primary.xml
+-rw-rw-r--   0 root         (0) root         (0)      657 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_02-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      889 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_02-other.xml
+-rw-rw-r--   0 root         (0) root         (0)     3342 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_02-primary.xml
+-rw-rw-r--   0 root         (0) root         (0)     1277 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/modified_repo_files/updateinfo_ampersand.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.299782 createrepo_c-1.1.0/tests/testdata/other_metadata/
+-rw-rw-r--   0 root         (0) root         (0)      894 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/other_metadata/0402e012013246e7e2f2f638c8a6046efdfd71ae1cbeff9c391d9c1ae5d7d431-comps-f19.xml.bz2
+-rw-rw-r--   0 root         (0) root         (0)     2364 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/other_metadata/36c4f2d6dda3b015b4a7da59552c7c76eff99a59979178513cb51341f6eead44-comps-f19.xml
+-rw-rw-r--   0 root         (0) root         (0)      760 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/other_metadata/71d988ca33b31a18b0d775478d6f59b40583c794ae76393284850ee97bfba4dc-comps-f19.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      804 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/other_metadata/c941e2c77a27cdca324c0e0bc3190e134fddddb36a03fb5517e55d156b955205-comps-f19.xml.xz
+-rw-rw-r--   0 root         (0) root         (0)     2364 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/other_metadata/comps-f19.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.299782 createrepo_c-1.1.0/tests/testdata/packages/
+-rw-rw-r--   0 root         (0) root         (0)     3101 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/packages/Archer-3.4.5-6.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     3096 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/packages/Rimmer-1.0.2-2.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     1717 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/packages/balicek-iso88591-1.1.1-1.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     1741 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/packages/balicek-iso88592-1.1.1-1.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     1789 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/packages/balicek-utf8-1.1.1-1.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     1488 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/packages/empty-0-0.src.rpm
+-rw-rw-r--   0 root         (0) root         (0)     1401 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/packages/empty-0-0.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     2237 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/packages/fake_bash-1.1.1-1.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     2845 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/packages/super_kernel-6.0.1-2.x86_64.rpm
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.215782 createrepo_c-1.1.0/tests/testdata/repo_00/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.303782 createrepo_c-1.1.0/tests/testdata/repo_00/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      134 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_00/repodata/1cb61ea996355add02b1426ed4c1780ea75ce0c04c5d1107c025c3fbd7d8bcae-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      262 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_00/repodata/2e7db4492173b6c437fd1299dc335e63d09f24cbdadeac5175a61b787c2f7a44-filelists.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      123 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_00/repodata/95a4415d859d7120efb6b3cf964c07bebbff9a5275ca673e6e74a97bcbfb2a5f-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      263 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_00/repodata/a939c4765106655c3f7a13fb41d0f239824efa66bcd6c1e6c044a854012bda75-other.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      269 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_00/repodata/e0ac03cd77e95e724dbf90ded0dba664e233315a8940051dd8882c56b9878595-primary.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      123 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_00/repodata/ef3e20691954c3d1318ec3071a982da339f4ed76967ded668b795c9e070aaab6-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     3381 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_00/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.215782 createrepo_c-1.1.0/tests/testdata/repo_01/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.303782 createrepo_c-1.1.0/tests/testdata/repo_01/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      783 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_01/repodata/6c662d665c24de9a0f62c17d8fa50622307739d7376f0d19097ca96c6d7f5e3e-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      332 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_01/repodata/b752a73d9efd4006d740f943db5fb7c2dd77a8324bd99da92e86bd55a2c126ef-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      273 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_01/repodata/c7db035d0e6f1b2e883a7fa3229e2d2be70c05a8b8d2b57dbb5f9c1a67483b6c-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1497 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_01/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.215782 createrepo_c-1.1.0/tests/testdata/repo_02/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.303782 createrepo_c-1.1.0/tests/testdata/repo_02/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      341 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_02/repodata/3b7e6ecd01af9cb674aff6458186911d7081bb5676d5562a21a963afc8a8bcc7-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      403 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_02/repodata/ab5d3edeea50f9b4ec5ee13e4d25c147e318e3a433dbabc94d3461f58ac28255-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      973 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_02/repodata/bcde64b04916a2a72fdc257d61bc922c70b3d58e953499180585f7a360ce86cf-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1497 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_02/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.215782 createrepo_c-1.1.0/tests/testdata/repo_03/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.303782 createrepo_c-1.1.0/tests/testdata/repo_03/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      134 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_03/repodata/1cb61ea996355add02b1426ed4c1780ea75ce0c04c5d1107c025c3fbd7d8bcae-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      262 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_03/repodata/2e7db4492173b6c437fd1299dc335e63d09f24cbdadeac5175a61b787c2f7a44-filelists.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      123 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_03/repodata/95a4415d859d7120efb6b3cf964c07bebbff9a5275ca673e6e74a97bcbfb2a5f-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1044 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_03/repodata/a850093e240506c728d6ce26a6fc51d6a7fe10730c67988d13afa7dd82df82d5-modules.yaml.xz
+-rw-rw-r--   0 root         (0) root         (0)      263 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_03/repodata/a939c4765106655c3f7a13fb41d0f239824efa66bcd6c1e6c044a854012bda75-other.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      269 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_03/repodata/e0ac03cd77e95e724dbf90ded0dba664e233315a8940051dd8882c56b9878595-primary.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      123 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_03/repodata/ef3e20691954c3d1318ec3071a982da339f4ed76967ded668b795c9e070aaab6-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     3838 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_03/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.215782 createrepo_c-1.1.0/tests/testdata/repo_04/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.307782 createrepo_c-1.1.0/tests/testdata/repo_04/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      987 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_04/repodata/6a5f64dd82a126a161657764fe8f4b4092c0a3b61b9a34bde2af89dc1df112a1-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      397 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_04/repodata/6d0101044d9b4683e4ddc76491b3eb2228cddaace9e1d148c5eb138de9f71c17-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      429 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_04/repodata/d1c632d489f1c72b68b5c0d5de38ed1cb5c7a521380a88bed86771d39fb19538-filelists-ext.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      336 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_04/repodata/d7b8b1b6caa124aa17e4c6a1867e50e6893791ade0ebe212ab6f536695b5ce84-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     2012 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_04/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.215782 createrepo_c-1.1.0/tests/testdata/repo_koji_01/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.307782 createrepo_c-1.1.0/tests/testdata/repo_koji_01/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      816 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_koji_01/repodata/5d039d9ec332d158c69d083f04ac88a187c6b68444472b802eaf0249aec83294-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1007 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_koji_01/repodata/b153f86915d1dacbb89b244da26e50adb204195262fd3562290de26725daa21d-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      487 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_koji_01/repodata/c0e88e9a81f76341e91cd06f8ded80d4c289bdb4977e7624068802654b6da506-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1549 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_koji_01/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.215782 createrepo_c-1.1.0/tests/testdata/repo_koji_02/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.307782 createrepo_c-1.1.0/tests/testdata/repo_koji_02/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      338 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_koji_02/repodata/118e790330a62cfb167ce670478b25f4bfc58d7fc671096e4fd294fe40cee201-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      913 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_koji_02/repodata/ee9261d1d2916d841cf24bb01743198ec63ed596f410784602eca2350e430e17-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      687 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_koji_02/repodata/feb0b5fdcb0ee1cf981b041f0749ec381145cd9f6b4397991ef5dafcb6807bba-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1547 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_koji_02/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.215782 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.311782 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      656 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/0219a2f1f9f32af6b7873905269ac1bc27b03e0caf3968c929a49e5a939e8935-updateinfo_01.xml.gz.zck
+-rw-rw-r--   0 root         (0) root         (0)     2366 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/04460bfaf6cb5af6b0925d8c99401a44e5192d287796aed4cced5f7ce881761f-comps.f20.xml
+-rw-rw-r--   0 root         (0) root         (0)     3775 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/1e12239bf5cb07ec73c74482c35e80dabe30dbe2fdd57bd9e557d987cbacc8c2-primary.sqlite.bz2
+-rw-rw-r--   0 root         (0) root         (0)      864 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.gz.zck
+-rw-rw-r--   0 root         (0) root         (0)      864 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      932 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/3d6eaa7c77ef92586470dd6a542478e42cc421a85f12e0db93aa783077704cd0-filelists.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)     1287 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/490a2a494a3827b8a356f728ac36bc02fb009b0eaea173c890e727bb54219037-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1519 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/4f4de7d3254a033b84626f330bc6adb8a3c1a4a20f0ddbe30a5692a041318c81-filelists.sqlite.bz2
+-rw-rw-r--   0 root         (0) root         (0)    88281 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/4fbad65c641f4f8fb3cec9b1672fcec2357443e1ea6e93541a0bb559c7dc9238-modules.yaml.gz
+-rw-rw-r--   0 root         (0) root         (0)      533 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/88514679cb03d8f51e850ad3639c089f899e83407a2380ef9e62873a8eb1db13-updateinfo_01.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1301 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/8b13cba732c1a02b841f43d6791ca68788d45f376787d9f3ccf68e75f01af499-other.sqlite.bz2
+-rw-rw-r--   0 root         (0) root         (0)      749 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/ba5a4fdbb20e7b9b70d9a9abd974bcab1065b1e81d711f80e06ad8cae30c4183-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      850 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/c5582e660ed9a2d3c10ba44f0aeb02f2bb70e85dc3c8cda4266183d4e5235aa7-other.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)    86680 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/cb0f4b5df8268f248158e50d66ee1565591bca23ee2dbd84ae9c457962fa3122-modules.yaml.gz.zck
+-rw-rw-r--   0 root         (0) root         (0)     1482 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/e9e6ca4765de75cc3b2bf05e6cf631703c6557edd642300748d7747000547365-primary.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      748 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/f9d860ddcb64fbdc88a9b71a14ddb9f5670968d5dd3430412565c13d42b6804d-comps.f20.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      687 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/fd458a424a3f3e0dadc95b806674b79055c24e73637e47ad5a6e57926aa1b9d1-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     8640 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.215782 createrepo_c-1.1.0/tests/testdata/repo_with_duplicate_packages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.311782 createrepo_c-1.1.0/tests/testdata/repo_with_duplicate_packages/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      341 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_duplicate_packages/repodata/filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      405 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_duplicate_packages/repodata/other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1017 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_duplicate_packages/repodata/primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1354 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repo_with_duplicate_packages/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.315782 createrepo_c-1.1.0/tests/testdata/repodata_snippets/
+-rw-rw-r--   0 root         (0) root         (0)      436 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repodata_snippets/filelists_ext_snippet_01.xml
+-rw-rw-r--   0 root         (0) root         (0)      745 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repodata_snippets/filelists_ext_snippet_02.xml
+-rw-rw-r--   0 root         (0) root         (0)      263 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repodata_snippets/filelists_snippet_01.xml
+-rw-rw-r--   0 root         (0) root         (0)      471 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repodata_snippets/filelists_snippet_02.xml
+-rw-rw-r--   0 root         (0) root         (0)      408 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repodata_snippets/other_snippet_01.xml
+-rw-rw-r--   0 root         (0) root         (0)      697 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repodata_snippets/other_snippet_02.xml
+-rw-rw-r--   0 root         (0) root         (0)     1918 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repodata_snippets/primary_snippet_01.xml
+-rw-rw-r--   0 root         (0) root         (0)     3085 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/repodata_snippets/primary_snippet_02.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.315782 createrepo_c-1.1.0/tests/testdata/specs/
+-rwxrwxr-x   0 root         (0) root         (0)       67 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/specs/build.sh
+-rw-rw-r--   0 root         (0) root         (0)     1369 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/specs/fake-Archer.spec
+-rw-rw-r--   0 root         (0) root         (0)     1023 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/specs/fake-Rimmer.spec
+-rw-rw-r--   0 root         (0) root         (0)      571 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/specs/fake-balicek-iso88591.spec
+-rw-rw-r--   0 root         (0) root         (0)      594 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/specs/fake-balicek-iso88592.spec
+-rw-rw-r--   0 root         (0) root         (0)      653 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/specs/fake-balicek-utf8.spec
+-rw-rw-r--   0 root         (0) root         (0)      176 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/specs/fake-empty.spec
+-rw-rw-r--   0 root         (0) root         (0)      632 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/specs/fake-fake_bash.spec
+-rw-rw-r--   0 root         (0) root         (0)     1236 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/specs/fake-super_kernel.spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.319782 createrepo_c-1.1.0/tests/testdata/test_files/
+-rw-rw-r--   0 root         (0) root         (0)     1523 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/test_files/binary_file
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/test_files/empty_file
+-rw-rw-r--   0 root         (0) root         (0)    24576 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/test_files/sqlite_file.sqlite
+-rw-rw-r--   0 root         (0) root         (0)      910 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/test_files/text_file
+-rw-rw-r--   0 root         (0) root         (0)      522 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/test_files/text_file.gz
+-rw-rw-r--   0 root         (0) root         (0)      628 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/test_files/text_file.xz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 07:20:20.319782 createrepo_c-1.1.0/tests/testdata/updateinfo_files/
+-rw-rw-r--   0 root         (0) root         (0)       60 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/updateinfo_files/updateinfo_00.xml
+-rw-rw-r--   0 root         (0) root         (0)     1222 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/updateinfo_files/updateinfo_01.xml
+-rw-rw-r--   0 root         (0) root         (0)      188 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/updateinfo_files/updateinfo_02.xml.xz
+-rw-rw-r--   0 root         (0) root         (0)     4805 2024-03-11 07:14:00.000000 createrepo_c-1.1.0/tests/testdata/updateinfo_files/updateinfo_03.xml
```

### Comparing `createrepo_c-1.0.4/CMakeLists.txt` & `createrepo_c-1.1.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/COPYING` & `createrepo_c-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/PKG-INFO` & `createrepo_c-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: createrepo_c
-Version: 1.0.4
+Version: 1.1.0
 Summary: C implementation of createrepo
 Home-page: https://github.com/rpm-software-management
 Author: RPM Software Management
 Author-email: rpm-ecosystem@lists.rpm.org
 License: GPLv2+
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `createrepo_c-1.0.4/README.md` & `createrepo_c-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/doc/CMakeLists.txt` & `createrepo_c-1.1.0/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/doc/Doxyfile.in.in` & `createrepo_c-1.1.0/doc/Doxyfile.in.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/doc/createrepo_c.8` & `createrepo_c-1.1.0/doc/createrepo_c.8`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/doc/logo.png` & `createrepo_c-1.1.0/doc/logo.png`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/doc/logo.xcf` & `createrepo_c-1.1.0/doc/logo.xcf`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/doc/mergerepo_c.8` & `createrepo_c-1.1.0/doc/mergerepo_c.8`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/doc/modifyrepo_c.8` & `createrepo_c-1.1.0/doc/modifyrepo_c.8`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/doc/python/conf.py` & `createrepo_c-1.1.0/doc/python/conf.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/doc/python/lib.rst` & `createrepo_c-1.1.0/doc/python/lib.rst`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/doc/sqliterepo_c.8` & `createrepo_c-1.1.0/doc/sqliterepo_c.8`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/setup.py` & `createrepo_c-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/CMakeLists.txt` & `createrepo_c-1.1.0/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/checksum.c` & `createrepo_c-1.1.0/src/checksum.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/checksum.h` & `createrepo_c-1.1.0/src/checksum.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/cleanup.h` & `createrepo_c-1.1.0/src/cleanup.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/cmd_parser.c` & `createrepo_c-1.1.0/src/cmd_parser.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/cmd_parser.h` & `createrepo_c-1.1.0/src/cmd_parser.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/compression_wrapper.c` & `createrepo_c-1.1.0/src/compression_wrapper.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/compression_wrapper.h` & `createrepo_c-1.1.0/src/compression_wrapper.h`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
  */
 typedef enum {
     CR_CW_MODE_READ,            /*!< Read mode */
     CR_CW_MODE_WRITE,           /*!< Write mode */
     CR_CW_MODE_SENTINEL,        /*!< Sentinel of the list */
 } cr_OpenMode;
 
-/** Stat build about open content during compression (writting).
+/** Stat build about open content during compression (writing).
  */
 typedef struct {
     gint64          size;               /*!< Size of content */
     cr_ChecksumType checksum_type;      /*!< Checksum type */
     char            *checksum;          /*!< Checksum */
     gint64          hdr_size;           /*!< Size of content */
     cr_ChecksumType hdr_checksum_type;  /*!< Checksum type */
@@ -83,15 +83,15 @@
  */
 typedef struct {
     cr_CompressionType  type;           /*!< Type of compression */
     void                *FILE;          /*!< Pointer to gzFile, BZFILE, ... */
     void                *INNERFILE;     /*!< Pointer to underlying FILE */
     cr_OpenMode         mode;           /*!< Mode */
     cr_ContentStat      *stat;          /*!< Content stats */
-    cr_ChecksumCtx      *checksum_ctx;  /*!< Checksum contenxt */
+    cr_ChecksumCtx      *checksum_ctx;  /*!< Checksum context */
 } CR_FILE;
 
 #define CR_CW_ERR       -1      /*!< Return value - Error */
 
 /** Returns a common suffix for the specified cr_CompressionType.
  * @param comtype       compression type
  * @return              common file suffix
```

### Comparing `createrepo_c-1.0.4/src/constants.h` & `createrepo_c-1.1.0/src/constants.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/createrepo_c.c` & `createrepo_c-1.1.0/src/createrepo_c.c`

 * *Files 0% similar despite different names*

```diff
@@ -1161,15 +1161,15 @@
             g_debug("Creating databases");
             pri_db_filename = g_strconcat(tmp_out_repo, "/primary.sqlite", NULL);
             fil_db_filename = g_strconcat(tmp_out_repo, "/filelists.sqlite", NULL);
 	    if (cmd_options->filelists_ext)
                 fex_db_filename = g_strconcat(tmp_out_repo, "/filelists-ext.sqlite", NULL);
             oth_db_filename = g_strconcat(tmp_out_repo, "/other.sqlite", NULL);
         } else {
-            g_debug("Creating databases localy");
+            g_debug("Creating databases locally");
             const gchar *tmpdir = g_get_tmp_dir();
             pri_db_filename = g_build_filename(tmpdir, "primary.XXXXXX.sqlite", NULL);
             fil_db_filename = g_build_filename(tmpdir, "filelists.XXXXXX.sqlite", NULL);
 	    if (cmd_options->filelists_ext)
                 fex_db_filename = g_build_filename(tmpdir, "filelists-ext.XXXXXX.sqlite", NULL);
             oth_db_filename = g_build_filename(tmpdir, "other.XXXXXXX.sqlite", NULL);
             pri_db_fd = g_mkstemp(pri_db_filename);
```

### Comparing `createrepo_c-1.0.4/src/createrepo_c.h` & `createrepo_c-1.1.0/src/createrepo_c.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/createrepo_shared.c` & `createrepo_c-1.1.0/src/createrepo_shared.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/createrepo_shared.h` & `createrepo_c-1.1.0/src/createrepo_shared.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/deltarpms.c` & `createrepo_c-1.1.0/src/deltarpms.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/deltarpms.h.in` & `createrepo_c-1.1.0/src/deltarpms.h.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/dumper_thread.c` & `createrepo_c-1.1.0/src/dumper_thread.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/dumper_thread.h` & `createrepo_c-1.1.0/src/dumper_thread.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/error.c` & `createrepo_c-1.1.0/src/error.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/error.h` & `createrepo_c-1.1.0/src/error.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/helpers.c` & `createrepo_c-1.1.0/src/helpers.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/helpers.h` & `createrepo_c-1.1.0/src/helpers.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/koji.c` & `createrepo_c-1.1.0/src/koji.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/koji.h` & `createrepo_c-1.1.0/src/koji.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/load_metadata.c` & `createrepo_c-1.1.0/src/load_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/load_metadata.h` & `createrepo_c-1.1.0/src/load_metadata.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/locate_metadata.c` & `createrepo_c-1.1.0/src/locate_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/locate_metadata.h` & `createrepo_c-1.1.0/src/locate_metadata.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/mergerepo_c.c` & `createrepo_c-1.1.0/src/mergerepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/mergerepo_c.h` & `createrepo_c-1.1.0/src/mergerepo_c.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/metadata_internal.h` & `createrepo_c-1.1.0/src/metadata_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/misc.c` & `createrepo_c-1.1.0/src/misc.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/misc.h` & `createrepo_c-1.1.0/src/misc.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/modifyrepo_c.c` & `createrepo_c-1.1.0/src/modifyrepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/modifyrepo_shared.c` & `createrepo_c-1.1.0/src/modifyrepo_shared.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/modifyrepo_shared.h` & `createrepo_c-1.1.0/src/modifyrepo_shared.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/package.c` & `createrepo_c-1.1.0/src/package.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/package.h` & `createrepo_c-1.1.0/src/package.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/package_internal.h` & `createrepo_c-1.1.0/src/package_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/parsehdr.c` & `createrepo_c-1.1.0/src/parsehdr.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/parsehdr.h` & `createrepo_c-1.1.0/src/parsehdr.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/parsepkg.c` & `createrepo_c-1.1.0/src/parsepkg.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/parsepkg.h` & `createrepo_c-1.1.0/src/parsepkg.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/CMakeLists.txt` & `createrepo_c-1.1.0/src/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/checksum-py.c` & `createrepo_c-1.1.0/src/python/checksum-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/checksum-py.h` & `createrepo_c-1.1.0/src/python/checksum-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/compression_wrapper-py.c` & `createrepo_c-1.1.0/src/python/compression_wrapper-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/compression_wrapper-py.h` & `createrepo_c-1.1.0/src/python/compression_wrapper-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/contentstat-py.c` & `createrepo_c-1.1.0/src/python/contentstat-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/contentstat-py.h` & `createrepo_c-1.1.0/src/python/contentstat-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/createrepo_c.egg-info/PKG-INFO` & `createrepo_c-1.1.0/src/python/createrepo_c.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: createrepo-c
-Version: 1.0.4
+Version: 1.1.0
 Summary: C implementation of createrepo
 Home-page: https://github.com/rpm-software-management
 Author: RPM Software Management
 Author-email: rpm-ecosystem@lists.rpm.org
 License: GPLv2+
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `createrepo_c-1.0.4/src/python/createrepo_c.egg-info/SOURCES.txt` & `createrepo_c-1.1.0/src/python/createrepo_c.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -301,14 +301,15 @@
 tests/python/tests/test_load_metadata.py
 tests/python/tests/test_locate_metadata.py
 tests/python/tests/test_misc.py
 tests/python/tests/test_package.py
 tests/python/tests/test_parsepkg.py
 tests/python/tests/test_repomd.py
 tests/python/tests/test_repomdrecord.py
+tests/python/tests/test_repository.py
 tests/python/tests/test_sqlite.py
 tests/python/tests/test_updatecollection.py
 tests/python/tests/test_updatecollectionmodule.py
 tests/python/tests/test_updatecollectionpackage.py
 tests/python/tests/test_updateinfo.py
 tests/python/tests/test_updaterecord.py
 tests/python/tests/test_updatereference.py
```

### Comparing `createrepo_c-1.0.4/src/python/createrepo_cmodule.c` & `createrepo_c-1.1.0/src/python/createrepo_cmodule.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/exception-py.c` & `createrepo_c-1.1.0/src/python/exception-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/exception-py.h` & `createrepo_c-1.1.0/src/python/exception-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/load_metadata-py.c` & `createrepo_c-1.1.0/src/python/load_metadata-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/load_metadata-py.h` & `createrepo_c-1.1.0/src/python/load_metadata-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/locate_metadata-py.c` & `createrepo_c-1.1.0/src/python/locate_metadata-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/locate_metadata-py.h` & `createrepo_c-1.1.0/src/python/locate_metadata-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/misc-py.c` & `createrepo_c-1.1.0/src/python/misc-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/misc-py.h` & `createrepo_c-1.1.0/src/python/misc-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/package-py.c` & `createrepo_c-1.1.0/src/python/package-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/package-py.h` & `createrepo_c-1.1.0/src/python/package-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/parsepkg-py.c` & `createrepo_c-1.1.0/src/python/parsepkg-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/parsepkg-py.h` & `createrepo_c-1.1.0/src/python/parsepkg-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/repomd-py.c` & `createrepo_c-1.1.0/src/python/repomd-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/repomd-py.h` & `createrepo_c-1.1.0/src/python/repomd-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/repomdrecord-py.c` & `createrepo_c-1.1.0/src/python/repomdrecord-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/repomdrecord-py.h` & `createrepo_c-1.1.0/src/python/repomdrecord-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/sqlite-py.c` & `createrepo_c-1.1.0/src/python/sqlite-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/sqlite-py.h` & `createrepo_c-1.1.0/src/python/sqlite-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/typeconversion.c` & `createrepo_c-1.1.0/src/python/typeconversion.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/typeconversion.h` & `createrepo_c-1.1.0/src/python/typeconversion.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/updatecollection-py.c` & `createrepo_c-1.1.0/src/python/updatecollection-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/updatecollection-py.h` & `createrepo_c-1.1.0/src/python/updatecollection-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/updatecollectionmodule-py.c` & `createrepo_c-1.1.0/src/python/updatecollectionmodule-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/updatecollectionmodule-py.h` & `createrepo_c-1.1.0/src/python/updatecollectionmodule-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/updatecollectionpackage-py.c` & `createrepo_c-1.1.0/src/python/updatecollectionpackage-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/updatecollectionpackage-py.h` & `createrepo_c-1.1.0/src/python/updatecollectionpackage-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/updateinfo-py.c` & `createrepo_c-1.1.0/src/python/updateinfo-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/updateinfo-py.h` & `createrepo_c-1.1.0/src/python/updateinfo-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/updaterecord-py.c` & `createrepo_c-1.1.0/src/python/updaterecord-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/updaterecord-py.h` & `createrepo_c-1.1.0/src/python/updaterecord-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/updatereference-py.c` & `createrepo_c-1.1.0/src/python/updatereference-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/updatereference-py.h` & `createrepo_c-1.1.0/src/python/updatereference-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/xml_dump-py.c` & `createrepo_c-1.1.0/src/python/xml_dump-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/xml_dump-py.h` & `createrepo_c-1.1.0/src/python/xml_dump-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/xml_file-py.c` & `createrepo_c-1.1.0/src/python/xml_file-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/xml_file-py.h` & `createrepo_c-1.1.0/src/python/xml_file-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/xml_parser-py.c` & `createrepo_c-1.1.0/src/python/xml_parser-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/python/xml_parser-py.h` & `createrepo_c-1.1.0/src/python/xml_parser-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/repomd.c` & `createrepo_c-1.1.0/src/repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/repomd.h` & `createrepo_c-1.1.0/src/repomd.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/repomd_internal.h` & `createrepo_c-1.1.0/src/repomd_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/sqlite.c` & `createrepo_c-1.1.0/src/sqlite.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/sqlite.h` & `createrepo_c-1.1.0/src/sqlite.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/sqliterepo_c.c` & `createrepo_c-1.1.0/src/sqliterepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/threads.c` & `createrepo_c-1.1.0/src/threads.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/threads.h` & `createrepo_c-1.1.0/src/threads.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/updateinfo.c` & `createrepo_c-1.1.0/src/updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/updateinfo.h` & `createrepo_c-1.1.0/src/updateinfo.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/version.h.in` & `createrepo_c-1.1.0/src/version.h.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_dump.h` & `createrepo_c-1.1.0/src/xml_dump.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_dump_deltapackage.c` & `createrepo_c-1.1.0/src/xml_dump_deltapackage.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_dump_filelists.c` & `createrepo_c-1.1.0/src/xml_dump_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_dump_internal.h` & `createrepo_c-1.1.0/src/xml_dump_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_dump_other.c` & `createrepo_c-1.1.0/src/xml_dump_other.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_dump_primary.c` & `createrepo_c-1.1.0/src/xml_dump_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_dump_repomd.c` & `createrepo_c-1.1.0/src/xml_dump_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_dump_updateinfo.c` & `createrepo_c-1.1.0/src/xml_dump_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_file.c` & `createrepo_c-1.1.0/src/xml_file.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_file.h` & `createrepo_c-1.1.0/src/xml_file.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_parser.c` & `createrepo_c-1.1.0/src/xml_parser.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_parser.h` & `createrepo_c-1.1.0/src/xml_parser.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_parser_filelists.c` & `createrepo_c-1.1.0/src/xml_parser_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_parser_internal.h` & `createrepo_c-1.1.0/src/xml_parser_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_parser_main_metadata_together.c` & `createrepo_c-1.1.0/src/xml_parser_main_metadata_together.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_parser_other.c` & `createrepo_c-1.1.0/src/xml_parser_other.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_parser_primary.c` & `createrepo_c-1.1.0/src/xml_parser_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_parser_repomd.c` & `createrepo_c-1.1.0/src/xml_parser_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/src/xml_parser_updateinfo.c` & `createrepo_c-1.1.0/src/xml_parser_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/CMakeLists.txt` & `createrepo_c-1.1.0/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/CMakeLists.txt` & `createrepo_c-1.1.0/tests/createrepo/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/checksum.c` & `createrepo_c-1.1.0/tests/createrepo/checksum.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/checksum.h` & `createrepo_c-1.1.0/tests/createrepo/checksum.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/cleanup.h` & `createrepo_c-1.1.0/tests/createrepo/cleanup.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/cmd_parser.c` & `createrepo_c-1.1.0/tests/createrepo/cmd_parser.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/cmd_parser.h` & `createrepo_c-1.1.0/tests/createrepo/cmd_parser.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/compression_wrapper.c` & `createrepo_c-1.1.0/tests/createrepo/compression_wrapper.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/compression_wrapper.h` & `createrepo_c-1.1.0/tests/createrepo/compression_wrapper.h`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
  */
 typedef enum {
     CR_CW_MODE_READ,            /*!< Read mode */
     CR_CW_MODE_WRITE,           /*!< Write mode */
     CR_CW_MODE_SENTINEL,        /*!< Sentinel of the list */
 } cr_OpenMode;
 
-/** Stat build about open content during compression (writting).
+/** Stat build about open content during compression (writing).
  */
 typedef struct {
     gint64          size;               /*!< Size of content */
     cr_ChecksumType checksum_type;      /*!< Checksum type */
     char            *checksum;          /*!< Checksum */
     gint64          hdr_size;           /*!< Size of content */
     cr_ChecksumType hdr_checksum_type;  /*!< Checksum type */
@@ -83,15 +83,15 @@
  */
 typedef struct {
     cr_CompressionType  type;           /*!< Type of compression */
     void                *FILE;          /*!< Pointer to gzFile, BZFILE, ... */
     void                *INNERFILE;     /*!< Pointer to underlying FILE */
     cr_OpenMode         mode;           /*!< Mode */
     cr_ContentStat      *stat;          /*!< Content stats */
-    cr_ChecksumCtx      *checksum_ctx;  /*!< Checksum contenxt */
+    cr_ChecksumCtx      *checksum_ctx;  /*!< Checksum context */
 } CR_FILE;
 
 #define CR_CW_ERR       -1      /*!< Return value - Error */
 
 /** Returns a common suffix for the specified cr_CompressionType.
  * @param comtype       compression type
  * @return              common file suffix
```

### Comparing `createrepo_c-1.0.4/tests/createrepo/constants.h` & `createrepo_c-1.1.0/tests/createrepo/constants.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/createrepo_c.c` & `createrepo_c-1.1.0/tests/createrepo/createrepo_c.c`

 * *Files 0% similar despite different names*

```diff
@@ -1161,15 +1161,15 @@
             g_debug("Creating databases");
             pri_db_filename = g_strconcat(tmp_out_repo, "/primary.sqlite", NULL);
             fil_db_filename = g_strconcat(tmp_out_repo, "/filelists.sqlite", NULL);
 	    if (cmd_options->filelists_ext)
                 fex_db_filename = g_strconcat(tmp_out_repo, "/filelists-ext.sqlite", NULL);
             oth_db_filename = g_strconcat(tmp_out_repo, "/other.sqlite", NULL);
         } else {
-            g_debug("Creating databases localy");
+            g_debug("Creating databases locally");
             const gchar *tmpdir = g_get_tmp_dir();
             pri_db_filename = g_build_filename(tmpdir, "primary.XXXXXX.sqlite", NULL);
             fil_db_filename = g_build_filename(tmpdir, "filelists.XXXXXX.sqlite", NULL);
 	    if (cmd_options->filelists_ext)
                 fex_db_filename = g_build_filename(tmpdir, "filelists-ext.XXXXXX.sqlite", NULL);
             oth_db_filename = g_build_filename(tmpdir, "other.XXXXXXX.sqlite", NULL);
             pri_db_fd = g_mkstemp(pri_db_filename);
```

### Comparing `createrepo_c-1.0.4/tests/createrepo/createrepo_c.h` & `createrepo_c-1.1.0/tests/createrepo/createrepo_c.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/createrepo_shared.c` & `createrepo_c-1.1.0/tests/createrepo/createrepo_shared.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/createrepo_shared.h` & `createrepo_c-1.1.0/tests/createrepo/createrepo_shared.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/deltarpms.c` & `createrepo_c-1.1.0/tests/createrepo/deltarpms.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/deltarpms.h.in` & `createrepo_c-1.1.0/tests/createrepo/deltarpms.h.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/dumper_thread.c` & `createrepo_c-1.1.0/tests/createrepo/dumper_thread.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/dumper_thread.h` & `createrepo_c-1.1.0/tests/createrepo/dumper_thread.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/error.c` & `createrepo_c-1.1.0/tests/createrepo/error.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/error.h` & `createrepo_c-1.1.0/tests/createrepo/error.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/helpers.c` & `createrepo_c-1.1.0/tests/createrepo/helpers.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/helpers.h` & `createrepo_c-1.1.0/tests/createrepo/helpers.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/koji.c` & `createrepo_c-1.1.0/tests/createrepo/koji.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/koji.h` & `createrepo_c-1.1.0/tests/createrepo/koji.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/load_metadata.c` & `createrepo_c-1.1.0/tests/createrepo/load_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/load_metadata.h` & `createrepo_c-1.1.0/tests/createrepo/load_metadata.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/locate_metadata.c` & `createrepo_c-1.1.0/tests/createrepo/locate_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/locate_metadata.h` & `createrepo_c-1.1.0/tests/createrepo/locate_metadata.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/mergerepo_c.c` & `createrepo_c-1.1.0/tests/createrepo/mergerepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/mergerepo_c.h` & `createrepo_c-1.1.0/tests/createrepo/mergerepo_c.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/metadata_internal.h` & `createrepo_c-1.1.0/tests/createrepo/metadata_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/misc.c` & `createrepo_c-1.1.0/tests/createrepo/misc.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/misc.h` & `createrepo_c-1.1.0/tests/createrepo/misc.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/modifyrepo_c.c` & `createrepo_c-1.1.0/tests/createrepo/modifyrepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/modifyrepo_shared.c` & `createrepo_c-1.1.0/tests/createrepo/modifyrepo_shared.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/modifyrepo_shared.h` & `createrepo_c-1.1.0/tests/createrepo/modifyrepo_shared.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/package.c` & `createrepo_c-1.1.0/tests/createrepo/package.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/package.h` & `createrepo_c-1.1.0/tests/createrepo/package.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/package_internal.h` & `createrepo_c-1.1.0/tests/createrepo/package_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/parsehdr.c` & `createrepo_c-1.1.0/tests/createrepo/parsehdr.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/parsehdr.h` & `createrepo_c-1.1.0/tests/createrepo/parsehdr.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/parsepkg.c` & `createrepo_c-1.1.0/tests/createrepo/parsepkg.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/parsepkg.h` & `createrepo_c-1.1.0/tests/createrepo/parsepkg.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/CMakeLists.txt` & `createrepo_c-1.1.0/tests/createrepo/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/checksum-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/checksum-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/checksum-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/checksum-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/compression_wrapper-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/compression_wrapper-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/compression_wrapper-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/compression_wrapper-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/contentstat-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/contentstat-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/contentstat-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/contentstat-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/createrepo_c.egg-info/PKG-INFO` & `createrepo_c-1.1.0/tests/createrepo/python/createrepo_c.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: createrepo-c
-Version: 1.0.4
+Version: 1.1.0
 Summary: C implementation of createrepo
 Home-page: https://github.com/rpm-software-management
 Author: RPM Software Management
 Author-email: rpm-ecosystem@lists.rpm.org
 License: GPLv2+
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/createrepo_c.egg-info/SOURCES.txt` & `createrepo_c-1.1.0/tests/createrepo/python/createrepo_c.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -301,14 +301,15 @@
 tests/python/tests/test_load_metadata.py
 tests/python/tests/test_locate_metadata.py
 tests/python/tests/test_misc.py
 tests/python/tests/test_package.py
 tests/python/tests/test_parsepkg.py
 tests/python/tests/test_repomd.py
 tests/python/tests/test_repomdrecord.py
+tests/python/tests/test_repository.py
 tests/python/tests/test_sqlite.py
 tests/python/tests/test_updatecollection.py
 tests/python/tests/test_updatecollectionmodule.py
 tests/python/tests/test_updatecollectionpackage.py
 tests/python/tests/test_updateinfo.py
 tests/python/tests/test_updaterecord.py
 tests/python/tests/test_updatereference.py
```

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/createrepo_cmodule.c` & `createrepo_c-1.1.0/tests/createrepo/python/createrepo_cmodule.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/exception-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/exception-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/exception-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/exception-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/load_metadata-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/load_metadata-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/load_metadata-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/load_metadata-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/locate_metadata-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/locate_metadata-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/locate_metadata-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/locate_metadata-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/misc-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/misc-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/misc-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/misc-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/package-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/package-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/package-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/package-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/parsepkg-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/parsepkg-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/parsepkg-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/parsepkg-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/repomd-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/repomd-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/repomd-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/repomd-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/repomdrecord-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/repomdrecord-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/repomdrecord-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/repomdrecord-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/sqlite-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/sqlite-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/sqlite-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/sqlite-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/typeconversion.c` & `createrepo_c-1.1.0/tests/createrepo/python/typeconversion.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/typeconversion.h` & `createrepo_c-1.1.0/tests/createrepo/python/typeconversion.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/updatecollection-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/updatecollection-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/updatecollection-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/updatecollection-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/updatecollectionmodule-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/updatecollectionmodule-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/updatecollectionmodule-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/updatecollectionmodule-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/updatecollectionpackage-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/updatecollectionpackage-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/updatecollectionpackage-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/updatecollectionpackage-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/updateinfo-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/updateinfo-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/updateinfo-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/updateinfo-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/updaterecord-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/updaterecord-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/updaterecord-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/updaterecord-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/updatereference-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/updatereference-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/updatereference-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/updatereference-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/xml_dump-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/xml_dump-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/xml_dump-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/xml_dump-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/xml_file-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/xml_file-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/xml_file-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/xml_file-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/xml_parser-py.c` & `createrepo_c-1.1.0/tests/createrepo/python/xml_parser-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/python/xml_parser-py.h` & `createrepo_c-1.1.0/tests/createrepo/python/xml_parser-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/repomd.c` & `createrepo_c-1.1.0/tests/createrepo/repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/repomd.h` & `createrepo_c-1.1.0/tests/createrepo/repomd.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/repomd_internal.h` & `createrepo_c-1.1.0/tests/createrepo/repomd_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/sqlite.c` & `createrepo_c-1.1.0/tests/createrepo/sqlite.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/sqlite.h` & `createrepo_c-1.1.0/tests/createrepo/sqlite.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/sqliterepo_c.c` & `createrepo_c-1.1.0/tests/createrepo/sqliterepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/threads.c` & `createrepo_c-1.1.0/tests/createrepo/threads.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/threads.h` & `createrepo_c-1.1.0/tests/createrepo/threads.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/updateinfo.c` & `createrepo_c-1.1.0/tests/createrepo/updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/updateinfo.h` & `createrepo_c-1.1.0/tests/createrepo/updateinfo.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/version.h.in` & `createrepo_c-1.1.0/tests/createrepo/version.h.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_dump.h` & `createrepo_c-1.1.0/tests/createrepo/xml_dump.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_dump_deltapackage.c` & `createrepo_c-1.1.0/tests/createrepo/xml_dump_deltapackage.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_dump_filelists.c` & `createrepo_c-1.1.0/tests/createrepo/xml_dump_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_dump_internal.h` & `createrepo_c-1.1.0/tests/createrepo/xml_dump_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_dump_other.c` & `createrepo_c-1.1.0/tests/createrepo/xml_dump_other.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_dump_primary.c` & `createrepo_c-1.1.0/tests/createrepo/xml_dump_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_dump_repomd.c` & `createrepo_c-1.1.0/tests/createrepo/xml_dump_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_dump_updateinfo.c` & `createrepo_c-1.1.0/tests/createrepo/xml_dump_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_file.c` & `createrepo_c-1.1.0/tests/createrepo/xml_file.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_file.h` & `createrepo_c-1.1.0/tests/createrepo/xml_file.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_parser.c` & `createrepo_c-1.1.0/tests/createrepo/xml_parser.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_parser.h` & `createrepo_c-1.1.0/tests/createrepo/xml_parser.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_parser_filelists.c` & `createrepo_c-1.1.0/tests/createrepo/xml_parser_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_parser_internal.h` & `createrepo_c-1.1.0/tests/createrepo/xml_parser_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_parser_main_metadata_together.c` & `createrepo_c-1.1.0/tests/createrepo/xml_parser_main_metadata_together.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_parser_other.c` & `createrepo_c-1.1.0/tests/createrepo/xml_parser_other.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_parser_primary.c` & `createrepo_c-1.1.0/tests/createrepo/xml_parser_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_parser_repomd.c` & `createrepo_c-1.1.0/tests/createrepo/xml_parser_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/createrepo/xml_parser_updateinfo.c` & `createrepo_c-1.1.0/tests/createrepo/xml_parser_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/fixtures.h` & `createrepo_c-1.1.0/tests/fixtures.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_checksum.py` & `createrepo_c-1.1.0/tests/python/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_compression_wrapper.py` & `createrepo_c-1.1.0/tests/python/tests/test_compression_wrapper.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_contentstat.py` & `createrepo_c-1.1.0/tests/python/tests/test_contentstat.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_crfile.py` & `createrepo_c-1.1.0/tests/python/tests/test_crfile.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_load_metadata.py` & `createrepo_c-1.1.0/tests/python/tests/test_load_metadata.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_locate_metadata.py` & `createrepo_c-1.1.0/tests/python/tests/test_locate_metadata.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_misc.py` & `createrepo_c-1.1.0/tests/python/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_package.py` & `createrepo_c-1.1.0/tests/python/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_parsepkg.py` & `createrepo_c-1.1.0/tests/python/tests/test_parsepkg.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_repomd.py` & `createrepo_c-1.1.0/tests/python/tests/test_repomd.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_repomdrecord.py` & `createrepo_c-1.1.0/tests/python/tests/test_repomdrecord.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_sqlite.py` & `createrepo_c-1.1.0/tests/python/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_updatecollection.py` & `createrepo_c-1.1.0/tests/python/tests/test_updatecollection.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_updatecollectionmodule.py` & `createrepo_c-1.1.0/tests/python/tests/test_updatecollectionmodule.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_updatecollectionpackage.py` & `createrepo_c-1.1.0/tests/python/tests/test_updatecollectionpackage.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_updateinfo.py` & `createrepo_c-1.1.0/tests/python/tests/test_updateinfo.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_updaterecord.py` & `createrepo_c-1.1.0/tests/python/tests/test_updaterecord.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_updatereference.py` & `createrepo_c-1.1.0/tests/python/tests/test_updatereference.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_xml_file.py` & `createrepo_c-1.1.0/tests/python/tests/test_xml_file.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/python/tests/test_xml_parser.py` & `createrepo_c-1.1.0/tests/python/tests/test_xml_parser.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/run_tests.sh.in` & `createrepo_c-1.1.0/tests/run_tests.sh.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_checksum.c` & `createrepo_c-1.1.0/tests/test_checksum.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_compression_wrapper.c` & `createrepo_c-1.1.0/tests/test_compression_wrapper.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_koji.c` & `createrepo_c-1.1.0/tests/test_koji.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_load_metadata.c` & `createrepo_c-1.1.0/tests/test_load_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_locate_metadata.c` & `createrepo_c-1.1.0/tests/test_locate_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_misc.c` & `createrepo_c-1.1.0/tests/test_misc.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_modifyrepo_shared.c` & `createrepo_c-1.1.0/tests/test_modifyrepo_shared.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_sqlite.c` & `createrepo_c-1.1.0/tests/test_sqlite.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_xml_dump.c` & `createrepo_c-1.1.0/tests/test_xml_dump.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_xml_dump_primary.c` & `createrepo_c-1.1.0/tests/test_xml_dump_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_xml_file.c` & `createrepo_c-1.1.0/tests/test_xml_file.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_xml_parser_filelists.c` & `createrepo_c-1.1.0/tests/test_xml_parser_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_xml_parser_main_metadata_together.c` & `createrepo_c-1.1.0/tests/test_xml_parser_main_metadata_together.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_xml_parser_repomd.c` & `createrepo_c-1.1.0/tests/test_xml_parser_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/test_xml_parser_updateinfo.c` & `createrepo_c-1.1.0/tests/test_xml_parser_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/comps_files/comps_00.xml` & `createrepo_c-1.1.0/tests/testdata/comps_files/comps_00.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/bad_file_type-filelists.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/bad_file_type-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/error_00-filelists.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/error_00-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/error_00-other.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/error_00-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/error_00-primary.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/error_00-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/long_primary.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/long_primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/missing_type-repomd.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/missing_type-repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/multiple_warnings_00-filelists.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/multiple_warnings_00-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/multiple_warnings_00-other.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/multiple_warnings_00-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/multiple_warnings_00-primary.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/multiple_warnings_00-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/no_pkgid-other.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/no_pkgid-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/repo_01_ampersand-other.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/repo_01_ampersand-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/repo_01_ampersand-primary.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/repo_01_ampersand-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/repo_02_different_order_filelists.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/repo_02_different_order_filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_00-filelists.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_00-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_00-other.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_00-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_00-primary.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_00-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_01-filelists.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_01-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_01-other.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_01-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_01-primary.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_01-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_02-filelists.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_02-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_02-other.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_02-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/unknown_element_02-primary.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/unknown_element_02-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/modified_repo_files/updateinfo_ampersand.xml` & `createrepo_c-1.1.0/tests/testdata/modified_repo_files/updateinfo_ampersand.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/other_metadata/0402e012013246e7e2f2f638c8a6046efdfd71ae1cbeff9c391d9c1ae5d7d431-comps-f19.xml.bz2` & `createrepo_c-1.1.0/tests/testdata/other_metadata/0402e012013246e7e2f2f638c8a6046efdfd71ae1cbeff9c391d9c1ae5d7d431-comps-f19.xml.bz2`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/other_metadata/36c4f2d6dda3b015b4a7da59552c7c76eff99a59979178513cb51341f6eead44-comps-f19.xml` & `createrepo_c-1.1.0/tests/testdata/other_metadata/36c4f2d6dda3b015b4a7da59552c7c76eff99a59979178513cb51341f6eead44-comps-f19.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/other_metadata/71d988ca33b31a18b0d775478d6f59b40583c794ae76393284850ee97bfba4dc-comps-f19.xml.gz` & `createrepo_c-1.1.0/tests/testdata/other_metadata/71d988ca33b31a18b0d775478d6f59b40583c794ae76393284850ee97bfba4dc-comps-f19.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/other_metadata/c941e2c77a27cdca324c0e0bc3190e134fddddb36a03fb5517e55d156b955205-comps-f19.xml.xz` & `createrepo_c-1.1.0/tests/testdata/other_metadata/c941e2c77a27cdca324c0e0bc3190e134fddddb36a03fb5517e55d156b955205-comps-f19.xml.xz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/other_metadata/comps-f19.xml` & `createrepo_c-1.1.0/tests/testdata/other_metadata/comps-f19.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/packages/Archer-3.4.5-6.x86_64.rpm` & `createrepo_c-1.1.0/tests/testdata/packages/Archer-3.4.5-6.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/packages/Rimmer-1.0.2-2.x86_64.rpm` & `createrepo_c-1.1.0/tests/testdata/packages/Rimmer-1.0.2-2.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/packages/balicek-iso88591-1.1.1-1.x86_64.rpm` & `createrepo_c-1.1.0/tests/testdata/packages/balicek-iso88591-1.1.1-1.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/packages/balicek-iso88592-1.1.1-1.x86_64.rpm` & `createrepo_c-1.1.0/tests/testdata/packages/balicek-iso88592-1.1.1-1.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/packages/balicek-utf8-1.1.1-1.x86_64.rpm` & `createrepo_c-1.1.0/tests/testdata/packages/balicek-utf8-1.1.1-1.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/packages/empty-0-0.src.rpm` & `createrepo_c-1.1.0/tests/testdata/packages/empty-0-0.src.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/packages/empty-0-0.x86_64.rpm` & `createrepo_c-1.1.0/tests/testdata/packages/empty-0-0.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/packages/fake_bash-1.1.1-1.x86_64.rpm` & `createrepo_c-1.1.0/tests/testdata/packages/fake_bash-1.1.1-1.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/packages/super_kernel-6.0.1-2.x86_64.rpm` & `createrepo_c-1.1.0/tests/testdata/packages/super_kernel-6.0.1-2.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_00/repodata/repomd.xml` & `createrepo_c-1.1.0/tests/testdata/repo_00/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_01/repodata/6c662d665c24de9a0f62c17d8fa50622307739d7376f0d19097ca96c6d7f5e3e-primary.xml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_01/repodata/6c662d665c24de9a0f62c17d8fa50622307739d7376f0d19097ca96c6d7f5e3e-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_01/repodata/repomd.xml` & `createrepo_c-1.1.0/tests/testdata/repo_01/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_02/repodata/bcde64b04916a2a72fdc257d61bc922c70b3d58e953499180585f7a360ce86cf-primary.xml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_02/repodata/bcde64b04916a2a72fdc257d61bc922c70b3d58e953499180585f7a360ce86cf-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_02/repodata/repomd.xml` & `createrepo_c-1.1.0/tests/testdata/repo_02/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_03/repodata/a850093e240506c728d6ce26a6fc51d6a7fe10730c67988d13afa7dd82df82d5-modules.yaml.xz` & `createrepo_c-1.1.0/tests/testdata/repo_03/repodata/a850093e240506c728d6ce26a6fc51d6a7fe10730c67988d13afa7dd82df82d5-modules.yaml.xz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_03/repodata/repomd.xml` & `createrepo_c-1.1.0/tests/testdata/repo_03/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_04/repodata/6a5f64dd82a126a161657764fe8f4b4092c0a3b61b9a34bde2af89dc1df112a1-primary.xml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_04/repodata/6a5f64dd82a126a161657764fe8f4b4092c0a3b61b9a34bde2af89dc1df112a1-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_04/repodata/repomd.xml` & `createrepo_c-1.1.0/tests/testdata/repo_04/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_koji_01/repodata/5d039d9ec332d158c69d083f04ac88a187c6b68444472b802eaf0249aec83294-other.xml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_koji_01/repodata/5d039d9ec332d158c69d083f04ac88a187c6b68444472b802eaf0249aec83294-other.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_koji_01/repodata/b153f86915d1dacbb89b244da26e50adb204195262fd3562290de26725daa21d-primary.xml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_koji_01/repodata/b153f86915d1dacbb89b244da26e50adb204195262fd3562290de26725daa21d-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_koji_01/repodata/repomd.xml` & `createrepo_c-1.1.0/tests/testdata/repo_koji_01/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_koji_02/repodata/ee9261d1d2916d841cf24bb01743198ec63ed596f410784602eca2350e430e17-primary.xml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_koji_02/repodata/ee9261d1d2916d841cf24bb01743198ec63ed596f410784602eca2350e430e17-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_koji_02/repodata/feb0b5fdcb0ee1cf981b041f0749ec381145cd9f6b4397991ef5dafcb6807bba-other.xml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_koji_02/repodata/feb0b5fdcb0ee1cf981b041f0749ec381145cd9f6b4397991ef5dafcb6807bba-other.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_koji_02/repodata/repomd.xml` & `createrepo_c-1.1.0/tests/testdata/repo_koji_02/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/0219a2f1f9f32af6b7873905269ac1bc27b03e0caf3968c929a49e5a939e8935-updateinfo_01.xml.gz.zck` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/0219a2f1f9f32af6b7873905269ac1bc27b03e0caf3968c929a49e5a939e8935-updateinfo_01.xml.gz.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/04460bfaf6cb5af6b0925d8c99401a44e5192d287796aed4cced5f7ce881761f-comps.f20.xml` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/04460bfaf6cb5af6b0925d8c99401a44e5192d287796aed4cced5f7ce881761f-comps.f20.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/1e12239bf5cb07ec73c74482c35e80dabe30dbe2fdd57bd9e557d987cbacc8c2-primary.sqlite.bz2` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/1e12239bf5cb07ec73c74482c35e80dabe30dbe2fdd57bd9e557d987cbacc8c2-primary.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.gz.zck` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.gz.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.zck` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/3d6eaa7c77ef92586470dd6a542478e42cc421a85f12e0db93aa783077704cd0-filelists.xml.zck` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/3d6eaa7c77ef92586470dd6a542478e42cc421a85f12e0db93aa783077704cd0-filelists.xml.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/490a2a494a3827b8a356f728ac36bc02fb009b0eaea173c890e727bb54219037-primary.xml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/490a2a494a3827b8a356f728ac36bc02fb009b0eaea173c890e727bb54219037-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/4f4de7d3254a033b84626f330bc6adb8a3c1a4a20f0ddbe30a5692a041318c81-filelists.sqlite.bz2` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/4f4de7d3254a033b84626f330bc6adb8a3c1a4a20f0ddbe30a5692a041318c81-filelists.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/4fbad65c641f4f8fb3cec9b1672fcec2357443e1ea6e93541a0bb559c7dc9238-modules.yaml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/4fbad65c641f4f8fb3cec9b1672fcec2357443e1ea6e93541a0bb559c7dc9238-modules.yaml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/88514679cb03d8f51e850ad3639c089f899e83407a2380ef9e62873a8eb1db13-updateinfo_01.xml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/88514679cb03d8f51e850ad3639c089f899e83407a2380ef9e62873a8eb1db13-updateinfo_01.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/8b13cba732c1a02b841f43d6791ca68788d45f376787d9f3ccf68e75f01af499-other.sqlite.bz2` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/8b13cba732c1a02b841f43d6791ca68788d45f376787d9f3ccf68e75f01af499-other.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/ba5a4fdbb20e7b9b70d9a9abd974bcab1065b1e81d711f80e06ad8cae30c4183-filelists.xml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/ba5a4fdbb20e7b9b70d9a9abd974bcab1065b1e81d711f80e06ad8cae30c4183-filelists.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/c5582e660ed9a2d3c10ba44f0aeb02f2bb70e85dc3c8cda4266183d4e5235aa7-other.xml.zck` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/c5582e660ed9a2d3c10ba44f0aeb02f2bb70e85dc3c8cda4266183d4e5235aa7-other.xml.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/cb0f4b5df8268f248158e50d66ee1565591bca23ee2dbd84ae9c457962fa3122-modules.yaml.gz.zck` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/cb0f4b5df8268f248158e50d66ee1565591bca23ee2dbd84ae9c457962fa3122-modules.yaml.gz.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/e9e6ca4765de75cc3b2bf05e6cf631703c6557edd642300748d7747000547365-primary.xml.zck` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/e9e6ca4765de75cc3b2bf05e6cf631703c6557edd642300748d7747000547365-primary.xml.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/f9d860ddcb64fbdc88a9b71a14ddb9f5670968d5dd3430412565c13d42b6804d-comps.f20.xml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/f9d860ddcb64fbdc88a9b71a14ddb9f5670968d5dd3430412565c13d42b6804d-comps.f20.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/fd458a424a3f3e0dadc95b806674b79055c24e73637e47ad5a6e57926aa1b9d1-other.xml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/fd458a424a3f3e0dadc95b806674b79055c24e73637e47ad5a6e57926aa1b9d1-other.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_additional_metadata/repodata/repomd.xml` & `createrepo_c-1.1.0/tests/testdata/repo_with_additional_metadata/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_duplicate_packages/repodata/primary.xml.gz` & `createrepo_c-1.1.0/tests/testdata/repo_with_duplicate_packages/repodata/primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repo_with_duplicate_packages/repodata/repomd.xml` & `createrepo_c-1.1.0/tests/testdata/repo_with_duplicate_packages/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repodata_snippets/filelists_ext_snippet_02.xml` & `createrepo_c-1.1.0/tests/testdata/repodata_snippets/filelists_ext_snippet_02.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repodata_snippets/other_snippet_02.xml` & `createrepo_c-1.1.0/tests/testdata/repodata_snippets/other_snippet_02.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repodata_snippets/primary_snippet_01.xml` & `createrepo_c-1.1.0/tests/testdata/repodata_snippets/primary_snippet_01.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/repodata_snippets/primary_snippet_02.xml` & `createrepo_c-1.1.0/tests/testdata/repodata_snippets/primary_snippet_02.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/specs/fake-Archer.spec` & `createrepo_c-1.1.0/tests/testdata/specs/fake-Archer.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/specs/fake-Rimmer.spec` & `createrepo_c-1.1.0/tests/testdata/specs/fake-Rimmer.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/specs/fake-balicek-iso88591.spec` & `createrepo_c-1.1.0/tests/testdata/specs/fake-balicek-iso88591.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/specs/fake-balicek-iso88592.spec` & `createrepo_c-1.1.0/tests/testdata/specs/fake-balicek-iso88592.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/specs/fake-balicek-utf8.spec` & `createrepo_c-1.1.0/tests/testdata/specs/fake-balicek-utf8.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/specs/fake-fake_bash.spec` & `createrepo_c-1.1.0/tests/testdata/specs/fake-fake_bash.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/specs/fake-super_kernel.spec` & `createrepo_c-1.1.0/tests/testdata/specs/fake-super_kernel.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/test_files/binary_file` & `createrepo_c-1.1.0/tests/testdata/test_files/binary_file`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/test_files/sqlite_file.sqlite` & `createrepo_c-1.1.0/tests/testdata/test_files/sqlite_file.sqlite`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/test_files/text_file` & `createrepo_c-1.1.0/tests/testdata/test_files/text_file`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/test_files/text_file.gz` & `createrepo_c-1.1.0/tests/testdata/test_files/text_file.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/test_files/text_file.xz` & `createrepo_c-1.1.0/tests/testdata/test_files/text_file.xz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/updateinfo_files/updateinfo_01.xml` & `createrepo_c-1.1.0/tests/testdata/updateinfo_files/updateinfo_01.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.0.4/tests/testdata/updateinfo_files/updateinfo_03.xml` & `createrepo_c-1.1.0/tests/testdata/updateinfo_files/updateinfo_03.xml`

 * *Files identical despite different names*

