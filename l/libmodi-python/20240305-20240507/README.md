# Comparing `tmp/libmodi-python-20240305.tar.gz` & `tmp/libmodi-python-20240507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmodi-python-20240305.tar", last modified: Tue Mar  5 05:38:52 2024, max compression
+gzip compressed data, was "libmodi-python-20240507.tar", last modified: Tue May  7 05:20:20 2024, max compression
```

## Comparing `libmodi-python-20240305.tar` & `libmodi-python-20240507.tar`

### file list

```diff
@@ -1,1002 +1,1002 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:49.000000 libmodi-20240305/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36887 2024-03-05 05:16:16.000000 libmodi-20240305/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-03-05 05:15:52.000000 libmodi-20240305/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2024-03-05 05:16:34.000000 libmodi-20240305/libmodi.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/moditools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37173 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2987 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26443 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1934 2024-03-05 04:57:47.000000 libmodi-20240305/moditools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5414 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1406 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18958 2024-03-05 04:57:47.000000 libmodi-20240305/moditools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_libmodi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10552 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/byte_size_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1210 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2158 2023-12-03 09:11:31.000000 libmodi-20240305/moditools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20750 2024-03-05 04:57:47.000000 libmodi-20240305/moditools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9045 2024-03-05 04:57:47.000000 libmodi-20240305/moditools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5900 2024-03-05 04:57:47.000000 libmodi-20240305/moditools/modiinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3618 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1778 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2258 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15149 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/modimount.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12659 2024-03-05 04:57:47.000000 libmodi-20240305/moditools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37809 2024-03-05 05:16:17.000000 libmodi-20240305/moditools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/byte_size_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3927 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/moditools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2762 2024-03-05 04:56:28.000000 libmodi-20240305/moditools/mount_fuse.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/libmodi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13950 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_sparse_image_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2331 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_udif_resource_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3856 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_bzip.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1390 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7911 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1812 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1072 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2907 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_block_chunks_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libfmos.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2264 2024-03-05 04:58:22.000000 libmodi-20240305/libmodi/libmodi_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12089 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_compression.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2786 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_udif_xml_plist.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2176 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_sparse_bundle_xml_plist.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3450 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/modi_udif_resource_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2103 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1445 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libfplist.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16103 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_data_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7546 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3338 2023-12-03 09:11:30.000000 libmodi-20240305/libmodi/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14786 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14983 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_sparse_bundle_xml_plist.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1070 2024-03-05 05:16:34.000000 libmodi-20240305/libmodi/libmodi.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_udif_block_table_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2649 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_data_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3338 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2243 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_udif_block_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1322 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_compression.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12981 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_block_chunks_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12500 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2169 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_sparse_image_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1940 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/modi_sparse_image_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2739 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_bands_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3457 2024-03-05 04:58:22.000000 libmodi-20240305/libmodi/libmodi_deflate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6394 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_udif_block_table_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1788 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20811 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_udif_xml_plist.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libcdirectory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   108282 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_huffman_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_i18n.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15475 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_udif_block_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3686 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48615 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_deflate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13493 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_udif_resource_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42269 2024-03-05 05:16:17.000000 libmodi-20240305/libmodi/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-03-05 05:16:34.000000 libmodi-20240305/libmodi/libmodi_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1892 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2937 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/modi_udif_block_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3706 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47348 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_bzip.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12487 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_bands_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-03-05 04:56:28.000000 libmodi-20240305/libmodi/libmodi_libcfile.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/libfmos/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2023 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_lzfse_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2269 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2964 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_lzfse_decoder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7799 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_adc.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3441 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_lzfse.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1321 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_adc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      961 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25840 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_lzvn.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6380 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_lzfse_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3271 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_lzfse_decoder.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60280 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_lzfse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1326 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_lzvn.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-05 05:15:55.000000 libmodi-20240305/libfmos/libfmos_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34824 2024-03-05 05:16:16.000000 libmodi-20240305/libfmos/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-03-05 04:56:26.000000 libmodi-20240305/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-03-05 05:16:16.000000 libmodi-20240305/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 04:56:26.000000 libmodi-20240305/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-03-05 05:16:17.000000 libmodi-20240305/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/libfplist/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1401 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5928 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_xml_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1635 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6651 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_xml_scanner.l
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)  8431465 2024-03-05 05:17:23.000000 libmodi-20240305/libfplist/libfplist_xml_scanner.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56503 2024-03-05 05:17:23.000000 libmodi-20240305/libfplist/libfplist_xml_parser.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1516 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1788 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_xml_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12481 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_xml_parser.y
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4066 2024-03-05 05:17:23.000000 libmodi-20240305/libfplist/libfplist_xml_parser.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15149 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_property_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3419 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_property.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34608 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_property.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15574 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_xml_tag.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2497 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_property_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37681 2024-03-05 05:16:17.000000 libmodi-20240305/libfplist/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2894 2024-03-05 05:15:56.000000 libmodi-20240305/libfplist/libfplist_xml_tag.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/libcaes/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/libcaes_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2885 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/libcaes_tweaked_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4464 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/libcaes_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/libcaes_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82616 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/libcaes_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/libcaes_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/libcaes_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/libcaes_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/libcaes_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/libcaes_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/libcaes_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/libcaes_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33360 2024-03-05 05:16:16.000000 libmodi-20240305/libcaes/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33103 2024-03-05 05:15:39.000000 libmodi-20240305/libcaes/libcaes_tweaked_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:49.000000 libmodi-20240305/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-05 05:15:53.000000 libmodi-20240305/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-03-05 05:15:53.000000 libmodi-20240305/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-03-05 05:15:53.000000 libmodi-20240305/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-05 05:15:53.000000 libmodi-20240305/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-03-05 05:15:53.000000 libmodi-20240305/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-05 05:15:53.000000 libmodi-20240305/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-05 05:15:53.000000 libmodi-20240305/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-03-05 05:15:53.000000 libmodi-20240305/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-03-05 05:15:53.000000 libmodi-20240305/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-03-05 05:15:53.000000 libmodi-20240305/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-03-05 05:15:53.000000 libmodi-20240305/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33102 2024-03-05 05:16:16.000000 libmodi-20240305/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-05 05:15:53.000000 libmodi-20240305/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:48.000000 libmodi-20240305/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4428 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libfmos.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:11:27.000000 libmodi-20240305/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:11:27.000000 libmodi-20240305/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:11:27.000000 libmodi-20240305/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:11:27.000000 libmodi-20240305/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:11:27.000000 libmodi-20240305/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:11:27.000000 libmodi-20240305/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-03-05 05:16:08.000000 libmodi-20240305/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-03-05 05:16:08.000000 libmodi-20240305/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:11:27.000000 libmodi-20240305/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-03-05 05:16:08.000000 libmodi-20240305/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:11:27.000000 libmodi-20240305/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3739 2023-12-03 09:11:27.000000 libmodi-20240305/m4/bzip2.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8319 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libhmac.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:11:27.000000 libmodi-20240305/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-03-05 05:16:08.000000 libmodi-20240305/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:11:27.000000 libmodi-20240305/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:11:27.000000 libmodi-20240305/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-03-05 05:16:08.000000 libmodi-20240305/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:11:27.000000 libmodi-20240305/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:11:27.000000 libmodi-20240305/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27481 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libcrypto.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8654 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libcdirectory.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:11:27.000000 libmodi-20240305/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:11:27.000000 libmodi-20240305/m4/pthread.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6201 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libfplist.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3671 2023-12-03 09:11:27.000000 libmodi-20240305/m4/lzma.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7383 2023-12-03 09:11:27.000000 libmodi-20240305/m4/zlib.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6269 2023-12-03 09:11:27.000000 libmodi-20240305/m4/libcaes.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:48.000000 libmodi-20240305/include/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:48.000000 libmodi-20240305/include/libmodi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1917 2024-03-05 04:56:27.000000 libmodi-20240305/include/libmodi/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1915 2024-03-05 05:16:34.000000 libmodi-20240305/include/libmodi/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4935 2024-03-05 04:56:27.000000 libmodi-20240305/include/libmodi/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4804 2024-03-05 05:16:34.000000 libmodi-20240305/include/libmodi/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-03-05 04:56:27.000000 libmodi-20240305/include/libmodi/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-03-05 04:56:27.000000 libmodi-20240305/include/libmodi/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-05 04:56:27.000000 libmodi-20240305/include/libmodi/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2024-03-05 05:16:34.000000 libmodi-20240305/include/libmodi/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-03-05 04:56:27.000000 libmodi-20240305/include/libmodi/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10784 2024-03-05 04:56:27.000000 libmodi-20240305/include/libmodi.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      459 2024-03-05 04:56:26.000000 libmodi-20240305/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10784 2024-03-05 05:16:34.000000 libmodi-20240305/include/libmodi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31629 2024-03-05 05:16:16.000000 libmodi-20240305/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/pymodi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_libmodi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33791 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3174 2024-03-05 04:57:47.000000 libmodi-20240305/pymodi/pymodi_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1851 2024-03-05 04:57:47.000000 libmodi-20240305/pymodi/pymodi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1118 2023-12-03 09:11:31.000000 libmodi-20240305/pymodi/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14118 2024-03-05 04:57:47.000000 libmodi-20240305/pymodi/pymodi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4080 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32818 2024-03-05 04:57:47.000000 libmodi-20240305/pymodi/pymodi_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4960 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_file_objects_io_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44508 2024-03-05 05:16:17.000000 libmodi-20240305/pymodi/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_file_objects_io_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-03-05 04:56:28.000000 libmodi-20240305/pymodi/pymodi_integer.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:48.000000 libmodi-20240305/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-03-05 04:56:27.000000 libmodi-20240305/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-03-05 04:56:27.000000 libmodi-20240305/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-03-05 04:56:27.000000 libmodi-20240305/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-03-05 04:56:27.000000 libmodi-20240305/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-05 04:56:27.000000 libmodi-20240305/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-03-05 04:56:27.000000 libmodi-20240305/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-03-05 04:56:27.000000 libmodi-20240305/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-03-05 04:56:26.000000 libmodi-20240305/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-03-05 04:56:27.000000 libmodi-20240305/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-03-05 05:16:34.000000 libmodi-20240305/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21078 2024-03-05 05:16:15.000000 libmodi-20240305/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22281 2024-03-05 05:16:34.000000 libmodi-20240305/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-03-05 04:56:27.000000 libmodi-20240305/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-03-05 04:56:27.000000 libmodi-20240305/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-03-05 04:56:27.000000 libmodi-20240305/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28655 2024-03-05 05:16:16.000000 libmodi-20240305/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:49.000000 libmodi-20240305/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-03-05 05:15:45.000000 libmodi-20240305/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-05 05:15:45.000000 libmodi-20240305/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-03-05 05:15:45.000000 libmodi-20240305/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-03-05 05:15:45.000000 libmodi-20240305/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-05 05:15:45.000000 libmodi-20240305/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-05 05:15:45.000000 libmodi-20240305/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-03-05 05:15:45.000000 libmodi-20240305/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-03-05 05:15:45.000000 libmodi-20240305/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-03-05 05:15:45.000000 libmodi-20240305/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-03-05 05:15:45.000000 libmodi-20240305/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33658 2024-03-05 05:16:16.000000 libmodi-20240305/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-05 05:15:45.000000 libmodi-20240305/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-03-05 05:15:45.000000 libmodi-20240305/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-03-05 05:15:45.000000 libmodi-20240305/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:49.000000 libmodi-20240305/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34131 2024-03-05 05:16:16.000000 libmodi-20240305/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-03-05 05:15:51.000000 libmodi-20240305/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2599 2023-12-03 09:11:14.000000 libmodi-20240305/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:49.000000 libmodi-20240305/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37117 2024-03-05 05:16:16.000000 libmodi-20240305/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-03-05 05:15:38.000000 libmodi-20240305/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:11:14.000000 libmodi-20240305/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-03-05 05:16:16.000000 libmodi-20240305/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:48.000000 libmodi-20240305/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-03-05 04:56:26.000000 libmodi-20240305/dpkg/libmodi.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-03-05 04:56:29.000000 libmodi-20240305/dpkg/copyright
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-03-05 04:56:26.000000 libmodi-20240305/dpkg/libmodi-python3.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:48.000000 libmodi-20240305/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-03-05 04:56:26.000000 libmodi-20240305/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2066 2024-03-05 04:56:26.000000 libmodi-20240305/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      761 2024-03-05 04:56:26.000000 libmodi-20240305/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-03-05 04:56:26.000000 libmodi-20240305/dpkg/libmodi-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-03-05 04:56:26.000000 libmodi-20240305/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-03-05 05:16:34.000000 libmodi-20240305/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-03-05 04:56:26.000000 libmodi-20240305/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-03-05 04:56:26.000000 libmodi-20240305/dpkg/libmodi-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-03-05 05:16:34.000000 libmodi-20240305/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-03-05 04:56:26.000000 libmodi-20240305/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2209964 2024-03-05 05:16:14.000000 libmodi-20240305/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-03-05 05:16:16.000000 libmodi-20240305/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-03-05 05:16:16.000000 libmodi-20240305/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modimount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7486 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/modimount/modimount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_udif_block_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6242 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_udif_block_table/modi_test_udif_block_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_sparse_bundle_xml_plist/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6510 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_sparse_bundle_xml_plist/modi_test_sparse_bundle_xml_plist.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libmodi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11408 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libmodi/libmodi.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_bzip/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6130 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_bzip/modi_test_bzip.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libfmos/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5663 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libfmos/libfmos.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/zlib/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/zlib/zlib.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libfplist/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6237 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libfplist/libfplist.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libcaes/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4777 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libcaes/libcaes.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/pymodi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6196 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/pymodi/pymodi.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5966 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_error/modi_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2034 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6221 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_io_handle/modi_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_system_string/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6073 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_system_string/modi_test_system_string.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_data_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6471 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_data_block/modi_test_data_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6052 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_notify/modi_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_udif_xml_plist/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6483 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_udif_xml_plist/modi_test_udif_xml_plist.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_udif_resource_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6495 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_udif_resource_file/modi_test_udif_resource_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_huffman_tree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6230 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_huffman_tree/modi_test_huffman_tree.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/modi_test_bands_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6245 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_bands_data_handle/modi_test_bands_data_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6157 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_tools_signal/modi_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_sparse_image_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6498 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_sparse_image_header/modi_test_sparse_image_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6157 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_tools_output/modi_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_udif_block_table_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_udif_block_table_entry/modi_test_udif_block_table_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_deflate/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6299 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_deflate/modi_test_deflate.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7036 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_handle/modi_test_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6490 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_tools_info_handle/modi_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libcpath/libcpath.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42413 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/libmodi.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/bzip2/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4786 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/bzip2/bzip2.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7039 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_support/modi_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/libhmac/libhmac.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27657 2024-03-05 05:16:17.000000 libmodi-20240305/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7924 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modiinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6673 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/modiinfo/modiinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:51.000000 libmodi-20240305/msvscpp/modi_test_bit_stream/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6224 2024-03-05 04:57:22.000000 libmodi-20240305/msvscpp/modi_test_bit_stream/modi_test_bit_stream.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/msvscpp/libcdirectory/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5681 2024-03-05 04:56:56.000000 libmodi-20240305/msvscpp/libcdirectory/libcdirectory.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-03-05 04:56:27.000000 libmodi-20240305/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:49.000000 libmodi-20240305/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34422 2024-03-05 05:16:16.000000 libmodi-20240305/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-03-05 05:15:44.000000 libmodi-20240305/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      807 2024-03-05 04:56:26.000000 libmodi-20240305/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-03-05 05:16:16.000000 libmodi-20240305/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:49.000000 libmodi-20240305/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36106 2024-03-05 05:16:16.000000 libmodi-20240305/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-05 05:15:40.000000 libmodi-20240305/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-03-05 04:56:26.000000 libmodi-20240305/pyproject.toml
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6860 2024-03-05 05:16:17.000000 libmodi-20240305/ylwrap
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-03-05 04:56:26.000000 libmodi-20240305/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-03-05 05:16:16.000000 libmodi-20240305/config.sub
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-03-05 04:56:26.000000 libmodi-20240305/libmodi.pc.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-03-05 04:56:26.000000 libmodi-20240305/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-03-05 04:56:26.000000 libmodi-20240305/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:11:14.000000 libmodi-20240305/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:48.000000 libmodi-20240305/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36512 2024-03-05 05:16:16.000000 libmodi-20240305/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-03-05 05:15:50.000000 libmodi-20240305/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-03-05 05:16:17.000000 libmodi-20240305/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:49.000000 libmodi-20240305/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33700 2024-03-05 05:16:16.000000 libmodi-20240305/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-03-05 05:15:47.000000 libmodi-20240305/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2023-12-03 09:11:14.000000 libmodi-20240305/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5119 2024-03-05 04:58:22.000000 libmodi-20240305/manuals/libmodi.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      154 2023-12-03 09:11:31.000000 libmodi-20240305/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1226 2024-03-05 04:56:29.000000 libmodi-20240305/manuals/modiinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30621 2024-03-05 05:16:17.000000 libmodi-20240305/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2830 2024-03-05 04:57:22.000000 libmodi-20240305/tests/modi_test_bands_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7956 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66883 2024-03-05 04:57:22.000000 libmodi-20240305/tests/modi_test_udif_xml_plist.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16939 2024-03-05 04:57:22.000000 libmodi-20240305/tests/modi_test_udif_resource_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16001 2024-03-05 04:57:22.000000 libmodi-20240305/tests/modi_test_udif_block_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13247 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47609 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_bzip.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19021 2024-03-05 04:57:22.000000 libmodi-20240305/tests/modi_test_sparse_bundle_xml_plist.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4065 2024-03-05 04:57:47.000000 libmodi-20240305/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100206 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_deflate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9561 2024-03-05 04:57:22.000000 libmodi-20240305/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13622 2024-03-05 04:57:22.000000 libmodi-20240305/tests/modi_test_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_libcdirectory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1367 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40690 2024-03-05 04:57:22.000000 libmodi-20240305/tests/modi_test_sparse_image_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20021 2024-03-05 04:57:22.000000 libmodi-20240305/tests/modi_test_data_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9811 2024-03-05 04:57:22.000000 libmodi-20240305/tests/modi_test_udif_block_table_entry.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-03-05 04:56:29.000000 libmodi-20240305/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4075 2024-03-05 04:56:29.000000 libmodi-20240305/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_libmodi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11225 2024-03-05 04:58:22.000000 libmodi-20240305/tests/pymodi_test_handle.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-03-05 04:56:29.000000 libmodi-20240305/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3436 2024-03-05 04:58:22.000000 libmodi-20240305/tests/pymodi_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4123 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15900 2024-03-05 04:57:22.000000 libmodi-20240305/tests/modi_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30660 2024-03-05 04:57:22.000000 libmodi-20240305/tests/modi_test_huffman_tree.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3313 2024-03-05 04:56:29.000000 libmodi-20240305/tests/test_modiinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5590 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74556 2024-03-05 05:16:17.000000 libmodi-20240305/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49072 2024-03-05 04:57:22.000000 libmodi-20240305/tests/modi_test_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2429 2024-03-05 04:57:22.000000 libmodi-20240305/tests/modi_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19103 2024-03-05 04:56:29.000000 libmodi-20240305/tests/modi_test_system_string.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4272 2024-03-05 04:57:47.000000 libmodi-20240305/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2223 2024-03-05 04:56:28.000000 libmodi-20240305/ossfuzz/handle_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      901 2023-12-03 09:11:26.000000 libmodi-20240305/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-03-05 04:56:28.000000 libmodi-20240305/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35904 2024-03-05 05:16:17.000000 libmodi-20240305/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-03-05 04:56:28.000000 libmodi-20240305/ossfuzz/ossfuzz_libmodi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-03-05 05:16:08.000000 libmodi-20240305/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha1_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha224.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha512_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_md5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_md5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha512.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha256_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha224.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha256_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1121 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha224_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_md5_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha1_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36232 2024-03-05 05:16:17.000000 libmodi-20240305/libhmac/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha224_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha512_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha512.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_sha1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-03-05 05:15:59.000000 libmodi-20240305/libhmac/libhmac_md5_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:49.000000 libmodi-20240305/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34480 2024-03-05 05:16:16.000000 libmodi-20240305/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-03-05 05:15:49.000000 libmodi-20240305/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:50.000000 libmodi-20240305/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:11:32.000000 libmodi-20240305/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:11:32.000000 libmodi-20240305/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:11:32.000000 libmodi-20240305/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:11:32.000000 libmodi-20240305/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:11:32.000000 libmodi-20240305/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:11:32.000000 libmodi-20240305/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:11:32.000000 libmodi-20240305/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:11:32.000000 libmodi-20240305/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:11:32.000000 libmodi-20240305/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-03-05 05:16:34.000000 libmodi-20240305/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:11:32.000000 libmodi-20240305/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:11:32.000000 libmodi-20240305/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:49.000000 libmodi-20240305/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57224 2024-03-05 05:16:17.000000 libmodi-20240305/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-03-05 05:16:02.000000 libmodi-20240305/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45013 2024-03-05 05:16:16.000000 libmodi-20240305/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:49.000000 libmodi-20240305/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1657 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38883 2024-03-05 05:16:17.000000 libmodi-20240305/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-03-05 05:15:57.000000 libmodi-20240305/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:49.000000 libmodi-20240305/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-05 05:15:46.000000 libmodi-20240305/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-05 05:15:46.000000 libmodi-20240305/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-03-05 05:15:46.000000 libmodi-20240305/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-03-05 05:15:46.000000 libmodi-20240305/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-03-05 05:15:46.000000 libmodi-20240305/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-05 05:15:46.000000 libmodi-20240305/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-03-05 05:15:46.000000 libmodi-20240305/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-03-05 05:15:46.000000 libmodi-20240305/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-03-05 05:15:46.000000 libmodi-20240305/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-03-05 05:15:46.000000 libmodi-20240305/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-03-05 05:15:46.000000 libmodi-20240305/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33534 2024-03-05 05:16:16.000000 libmodi-20240305/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-05 05:15:46.000000 libmodi-20240305/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-03-05 05:15:46.000000 libmodi-20240305/libcnotify/libcnotify_print.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3803 2024-03-05 04:59:17.000000 libmodi-20240305/libmodi.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:48.000000 libmodi-20240305/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-03-05 05:15:43.000000 libmodi-20240305/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-03-05 05:15:43.000000 libmodi-20240305/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-05 05:15:43.000000 libmodi-20240305/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-03-05 05:15:43.000000 libmodi-20240305/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-03-05 05:15:43.000000 libmodi-20240305/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-05 05:15:43.000000 libmodi-20240305/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-03-05 05:15:43.000000 libmodi-20240305/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-03-05 05:15:43.000000 libmodi-20240305/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-03-05 05:15:43.000000 libmodi-20240305/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-05 05:15:43.000000 libmodi-20240305/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-05 05:15:43.000000 libmodi-20240305/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33047 2024-03-05 05:16:16.000000 libmodi-20240305/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57077 2024-03-05 05:16:11.000000 libmodi-20240305/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9669 2024-03-05 04:59:02.000000 libmodi-20240305/configure.ac
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-05 05:38:49.000000 libmodi-20240305/libcdirectory/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21136 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_directory_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25660 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2886 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1050 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2396 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1809 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2980 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3347 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_directory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1975 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42170 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_directory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35083 2024-03-05 05:16:16.000000 libmodi-20240305/libcdirectory/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1910 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3214 2024-03-05 05:15:41.000000 libmodi-20240305/libcdirectory/libcdirectory_directory_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      415 2024-03-05 05:38:52.342068 libmodi-20240305/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:16.000000 libmodi-20240507/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37507 2024-05-07 04:45:25.000000 libmodi-20240507/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-05-07 04:44:50.000000 libmodi-20240507/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2416 2024-05-07 04:45:48.000000 libmodi-20240507/libmodi.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:17.000000 libmodi-20240507/moditools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37173 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2987 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26443 2024-05-07 04:11:14.000000 libmodi-20240507/moditools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1934 2024-05-07 04:11:14.000000 libmodi-20240507/moditools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5414 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1406 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18958 2024-05-07 04:11:14.000000 libmodi-20240507/moditools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_libmodi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10552 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/byte_size_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1210 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2154 2024-05-07 04:19:22.000000 libmodi-20240507/moditools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20750 2024-05-07 04:11:14.000000 libmodi-20240507/moditools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9045 2024-05-07 04:11:14.000000 libmodi-20240507/moditools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5900 2024-05-07 04:11:14.000000 libmodi-20240507/moditools/modiinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3618 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1778 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2258 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15149 2024-05-07 04:11:14.000000 libmodi-20240507/moditools/modimount.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12659 2024-05-07 04:11:14.000000 libmodi-20240507/moditools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38337 2024-05-07 04:45:25.000000 libmodi-20240507/moditools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/byte_size_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3927 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-07 04:10:01.000000 libmodi-20240507/moditools/moditools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2762 2024-05-07 04:11:14.000000 libmodi-20240507/moditools/mount_fuse.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:17.000000 libmodi-20240507/libmodi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13950 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_sparse_image_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2331 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_udif_resource_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3856 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_bzip.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1390 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7911 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1812 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1072 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2907 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_block_chunks_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libfmos.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2264 2024-05-07 04:11:37.000000 libmodi-20240507/libmodi/libmodi_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12089 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_compression.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2786 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_udif_xml_plist.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2176 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_sparse_bundle_xml_plist.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3450 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/modi_udif_resource_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2103 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1445 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libfplist.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16103 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_data_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7546 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3324 2024-05-07 04:19:13.000000 libmodi-20240507/libmodi/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14786 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14983 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_sparse_bundle_xml_plist.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1070 2024-05-07 04:45:48.000000 libmodi-20240507/libmodi/libmodi.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_udif_block_table_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2649 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_data_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3338 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2243 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_udif_block_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1322 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_compression.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12981 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_block_chunks_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12500 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2169 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_sparse_image_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1940 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/modi_sparse_image_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2739 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_bands_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3457 2024-05-07 04:11:37.000000 libmodi-20240507/libmodi/libmodi_deflate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6394 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_udif_block_table_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1788 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20811 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_udif_xml_plist.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libcdirectory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   108282 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_huffman_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_i18n.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15475 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_udif_block_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3686 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48615 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_deflate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13493 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_udif_resource_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43361 2024-05-07 04:45:25.000000 libmodi-20240507/libmodi/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-05-07 04:45:47.000000 libmodi-20240507/libmodi/libmodi_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1892 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2937 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/modi_udif_block_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3706 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47348 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_bzip.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12487 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_bands_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-07 04:10:00.000000 libmodi-20240507/libmodi/libmodi_libcfile.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:17.000000 libmodi-20240507/libfmos/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2023 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_lzfse_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2269 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2964 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_lzfse_decoder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7799 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_adc.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3441 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_lzfse.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1321 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_adc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25840 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_lzvn.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6380 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_lzfse_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3271 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_lzfse_decoder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60280 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_lzfse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1326 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_lzvn.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-07 04:44:58.000000 libmodi-20240507/libfmos/libfmos_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35229 2024-05-07 04:45:25.000000 libmodi-20240507/libfmos/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-07 04:09:56.000000 libmodi-20240507/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-07 04:45:25.000000 libmodi-20240507/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 04:09:56.000000 libmodi-20240507/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-07 04:45:26.000000 libmodi-20240507/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:17.000000 libmodi-20240507/libfplist/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1401 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5928 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_xml_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1635 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6651 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_xml_scanner.l
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)  8431465 2024-05-07 04:46:43.000000 libmodi-20240507/libfplist/libfplist_xml_scanner.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56503 2024-05-07 04:46:44.000000 libmodi-20240507/libfplist/libfplist_xml_parser.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1492 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1788 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_xml_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12481 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_xml_parser.y
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4066 2024-05-07 04:46:44.000000 libmodi-20240507/libfplist/libfplist_xml_parser.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15149 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_property_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3419 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_property.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34608 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_property.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15574 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_xml_tag.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2497 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_property_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38097 2024-05-07 04:45:25.000000 libmodi-20240507/libfplist/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2894 2024-05-07 04:45:02.000000 libmodi-20240507/libfplist/libfplist_xml_tag.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:17.000000 libmodi-20240507/libcaes/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/libcaes_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2885 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/libcaes_tweaked_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4464 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/libcaes_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/libcaes_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82616 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/libcaes_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/libcaes_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      734 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/libcaes_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/libcaes_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/libcaes_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/libcaes_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/libcaes_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/libcaes_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33657 2024-05-07 04:45:25.000000 libmodi-20240507/libcaes/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33103 2024-05-07 04:44:09.000000 libmodi-20240507/libcaes/libcaes_tweaked_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:16.000000 libmodi-20240507/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-07 04:44:54.000000 libmodi-20240507/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-05-07 04:44:54.000000 libmodi-20240507/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-05-07 04:44:54.000000 libmodi-20240507/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-07 04:44:54.000000 libmodi-20240507/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-05-07 04:44:54.000000 libmodi-20240507/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-07 04:44:54.000000 libmodi-20240507/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-07 04:44:54.000000 libmodi-20240507/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-05-07 04:44:54.000000 libmodi-20240507/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-05-07 04:44:54.000000 libmodi-20240507/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-05-07 04:44:54.000000 libmodi-20240507/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-05-07 04:44:54.000000 libmodi-20240507/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33308 2024-05-07 04:45:25.000000 libmodi-20240507/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-07 04:44:54.000000 libmodi-20240507/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:15.000000 libmodi-20240507/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-07 04:10:02.000000 libmodi-20240507/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4659 2024-05-07 04:10:03.000000 libmodi-20240507/m4/libfmos.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:11:27.000000 libmodi-20240507/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-07 04:10:02.000000 libmodi-20240507/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:11:27.000000 libmodi-20240507/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:11:27.000000 libmodi-20240507/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-07 04:10:02.000000 libmodi-20240507/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:11:27.000000 libmodi-20240507/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:11:27.000000 libmodi-20240507/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-07 04:10:02.000000 libmodi-20240507/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-07 04:10:02.000000 libmodi-20240507/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-07 04:10:02.000000 libmodi-20240507/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-05-07 04:10:02.000000 libmodi-20240507/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-07 04:10:02.000000 libmodi-20240507/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-07 04:45:19.000000 libmodi-20240507/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-07 04:45:18.000000 libmodi-20240507/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-05-07 04:10:03.000000 libmodi-20240507/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:11:27.000000 libmodi-20240507/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-05-07 04:10:03.000000 libmodi-20240507/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-07 04:45:18.000000 libmodi-20240507/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:11:27.000000 libmodi-20240507/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-07 04:10:02.000000 libmodi-20240507/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-07 04:10:02.000000 libmodi-20240507/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-05-07 04:10:03.000000 libmodi-20240507/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-07 04:10:02.000000 libmodi-20240507/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3739 2023-12-03 09:11:27.000000 libmodi-20240507/m4/bzip2.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8550 2024-05-07 04:10:03.000000 libmodi-20240507/m4/libhmac.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:11:27.000000 libmodi-20240507/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-07 04:45:19.000000 libmodi-20240507/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:11:27.000000 libmodi-20240507/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:11:27.000000 libmodi-20240507/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-07 04:45:18.000000 libmodi-20240507/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:11:27.000000 libmodi-20240507/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-07 04:10:02.000000 libmodi-20240507/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27647 2024-05-07 04:10:02.000000 libmodi-20240507/m4/libcrypto.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-05-07 04:10:03.000000 libmodi-20240507/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8915 2024-05-07 04:10:02.000000 libmodi-20240507/m4/libcdirectory.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:11:27.000000 libmodi-20240507/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-05-07 04:10:03.000000 libmodi-20240507/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-05-07 04:10:02.000000 libmodi-20240507/m4/pthread.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6709 2024-05-07 04:10:03.000000 libmodi-20240507/m4/libfplist.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3671 2023-12-03 09:11:27.000000 libmodi-20240507/m4/lzma.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7819 2024-05-07 04:10:02.000000 libmodi-20240507/m4/zlib.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6500 2024-05-07 04:10:03.000000 libmodi-20240507/m4/libcaes.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:15.000000 libmodi-20240507/include/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:15.000000 libmodi-20240507/include/libmodi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1917 2024-05-07 04:09:59.000000 libmodi-20240507/include/libmodi/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1915 2024-05-07 04:45:47.000000 libmodi-20240507/include/libmodi/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4935 2024-05-07 04:09:59.000000 libmodi-20240507/include/libmodi/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4804 2024-05-07 04:45:47.000000 libmodi-20240507/include/libmodi/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-05-07 04:09:59.000000 libmodi-20240507/include/libmodi/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-05-07 04:09:59.000000 libmodi-20240507/include/libmodi/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-07 04:09:59.000000 libmodi-20240507/include/libmodi/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2024-05-07 04:45:47.000000 libmodi-20240507/include/libmodi/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-05-07 04:09:59.000000 libmodi-20240507/include/libmodi/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10784 2024-05-07 04:09:59.000000 libmodi-20240507/include/libmodi.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      410 2024-05-07 04:17:43.000000 libmodi-20240507/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10784 2024-05-07 04:45:47.000000 libmodi-20240507/include/libmodi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31665 2024-05-07 04:45:25.000000 libmodi-20240507/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:17.000000 libmodi-20240507/pymodi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_libmodi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33791 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3174 2024-05-07 04:11:14.000000 libmodi-20240507/pymodi/pymodi_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1851 2024-05-07 04:11:14.000000 libmodi-20240507/pymodi/pymodi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1114 2024-05-07 04:18:51.000000 libmodi-20240507/pymodi/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14118 2024-05-07 04:11:14.000000 libmodi-20240507/pymodi/pymodi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4080 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32818 2024-05-07 04:11:14.000000 libmodi-20240507/pymodi/pymodi_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4960 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_file_objects_io_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44900 2024-05-07 04:45:25.000000 libmodi-20240507/pymodi/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_file_objects_io_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-05-07 04:10:00.000000 libmodi-20240507/pymodi/pymodi_integer.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:15.000000 libmodi-20240507/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-07 04:09:58.000000 libmodi-20240507/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-07 04:09:58.000000 libmodi-20240507/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-07 04:09:58.000000 libmodi-20240507/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-07 04:09:58.000000 libmodi-20240507/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-07 04:09:58.000000 libmodi-20240507/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-07 04:09:58.000000 libmodi-20240507/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-07 04:09:58.000000 libmodi-20240507/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-07 04:17:43.000000 libmodi-20240507/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-07 04:09:58.000000 libmodi-20240507/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-05-07 04:45:47.000000 libmodi-20240507/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21161 2024-05-07 04:45:24.000000 libmodi-20240507/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22370 2024-05-07 04:45:48.000000 libmodi-20240507/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-07 04:09:58.000000 libmodi-20240507/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-07 04:09:58.000000 libmodi-20240507/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-07 04:09:58.000000 libmodi-20240507/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28718 2024-05-07 04:45:25.000000 libmodi-20240507/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:15.000000 libmodi-20240507/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-07 04:44:22.000000 libmodi-20240507/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-07 04:44:22.000000 libmodi-20240507/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-07 04:44:22.000000 libmodi-20240507/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-07 04:44:22.000000 libmodi-20240507/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-07 04:44:22.000000 libmodi-20240507/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-07 04:44:22.000000 libmodi-20240507/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-07 04:44:22.000000 libmodi-20240507/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-07 04:44:22.000000 libmodi-20240507/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-07 04:44:22.000000 libmodi-20240507/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-07 04:44:22.000000 libmodi-20240507/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33916 2024-05-07 04:45:25.000000 libmodi-20240507/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-07 04:44:22.000000 libmodi-20240507/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-07 04:44:22.000000 libmodi-20240507/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-07 04:44:22.000000 libmodi-20240507/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:16.000000 libmodi-20240507/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34425 2024-05-07 04:45:25.000000 libmodi-20240507/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-07 04:44:47.000000 libmodi-20240507/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-05-07 04:44:46.000000 libmodi-20240507/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2407 2024-05-07 04:19:52.000000 libmodi-20240507/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:16.000000 libmodi-20240507/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37768 2024-05-07 04:45:25.000000 libmodi-20240507/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-07 04:44:03.000000 libmodi-20240507/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:11:14.000000 libmodi-20240507/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-07 04:45:25.000000 libmodi-20240507/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:15.000000 libmodi-20240507/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-07 04:09:56.000000 libmodi-20240507/dpkg/libmodi.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-05-07 04:10:02.000000 libmodi-20240507/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-07 04:09:56.000000 libmodi-20240507/dpkg/libmodi-python3.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:15.000000 libmodi-20240507/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-07 04:09:56.000000 libmodi-20240507/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2066 2024-05-07 04:09:56.000000 libmodi-20240507/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      761 2024-05-07 04:09:56.000000 libmodi-20240507/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-07 04:09:56.000000 libmodi-20240507/dpkg/libmodi-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-05-07 04:09:56.000000 libmodi-20240507/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-05-07 04:45:47.000000 libmodi-20240507/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-07 04:09:56.000000 libmodi-20240507/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-07 04:09:56.000000 libmodi-20240507/dpkg/libmodi-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-05-07 04:45:48.000000 libmodi-20240507/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-07 04:09:56.000000 libmodi-20240507/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2218799 2024-05-07 04:45:23.000000 libmodi-20240507/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-07 04:45:25.000000 libmodi-20240507/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-07 04:45:25.000000 libmodi-20240507/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modimount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7486 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/modimount/modimount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_udif_block_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6242 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_udif_block_table/modi_test_udif_block_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_sparse_bundle_xml_plist/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6510 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_sparse_bundle_xml_plist/modi_test_sparse_bundle_xml_plist.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libmodi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11408 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libmodi/libmodi.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_bzip/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6130 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_bzip/modi_test_bzip.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libfmos/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5663 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libfmos/libfmos.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/zlib/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/zlib/zlib.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libfplist/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6237 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libfplist/libfplist.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libcaes/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4777 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libcaes/libcaes.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/pymodi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6196 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/pymodi/pymodi.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5966 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_error/modi_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2005 2024-05-07 04:18:42.000000 libmodi-20240507/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6221 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_io_handle/modi_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_system_string/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6073 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_system_string/modi_test_system_string.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_data_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6471 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_data_block/modi_test_data_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6052 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_notify/modi_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_udif_xml_plist/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6483 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_udif_xml_plist/modi_test_udif_xml_plist.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_udif_resource_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6495 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_udif_resource_file/modi_test_udif_resource_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_huffman_tree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6230 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_huffman_tree/modi_test_huffman_tree.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_bands_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6245 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_bands_data_handle/modi_test_bands_data_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6157 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_tools_signal/modi_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_sparse_image_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6498 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_sparse_image_header/modi_test_sparse_image_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6157 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_tools_output/modi_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_udif_block_table_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_udif_block_table_entry/modi_test_udif_block_table_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_deflate/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6299 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_deflate/modi_test_deflate.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7036 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_handle/modi_test_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6490 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_tools_info_handle/modi_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libcpath/libcpath.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42413 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/libmodi.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/bzip2/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4786 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/bzip2/bzip2.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7039 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_support/modi_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/libhmac/libhmac.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27713 2024-05-07 04:45:25.000000 libmodi-20240507/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7924 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modiinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6673 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/modiinfo/modiinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/modi_test_bit_stream/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6224 2024-05-07 04:11:08.000000 libmodi-20240507/msvscpp/modi_test_bit_stream/modi_test_bit_stream.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/msvscpp/libcdirectory/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5681 2024-05-07 04:10:30.000000 libmodi-20240507/msvscpp/libcdirectory/libcdirectory.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-07 04:09:58.000000 libmodi-20240507/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:16.000000 libmodi-20240507/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34749 2024-05-07 04:45:25.000000 libmodi-20240507/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-07 04:44:19.000000 libmodi-20240507/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      807 2024-05-07 04:09:56.000000 libmodi-20240507/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-07 04:45:25.000000 libmodi-20240507/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:15.000000 libmodi-20240507/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36662 2024-05-07 04:45:25.000000 libmodi-20240507/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-07 04:44:10.000000 libmodi-20240507/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-07 04:09:56.000000 libmodi-20240507/pyproject.toml
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6860 2024-05-07 04:45:25.000000 libmodi-20240507/ylwrap
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-05-07 04:09:56.000000 libmodi-20240507/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-07 04:45:25.000000 libmodi-20240507/config.sub
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-07 04:09:56.000000 libmodi-20240507/libmodi.pc.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-07 04:09:56.000000 libmodi-20240507/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-05-07 04:09:56.000000 libmodi-20240507/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:11:14.000000 libmodi-20240507/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:15.000000 libmodi-20240507/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37101 2024-05-07 04:45:25.000000 libmodi-20240507/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-07 04:44:42.000000 libmodi-20240507/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-07 04:45:26.000000 libmodi-20240507/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:16.000000 libmodi-20240507/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33947 2024-05-07 04:45:25.000000 libmodi-20240507/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-07 04:44:34.000000 libmodi-20240507/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2023-12-03 09:11:14.000000 libmodi-20240507/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5119 2024-05-07 04:11:37.000000 libmodi-20240507/manuals/libmodi.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      125 2024-05-07 04:18:35.000000 libmodi-20240507/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1226 2024-05-07 04:10:02.000000 libmodi-20240507/manuals/modiinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30677 2024-05-07 04:45:25.000000 libmodi-20240507/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2830 2024-05-07 04:11:08.000000 libmodi-20240507/tests/modi_test_bands_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7956 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66883 2024-05-07 04:11:08.000000 libmodi-20240507/tests/modi_test_udif_xml_plist.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16939 2024-05-07 04:11:08.000000 libmodi-20240507/tests/modi_test_udif_resource_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16001 2024-05-07 04:11:08.000000 libmodi-20240507/tests/modi_test_udif_block_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13247 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47609 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_bzip.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19021 2024-05-07 04:11:08.000000 libmodi-20240507/tests/modi_test_sparse_bundle_xml_plist.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4034 2024-05-07 04:13:48.000000 libmodi-20240507/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100206 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_deflate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9578 2024-05-07 04:18:25.000000 libmodi-20240507/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13622 2024-05-07 04:11:08.000000 libmodi-20240507/tests/modi_test_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_libcdirectory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1367 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40690 2024-05-07 04:11:08.000000 libmodi-20240507/tests/modi_test_sparse_image_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20021 2024-05-07 04:11:08.000000 libmodi-20240507/tests/modi_test_data_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9811 2024-05-07 04:11:08.000000 libmodi-20240507/tests/modi_test_udif_block_table_entry.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-07 04:10:02.000000 libmodi-20240507/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4405 2024-05-07 04:10:02.000000 libmodi-20240507/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_libmodi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11225 2024-05-07 04:11:14.000000 libmodi-20240507/tests/pymodi_test_handle.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-07 04:10:02.000000 libmodi-20240507/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3436 2024-05-07 04:11:14.000000 libmodi-20240507/tests/pymodi_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4123 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15900 2024-05-07 04:11:08.000000 libmodi-20240507/tests/modi_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30660 2024-05-07 04:11:08.000000 libmodi-20240507/tests/modi_test_huffman_tree.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3282 2024-05-07 04:10:02.000000 libmodi-20240507/tests/test_modiinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5590 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    75954 2024-05-07 04:45:26.000000 libmodi-20240507/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49072 2024-05-07 04:11:08.000000 libmodi-20240507/tests/modi_test_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2429 2024-05-07 04:11:08.000000 libmodi-20240507/tests/modi_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19103 2024-05-07 04:10:02.000000 libmodi-20240507/tests/modi_test_system_string.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4241 2024-05-07 04:13:30.000000 libmodi-20240507/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2223 2024-05-07 04:10:00.000000 libmodi-20240507/ossfuzz/handle_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      897 2024-05-07 04:17:56.000000 libmodi-20240507/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-07 04:10:00.000000 libmodi-20240507/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36023 2024-05-07 04:45:25.000000 libmodi-20240507/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-05-07 04:10:00.000000 libmodi-20240507/ossfuzz/ossfuzz_libmodi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-07 04:45:18.000000 libmodi-20240507/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:17.000000 libmodi-20240507/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha1_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha224.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha512_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_md5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_md5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha512.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha256_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha224.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha256_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1117 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha224_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_md5_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha1_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36812 2024-05-07 04:45:25.000000 libmodi-20240507/libhmac/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha224_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha512_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha512.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_sha1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-05-07 04:45:10.000000 libmodi-20240507/libhmac/libhmac_md5_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:16.000000 libmodi-20240507/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34844 2024-05-07 04:45:25.000000 libmodi-20240507/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-07 04:44:38.000000 libmodi-20240507/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:18.000000 libmodi-20240507/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:11:32.000000 libmodi-20240507/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:11:32.000000 libmodi-20240507/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:11:32.000000 libmodi-20240507/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:11:32.000000 libmodi-20240507/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:11:32.000000 libmodi-20240507/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:11:32.000000 libmodi-20240507/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:11:32.000000 libmodi-20240507/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:11:32.000000 libmodi-20240507/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:11:32.000000 libmodi-20240507/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-05-07 04:45:47.000000 libmodi-20240507/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:11:32.000000 libmodi-20240507/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:11:32.000000 libmodi-20240507/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:16.000000 libmodi-20240507/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60428 2024-05-07 04:45:25.000000 libmodi-20240507/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-07 04:45:13.000000 libmodi-20240507/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44951 2024-05-07 04:45:25.000000 libmodi-20240507/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:17.000000 libmodi-20240507/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39683 2024-05-07 04:45:25.000000 libmodi-20240507/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-07 04:45:06.000000 libmodi-20240507/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:15.000000 libmodi-20240507/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-07 04:44:26.000000 libmodi-20240507/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-07 04:44:26.000000 libmodi-20240507/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-07 04:44:26.000000 libmodi-20240507/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-07 04:44:26.000000 libmodi-20240507/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-07 04:44:26.000000 libmodi-20240507/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-07 04:44:26.000000 libmodi-20240507/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-07 04:44:26.000000 libmodi-20240507/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-07 04:44:26.000000 libmodi-20240507/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-07 04:44:26.000000 libmodi-20240507/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-07 04:44:26.000000 libmodi-20240507/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-07 04:44:26.000000 libmodi-20240507/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33785 2024-05-07 04:45:25.000000 libmodi-20240507/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-07 04:44:26.000000 libmodi-20240507/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-07 04:44:26.000000 libmodi-20240507/libcnotify/libcnotify_print.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3803 2024-05-07 04:16:45.000000 libmodi-20240507/libmodi.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:15.000000 libmodi-20240507/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-07 04:44:14.000000 libmodi-20240507/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-07 04:44:14.000000 libmodi-20240507/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-07 04:44:14.000000 libmodi-20240507/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-07 04:44:14.000000 libmodi-20240507/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-07 04:44:14.000000 libmodi-20240507/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-07 04:44:14.000000 libmodi-20240507/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-07 04:44:14.000000 libmodi-20240507/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-07 04:44:14.000000 libmodi-20240507/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-07 04:44:14.000000 libmodi-20240507/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-07 04:44:14.000000 libmodi-20240507/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-07 04:44:14.000000 libmodi-20240507/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33252 2024-05-07 04:45:25.000000 libmodi-20240507/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57077 2024-05-07 04:45:21.000000 libmodi-20240507/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9669 2024-05-07 04:15:19.000000 libmodi-20240507/configure.ac
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-07 05:20:16.000000 libmodi-20240507/libcdirectory/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21136 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_directory_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25660 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2886 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1046 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2396 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1809 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2980 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3347 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_directory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1975 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42170 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_directory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35459 2024-05-07 04:45:25.000000 libmodi-20240507/libcdirectory/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1910 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3214 2024-05-07 04:44:12.000000 libmodi-20240507/libcdirectory/libcdirectory_directory_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      415 2024-05-07 05:20:20.031093 libmodi-20240507/PKG-INFO
```

### Comparing `libmodi-20240305/libfdata/libfdata_error.h` & `libmodi-20240507/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_area.c` & `libmodi-20240507/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_stream.h` & `libmodi-20240507/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_cache.h` & `libmodi-20240507/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_range_list.c` & `libmodi-20240507/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_mapped_range.c` & `libmodi-20240507/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_libcerror.h` & `libmodi-20240507/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_definitions.h` & `libmodi-20240507/libfdata/libfdata_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFDATA )
 #include <libfdata/definitions.h>
 
 /* The definitions in <libfdata/definitions.h> are copied here
  * for local use of libfdata
  */
 #else
-#define LIBFDATA_VERSION						20240114
+#define LIBFDATA_VERSION						20240415
 
 /* The libfdata version string
  */
-#define LIBFDATA_VERSION_STRING						"20240114"
+#define LIBFDATA_VERSION_STRING						"20240415"
 
 /* The library flag definitions
  */
 enum LIBFDATA_FLAGS
 {
 	/* The data is not managed by the library
 	 */
```

### Comparing `libmodi-20240305/libfdata/libfdata_list.c` & `libmodi-20240507/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_libcdata.h` & `libmodi-20240507/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_list.h` & `libmodi-20240507/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_list_element.h` & `libmodi-20240507/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/Makefile.am` & `libmodi-20240507/libfdata/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBFCACHE_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -31,19 +31,17 @@
 	libfdata_stream.c libfdata_stream.h \
 	libfdata_support.c libfdata_support.h \
 	libfdata_types.h \
 	libfdata_unused.h \
 	libfdata_vector.c libfdata_vector.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
```

### Comparing `libmodi-20240305/libfdata/libfdata_libcnotify.h` & `libmodi-20240507/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_extern.h` & `libmodi-20240507/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_notify.c` & `libmodi-20240507/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_cache.c` & `libmodi-20240507/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_stream.c` & `libmodi-20240507/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_unused.h` & `libmodi-20240507/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_range.h` & `libmodi-20240507/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_area.h` & `libmodi-20240507/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_error.c` & `libmodi-20240507/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_support.h` & `libmodi-20240507/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_range.c` & `libmodi-20240507/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_mapped_range.h` & `libmodi-20240507/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_support.c` & `libmodi-20240507/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_list_element.c` & `libmodi-20240507/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_segments_array.c` & `libmodi-20240507/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_types.h` & `libmodi-20240507/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_notify.h` & `libmodi-20240507/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_range_list.h` & `libmodi-20240507/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_segments_array.h` & `libmodi-20240507/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/Makefile.in` & `libmodi-20240507/libfdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -548,14 +548,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -628,16 +630,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBFDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBFCACHE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -661,15 +663,16 @@
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_segments_array.c libfdata_segments_array.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_stream.c libfdata_stream.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_support.c libfdata_support.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_types.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_unused.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_vector.c libfdata_vector.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -881,24 +884,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdata_area.Plo
+	-rm -f ./$(DEPDIR)/libfdata_cache.Plo
+	-rm -f ./$(DEPDIR)/libfdata_error.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libfdata_mapped_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_notify.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_segments_array.Plo
+	-rm -f ./$(DEPDIR)/libfdata_stream.Plo
+	-rm -f ./$(DEPDIR)/libfdata_support.Plo
+	-rm -f ./$(DEPDIR)/libfdata_vector.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -994,17 +1012,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libfdata/libfdata_vector.c` & `libmodi-20240507/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_libfcache.h` & `libmodi-20240507/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfdata/libfdata_vector.h` & `libmodi-20240507/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi.spec` & `libmodi-20240507/libmodi.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libmodi
-Version: 20240305
+Version: 20240507
 Release: 1
 Summary: Library to access Mac OS disk image formats
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libmodi
 Requires: bzip2          openssl           xz-libs zlib
@@ -36,16 +36,16 @@
 
 %description -n libmodi-python3
 Python 3 bindings for libmodi
 
 %package -n libmodi-tools
 Summary: Several tools for reading Mac OS disk images
 Group: Applications/System
-Requires: libmodi = %{version}-%{release} fuse-libs
-BuildRequires: fuse-devel
+Requires: libmodi = %{version}-%{release} fuse3-libs
+BuildRequires: fuse3-devel
 
 %description -n libmodi-tools
 Several tools for reading Mac OS disk images
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libmodi-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Tue Mar  5 2024 Joachim Metz <joachim.metz@gmail.com> 20240305-1
+* Tue May  7 2024 Joachim Metz <joachim.metz@gmail.com> 20240507-1
 - Auto-generated
```

### Comparing `libmodi-20240305/moditools/mount_dokan.c` & `libmodi-20240507/moditools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/mount_file_system.h` & `libmodi-20240507/moditools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/mount_fuse.c` & `libmodi-20240507/moditools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/info_handle.h` & `libmodi-20240507/moditools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/mount_dokan.h` & `libmodi-20240507/moditools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_libcpath.h` & `libmodi-20240507/moditools/moditools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/mount_file_system.c` & `libmodi-20240507/moditools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_libmodi.h` & `libmodi-20240507/moditools/moditools_libmodi.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/byte_size_string.c` & `libmodi-20240507/moditools/byte_size_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_i18n.h` & `libmodi-20240507/moditools/moditools_i18n.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_libbfio.h` & `libmodi-20240507/moditools/moditools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_unused.h` & `libmodi-20240507/moditools/moditools_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_libcdata.h` & `libmodi-20240507/moditools/moditools_libcdata.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/Makefile.am` & `libmodi-20240507/moditools/Makefile.am`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -73,19 +73,17 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libmodi/libmodi.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on modiinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(modiinfo_SOURCES)
 	@echo "Running splint on modimount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(modimount_SOURCES)
```

### Comparing `libmodi-20240305/moditools/moditools_signal.h` & `libmodi-20240507/moditools/moditools_signal.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_libclocale.h` & `libmodi-20240507/moditools/moditools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/mount_file_entry.c` & `libmodi-20240507/moditools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/info_handle.c` & `libmodi-20240507/moditools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_getopt.h` & `libmodi-20240507/moditools/moditools_getopt.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/modiinfo.c` & `libmodi-20240507/moditools/modiinfo.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/mount_file_entry.h` & `libmodi-20240507/moditools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_libuna.h` & `libmodi-20240507/moditools/moditools_libuna.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_signal.c` & `libmodi-20240507/moditools/moditools_signal.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_getopt.c` & `libmodi-20240507/moditools/moditools_getopt.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/mount_handle.h` & `libmodi-20240507/moditools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_libcnotify.h` & `libmodi-20240507/moditools/moditools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_libcerror.h` & `libmodi-20240507/moditools/moditools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/modimount.c` & `libmodi-20240507/moditools/modimount.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/mount_handle.c` & `libmodi-20240507/moditools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/Makefile.in` & `libmodi-20240507/moditools/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -532,14 +532,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -612,16 +614,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -685,15 +687,16 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libmodi/libmodi.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -950,23 +953,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/byte_size_string.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/modiinfo.Po
+	-rm -f ./$(DEPDIR)/modimount.Po
+	-rm -f ./$(DEPDIR)/moditools_getopt.Po
+	-rm -f ./$(DEPDIR)/moditools_output.Po
+	-rm -f ./$(DEPDIR)/moditools_signal.Po
+	-rm -f ./$(DEPDIR)/mount_dokan.Po
+	-rm -f ./$(DEPDIR)/mount_file_entry.Po
+	-rm -f ./$(DEPDIR)/mount_file_system.Po
+	-rm -f ./$(DEPDIR)/mount_fuse.Po
+	-rm -f ./$(DEPDIR)/mount_handle.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1061,17 +1078,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on modiinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(modiinfo_SOURCES)
 	@echo "Running splint on modimount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(modimount_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/moditools/byte_size_string.h` & `libmodi-20240507/moditools/byte_size_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_output.c` & `libmodi-20240507/moditools/moditools_output.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/moditools_output.h` & `libmodi-20240507/moditools/moditools_output.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/moditools/mount_fuse.h` & `libmodi-20240507/moditools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_notify.c` & `libmodi-20240507/libmodi/libmodi_notify.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_sparse_image_header.c` & `libmodi-20240507/libmodi/libmodi_sparse_image_header.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_udif_resource_file.h` & `libmodi-20240507/libmodi/libmodi_udif_resource_file.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_bzip.h` & `libmodi-20240507/libmodi/libmodi_bzip.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_debug.h` & `libmodi-20240507/libmodi/libmodi_debug.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libfdata.h` & `libmodi-20240507/libmodi/libmodi_libfdata.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_bit_stream.c` & `libmodi-20240507/libmodi/libmodi_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi.c` & `libmodi-20240507/libmodi/libmodi.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi.rc.in` & `libmodi-20240507/libmodi/libmodi.rc.in`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_block_chunks_data_handle.h` & `libmodi-20240507/libmodi/libmodi_block_chunks_data_handle.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libfmos.h` & `libmodi-20240507/libmodi/libmodi_libfmos.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libcpath.h` & `libmodi-20240507/libmodi/libmodi_libcpath.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libcthreads.h` & `libmodi-20240507/libmodi/libmodi_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_bit_stream.h` & `libmodi-20240507/libmodi/libmodi_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_unused.h` & `libmodi-20240507/libmodi/libmodi_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_system_string.h` & `libmodi-20240507/libmodi/libmodi_system_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_notify.h` & `libmodi-20240507/libmodi/libmodi_notify.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_compression.c` & `libmodi-20240507/libmodi/libmodi_compression.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_udif_xml_plist.h` & `libmodi-20240507/libmodi/libmodi_udif_xml_plist.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libcdata.h` & `libmodi-20240507/libmodi/libmodi_libcdata.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libcnotify.h` & `libmodi-20240507/libmodi/libmodi_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_sparse_bundle_xml_plist.h` & `libmodi-20240507/libmodi/libmodi_sparse_bundle_xml_plist.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libcerror.h` & `libmodi-20240507/libmodi/libmodi_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_error.c` & `libmodi-20240507/libmodi/libmodi_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/modi_udif_resource_file.h` & `libmodi-20240507/libmodi/modi_udif_resource_file.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_support.h` & `libmodi-20240507/libmodi/libmodi_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libfplist.h` & `libmodi-20240507/libmodi/libmodi_libfplist.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_data_block.c` & `libmodi-20240507/libmodi/libmodi_data_block.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_handle.h` & `libmodi-20240507/libmodi/libmodi_handle.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_extern.h` & `libmodi-20240507/libmodi/libmodi_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_system_string.c` & `libmodi-20240507/libmodi/libmodi_system_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/Makefile.am` & `libmodi-20240507/libmodi/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -108,21 +108,19 @@
 libmodi_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libmodi_definitions.h.in \
 	libmodi.rc \
 	libmodi.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libmodi_definitions.h \
+	libmodi.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libmodi_definitions.h
-	-rm -f libmodi.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libmodi ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libmodi_la_SOURCES)
```

### Comparing `libmodi-20240305/libmodi/libmodi_support.c` & `libmodi-20240507/libmodi/libmodi_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_sparse_bundle_xml_plist.c` & `libmodi-20240507/libmodi/libmodi_sparse_bundle_xml_plist.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi.rc` & `libmodi-20240507/libmodi/libmodi.rc`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access Mac OS disk image formats\0"
-      VALUE "FileVersion",		"20240305" "\0"
+      VALUE "FileVersion",		"20240507" "\0"
       VALUE "InternalName",		"libmodi.dll\0"
       VALUE "LegalCopyright",		"(C) 2012-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libmodi.dll\0"
       VALUE "ProductName",		"libmodi\0"
-      VALUE "ProductVersion",		"20240305" "\0"
+      VALUE "ProductVersion",		"20240507" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libmodi/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libmodi-20240305/libmodi/libmodi_types.h` & `libmodi-20240507/libmodi/libmodi_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_udif_block_table_entry.h` & `libmodi-20240507/libmodi/libmodi_udif_block_table_entry.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libclocale.h` & `libmodi-20240507/libmodi/libmodi_libclocale.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_data_block.h` & `libmodi-20240507/libmodi/libmodi_data_block.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_definitions.h.in` & `libmodi-20240507/libmodi/libmodi_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_udif_block_table.h` & `libmodi-20240507/libmodi/libmodi_udif_block_table.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_compression.h` & `libmodi-20240507/libmodi/libmodi_compression.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_block_chunks_data_handle.c` & `libmodi-20240507/libmodi/libmodi_block_chunks_data_handle.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_huffman_tree.c` & `libmodi-20240507/libmodi/libmodi_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_sparse_image_header.h` & `libmodi-20240507/libmodi/libmodi_sparse_image_header.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/modi_sparse_image_header.h` & `libmodi-20240507/libmodi/modi_sparse_image_header.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_bands_data_handle.h` & `libmodi-20240507/libmodi/libmodi_bands_data_handle.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_deflate.h` & `libmodi-20240507/libmodi/libmodi_deflate.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_udif_block_table_entry.c` & `libmodi-20240507/libmodi/libmodi_udif_block_table_entry.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libfvalue.h` & `libmodi-20240507/libmodi/libmodi_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_error.h` & `libmodi-20240507/libmodi/libmodi_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_udif_xml_plist.c` & `libmodi-20240507/libmodi/libmodi_udif_xml_plist.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libfcache.h` & `libmodi-20240507/libmodi/libmodi_libfcache.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libcdirectory.h` & `libmodi-20240507/libmodi/libmodi_libcdirectory.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_handle.c` & `libmodi-20240507/libmodi/libmodi_handle.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_huffman_tree.h` & `libmodi-20240507/libmodi/libmodi_huffman_tree.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_i18n.h` & `libmodi-20240507/libmodi/libmodi_i18n.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_i18n.c` & `libmodi-20240507/libmodi/libmodi_i18n.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_udif_block_table.c` & `libmodi-20240507/libmodi/libmodi_udif_block_table.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_debug.c` & `libmodi-20240507/libmodi/libmodi_debug.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_deflate.c` & `libmodi-20240507/libmodi/libmodi_deflate.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libbfio.h` & `libmodi-20240507/libmodi/libmodi_libbfio.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_udif_resource_file.c` & `libmodi-20240507/libmodi/libmodi_udif_resource_file.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/Makefile.in` & `libmodi-20240507/libmodi/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -575,14 +575,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -656,16 +658,16 @@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -766,15 +768,18 @@
 
 libmodi_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libmodi_definitions.h.in \
 	libmodi.rc \
 	libmodi.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libmodi_definitions.h \
+	libmodi.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1027,24 +1032,49 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libmodi.Plo
+	-rm -f ./$(DEPDIR)/libmodi_bands_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libmodi_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libmodi_block_chunks_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libmodi_bzip.Plo
+	-rm -f ./$(DEPDIR)/libmodi_compression.Plo
+	-rm -f ./$(DEPDIR)/libmodi_data_block.Plo
+	-rm -f ./$(DEPDIR)/libmodi_debug.Plo
+	-rm -f ./$(DEPDIR)/libmodi_deflate.Plo
+	-rm -f ./$(DEPDIR)/libmodi_error.Plo
+	-rm -f ./$(DEPDIR)/libmodi_handle.Plo
+	-rm -f ./$(DEPDIR)/libmodi_huffman_tree.Plo
+	-rm -f ./$(DEPDIR)/libmodi_i18n.Plo
+	-rm -f ./$(DEPDIR)/libmodi_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libmodi_notify.Plo
+	-rm -f ./$(DEPDIR)/libmodi_sparse_bundle_xml_plist.Plo
+	-rm -f ./$(DEPDIR)/libmodi_sparse_image_header.Plo
+	-rm -f ./$(DEPDIR)/libmodi_support.Plo
+	-rm -f ./$(DEPDIR)/libmodi_system_string.Plo
+	-rm -f ./$(DEPDIR)/libmodi_udif_block_table.Plo
+	-rm -f ./$(DEPDIR)/libmodi_udif_block_table_entry.Plo
+	-rm -f ./$(DEPDIR)/libmodi_udif_resource_file.Plo
+	-rm -f ./$(DEPDIR)/libmodi_udif_xml_plist.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1150,19 +1180,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libmodi_definitions.h
-	-rm -f libmodi.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libmodi ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libmodi_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libmodi/libmodi_libuna.h` & `libmodi-20240507/libmodi/libmodi_libuna.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_codepage.h` & `libmodi-20240507/libmodi/libmodi_codepage.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_definitions.h` & `libmodi-20240507/libmodi/libmodi_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBMODI )
 #include <libmodi/definitions.h>
 
 /* The definitions in <libmodi/definitions.h> are copied here
  * for local use of libmodi
  */
 #else
-#define LIBMODI_VERSION						20240305
+#define LIBMODI_VERSION						20240507
 
 /* The version string
  */
-#define LIBMODI_VERSION_STRING					"20240305"
+#define LIBMODI_VERSION_STRING					"20240507"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBMODI_ACCESS_FLAGS
```

### Comparing `libmodi-20240305/libmodi/libmodi_io_handle.h` & `libmodi-20240507/libmodi/libmodi_io_handle.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/modi_udif_block_table.h` & `libmodi-20240507/libmodi/modi_udif_block_table.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_io_handle.c` & `libmodi-20240507/libmodi/libmodi_io_handle.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_bzip.c` & `libmodi-20240507/libmodi/libmodi_bzip.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_bands_data_handle.c` & `libmodi-20240507/libmodi/libmodi_bands_data_handle.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi/libmodi_libcfile.h` & `libmodi-20240507/libmodi/libmodi_libcfile.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_lzfse_bit_stream.h` & `libmodi-20240507/libfmos/libfmos_lzfse_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_definitions.h` & `libmodi-20240507/libfmos/libfmos_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfmos/definitions.h> are copied here
  * for local use of libfmos
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFMOS_VERSION					20240118
+#define LIBFMOS_VERSION					20240415
 
 /* The version string
  */
-#define LIBFMOS_VERSION_STRING				"20240118"
+#define LIBFMOS_VERSION_STRING				"20240415"
 
 #endif /* !defined( HAVE_LOCAL_LIBFMOS ) */
 
 #define LIBFMOS_LZFSE_NUMBER_OF_LITERAL_STATES		1024
 #define LIBFMOS_LZFSE_NUMBER_OF_LITERAL_SYMBOLS		256
 
 #define LIBFMOS_LZFSE_NUMBER_OF_L_VALUE_STATES		64
```

### Comparing `libmodi-20240305/libfmos/libfmos_lzfse_decoder.c` & `libmodi-20240507/libfmos/libfmos_lzfse_decoder.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_types.h` & `libmodi-20240507/libfmos/libfmos_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_adc.c` & `libmodi-20240507/libfmos/libfmos_adc.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_lzfse.h` & `libmodi-20240507/libfmos/libfmos_lzfse.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_notify.h` & `libmodi-20240507/libfmos/libfmos_notify.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_adc.h` & `libmodi-20240507/libfmos/libfmos_adc.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_support.c` & `libmodi-20240507/libfmos/libfmos_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_error.c` & `libmodi-20240507/libfmos/libfmos_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/Makefile.am` & `libmodi-20240507/libfmos/Makefile.am`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFMOS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfmos.la
 
@@ -22,19 +22,17 @@
 	libfmos_lzvn.c libfmos_lzvn.h \
 	libfmos_notify.c libfmos_notify.h \
 	libfmos_support.c libfmos_support.h \
 	libfmos_types.h \
 	libfmos_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfmos ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfmos_la_SOURCES)
```

### Comparing `libmodi-20240305/libfmos/libfmos_unused.h` & `libmodi-20240507/libfmos/libfmos_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_lzvn.c` & `libmodi-20240507/libfmos/libfmos_lzvn.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_libcnotify.h` & `libmodi-20240507/libfmos/libfmos_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_lzfse_bit_stream.c` & `libmodi-20240507/libfmos/libfmos_lzfse_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_lzfse_decoder.h` & `libmodi-20240507/libfmos/libfmos_lzfse_decoder.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_libcerror.h` & `libmodi-20240507/libfmos/libfmos_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_lzfse.c` & `libmodi-20240507/libfmos/libfmos_lzfse.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_notify.c` & `libmodi-20240507/libfmos/libfmos_notify.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_error.h` & `libmodi-20240507/libfmos/libfmos_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_support.h` & `libmodi-20240507/libfmos/libfmos_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_lzvn.h` & `libmodi-20240507/libfmos/libfmos_lzvn.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/libfmos_extern.h` & `libmodi-20240507/libfmos/libfmos_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfmos/Makefile.in` & `libmodi-20240507/libfmos/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -533,14 +533,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -613,16 +615,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBFMOS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFMOS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFMOS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFMOS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFMOS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFMOS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMOS_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMOS_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMOS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFMOS_TRUE@noinst_LTLIBRARIES = libfmos.la
 @HAVE_LOCAL_LIBFMOS_TRUE@libfmos_la_SOURCES = \
@@ -637,15 +639,16 @@
 @HAVE_LOCAL_LIBFMOS_TRUE@	libfmos_lzfse_decoder.c libfmos_lzfse_decoder.h \
 @HAVE_LOCAL_LIBFMOS_TRUE@	libfmos_lzvn.c libfmos_lzvn.h \
 @HAVE_LOCAL_LIBFMOS_TRUE@	libfmos_notify.c libfmos_notify.h \
 @HAVE_LOCAL_LIBFMOS_TRUE@	libfmos_support.c libfmos_support.h \
 @HAVE_LOCAL_LIBFMOS_TRUE@	libfmos_types.h \
 @HAVE_LOCAL_LIBFMOS_TRUE@	libfmos_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -852,24 +855,34 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfmos_adc.Plo
+	-rm -f ./$(DEPDIR)/libfmos_error.Plo
+	-rm -f ./$(DEPDIR)/libfmos_lzfse.Plo
+	-rm -f ./$(DEPDIR)/libfmos_lzfse_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libfmos_lzfse_decoder.Plo
+	-rm -f ./$(DEPDIR)/libfmos_lzvn.Plo
+	-rm -f ./$(DEPDIR)/libfmos_notify.Plo
+	-rm -f ./$(DEPDIR)/libfmos_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -960,17 +973,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfmos ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfmos_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/COPYING` & `libmodi-20240507/COPYING`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/install-sh` & `libmodi-20240507/install-sh`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/depcomp` & `libmodi-20240507/depcomp`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_libfguid.h` & `libmodi-20240507/libfplist/libfplist_libfguid.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_libuna.h` & `libmodi-20240507/libfplist/libfplist_libuna.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_xml_attribute.c` & `libmodi-20240507/libfplist/libfplist_xml_attribute.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_types.h` & `libmodi-20240507/libfplist/libfplist_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_xml_scanner.l` & `libmodi-20240507/libfplist/libfplist_xml_scanner.l`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_support.h` & `libmodi-20240507/libfplist/libfplist_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_xml_scanner.c` & `libmodi-20240507/libfplist/libfplist_xml_scanner.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_xml_parser.c` & `libmodi-20240507/libfplist/libfplist_xml_parser.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/Makefile.am` & `libmodi-20240507/libfplist/Makefile.am`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 AM_LFLAGS = -Cf
 AM_YFLAGS = -d -v -l -p libfplist_xml_scanner_
 
 if HAVE_LOCAL_LIBFPLIST
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
 	@LIBFVALUE_CPPFLAGS@ 
 
@@ -40,23 +40,21 @@
 	libfplist_xml_tag.c libfplist_xml_tag.h
 endif
 
 EXTRA_DIST = \
 	libfplist_xml_parser.c libfplist_xml_parser.h \
 	libfplist_xml_scanner.c
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfplist_xml_parser.c \
+	libfplist_xml_parser.h \
+	libfplist_xml_parser.output \
+	libfplist_xml_scanner.c \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libfplist_xml_parser.c
-	-rm -f libfplist_xml_parser.h
-	-rm -f libfplist_xml_parser.output
-	-rm -f libfplist_xml_scanner.c
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfplist ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfplist_la_SOURCES)
```

### Comparing `libmodi-20240305/libfplist/libfplist_unused.h` & `libmodi-20240507/libfplist/libfplist_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_error.h` & `libmodi-20240507/libfplist/libfplist_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_definitions.h` & `libmodi-20240507/libfplist/libfplist_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfplist/definitions.h> are copied here
  * for local use of libfplist
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFPLIST_VERSION			20240120
+#define LIBFPLIST_VERSION			20240415
 
 /* The version string
  */
-#define LIBFPLIST_VERSION_STRING		"20240120"
+#define LIBFPLIST_VERSION_STRING		"20240415"
 
 enum LIBFPLIST_VALUE_TYPES
 {
 	LIBFPLIST_VALUE_TYPE_UNKNOWN		= 0,
 	LIBFPLIST_VALUE_TYPE_ARRAY		= 1,
 	LIBFPLIST_VALUE_TYPE_BINARY_DATA	= 2,
 	LIBFPLIST_VALUE_TYPE_BOOLEAN		= 3,
```

### Comparing `libmodi-20240305/libfplist/libfplist_xml_attribute.h` & `libmodi-20240507/libfplist/libfplist_xml_attribute.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_libcdata.h` & `libmodi-20240507/libfplist/libfplist_libcdata.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_error.c` & `libmodi-20240507/libfplist/libfplist_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_libcnotify.h` & `libmodi-20240507/libfplist/libfplist_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_libcerror.h` & `libmodi-20240507/libfplist/libfplist_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_support.c` & `libmodi-20240507/libfplist/libfplist_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_xml_parser.y` & `libmodi-20240507/libfplist/libfplist_xml_parser.y`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_xml_parser.h` & `libmodi-20240507/libfplist/libfplist_xml_parser.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_property_list.c` & `libmodi-20240507/libfplist/libfplist_property_list.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_property.h` & `libmodi-20240507/libfplist/libfplist_property.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_property.c` & `libmodi-20240507/libfplist/libfplist_property.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_xml_tag.c` & `libmodi-20240507/libfplist/libfplist_xml_tag.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_property_list.h` & `libmodi-20240507/libfplist/libfplist_property_list.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_extern.h` & `libmodi-20240507/libfplist/libfplist_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/libfplist_libfvalue.h` & `libmodi-20240507/libfplist/libfplist_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfplist/Makefile.in` & `libmodi-20240507/libfplist/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -560,14 +560,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -642,16 +644,16 @@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 AM_LFLAGS = -Cf
 AM_YFLAGS = -d -v -l -p libfplist_xml_scanner_
 @HAVE_LOCAL_LIBFPLIST_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFPLIST_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFPLIST_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFPLIST_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFPLIST_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	@LIBFGUID_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	@LIBFVALUE_CPPFLAGS@ 
 
@@ -681,15 +683,20 @@
 @HAVE_LOCAL_LIBFPLIST_TRUE@	libfplist_xml_scanner.l \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	libfplist_xml_tag.c libfplist_xml_tag.h
 
 EXTRA_DIST = \
 	libfplist_xml_parser.c libfplist_xml_parser.h \
 	libfplist_xml_scanner.c
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfplist_xml_parser.c \
+	libfplist_xml_parser.h \
+	libfplist_xml_parser.output \
+	libfplist_xml_scanner.c \
+	Makefile \
 	Makefile.in
 
 all: $(BUILT_SOURCES)
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .l .lo .o .obj .y
@@ -909,28 +916,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
 	-rm -f libfplist_xml_parser.c
 	-rm -f libfplist_xml_parser.h
 	-rm -f libfplist_xml_scanner.c
 	-test -z "$(BUILT_SOURCES)" || rm -f $(BUILT_SOURCES)
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfplist_error.Plo
+	-rm -f ./$(DEPDIR)/libfplist_property.Plo
+	-rm -f ./$(DEPDIR)/libfplist_property_list.Plo
+	-rm -f ./$(DEPDIR)/libfplist_support.Plo
+	-rm -f ./$(DEPDIR)/libfplist_xml_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfplist_xml_parser.Plo
+	-rm -f ./$(DEPDIR)/libfplist_xml_scanner.Plo
+	-rm -f ./$(DEPDIR)/libfplist_xml_tag.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1021,21 +1038,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfplist_xml_parser.c
-	-rm -f libfplist_xml_parser.h
-	-rm -f libfplist_xml_parser.output
-	-rm -f libfplist_xml_scanner.c
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfplist ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfplist_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libfplist/libfplist_xml_tag.h` & `libmodi-20240507/libfplist/libfplist_xml_tag.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcaes/libcaes_unused.h` & `libmodi-20240507/libcaes/libcaes_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcaes/libcaes_tweaked_context.h` & `libmodi-20240507/libcaes/libcaes_tweaked_context.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcaes/libcaes_context.h` & `libmodi-20240507/libcaes/libcaes_context.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcaes/libcaes_error.c` & `libmodi-20240507/libcaes/libcaes_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcaes/libcaes_context.c` & `libmodi-20240507/libcaes/libcaes_context.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcaes/libcaes_definitions.h` & `libmodi-20240507/libcaes/libcaes_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBCAES )
 #include <libcaes/definitions.h>
 
 /* The definitions in <libcaes/definitions.h> are copied here
  * for local use of libcaes
  */
 #else
-#define LIBCAES_VERSION				20240114
+#define LIBCAES_VERSION				20240413
 
 /* The libcaes version string
  */
-#define LIBCAES_VERSION_STRING			"20240114"
+#define LIBCAES_VERSION_STRING			"20240413"
 
 /* The crypt modes
  */
 enum LIBCAES_CRYPT_MODES
 {
 	LIBCAES_CRYPT_MODE_DECRYPT		= 0,
 	LIBCAES_CRYPT_MODE_ENCRYPT		= 1
```

### Comparing `libmodi-20240305/libcaes/Makefile.am` & `libmodi-20240507/libcaes/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 if HAVE_LOCAL_LIBCAES
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
-	@LIBCERROR_CPPFLAGS@ 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
+	@LIBCERROR_CPPFLAGS@ \
+	@LIBCRYPTO_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcaes.la
 
 libcaes_la_SOURCES = \
 	libcaes_context.c libcaes_context.h \
 	libcaes_definitions.h \
 	libcaes_extern.h \
@@ -14,19 +15,17 @@
 	libcaes_libcerror.h \
 	libcaes_support.c libcaes_support.h \
 	libcaes_tweaked_context.c libcaes_tweaked_context.h \
 	libcaes_types.h \
 	libcaes_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcaes ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcaes_la_SOURCES)
```

### Comparing `libmodi-20240305/libcaes/libcaes_error.h` & `libmodi-20240507/libcaes/libcaes_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcaes/libcaes_types.h` & `libmodi-20240507/libcaes/libcaes_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcaes/libcaes_extern.h` & `libmodi-20240507/libcaes/libcaes_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcaes/libcaes_support.h` & `libmodi-20240507/libcaes/libcaes_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcaes/libcaes_libcerror.h` & `libmodi-20240507/libcaes/libcaes_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcaes/libcaes_support.c` & `libmodi-20240507/libcaes/libcaes_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcaes/Makefile.in` & `libmodi-20240507/libcaes/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -524,14 +524,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -604,31 +606,33 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCAES_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCAES_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCAES_TRUE@	-I$(top_srcdir)/common \
-@HAVE_LOCAL_LIBCAES_TRUE@	@LIBCERROR_CPPFLAGS@ 
+@HAVE_LOCAL_LIBCAES_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCAES_TRUE@	-I../common -I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCAES_TRUE@	@LIBCERROR_CPPFLAGS@ \
+@HAVE_LOCAL_LIBCAES_TRUE@	@LIBCRYPTO_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCAES_TRUE@noinst_LTLIBRARIES = libcaes.la
 @HAVE_LOCAL_LIBCAES_TRUE@libcaes_la_SOURCES = \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_context.c libcaes_context.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_definitions.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_extern.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_error.c libcaes_error.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_libcerror.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_support.c libcaes_support.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_tweaked_context.c libcaes_tweaked_context.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_types.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -831,24 +835,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcaes_context.Plo
+	-rm -f ./$(DEPDIR)/libcaes_error.Plo
+	-rm -f ./$(DEPDIR)/libcaes_support.Plo
+	-rm -f ./$(DEPDIR)/libcaes_tweaked_context.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -935,17 +945,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcaes ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcaes_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libcaes/libcaes_tweaked_context.c` & `libmodi-20240507/libcaes/libcaes_tweaked_context.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfguid/libfguid_error.c` & `libmodi-20240507/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfguid/libfguid_support.h` & `libmodi-20240507/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfguid/libfguid_identifier.h` & `libmodi-20240507/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfguid/libfguid_libcerror.h` & `libmodi-20240507/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfguid/Makefile.am` & `libmodi-20240507/libfguid/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFGUID
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfguid.la
 
 libfguid_la_SOURCES = \
 	libfguid_definitions.h \
 	libfguid_extern.h \
@@ -13,19 +13,17 @@
 	libfguid_libcerror.h \
 	libfguid_identifier.c libfguid_identifier.h \
 	libfguid_support.c libfguid_support.h \
 	libfguid_types.h \
 	libfguid_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
```

### Comparing `libmodi-20240305/libfguid/libfguid_unused.h` & `libmodi-20240507/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfguid/libfguid_extern.h` & `libmodi-20240507/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfguid/libfguid_types.h` & `libmodi-20240507/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfguid/libfguid_identifier.c` & `libmodi-20240507/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfguid/libfguid_support.c` & `libmodi-20240507/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfguid/libfguid_definitions.h` & `libmodi-20240507/libfguid/libfguid_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfguid/definitions.h> are copied here
  * for local use of libfguid
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFGUID_VERSION					20240116
+#define LIBFGUID_VERSION					20240415
 
 /* The version string
  */
-#define LIBFGUID_VERSION_STRING					"20240116"
+#define LIBFGUID_VERSION_STRING					"20240415"
 
 /* The byte order definitions
  */
 #define LIBFGUID_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFGUID_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The GUID identifier version definitions
```

### Comparing `libmodi-20240305/libfguid/Makefile.in` & `libmodi-20240507/libfguid/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -524,14 +524,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -604,30 +606,31 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBFGUID_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFGUID_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFGUID_TRUE@noinst_LTLIBRARIES = libfguid.la
 @HAVE_LOCAL_LIBFGUID_TRUE@libfguid_la_SOURCES = \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_definitions.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_extern.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_error.c libfguid_error.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_libcerror.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_identifier.c libfguid_identifier.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_support.c libfguid_support.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_types.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -829,24 +832,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfguid_error.Plo
+	-rm -f ./$(DEPDIR)/libfguid_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfguid_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -932,17 +940,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libfguid/libfguid_error.h` & `libmodi-20240507/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/libcfile.m4` & `libmodi-20240507/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/libfmos.m4` & `libmodi-20240507/m4/libfmos.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfmos required headers and functions
 dnl
-dnl Version: 20220804
+dnl Version: 20240413
 
 dnl Function to detect if libfmos is available
 dnl ac_libfmos_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFMOS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfmos" = xno],
     [ac_cv_libfmos=no],
     [ac_cv_libfmos=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfmos which returns "yes" and --with-libfmos= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect],
+      [test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect && test "x$ac_cv_with_libfmos" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfmos"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfmos}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfmos}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfmos],
           [1])
@@ -72,16 +74,17 @@
           fmos,
           libfmos_lzvn_decompress,
           [ac_cv_libfmos_dummy=yes],
           [ac_cv_libfmos=no])
 
         ac_cv_libfmos_LIBADD="-lfmos"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect && test "x$ac_cv_libfmos" != xyes],
+      [test "x$ac_cv_libfmos" != xyes && test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect && test "x$ac_cv_with_libfmos" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfmos in directory: $ac_cv_with_libfmos],
         [1])
       ])
     ])
 
   AS_IF(
@@ -103,15 +106,15 @@
     ])
   ])
 
 dnl Function to detect if libfmos dependencies are available
 AC_DEFUN([AX_LIBFMOS_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfmos_CPPFLAGS="-I../libfmos";
+  ac_cv_libfmos_CPPFLAGS="-I../libfmos -I\$(top_srcdir)/libfmos";
   ac_cv_libfmos_LIBADD="../libfmos/libfmos.la";
 
   ac_cv_libfmos=local
   ])
 
 dnl Function to detect how to enable libfmos
 AC_DEFUN([AX_LIBFMOS_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/tests.m4` & `libmodi-20240507/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/libcpath.m4` & `libmodi-20240507/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/lib-prefix.m4` & `libmodi-20240507/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/progtest.m4` & `libmodi-20240507/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/libuna.m4` & `libmodi-20240507/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/gettext.m4` & `libmodi-20240507/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/lib-ld.m4` & `libmodi-20240507/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/libclocale.m4` & `libmodi-20240507/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/libcdata.m4` & `libmodi-20240507/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/libcsplit.m4` & `libmodi-20240507/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/common.m4` & `libmodi-20240507/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libmodi-20240305/m4/libcthreads.m4` & `libmodi-20240507/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libmodi-20240305/m4/ltversion.m4` & `libmodi-20240507/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/ltsugar.m4` & `libmodi-20240507/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/libfdata.m4` & `libmodi-20240507/m4/libfdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Functions for libfdata
 dnl
-dnl Version: 20230318
+dnl Version: 20240413
 
 dnl Function to detect if libfdata is available
 dnl ac_libfdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno],
     [ac_cv_libfdata=no],
     [ac_cv_libfdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdata which returns "yes" and --with-libfdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect],
+      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdata],
           [1])
@@ -450,16 +452,17 @@
         dnl TODO: add functions
 
         dnl Vector list functions
         dnl TODO: add functions
 
         ac_cv_libfdata_LIBADD="-lfdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes],
+      [test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdata in directory: $ac_cv_with_libfdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -481,15 +484,15 @@
     ])
   ])
 
 dnl Function to detect if libfdata dependencies are available
 AC_DEFUN([AX_LIBFDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
   ])
 
 dnl Function to detect how to enable libfdata
 AC_DEFUN([AX_LIBFDATA_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/host-cpu-c-abi.m4` & `libmodi-20240507/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/libfuse.m4` & `libmodi-20240507/m4/libfuse.m4`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 dnl Checks for libfuse required headers and functions
 dnl
-dnl Version: 20220118
+dnl Version: 20240413
 
 dnl Function to detect if libfuse is available
 dnl ac_libfuse_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFUSE_CHECK_LIB],
-  [dnl Check if parameters were provided
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect],
-    [AS_IF(
-      [test -d "$ac_cv_with_libfuse"],
-      [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
-      [AC_MSG_WARN([no such directory: $ac_cv_with_libfuse])
-      ])
-    ])
-
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" = xno],
+  [AS_IF(
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno],
     [ac_cv_libfuse=no],
-    [dnl Check for a pkg-config file
+    [dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfuse which returns "yes" and --with-libfuse= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
-      [PKG_CHECK_MODULES(
-        [fuse],
-        [fuse >= 2.6],
-        [ac_cv_libfuse=libfuse],
-        [ac_cv_libfuse=no])
+      [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_libfuse"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
+        [AC_MSG_FAILURE(
+          [no such directory: $ac_cv_with_libfuse],
+          [1])
+        ])],
+      [dnl Check for a pkg-config file
+      AS_IF(
+        [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
+        [PKG_CHECK_MODULES(
+          [fuse3],
+          [fuse3 >= 3.0],
+          [ac_cv_libfuse=libfuse3],
+          [ac_cv_libfuse=no])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xno],
+          [PKG_CHECK_MODULES(
+            [fuse],
+            [fuse >= 2.6],
+            [ac_cv_libfuse=libfuse],
+            [ac_cv_libfuse=no])
+          ])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"])
+        ])
       ])
 
+    backup_CPPFLAGS="$CPPFLAGS"
+
+    dnl Check for libfuse and libfuse3
     AS_IF(
-      [test "x$ac_cv_libfuse" = xlibfuse],
-      [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"],
+      [test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3],
       [dnl Check for headers
-      AC_CHECK_HEADERS(
-        [fuse.h],
-        [ac_cv_header_fuse_h=yes],
-        [ac_cv_header_fuse_h=no])
 
-      dnl libfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      dnl macFuse requires -DFUSE_USE_VERSION=26 to be set
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      AC_CHECK_HEADERS([fuse.h])
+
       AS_IF(
-        [test "x$ac_cv_header_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+        [test "x$ac_cv_header_fuse_h" = xyes],
+        [ac_cv_libfuse=libfuse3],
+        [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         AC_CHECK_HEADERS([fuse.h])
-      ])
+
+        AS_IF(
+          [test "x$ac_cv_header_fuse_h" = xyes],
+          [ac_cv_libfuse=libfuse])
+        ])
 
       AS_IF(
         [test "x$ac_cv_header_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
-        ac_cv_libfuse=libfuse
+        AC_CHECK_LIB(
+          fuse,
+          fuse_invalidate,
+          [ac_cv_libfuse=libfuse],
+          [ac_cv_libfuse=libfuse3])
 
         AC_CHECK_LIB(
           fuse,
           fuse_daemonize,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
@@ -71,32 +99,30 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           fuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+        dnl libfuse and libfuse3 require -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_LIBADD="-lfuse3"],
+          [ac_cv_libfuse_LIBADD="-lfuse"])
         ])
       ])
 
     dnl Check for libosxfuse
     AS_IF(
       [test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno],
-      [CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
+      [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
       AC_CHECK_HEADERS([osxfuse/fuse.h])
 
-      dnl libosxfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      AS_IF(
-        [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_osxfuse_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        AC_CHECK_HEADERS([osxfuse/fuse.h])
-      ])
-
       AS_IF(
         [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
         ac_cv_libfuse=libosxfuse
 
         AC_CHECK_LIB(
@@ -116,27 +142,46 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           osxfuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
+        dnl libosxfuse requires -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported libfuse in directory: $ac_cv_with_libfuse],
+        [1])
+      ])
+
+    CPPFLAGS="$backup_CPPFLAGS"
     ])
 
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_DEFINE(
       [HAVE_LIBFUSE],
       [1],
       [Define to 1 if you have the 'fuse' library (-lfuse).])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_DEFINE(
+      [HAVE_LIBFUSE3],
+      [1],
+      [Define to 1 if you have the 'fuse3' library (-lfuse3).])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_DEFINE(
       [HAVE_LIBOSXFUSE],
       [1],
       [Define to 1 if you have the 'osxfuse' library (-losxfuse).])
     ])
 
@@ -179,14 +224,20 @@
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-lfuse])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_pc_libs_private],
+      [-lfuse3])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-losxfuse])
     ])
 
   AS_IF(
@@ -194,9 +245,18 @@
     [AC_SUBST(
       [ax_libfuse_spec_requires],
       [fuse-libs])
     AC_SUBST(
       [ax_libfuse_spec_build_requires],
       [fuse-devel])
     ])
+  AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_spec_requires],
+      [fuse3-libs])
+    AC_SUBST(
+      [ax_libfuse_spec_build_requires],
+      [fuse3-devel])
+    ])
   ])
```

### Comparing `libmodi-20240305/m4/libtool.m4` & `libmodi-20240507/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/po.m4` & `libmodi-20240507/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/libcerror.m4` & `libmodi-20240507/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/libcnotify.m4` & `libmodi-20240507/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/libfguid.m4` & `libmodi-20240507/m4/libfguid.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfguid required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfguid is available
 dnl ac_libfguid_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFGUID_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno],
     [ac_cv_libfguid=no],
     [ac_cv_libfguid=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfguid which returns "yes" and --with-libfguid= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect],
+      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfguid"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfguid],
           [1])
@@ -103,16 +105,17 @@
           fguid,
           libfguid_identifier_copy_to_utf32_string_with_index,
           [ac_cv_libfguid_dummy=yes],
           [ac_cv_libfguid=no])
 
         ac_cv_libfguid_LIBADD="-lfguid"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes],
+      [test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfguid in directory: $ac_cv_with_libfguid],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
     ])
   ])
 
 dnl Function to detect if libfguid dependencies are available
 AC_DEFUN([AX_LIBFGUID_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
   ])
 
 
 dnl Function to detect how to enable libfguid
```

### Comparing `libmodi-20240305/m4/libbfio.m4` & `libmodi-20240507/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/bzip2.m4` & `libmodi-20240507/m4/bzip2.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/libhmac.m4` & `libmodi-20240507/m4/libhmac.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libhmac required headers and functions
 dnl
-dnl Version: 20200104
+dnl Version: 20240413
 
 dnl Function to detect if libhmac is available
 dnl ac_libhmac_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBHMAC_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libhmac" = xno],
     [ac_cv_libhmac=no],
     [ac_cv_libhmac=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libhmac which returns "yes" and --with-libhmac= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect],
+      [test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libhmac"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libhmac}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libhmac}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libhmac],
           [1])
@@ -161,16 +163,17 @@
           hmac,
           libhmac_sha512_free,
           [ac_cv_libhmac_dummy=yes],
           [ac_cv_libhmac=no])
 
         ac_cv_libhmac_LIBADD="-lhmac"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_libhmac" != xyes],
+      [test "x$ac_cv_libhmac" != xyes && test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libhmac in directory: $ac_cv_with_libhmac],
         [1])
       ])
     ])
 
   AS_IF(
@@ -240,15 +243,15 @@
     [ac_cv_libhmac_sha256=$ac_cv_libcrypto_sha256])
 
   AS_IF(
     [test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_sha512" = xno],
     [ac_cv_libhmac_sha512=local],
     [ac_cv_libhmac_sha512=$ac_cv_libcrypto_sha512])
 
-  ac_cv_libhmac_CPPFLAGS="-I../libhmac";
+  ac_cv_libhmac_CPPFLAGS="-I../libhmac -I\$(top_srcdir)/libhmac";
   ac_cv_libhmac_LIBADD="../libhmac/libhmac.la";
 
   ac_cv_libhmac=local
   ])
 
 dnl Function to detect how to enable libhmac
 AC_DEFUN([AX_LIBHMAC_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/intlmacosx.m4` & `libmodi-20240507/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/lt~obsolete.m4` & `libmodi-20240507/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/lib-link.m4` & `libmodi-20240507/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/iconv.m4` & `libmodi-20240507/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/ltoptions.m4` & `libmodi-20240507/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/nls.m4` & `libmodi-20240507/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/python.m4` & `libmodi-20240507/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libmodi-20240305/m4/libcrypto.m4` & `libmodi-20240507/m4/libcrypto.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcrypto required headers and functions
 dnl
-dnl Version: 20231007
+dnl Version: 20240308
 
 dnl Function to detect whether openssl/evp.h can be used in combination with zlib.h
 AC_DEFUN([AX_LIBCRYPTO_CHECK_OPENSSL_EVP_ZLIB_COMPATIBILE],
   [AC_CACHE_CHECK(
     [if openssl/evp.h can be used in combination with zlib.h],
     [ac_cv_openssl_evp_zlib_compatible],
     [AC_LANG_PUSH(C)
@@ -619,16 +619,18 @@
 
 dnl Function to detect if libcrypto (openssl) dependencies are available
 AC_DEFUN([AX_LIBCRYPTO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno],
     [ac_cv_libcrypto=no],
     [dnl Check if the directory provided as parameter exists
+    dnl For both --with-openssl which returns "yes" and --with-openssl= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect],
+      [test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_openssl"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_openssl],
           [1])
```

### Comparing `libmodi-20240305/m4/libfvalue.m4` & `libmodi-20240507/m4/libfvalue.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfvalue required headers and functions
 dnl
-dnl Version: 20200711
+dnl Version: 20240413
 
 dnl Function to detect if libfvalue is available
 dnl ac_libfvalue_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFVALUE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno],
     [ac_cv_libfvalue=no],
     [ac_cv_libfvalue=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfvalue which returns "yes" and --with-libfvalue= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect],
+      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfvalue"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfvalue],
           [1])
@@ -585,16 +587,17 @@
           fvalue,
           libfvalue_value_type_set_data_strings_array,
           [ac_cv_libfvalue_dummy=yes],
           [ac_cv_libfvalue=no])
 
         ac_cv_libfvalue_LIBADD="-lfvalue"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes],
+      [test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfvalue in directory: $ac_cv_with_libfvalue],
         [1])
       ])
     ])
 
   AS_IF(
@@ -616,15 +619,15 @@
     ])
   ])
 
 dnl Function to detect if libfvalue dependencies are available
 AC_DEFUN([AX_LIBFVALUE_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
   ])
 
 dnl Function to detect how to enable libfvalue
 AC_DEFUN([AX_LIBFVALUE_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/libcdirectory.m4` & `libmodi-20240507/m4/libcdirectory.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdirectory required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcdirectory is available
 dnl ac_libcdirectory_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDIRECTORY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdirectory" = xno],
     [ac_cv_libcdirectory=no],
     [ac_cv_libcdirectory=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdirectory which returns "yes" and --with-libcdirectory= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect],
+      [test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect && test "x$ac_cv_with_libcdirectory" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdirectory"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdirectory}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdirectory}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdirectory],
           [1])
@@ -152,16 +154,17 @@
             libcdirectory_directory_entry_get_name_wide,
             [ac_cv_libcdirectory_dummy=yes],
             [ac_cv_libcdirectory=no])
           ])
 
         ac_cv_libcdirectory_LIBADD="-lcdirectory"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect && test "x$ac_cv_libcdirectory" != xyes],
+      [test "x$ac_cv_libcdirectory" != xyes && test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect && test "x$ac_cv_with_libcdirectory" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdirectory in directory: $ac_cv_with_libcdirectory],
         [1])
       ])
     ])
 
   AS_IF(
@@ -211,15 +214,15 @@
       [test "x$ac_cv_func_readdir_r" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: readdir_r],
         [1])
       ])
     ])
 
-  ac_cv_libcdirectory_CPPFLAGS="-I../libcdirectory";
+  ac_cv_libcdirectory_CPPFLAGS="-I../libcdirectory -I\$(top_srcdir)/libcdirectory";
   ac_cv_libcdirectory_LIBADD="../libcdirectory/libcdirectory.la";
 
   ac_cv_libcdirectory=local
   ])
 
 dnl Function to detect how to enable libcdirectory
 AC_DEFUN([AX_LIBCDIRECTORY_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/types.m4` & `libmodi-20240507/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/libfcache.m4` & `libmodi-20240507/m4/libfcache.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfcache required headers and functions
 dnl
-dnl Version: 20230115
+dnl Version: 20240413
 
 dnl Function to detect if libfcache is available
 dnl ac_libfcache_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCACHE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno],
     [ac_cv_libfcache=no],
     [ac_cv_libfcache=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfcache which returns "yes" and --with-libfcache= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect],
+      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfcache"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfcache],
           [1])
@@ -147,16 +149,17 @@
           fcache,
           libfcache_date_time_get_timestamp,
           [ac_cv_libfcache_dummy=yes],
           [ac_cv_libfcache=no])
 
         ac_cv_libfcache_LIBADD="-lfcache"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes],
+      [test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcache in directory: $ac_cv_with_libfcache],
         [1])
       ])
     ])
 
   AS_IF(
@@ -192,15 +195,15 @@
   AS_IF(
     [test "x$ac_cv_func_time" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: time],
       [1])
     ])
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
   ])
 
 dnl Function to detect how to enable libfcache
 AC_DEFUN([AX_LIBFCACHE_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/pthread.m4` & `libmodi-20240507/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libmodi-20240305/m4/libfplist.m4` & `libmodi-20240507/m4/libfplist.m4`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Functions for libfplist
 dnl
-dnl Version: 20230218
+dnl Version: 20240413
 
 dnl Function to detect if libfplist is available
 dnl ac_libfplist_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFPLIST_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfplist" = xno],
     [ac_cv_libfplist=no],
     [ac_cv_libfplist=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfplist which returns "yes" and --with-libfplist= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfplist" != x && test "x$ac_cv_with_libfplist" != xauto-detect],
+      [test "x$ac_cv_with_libfplist" != x && test "x$ac_cv_with_libfplist" != xauto-detect && test "x$ac_cv_with_libfplist" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfplist"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfplist}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfplist}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfplist],
           [1])
@@ -135,14 +137,21 @@
           libfplist_property_get_sub_property_by_utf8_name,
           [ac_cv_libfplist_dummy=yes],
           [ac_cv_libfplist=no])
 
         ac_cv_libfplist_LIBADD="-lfplist"
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_libfplist" != xyes && test "x$ac_cv_with_libfplist" != x && test "x$ac_cv_with_libfplist" != xauto-detect && test "x$ac_cv_with_libfplist" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported libfplist in directory: $ac_cv_with_libfplist],
+        [1])
+      ])
     ])
 
   AS_IF(
     [test "x$ac_cv_libfplist" = xyes],
     [AC_DEFINE(
       [HAVE_LIBFPLIST],
       [1],
@@ -161,15 +170,15 @@
   ])
 
 dnl Function to detect if libfplist dependencies are available
 AC_DEFUN([AX_LIBFPLIST_CHECK_LOCAL],
   [AC_PROG_LEX(noyywrap)
   AC_PROG_YACC
 
-  ac_cv_libfplist_CPPFLAGS="-I../libfplist";
+  ac_cv_libfplist_CPPFLAGS="-I../libfplist -I\$(top_srcdir)/libfplist";
   ac_cv_libfplist_LIBADD="../libfplist/libfplist.la";
 
   ac_cv_libfplist=local
   ])
 
 dnl Function to detect how to enable libfplist
 AC_DEFUN([AX_LIBFPLIST_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/m4/lzma.m4` & `libmodi-20240507/m4/lzma.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/m4/zlib.m4` & `libmodi-20240507/m4/zlib.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 dnl Checks for zlib required headers and functions
 dnl
-dnl Version: 20201230
+dnl Version: 20240314
 
 dnl Function to detect if zlib is available
 AC_DEFUN([AX_ZLIB_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_zlib" = xno],
     [ac_cv_zlib=no],
     [ac_cv_zlib=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-zlib which returns "yes" and --with-zlib= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect],
+      [test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_zlib"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_zlib}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_zlib}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_zlib],
           [1])
@@ -58,14 +60,21 @@
             [Missing function: zlibVersion in library: zlib.],
             [1])
           ])
 
         ac_cv_zlib_LIBADD="-lz";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_zlib" != xyes && test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported zlib in directory: $ac_cv_with_zlib],
+        [1])
+      ])
     ])
 
   AS_IF(
     [test "x$ac_cv_zlib" = xzlib],
     [AC_DEFINE(
       [HAVE_ZLIB],
       [1],
```

### Comparing `libmodi-20240305/m4/libcaes.m4` & `libmodi-20240507/m4/libcaes.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcaes required headers and functions
 dnl
-dnl Version: 20220529
+dnl Version: 20240413
 
 dnl Function to detect if libcaes is available
 dnl ac_libcaes_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCAES_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcaes" = xno],
     [ac_cv_libcaes=no],
     [ac_cv_libcaes=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcaes which returns "yes" and --with-libcaes= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect],
+      [test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_with_libcaes" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcaes"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcaes}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcaes}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcaes],
           [1])
@@ -107,16 +109,17 @@
           caes,
           libcaes_crypt_xts,
           [ac_cv_libcaes_dummy=yes],
           [ac_cv_libcaes=no])
 
         ac_cv_libcaes_LIBADD="-lcaes"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_libcaes" != xyes],
+      [test "x$ac_cv_libcaes" != xyes && test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_with_libcaes" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcaes in directory: $ac_cv_with_libcaes],
         [1])
       ])
     ])
 
   AS_IF(
@@ -165,15 +168,15 @@
     [ac_cv_libcaes_aes_ecb=$ac_cv_libcrypto_aes_ecb])
 
   AS_IF(
     [test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_aes_xts" = xno],
     [ac_cv_libcaes_aes_xts=local],
     [ac_cv_libcaes_aes_xts=$ac_cv_libcrypto_aes_xts])
 
-  ac_cv_libcaes_CPPFLAGS="-I../libcaes";
+  ac_cv_libcaes_CPPFLAGS="-I../libcaes -I\$(top_srcdir)/libcaes";
   ac_cv_libcaes_LIBADD="../libcaes/libcaes.la";
 
   ac_cv_libcaes=local
   ])
 
 dnl Function to detect how to enable libcaes
 AC_DEFUN([AX_LIBCAES_CHECK_ENABLE],
```

### Comparing `libmodi-20240305/include/libmodi/definitions.h.in` & `libmodi-20240507/include/libmodi/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/include/libmodi/definitions.h` & `libmodi-20240507/include/libmodi/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBMODI_DEFINITIONS_H )
 #define _LIBMODI_DEFINITIONS_H
 
 #include <libmodi/types.h>
 
-#define LIBMODI_VERSION			20240305
+#define LIBMODI_VERSION			20240507
 
 /* The version string
  */
-#define LIBMODI_VERSION_STRING		"20240305"
+#define LIBMODI_VERSION_STRING		"20240507"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBMODI_ACCESS_FLAGS
```

### Comparing `libmodi-20240305/include/libmodi/types.h.in` & `libmodi-20240507/include/libmodi/types.h.in`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/include/libmodi/types.h` & `libmodi-20240507/include/libmodi/types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/include/libmodi/features.h.in` & `libmodi-20240507/include/libmodi/features.h.in`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/include/libmodi/error.h` & `libmodi-20240507/include/libmodi/error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/include/libmodi/extern.h` & `libmodi-20240507/include/libmodi/extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/include/libmodi/features.h` & `libmodi-20240507/include/libmodi/features.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/include/libmodi/codepage.h` & `libmodi-20240507/include/libmodi/codepage.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/include/libmodi.h.in` & `libmodi-20240507/include/libmodi.h.in`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/include/libmodi.h` & `libmodi-20240507/include/libmodi.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/include/Makefile.in` & `libmodi-20240507/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -514,14 +514,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -610,15 +612,20 @@
 
 EXTRA_DIST = \
 	libmodi.h.in \
 	libmodi/definitions.h.in \
 	libmodi/features.h.in \
 	libmodi/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libmodi.h \
+	libmodi/definitions.h \
+	libmodi/features.h \
+	libmodi/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -815,23 +822,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -913,17 +922,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libmodi.h
-	-rm -f libmodi/definitions.h
-	-rm -f libmodi/features.h
-	-rm -f libmodi/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmodi-20240305/pymodi/pymodi_libmodi.h` & `libmodi-20240507/pymodi/pymodi_libmodi.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_python.h` & `libmodi-20240507/pymodi/pymodi_python.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_libbfio.h` & `libmodi-20240507/pymodi/pymodi_libbfio.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_file_object_io_handle.c` & `libmodi-20240507/pymodi/pymodi_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_handle.h` & `libmodi-20240507/pymodi/pymodi_handle.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi.h` & `libmodi-20240507/pymodi/pymodi.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/Makefile.am` & `libmodi-20240507/pymodi/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -40,13 +40,11 @@
 	@LIBBFIO_LIBADD@
 
 pymodi_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pymodi_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libmodi-20240305/pymodi/pymodi.c` & `libmodi-20240507/pymodi/pymodi.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_libcerror.h` & `libmodi-20240507/pymodi/pymodi_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_file_object_io_handle.h` & `libmodi-20240507/pymodi/pymodi_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_error.h` & `libmodi-20240507/pymodi/pymodi_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_libclocale.h` & `libmodi-20240507/pymodi/pymodi_libclocale.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_handle.c` & `libmodi-20240507/pymodi/pymodi_handle.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_file_objects_io_pool.c` & `libmodi-20240507/pymodi/pymodi_file_objects_io_pool.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_error.c` & `libmodi-20240507/pymodi/pymodi_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_unused.h` & `libmodi-20240507/pymodi/pymodi_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/Makefile.in` & `libmodi-20240507/pymodi/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -563,14 +563,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -643,16 +645,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -683,15 +685,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pymodi_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pymodi_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -965,24 +968,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pymodi_la-pymodi.Plo
+	-rm -f ./$(DEPDIR)/pymodi_la-pymodi_error.Plo
+	-rm -f ./$(DEPDIR)/pymodi_la-pymodi_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pymodi_la-pymodi_file_objects_io_pool.Plo
+	-rm -f ./$(DEPDIR)/pymodi_la-pymodi_handle.Plo
+	-rm -f ./$(DEPDIR)/pymodi_la-pymodi_integer.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1072,13 +1083,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmodi-20240305/pymodi/pymodi_integer.c` & `libmodi-20240507/pymodi/pymodi_integer.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_file_objects_io_pool.h` & `libmodi-20240507/pymodi/pymodi_file_objects_io_pool.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/pymodi/pymodi_integer.h` & `libmodi-20240507/pymodi/pymodi_integer.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/common/config_borlandc.h` & `libmodi-20240507/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/common/file_stream.h` & `libmodi-20240507/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/common/memory.h` & `libmodi-20240507/common/memory.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/common/byte_stream.h` & `libmodi-20240507/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/common/common.h` & `libmodi-20240507/common/common.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/common/config_winapi.h` & `libmodi-20240507/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/common/system_string.h` & `libmodi-20240507/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/common/types.h.in` & `libmodi-20240507/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/common/types.h` & `libmodi-20240507/common/types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/common/config.h.in` & `libmodi-20240507/common/config.h.in`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,17 @@
 
 /* Define to 1 if you have the <libfplist.h> header file. */
 #undef HAVE_LIBFPLIST_H
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
 #undef HAVE_LIBFUSE
 
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#undef HAVE_LIBFUSE3
+
 /* Define to 1 if you have the `fvalue' library (-lfvalue). */
 #undef HAVE_LIBFVALUE
 
 /* Define to 1 if you have the <libfvalue.h> header file. */
 #undef HAVE_LIBFVALUE_H
 
 /* Define to 1 if you have the `hmac' library (-lhmac). */
```

### Comparing `libmodi-20240305/common/config.h` & `libmodi-20240507/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,18 @@
 /* Define to 1 if you have the `fplist' library (-lfplist). */
 /* #undef HAVE_LIBFPLIST */
 
 /* Define to 1 if you have the <libfplist.h> header file. */
 /* #undef HAVE_LIBFPLIST_H */
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
-#define HAVE_LIBFUSE 1
+/* #undef HAVE_LIBFUSE */
+
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#define HAVE_LIBFUSE3 1
 
 /* Define to 1 if you have the `fvalue' library (-lfvalue). */
 /* #undef HAVE_LIBFVALUE */
 
 /* Define to 1 if you have the <libfvalue.h> header file. */
 /* #undef HAVE_LIBFVALUE_H */
 
@@ -697,24 +700,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libmodi"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libmodi 20240305"
+#define PACKAGE_STRING "libmodi 20240507"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libmodi"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240305"
+#define PACKAGE_VERSION "20240507"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -735,15 +738,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240305"
+#define VERSION "20240507"
 
 /* Define to 1 if `lex' declares `yytext' as a `char *' by default, not a
    `char[]'. */
 #define YYTEXT_POINTER 1
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
```

### Comparing `libmodi-20240305/common/wide_string.h` & `libmodi-20240507/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/common/narrow_string.h` & `libmodi-20240507/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/common/config_msc.h` & `libmodi-20240507/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/common/Makefile.in` & `libmodi-20240507/common/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -484,14 +484,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -563,15 +565,17 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -579,15 +583,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -755,23 +762,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -851,15 +860,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmodi-20240305/libclocale/libclocale_wide_string.c` & `libmodi-20240507/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libclocale/libclocale_support.h` & `libmodi-20240507/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libclocale/Makefile.am` & `libmodi-20240507/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libmodi-20240305/libclocale/libclocale_definitions.h` & `libmodi-20240507/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libmodi-20240305/libclocale/libclocale_unused.h` & `libmodi-20240507/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libclocale/libclocale_libcerror.h` & `libmodi-20240507/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libclocale/libclocale_locale.h` & `libmodi-20240507/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libclocale/libclocale_support.c` & `libmodi-20240507/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libclocale/libclocale_codepage.c` & `libmodi-20240507/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libclocale/libclocale_locale.c` & `libmodi-20240507/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libclocale/Makefile.in` & `libmodi-20240507/libclocale/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -528,14 +528,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -609,30 +611,31 @@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -835,24 +838,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -939,17 +948,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libclocale/libclocale_extern.h` & `libmodi-20240507/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libclocale/libclocale_wide_string.h` & `libmodi-20240507/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libclocale/libclocale_codepage.h` & `libmodi-20240507/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/libfcache_libcdata.h` & `libmodi-20240507/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/libfcache_types.h` & `libmodi-20240507/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/libfcache_cache_value.c` & `libmodi-20240507/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/libfcache_unused.h` & `libmodi-20240507/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/Makefile.am` & `libmodi-20240507/libfcache/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCACHE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcache.la
 
@@ -19,19 +19,17 @@
 	libfcache_libcdata.h \
 	libfcache_libcerror.h \
 	libfcache_support.c libfcache_support.h \
 	libfcache_types.h \
 	libfcache_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
```

### Comparing `libmodi-20240305/libfcache/libfcache_support.h` & `libmodi-20240507/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/libfcache_error.h` & `libmodi-20240507/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/libfcache_support.c` & `libmodi-20240507/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/libfcache_cache.h` & `libmodi-20240507/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/libfcache_error.c` & `libmodi-20240507/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/libfcache_libcerror.h` & `libmodi-20240507/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/libfcache_date_time.c` & `libmodi-20240507/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/libfcache_extern.h` & `libmodi-20240507/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/libfcache_cache_value.h` & `libmodi-20240507/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/Makefile.in` & `libmodi-20240507/libfcache/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -531,14 +531,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -611,16 +613,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBFCACHE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCACHE_TRUE@noinst_LTLIBRARIES = libfcache.la
 @HAVE_LOCAL_LIBFCACHE_TRUE@libfcache_la_SOURCES = \
@@ -632,15 +634,16 @@
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_extern.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcdata.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcerror.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_support.c libfcache_support.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_types.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -844,24 +847,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcache_cache.Plo
+	-rm -f ./$(DEPDIR)/libfcache_cache_value.Plo
+	-rm -f ./$(DEPDIR)/libfcache_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfcache_error.Plo
+	-rm -f ./$(DEPDIR)/libfcache_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -949,17 +959,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libfcache/libfcache_date_time.h` & `libmodi-20240507/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfcache/libfcache_definitions.h` & `libmodi-20240507/libfcache/libfcache_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFCACHE )
 #include <libfcache/definitions.h>
 
 /* The definitions in <libfcache/definitions.h> are copied here
  * for local use of libfcache
  */
 #else
-#define LIBFCACHE_VERSION					20240112
+#define LIBFCACHE_VERSION					20240414
 
 /* The libfcache version string
  */
-#define LIBFCACHE_VERSION_STRING				"20240112"
+#define LIBFCACHE_VERSION_STRING				"20240414"
 
 /* The cache value flags definitions
  */
 enum LIBFCACHE_CACHE_VALUE_FLAGS
 {
 	/* The cache value is not managed by the library
 	 */
```

### Comparing `libmodi-20240305/libfcache/libfcache_cache.c` & `libmodi-20240507/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/Makefile.am` & `libmodi-20240507/Makefile.am`

 * *Files 10% similar despite different names*

```diff
@@ -64,16 +64,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libmodi.pc \
+	libmodi.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libmodi.pc
 
 libtool:
@@ -102,19 +109,7 @@
 	(cd $(srcdir)/libfmos && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfplist && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libhmac && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcaes && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libmodi && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libmodi.pc
-	-rm -f libmodi.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libmodi-20240305/libbfio/libbfio_file_range.h` & `libmodi-20240507/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_file_range_io_handle.c` & `libmodi-20240507/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_support.c` & `libmodi-20240507/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_libcpath.h` & `libmodi-20240507/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_error.h` & `libmodi-20240507/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_libclocale.h` & `libmodi-20240507/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_error.c` & `libmodi-20240507/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_libuna.h` & `libmodi-20240507/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_file_io_handle.h` & `libmodi-20240507/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_file_pool.h` & `libmodi-20240507/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_file_range.c` & `libmodi-20240507/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_types.h` & `libmodi-20240507/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_unused.h` & `libmodi-20240507/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_libcdata.h` & `libmodi-20240507/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_file.h` & `libmodi-20240507/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/Makefile.am` & `libmodi-20240507/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libmodi-20240305/libbfio/libbfio_libcfile.h` & `libmodi-20240507/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_definitions.h` & `libmodi-20240507/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libmodi-20240305/libbfio/libbfio_codepage.h` & `libmodi-20240507/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_file_io_handle.c` & `libmodi-20240507/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_support.h` & `libmodi-20240507/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_memory_range.h` & `libmodi-20240507/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_file_pool.c` & `libmodi-20240507/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_file_range_io_handle.h` & `libmodi-20240507/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_libcthreads.h` & `libmodi-20240507/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_system_string.h` & `libmodi-20240507/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_memory_range_io_handle.c` & `libmodi-20240507/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_handle.c` & `libmodi-20240507/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_file.c` & `libmodi-20240507/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_handle.h` & `libmodi-20240507/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_memory_range.c` & `libmodi-20240507/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_pool.c` & `libmodi-20240507/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_libcerror.h` & `libmodi-20240507/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/Makefile.in` & `libmodi-20240507/libbfio/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -549,14 +549,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -629,16 +631,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -669,15 +671,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -888,24 +891,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -974,14 +991,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -992,23 +1011,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmodi-20240305/libbfio/libbfio_system_string.c` & `libmodi-20240507/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_memory_range_io_handle.h` & `libmodi-20240507/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_extern.h` & `libmodi-20240507/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/libbfio/libbfio_pool.h` & `libmodi-20240507/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmodi-20240305/config.guess` & `libmodi-20240507/config.guess`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/dpkg/copyright` & `libmodi-20240507/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/dpkg/control` & `libmodi-20240507/dpkg/control`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/dpkg/rules` & `libmodi-20240507/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/COPYING.LESSER` & `libmodi-20240507/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/configure` & `libmodi-20240507/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libmodi 20240305.
+# Generated by GNU Autoconf 2.71 for libmodi 20240507.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libmodi'
 PACKAGE_TARNAME='libmodi'
-PACKAGE_VERSION='20240305'
-PACKAGE_STRING='libmodi 20240305'
+PACKAGE_VERSION='20240507'
+PACKAGE_STRING='libmodi 20240507'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libmodi.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -678,14 +678,16 @@
 ax_libfuse_spec_requires
 ax_libfuse_pc_libs_private
 LIBFUSE_LIBADD
 LIBFUSE_CPPFLAGS
 HAVE_LIBFUSE
 fuse_LIBS
 fuse_CFLAGS
+fuse3_LIBS
+fuse3_CFLAGS
 HAVE_PYTHON_TESTS_FALSE
 HAVE_PYTHON_TESTS_TRUE
 HAVE_PYTHON_FALSE
 HAVE_PYTHON_TRUE
 PYTHON_PACKAGE_DIR
 PYTHON_LIBRARY_DIR
 pyexecdir
@@ -1231,14 +1233,16 @@
 liblzma_LIBS
 libhmac_CFLAGS
 libhmac_LIBS
 openssl_CFLAGS
 openssl_LIBS
 libcaes_CFLAGS
 libcaes_LIBS
+fuse3_CFLAGS
+fuse3_LIBS
 fuse_CFLAGS
 fuse_LIBS'
 
 
 # Initialize some variables set by options.
 ac_init_help=
 ac_init_version=false
@@ -1781,15 +1785,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libmodi 20240305 to adapt to many kinds of systems.
+\`configure' configures libmodi 20240507 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1852,15 +1856,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libmodi 20240305:";;
+     short | recursive ) echo "Configuration of libmodi 20240507:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -2103,14 +2107,17 @@
               C compiler flags for openssl, overriding pkg-config
   openssl_LIBS
               linker flags for openssl, overriding pkg-config
   libcaes_CFLAGS
               C compiler flags for libcaes, overriding pkg-config
   libcaes_LIBS
               linker flags for libcaes, overriding pkg-config
+  fuse3_CFLAGS
+              C compiler flags for fuse3, overriding pkg-config
+  fuse3_LIBS  linker flags for fuse3, overriding pkg-config
   fuse_CFLAGS C compiler flags for fuse, overriding pkg-config
   fuse_LIBS   linker flags for fuse, overriding pkg-config
 
 Use these variables to override the choices made by `configure' or to help
 it to find libraries and programs with nonstandard names/locations.
 
 Report bugs to <joachim.metz@gmail.com>.
@@ -2173,15 +2180,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libmodi configure 20240305
+libmodi configure 20240507
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2894,15 +2901,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libmodi $as_me 20240305, which was
+It was created by libmodi $as_me 20240507, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4383,15 +4390,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libmodi'
- VERSION='20240305'
+ VERSION='20240507'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23978,15 +23985,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24477,15 +24484,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24627,15 +24635,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24729,15 +24737,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26369,15 +26377,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26431,47 +26439,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26505,15 +26518,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26547,15 +26560,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26590,15 +26603,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26632,15 +26645,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26674,15 +26687,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26716,15 +26729,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26758,15 +26771,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26801,15 +26814,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26843,15 +26856,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26885,15 +26898,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26927,15 +26940,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26969,15 +26982,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27012,15 +27025,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27054,15 +27067,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27096,15 +27109,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27138,15 +27151,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27180,15 +27193,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27223,67 +27236,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
 
 fi
 
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
+
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+fi
+
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27371,15 +27393,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31150,15 +31172,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31183,15 +31206,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31261,15 +31284,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31816,15 +31839,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31980,15 +32004,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -32058,15 +32082,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32516,15 +32540,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32579,15 +32604,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32657,15 +32682,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33380,15 +33405,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33413,15 +33439,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33491,15 +33517,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40701,15 +40727,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40734,15 +40761,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40812,15 +40839,15 @@
 printf "%s\n" "$ac_cv_with_libcdirectory" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdirectory" = xno
 then :
   ac_cv_libcdirectory=no
 else $as_nop
   ac_cv_libcdirectory=check
-        if test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect
+                if test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect && test "x$ac_cv_with_libcdirectory" != xyes
 then :
   if test -d "$ac_cv_with_libcdirectory"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdirectory}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdirectory}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41584,15 +41611,16 @@
 
 fi
 
         ac_cv_libcdirectory_LIBADD="-lcdirectory"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect && test "x$ac_cv_libcdirectory" != xyes
+
+    if test "x$ac_cv_libcdirectory" != xyes && test "x$ac_cv_with_libcdirectory" != x && test "x$ac_cv_with_libcdirectory" != xauto-detect && test "x$ac_cv_with_libcdirectory" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdirectory in directory: $ac_cv_with_libcdirectory
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -41687,15 +41715,15 @@
 as_fn_error 1 "Missing functions: readdir_r
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcdirectory_CPPFLAGS="-I../libcdirectory";
+  ac_cv_libcdirectory_CPPFLAGS="-I../libcdirectory -I\$(top_srcdir)/libcdirectory";
   ac_cv_libcdirectory_LIBADD="../libcdirectory/libcdirectory.la";
 
   ac_cv_libcdirectory=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDIRECTORY 1" >>confdefs.h
@@ -41765,15 +41793,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -42954,15 +42982,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43276,15 +43305,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -43354,15 +43383,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -44159,15 +44188,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -44357,15 +44387,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -44435,15 +44465,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -46553,15 +46583,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -46586,15 +46617,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -46664,15 +46695,15 @@
 printf "%s\n" "$ac_cv_with_libfcache" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno
 then :
   ac_cv_libfcache=no
 else $as_nop
   ac_cv_libfcache=check
-        if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect
+                if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   if test -d "$ac_cv_with_libfcache"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -47584,15 +47615,16 @@
 fi
 
 
         ac_cv_libfcache_LIBADD="-lfcache"
 fi
 
 fi
-    if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes
+
+    if test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcache in directory: $ac_cv_with_libfcache
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -47685,15 +47717,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: time
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCACHE 1" >>confdefs.h
@@ -47763,15 +47795,15 @@
 printf "%s\n" "$ac_cv_with_libfdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno
 then :
   ac_cv_libfdata=no
 else $as_nop
   ac_cv_libfdata=check
-        if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect
+                if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   if test -d "$ac_cv_with_libfdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -51051,15 +51083,16 @@
 
 
 
         ac_cv_libfdata_LIBADD="-lfdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes
+
+    if test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdata in directory: $ac_cv_with_libfdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -51084,15 +51117,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -51162,15 +51195,15 @@
 printf "%s\n" "$ac_cv_with_libfguid" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno
 then :
   ac_cv_libfguid=no
 else $as_nop
   ac_cv_libfguid=check
-        if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect
+                if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   if test -d "$ac_cv_with_libfguid"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -51744,15 +51777,16 @@
 fi
 
 
         ac_cv_libfguid_LIBADD="-lfguid"
 fi
 
 fi
-    if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes
+
+    if test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfguid in directory: $ac_cv_with_libfguid
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -51777,15 +51811,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -51855,15 +51889,15 @@
 printf "%s\n" "$ac_cv_with_libfvalue" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno
 then :
   ac_cv_libfvalue=no
 else $as_nop
   ac_cv_libfvalue=check
-        if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect
+                if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   if test -d "$ac_cv_with_libfvalue"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -56169,15 +56203,16 @@
 fi
 
 
         ac_cv_libfvalue_LIBADD="-lfvalue"
 fi
 
 fi
-    if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes
+
+    if test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfvalue in directory: $ac_cv_with_libfvalue
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -56202,15 +56237,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfvalue" != xyes
 then :
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFVALUE 1" >>confdefs.h
@@ -56280,15 +56315,15 @@
 printf "%s\n" "$ac_cv_with_libfmos" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfmos" = xno
 then :
   ac_cv_libfmos=no
 else $as_nop
   ac_cv_libfmos=check
-        if test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect
+                if test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect && test "x$ac_cv_with_libfmos" != xyes
 then :
   if test -d "$ac_cv_with_libfmos"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfmos}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfmos}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -56570,15 +56605,16 @@
 fi
 
 
         ac_cv_libfmos_LIBADD="-lfmos"
 fi
 
 fi
-    if test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect && test "x$ac_cv_libfmos" != xyes
+
+    if test "x$ac_cv_libfmos" != xyes && test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect && test "x$ac_cv_with_libfmos" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfmos in directory: $ac_cv_with_libfmos
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -56603,15 +56639,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfmos" != xyes
 then :
 
-  ac_cv_libfmos_CPPFLAGS="-I../libfmos";
+  ac_cv_libfmos_CPPFLAGS="-I../libfmos -I\$(top_srcdir)/libfmos";
   ac_cv_libfmos_LIBADD="../libfmos/libfmos.la";
 
   ac_cv_libfmos=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFMOS 1" >>confdefs.h
@@ -56681,15 +56717,15 @@
 printf "%s\n" "$ac_cv_with_libfplist" >&6; }
 
   if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfplist" = xno
 then :
   ac_cv_libfplist=no
 else $as_nop
   ac_cv_libfplist=check
-        if test "x$ac_cv_with_libfplist" != x && test "x$ac_cv_with_libfplist" != xauto-detect
+                if test "x$ac_cv_with_libfplist" != x && test "x$ac_cv_with_libfplist" != xauto-detect && test "x$ac_cv_with_libfplist" != xyes
 then :
   if test -d "$ac_cv_with_libfplist"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfplist}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfplist}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -57480,14 +57516,23 @@
 
         ac_cv_libfplist_LIBADD="-lfplist"
 
 fi
 
 fi
 
+    if test "x$ac_cv_libfplist" != xyes && test "x$ac_cv_with_libfplist" != x && test "x$ac_cv_with_libfplist" != xauto-detect && test "x$ac_cv_with_libfplist" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported libfplist in directory: $ac_cv_with_libfplist
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
 fi
 
   if test "x$ac_cv_libfplist" = xyes
 then :
 
 printf "%s\n" "#define HAVE_LIBFPLIST 1" >>confdefs.h
 
@@ -57770,15 +57815,15 @@
 
 
   test -n "$YACC" && break
 done
 test -n "$YACC" || YACC="yacc"
 
 
-  ac_cv_libfplist_CPPFLAGS="-I../libfplist";
+  ac_cv_libfplist_CPPFLAGS="-I../libfplist -I\$(top_srcdir)/libfplist";
   ac_cv_libfplist_LIBADD="../libfplist/libfplist.la";
 
   ac_cv_libfplist=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFPLIST 1" >>confdefs.h
@@ -57848,15 +57893,15 @@
 printf "%s\n" "$ac_cv_with_zlib" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_zlib" = xno
 then :
   ac_cv_zlib=no
 else $as_nop
   ac_cv_zlib=check
-        if test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect
+                if test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes
 then :
   if test -d "$ac_cv_with_zlib"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_zlib}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_zlib}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -58023,14 +58068,23 @@
 
         ac_cv_zlib_LIBADD="-lz";
 
 fi
 
 fi
 
+    if test "x$ac_cv_zlib" != xyes && test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported zlib in directory: $ac_cv_with_zlib
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
 fi
 
   if test "x$ac_cv_zlib" = xzlib
 then :
 
 printf "%s\n" "#define HAVE_ZLIB 1" >>confdefs.h
 
@@ -58730,15 +58784,15 @@
 printf "%s\n" "$ac_cv_with_libhmac" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libhmac" = xno
 then :
   ac_cv_libhmac=no
 else $as_nop
   ac_cv_libhmac=check
-        if test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect
+                if test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes
 then :
   if test -d "$ac_cv_with_libhmac"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libhmac}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libhmac}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -59736,15 +59790,16 @@
 fi
 
 
         ac_cv_libhmac_LIBADD="-lhmac"
 fi
 
 fi
-    if test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_libhmac" != xyes
+
+    if test "x$ac_cv_libhmac" != xyes && test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libhmac in directory: $ac_cv_with_libhmac
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -59850,15 +59905,15 @@
 
   if test "x$ac_cv_enable_static_executables" != xyes
 then :
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno
 then :
   ac_cv_libcrypto=no
 else $as_nop
-      if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect
+              if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes
 then :
   if test -d "$ac_cv_with_openssl"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -64036,15 +64091,15 @@
   if test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_sha512" = xno
 then :
   ac_cv_libhmac_sha512=local
 else $as_nop
   ac_cv_libhmac_sha512=$ac_cv_libcrypto_sha512
 fi
 
-  ac_cv_libhmac_CPPFLAGS="-I../libhmac";
+  ac_cv_libhmac_CPPFLAGS="-I../libhmac -I\$(top_srcdir)/libhmac";
   ac_cv_libhmac_LIBADD="../libhmac/libhmac.la";
 
   ac_cv_libhmac=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBHMAC 1" >>confdefs.h
@@ -64114,15 +64169,15 @@
 printf "%s\n" "$ac_cv_with_libcaes" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcaes" = xno
 then :
   ac_cv_libcaes=no
 else $as_nop
   ac_cv_libcaes=check
-        if test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect
+                if test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_with_libcaes" != xyes
 then :
   if test -d "$ac_cv_with_libcaes"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcaes}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcaes}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -64698,15 +64753,16 @@
 fi
 
 
         ac_cv_libcaes_LIBADD="-lcaes"
 fi
 
 fi
-    if test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_libcaes" != xyes
+
+    if test "x$ac_cv_libcaes" != xyes && test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_with_libcaes" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcaes in directory: $ac_cv_with_libcaes
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -64804,15 +64860,15 @@
 
   if test "x$ac_cv_enable_static_executables" != xyes
 then :
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno
 then :
   ac_cv_libcrypto=no
 else $as_nop
-      if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect
+              if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes
 then :
   if test -d "$ac_cv_with_openssl"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -67639,15 +67695,15 @@
   if test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_aes_xts" = xno
 then :
   ac_cv_libcaes_aes_xts=local
 else $as_nop
   ac_cv_libcaes_aes_xts=$ac_cv_libcrypto_aes_xts
 fi
 
-  ac_cv_libcaes_CPPFLAGS="-I../libcaes";
+  ac_cv_libcaes_CPPFLAGS="-I../libcaes -I\$(top_srcdir)/libcaes";
   ac_cv_libcaes_LIBADD="../libcaes/libcaes.la";
 
   ac_cv_libcaes=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCAES 1" >>confdefs.h
@@ -67958,16 +68014,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -68125,33 +68185,107 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_libfuse=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_libfuse" >&5
 printf "%s\n" "$ac_cv_with_libfuse" >&6; }
 
-      if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno
+then :
+  ac_cv_libfuse=no
+else $as_nop
+              if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
 then :
   if test -d "$ac_cv_with_libfuse"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
 else $as_nop
-  { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_libfuse" >&5
-printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_libfuse" >&2;}
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "no such directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
+else $as_nop
+        if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+then :
 
+pkg_failed=no
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse3 >= 3.0" >&5
+printf %s "checking for fuse3 >= 3.0... " >&6; }
+
+if test -n "$fuse3_CFLAGS"; then
+    pkg_cv_fuse3_CFLAGS="$fuse3_CFLAGS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_CFLAGS=`$PKG_CONFIG --cflags "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
+fi
+if test -n "$fuse3_LIBS"; then
+    pkg_cv_fuse3_LIBS="$fuse3_LIBS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_LIBS=`$PKG_CONFIG --libs "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
 fi
 
-  if test "x$ac_cv_with_libfuse" = xno
-then :
-  ac_cv_libfuse=no
-else $as_nop
-      if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+
+
+if test $pkg_failed = yes; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+
+if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
+        _pkg_short_errors_supported=yes
+else
+        _pkg_short_errors_supported=no
+fi
+        if test $_pkg_short_errors_supported = yes; then
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        else
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        fi
+        # Put the nasty error message in config.log where it belongs
+        echo "$fuse3_PKG_ERRORS" >&5
+
+        ac_cv_libfuse=no
+elif test $pkg_failed = untried; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+        ac_cv_libfuse=no
+else
+        fuse3_CFLAGS=$pkg_cv_fuse3_CFLAGS
+        fuse3_LIBS=$pkg_cv_fuse3_LIBS
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
+printf "%s\n" "yes" >&6; }
+        ac_cv_libfuse=libfuse3
+fi
+
+        if test "x$ac_cv_libfuse" = xno
 then :
 
 pkg_failed=no
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse >= 2.6" >&5
 printf %s "checking for fuse >= 2.6... " >&6; }
 
 if test -n "$fuse_CFLAGS"; then
@@ -68219,51 +68353,110 @@
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
 printf "%s\n" "yes" >&6; }
         ac_cv_libfuse=libfuse
 fi
 
 fi
 
-    if test "x$ac_cv_libfuse" = xlibfuse
+        if test "x$ac_cv_libfuse" = xlibfuse3
 then :
-  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
-else $as_nop
-               for ac_header in fuse.h
-do :
-  ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"
+fi
+
+        if test "x$ac_cv_libfuse" = xlibfuse
+then :
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
+fi
+
+fi
+
+fi
+
+    backup_CPPFLAGS="$CPPFLAGS"
+
+        if test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3
+then :
+
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
- ac_cv_header_fuse_h=yes
-else $as_nop
-  ac_cv_header_fuse_h=no
+
 fi
 
-done
 
-                  if test "x$ac_cv_header_fuse_h" = xno
+      if test "x$ac_cv_header_fuse_h" = xyes
 then :
-  { ac_cv_header_fuse_h=; unset ac_cv_header_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+  ac_cv_libfuse=libfuse3
+else $as_nop
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
+        if test "x$ac_cv_header_fuse_h" = xyes
+then :
+  ac_cv_libfuse=libfuse
+fi
+
 fi
 
       if test "x$ac_cv_header_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
-          ac_cv_libfuse=libfuse
+          { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_invalidate in -lfuse" >&5
+printf %s "checking for fuse_invalidate in -lfuse... " >&6; }
+if test ${ac_cv_lib_fuse_fuse_invalidate+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfuse  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char fuse_invalidate ();
+int
+main (void)
+{
+return fuse_invalidate ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fuse_fuse_invalidate=yes
+else $as_nop
+  ac_cv_lib_fuse_fuse_invalidate=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fuse_fuse_invalidate" >&5
+printf "%s\n" "$ac_cv_lib_fuse_fuse_invalidate" >&6; }
+if test "x$ac_cv_lib_fuse_fuse_invalidate" = xyes
+then :
+  ac_cv_libfuse=libfuse
+else $as_nop
+  ac_cv_libfuse=libfuse3
+fi
+
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -lfuse" >&5
 printf %s "checking for fuse_daemonize in -lfuse... " >&6; }
 if test ${ac_cv_lib_fuse_fuse_daemonize+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
@@ -68426,45 +68619,38 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
 
+        if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ac_cv_libfuse_LIBADD="-lfuse3"
+else $as_nop
+  ac_cv_libfuse_LIBADD="-lfuse"
 fi
 
 fi
 
-        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
-then :
-  CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
-      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
-if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
-then :
-  printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
-
 fi
 
-
-            if test "x$ac_cv_header_osxfuse_fuse_h" = xno
+        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
 then :
-  { ac_cv_header_osxfuse_fuse_h=; unset ac_cv_header_osxfuse_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
+      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
-fi
-
       if test "x$ac_cv_header_osxfuse_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
           ac_cv_libfuse=libosxfuse
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -losxfuse" >&5
@@ -68632,29 +68818,49 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
 
 fi
 
 fi
 
+    if test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported libfuse in directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
+    CPPFLAGS="$backup_CPPFLAGS"
+
 fi
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBFUSE 1" >>confdefs.h
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+
+printf "%s\n" "#define HAVE_LIBFUSE3 1" >>confdefs.h
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBOSXFUSE 1" >>confdefs.h
 
 
 fi
@@ -68685,14 +68891,20 @@
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
   ax_libfuse_pc_libs_private=-lfuse
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_pc_libs_private=-lfuse3
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
   ax_libfuse_pc_libs_private=-losxfuse
 
 
 fi
 
@@ -68700,14 +68912,22 @@
 then :
   ax_libfuse_spec_requires=fuse-libs
 
     ax_libfuse_spec_build_requires=fuse-devel
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_spec_requires=fuse3-libs
+
+    ax_libfuse_spec_build_requires=fuse3-devel
+
+
+fi
 
 
 ac_fn_c_check_header_compile "$LINENO" "signal.h" "ac_cv_header_signal_h" "$ac_includes_default"
 if test "x$ac_cv_header_signal_h" = xyes
 then :
   printf "%s\n" "#define HAVE_SIGNAL_H 1" >>confdefs.h
 
@@ -69657,15 +69877,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libmodi $as_me 20240305, which was
+This file was extended by libmodi $as_me 20240507, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -69725,15 +69945,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libmodi config.status 20240305
+libmodi config.status 20240507
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libmodi-20240305/compile` & `libmodi-20240507/compile`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/missing` & `libmodi-20240507/missing`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libfdata/libfdata.vcproj` & `libmodi-20240507/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modimount/modimount.vcproj` & `libmodi-20240507/msvscpp/modimount/modimount.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_udif_block_table/modi_test_udif_block_table.vcproj` & `libmodi-20240507/msvscpp/modi_test_udif_block_table/modi_test_udif_block_table.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_sparse_bundle_xml_plist/modi_test_sparse_bundle_xml_plist.vcproj` & `libmodi-20240507/msvscpp/modi_test_sparse_bundle_xml_plist/modi_test_sparse_bundle_xml_plist.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libmodi/libmodi.vcproj` & `libmodi-20240507/msvscpp/libmodi/libmodi.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_bzip/modi_test_bzip.vcproj` & `libmodi-20240507/msvscpp/modi_test_bzip/modi_test_bzip.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libfmos/libfmos.vcproj` & `libmodi-20240507/msvscpp/libfmos/libfmos.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/zlib/zlib.vcproj` & `libmodi-20240507/msvscpp/zlib/zlib.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libfplist/libfplist.vcproj` & `libmodi-20240507/msvscpp/libfplist/libfplist.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libcaes/libcaes.vcproj` & `libmodi-20240507/msvscpp/libcaes/libcaes.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libfguid/libfguid.vcproj` & `libmodi-20240507/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/pymodi/pymodi.vcproj` & `libmodi-20240507/msvscpp/pymodi/pymodi.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_error/modi_test_error.vcproj` & `libmodi-20240507/msvscpp/modi_test_error/modi_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libclocale/libclocale.vcproj` & `libmodi-20240507/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libfcache/libfcache.vcproj` & `libmodi-20240507/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/Makefile.am` & `libmodi-20240507/msvscpp/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -46,13 +46,11 @@
 	pymodi/pymodi.vcproj \
 	zlib/zlib.vcproj \
 	libmodi.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libmodi-20240305/msvscpp/libbfio/libbfio.vcproj` & `libmodi-20240507/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_io_handle/modi_test_io_handle.vcproj` & `libmodi-20240507/msvscpp/modi_test_io_handle/modi_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_system_string/modi_test_system_string.vcproj` & `libmodi-20240507/msvscpp/modi_test_system_string/modi_test_system_string.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_data_block/modi_test_data_block.vcproj` & `libmodi-20240507/msvscpp/modi_test_data_block/modi_test_data_block.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_notify/modi_test_notify.vcproj` & `libmodi-20240507/msvscpp/modi_test_notify/modi_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_udif_xml_plist/modi_test_udif_xml_plist.vcproj` & `libmodi-20240507/msvscpp/modi_test_udif_xml_plist/modi_test_udif_xml_plist.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_udif_resource_file/modi_test_udif_resource_file.vcproj` & `libmodi-20240507/msvscpp/modi_test_udif_resource_file/modi_test_udif_resource_file.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_huffman_tree/modi_test_huffman_tree.vcproj` & `libmodi-20240507/msvscpp/modi_test_huffman_tree/modi_test_huffman_tree.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_bands_data_handle/modi_test_bands_data_handle.vcproj` & `libmodi-20240507/msvscpp/modi_test_bands_data_handle/modi_test_bands_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libcfile/libcfile.vcproj` & `libmodi-20240507/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_tools_signal/modi_test_tools_signal.vcproj` & `libmodi-20240507/msvscpp/modi_test_tools_signal/modi_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_sparse_image_header/modi_test_sparse_image_header.vcproj` & `libmodi-20240507/msvscpp/modi_test_sparse_image_header/modi_test_sparse_image_header.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_tools_output/modi_test_tools_output.vcproj` & `libmodi-20240507/msvscpp/modi_test_tools_output/modi_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_udif_block_table_entry/modi_test_udif_block_table_entry.vcproj` & `libmodi-20240507/msvscpp/modi_test_udif_block_table_entry/modi_test_udif_block_table_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libcdata/libcdata.vcproj` & `libmodi-20240507/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_deflate/modi_test_deflate.vcproj` & `libmodi-20240507/msvscpp/modi_test_deflate/modi_test_deflate.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_handle/modi_test_handle.vcproj` & `libmodi-20240507/msvscpp/modi_test_handle/modi_test_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libcthreads/libcthreads.vcproj` & `libmodi-20240507/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_tools_info_handle/modi_test_tools_info_handle.vcproj` & `libmodi-20240507/msvscpp/modi_test_tools_info_handle/modi_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libcpath/libcpath.vcproj` & `libmodi-20240507/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libmodi.sln` & `libmodi-20240507/msvscpp/libmodi.sln`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/bzip2/bzip2.vcproj` & `libmodi-20240507/msvscpp/bzip2/bzip2.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_support/modi_test_support.vcproj` & `libmodi-20240507/msvscpp/modi_test_support/modi_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libhmac/libhmac.vcproj` & `libmodi-20240507/msvscpp/libhmac/libhmac.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libcsplit/libcsplit.vcproj` & `libmodi-20240507/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libuna/libuna.vcproj` & `libmodi-20240507/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/Makefile.in` & `libmodi-20240507/msvscpp/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -466,14 +466,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -597,15 +599,16 @@
 	pymodi/pymodi.vcproj \
 	zlib/zlib.vcproj \
 	libmodi.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -709,23 +712,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -804,13 +809,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmodi-20240305/msvscpp/libfvalue/libfvalue.vcproj` & `libmodi-20240507/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modiinfo/modiinfo.vcproj` & `libmodi-20240507/msvscpp/modiinfo/modiinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libcnotify/libcnotify.vcproj` & `libmodi-20240507/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/modi_test_bit_stream/modi_test_bit_stream.vcproj` & `libmodi-20240507/msvscpp/modi_test_bit_stream/modi_test_bit_stream.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libcerror/libcerror.vcproj` & `libmodi-20240507/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/msvscpp/libcdirectory/libcdirectory.vcproj` & `libmodi-20240507/msvscpp/libcdirectory/libcdirectory.vcproj`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_extern.h` & `libmodi-20240507/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_support.h` & `libmodi-20240507/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_unused.h` & `libmodi-20240507/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_notify.h` & `libmodi-20240507/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_support.c` & `libmodi-20240507/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_types.h` & `libmodi-20240507/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/Makefile.am` & `libmodi-20240507/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libmodi-20240305/libcfile/libcfile_notify.c` & `libmodi-20240507/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_system_string.h` & `libmodi-20240507/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_file.h` & `libmodi-20240507/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_libcnotify.h` & `libmodi-20240507/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_system_string.c` & `libmodi-20240507/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_error.h` & `libmodi-20240507/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_libcerror.h` & `libmodi-20240507/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_file.c` & `libmodi-20240507/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_libclocale.h` & `libmodi-20240507/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_winapi.h` & `libmodi-20240507/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/Makefile.in` & `libmodi-20240507/libcfile/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -531,14 +531,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -611,16 +613,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -635,15 +637,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -848,24 +851,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -954,17 +965,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libcfile/libcfile_error.c` & `libmodi-20240507/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_libuna.h` & `libmodi-20240507/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_winapi.c` & `libmodi-20240507/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcfile/libcfile_definitions.h` & `libmodi-20240507/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libmodi-20240305/README` & `libmodi-20240507/README`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/INSTALL` & `libmodi-20240507/INSTALL`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_list_element.h` & `libmodi-20240507/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_array.h` & `libmodi-20240507/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_definitions.h` & `libmodi-20240507/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libmodi-20240305/libcdata/libcdata_libcerror.h` & `libmodi-20240507/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_unused.h` & `libmodi-20240507/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_btree.h` & `libmodi-20240507/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_btree.c` & `libmodi-20240507/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_support.c` & `libmodi-20240507/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_list.c` & `libmodi-20240507/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_extern.h` & `libmodi-20240507/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_list.h` & `libmodi-20240507/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_btree_values_list.h` & `libmodi-20240507/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/Makefile.am` & `libmodi-20240507/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libmodi-20240305/libcdata/libcdata_btree_node.h` & `libmodi-20240507/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_range_list_value.h` & `libmodi-20240507/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_range_list.h` & `libmodi-20240507/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_range_list.c` & `libmodi-20240507/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_array.c` & `libmodi-20240507/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_list_element.c` & `libmodi-20240507/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_libcthreads.h` & `libmodi-20240507/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_tree_node.h` & `libmodi-20240507/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_error.h` & `libmodi-20240507/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_types.h` & `libmodi-20240507/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_btree_node.c` & `libmodi-20240507/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_tree_node.c` & `libmodi-20240507/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_support.h` & `libmodi-20240507/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/Makefile.in` & `libmodi-20240507/libcdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -545,14 +545,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -625,16 +627,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -651,15 +653,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -869,24 +872,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -980,17 +996,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libcdata/libcdata_range_list_value.c` & `libmodi-20240507/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_btree_values_list.c` & `libmodi-20240507/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdata/libcdata_error.c` & `libmodi-20240507/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/ylwrap` & `libmodi-20240507/ylwrap`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/config.sub` & `libmodi-20240507/config.sub`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi.pc.in` & `libmodi-20240507/libmodi.pc.in`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/setup.py` & `libmodi-20240507/setup.py`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/acinclude.m4` & `libmodi-20240507/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/config.rpath` & `libmodi-20240507/config.rpath`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_thread.h` & `libmodi-20240507/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_read_write_lock.h` & `libmodi-20240507/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_thread.c` & `libmodi-20240507/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_thread_pool.h` & `libmodi-20240507/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_support.h` & `libmodi-20240507/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_lock.h` & `libmodi-20240507/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_unused.h` & `libmodi-20240507/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_lock.c` & `libmodi-20240507/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_condition.h` & `libmodi-20240507/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_repeating_thread.h` & `libmodi-20240507/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/Makefile.am` & `libmodi-20240507/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libmodi-20240305/libcthreads/libcthreads_support.c` & `libmodi-20240507/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_mutex.c` & `libmodi-20240507/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_queue.c` & `libmodi-20240507/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_mutex.h` & `libmodi-20240507/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_types.h` & `libmodi-20240507/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_thread_attributes.h` & `libmodi-20240507/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_condition.c` & `libmodi-20240507/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_error.c` & `libmodi-20240507/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_read_write_lock.c` & `libmodi-20240507/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_libcerror.h` & `libmodi-20240507/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_definitions.h` & `libmodi-20240507/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libmodi-20240305/libcthreads/libcthreads_thread_pool.c` & `libmodi-20240507/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_error.h` & `libmodi-20240507/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_thread_attributes.c` & `libmodi-20240507/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_extern.h` & `libmodi-20240507/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/libcthreads_repeating_thread.c` & `libmodi-20240507/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcthreads/Makefile.in` & `libmodi-20240507/libcthreads/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -549,14 +549,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -629,16 +631,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -653,15 +655,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -871,24 +874,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -982,17 +998,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libcthreads/libcthreads_queue.h` & `libmodi-20240507/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/test-driver` & `libmodi-20240507/test-driver`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/libcpath_support.c` & `libmodi-20240507/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/libcpath_libcerror.h` & `libmodi-20240507/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/libcpath_definitions.h` & `libmodi-20240507/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libmodi-20240305/libcpath/Makefile.am` & `libmodi-20240507/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libmodi-20240305/libcpath/libcpath_error.c` & `libmodi-20240507/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/libcpath_extern.h` & `libmodi-20240507/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/libcpath_system_string.h` & `libmodi-20240507/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/libcpath_support.h` & `libmodi-20240507/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/libcpath_libcsplit.h` & `libmodi-20240507/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/libcpath_system_string.c` & `libmodi-20240507/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/libcpath_libclocale.h` & `libmodi-20240507/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/libcpath_error.h` & `libmodi-20240507/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/Makefile.in` & `libmodi-20240507/libcpath/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -525,14 +525,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -605,16 +607,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -626,15 +628,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -837,24 +840,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -941,17 +950,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libcpath/libcpath_libuna.h` & `libmodi-20240507/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/libcpath_unused.h` & `libmodi-20240507/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/libcpath_path.c` & `libmodi-20240507/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcpath/libcpath_path.h` & `libmodi-20240507/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/ChangeLog` & `libmodi-20240507/ChangeLog`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/manuals/libmodi.3` & `libmodi-20240507/manuals/libmodi.3`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/manuals/modiinfo.1` & `libmodi-20240507/manuals/modiinfo.1`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/manuals/Makefile.in` & `libmodi-20240507/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -498,14 +498,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -585,15 +587,16 @@
 	libmodi.3 \
 	modiinfo.1
 
 EXTRA_DIST = \
 	libmodi.3 \
 	modiinfo.1
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -786,23 +789,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -884,13 +889,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmodi-20240305/tests/modi_test_unused.h` & `libmodi-20240507/tests/modi_test_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_getopt.h` & `libmodi-20240507/tests/modi_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_bands_data_handle.c` & `libmodi-20240507/tests/modi_test_bands_data_handle.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_io_handle.c` & `libmodi-20240507/tests/modi_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_error.c` & `libmodi-20240507/tests/modi_test_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_udif_xml_plist.c` & `libmodi-20240507/tests/modi_test_udif_xml_plist.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_udif_resource_file.c` & `libmodi-20240507/tests/modi_test_udif_resource_file.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_libcerror.h` & `libmodi-20240507/tests/modi_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_udif_block_table.c` & `libmodi-20240507/tests/modi_test_udif_block_table.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_functions.c` & `libmodi-20240507/tests/modi_test_functions.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_bzip.c` & `libmodi-20240507/tests/modi_test_bzip.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_notify.c` & `libmodi-20240507/tests/modi_test_notify.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_macros.h` & `libmodi-20240507/tests/modi_test_macros.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_sparse_bundle_xml_plist.c` & `libmodi-20240507/tests/modi_test_sparse_bundle_xml_plist.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/test_tools.sh` & `libmodi-20240507/tests/test_tools.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TOOLS_TESTS="info_handle output signal";
 TOOLS_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libmodi-20240305/tests/modi_test_deflate.c` & `libmodi-20240507/tests/modi_test_deflate.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/Makefile.am` & `libmodi-20240507/tests/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -406,13 +406,12 @@
 	@LIBCSPLIT_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libmodi/libmodi.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libmodi-20240305/tests/modi_test_bit_stream.c` & `libmodi-20240507/tests/modi_test_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_memory.c` & `libmodi-20240507/tests/modi_test_memory.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_libcdirectory.h` & `libmodi-20240507/tests/modi_test_libcdirectory.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_libcpath.h` & `libmodi-20240507/tests/modi_test_libcpath.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_libclocale.h` & `libmodi-20240507/tests/modi_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_sparse_image_header.c` & `libmodi-20240507/tests/modi_test_sparse_image_header.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_libuna.h` & `libmodi-20240507/tests/modi_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_libbfio.h` & `libmodi-20240507/tests/modi_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_data_block.c` & `libmodi-20240507/tests/modi_test_data_block.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_udif_block_table_entry.c` & `libmodi-20240507/tests/modi_test_udif_block_table_entry.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/test_python_module.sh` & `libmodi-20240507/tests/test_python_module.sh`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="handle";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libmodi";
+PYTHON_MODULE="pymodi";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pymodi_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pymodi_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pymodi");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libmodi-20240305/tests/modi_test_libmodi.h` & `libmodi-20240507/tests/modi_test_libmodi.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_getopt.c` & `libmodi-20240507/tests/modi_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/pymodi_test_handle.py` & `libmodi-20240507/tests/pymodi_test_handle.py`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/test_runner.sh` & `libmodi-20240507/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/pymodi_test_support.py` & `libmodi-20240507/tests/pymodi_test_support.py`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_tools_signal.c` & `libmodi-20240507/tests/modi_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_support.c` & `libmodi-20240507/tests/modi_test_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_functions.h` & `libmodi-20240507/tests/modi_test_functions.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_huffman_tree.c` & `libmodi-20240507/tests/modi_test_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/test_modiinfo.sh` & `libmodi-20240507/tests/test_modiinfo.sh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("modiinfo");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libmodi-20240305/tests/modi_test_tools_info_handle.c` & `libmodi-20240507/tests/modi_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/Makefile.in` & `libmodi-20240507/tests/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -893,14 +893,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -974,16 +976,16 @@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1358,16 +1360,18 @@
 	@LIBCSPLIT_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libmodi/libmodi.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1881,24 +1885,54 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../moditools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../moditools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../moditools/$(DEPDIR)/byte_size_string.Po
+	-rm -f ../moditools/$(DEPDIR)/info_handle.Po
+	-rm -f ../moditools/$(DEPDIR)/moditools_output.Po
+	-rm -f ../moditools/$(DEPDIR)/moditools_signal.Po
+	-rm -f ./$(DEPDIR)/modi_test_bands_data_handle.Po
+	-rm -f ./$(DEPDIR)/modi_test_bit_stream.Po
+	-rm -f ./$(DEPDIR)/modi_test_bzip.Po
+	-rm -f ./$(DEPDIR)/modi_test_data_block.Po
+	-rm -f ./$(DEPDIR)/modi_test_deflate.Po
+	-rm -f ./$(DEPDIR)/modi_test_error.Po
+	-rm -f ./$(DEPDIR)/modi_test_functions.Po
+	-rm -f ./$(DEPDIR)/modi_test_getopt.Po
+	-rm -f ./$(DEPDIR)/modi_test_handle.Po
+	-rm -f ./$(DEPDIR)/modi_test_huffman_tree.Po
+	-rm -f ./$(DEPDIR)/modi_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/modi_test_memory.Po
+	-rm -f ./$(DEPDIR)/modi_test_notify.Po
+	-rm -f ./$(DEPDIR)/modi_test_sparse_bundle_xml_plist.Po
+	-rm -f ./$(DEPDIR)/modi_test_sparse_image_header.Po
+	-rm -f ./$(DEPDIR)/modi_test_support.Po
+	-rm -f ./$(DEPDIR)/modi_test_system_string.Po
+	-rm -f ./$(DEPDIR)/modi_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/modi_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/modi_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/modi_test_udif_block_table.Po
+	-rm -f ./$(DEPDIR)/modi_test_udif_block_table_entry.Po
+	-rm -f ./$(DEPDIR)/modi_test_udif_resource_file.Po
+	-rm -f ./$(DEPDIR)/modi_test_udif_xml_plist.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -2009,13 +2043,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmodi-20240305/tests/modi_test_libcnotify.h` & `libmodi-20240507/tests/modi_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_handle.c` & `libmodi-20240507/tests/modi_test_handle.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_memory.h` & `libmodi-20240507/tests/modi_test_memory.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_tools_output.c` & `libmodi-20240507/tests/modi_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/modi_test_system_string.c` & `libmodi-20240507/tests/modi_test_system_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/tests/test_library.sh` & `libmodi-20240507/tests/test_library.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="bands_data_handle bit_stream bzip data_block deflate error huffman_tree io_handle notify sparse_bundle_xml_plist sparse_image_header system_string udif_block_table udif_block_table_entry udif_resource_file udif_xml_plist";
 LIBRARY_TESTS_WITH_INPUT="handle support";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libmodi-20240305/ossfuzz/handle_fuzzer.cc` & `libmodi-20240507/ossfuzz/handle_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/ossfuzz/Makefile.am` & `libmodi-20240507/ossfuzz/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -29,17 +29,15 @@
 	../libmodi/libmodi.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on handle_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(handle_fuzzer_SOURCES)
```

### Comparing `libmodi-20240305/ossfuzz/ossfuzz_libbfio.h` & `libmodi-20240507/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/ossfuzz/Makefile.in` & `libmodi-20240507/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -538,14 +538,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -618,16 +620,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -647,15 +649,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libmodi/libmodi.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -897,23 +900,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/handle_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -997,17 +1003,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on handle_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(handle_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmodi-20240305/ossfuzz/ossfuzz_libmodi.h` & `libmodi-20240507/ossfuzz/ossfuzz_libmodi.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/ltmain.sh` & `libmodi-20240507/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha1_context.c` & `libmodi-20240507/libhmac/libhmac_sha1_context.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha224.h` & `libmodi-20240507/libhmac/libhmac_sha224.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha512_context.c` & `libmodi-20240507/libhmac/libhmac_sha512_context.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_extern.h` & `libmodi-20240507/libhmac/libhmac_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_md5.c` & `libmodi-20240507/libhmac/libhmac_md5.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_md5.h` & `libmodi-20240507/libhmac/libhmac_md5.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_error.h` & `libmodi-20240507/libhmac/libhmac_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_types.h` & `libmodi-20240507/libhmac/libhmac_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_byte_stream.h` & `libmodi-20240507/libhmac/libhmac_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha512.c` & `libmodi-20240507/libhmac/libhmac_sha512.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha256_context.c` & `libmodi-20240507/libhmac/libhmac_sha256_context.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha224.c` & `libmodi-20240507/libhmac/libhmac_sha224.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_definitions.h` & `libmodi-20240507/libhmac/libhmac_definitions.h`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBHMAC )
 #include <libhmac/definitions.h>
 
 /* The definitions in <libhmac/definitions.h> are copied here
  * for local use of libhmac
  */
 #else
-#define LIBHMAC_VERSION			20240129
+#define LIBHMAC_VERSION			20240417
 
 /* The libhmac version string
  */
-#define LIBHMAC_VERSION_STRING		"20240129"
+#define LIBHMAC_VERSION_STRING		"20240417"
 
 /* The digest hash sizes
  */
 #define LIBHMAC_MD5_HASH_SIZE		16
 #define LIBHMAC_SHA1_HASH_SIZE		20
 #define LIBHMAC_SHA224_HASH_SIZE	28
 #define LIBHMAC_SHA256_HASH_SIZE	32
```

### Comparing `libmodi-20240305/libhmac/libhmac_unused.h` & `libmodi-20240507/libhmac/libhmac_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha1.h` & `libmodi-20240507/libhmac/libhmac_sha1.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha256_context.h` & `libmodi-20240507/libhmac/libhmac_sha256_context.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/Makefile.am` & `libmodi-20240507/libhmac/Makefile.am`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBHMAC
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCRYPTO_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libhmac.la
 
 libhmac_la_SOURCES = \
@@ -25,19 +25,17 @@
 	libhmac_sha512.c libhmac_sha512.h \
 	libhmac_sha512_context.c libhmac_sha512_context.h \
 	libhmac_support.c libhmac_support.h \
 	libhmac_types.h \
 	libhmac_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libhmac ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libhmac_la_SOURCES)
```

### Comparing `libmodi-20240305/libhmac/libhmac_sha224_context.c` & `libmodi-20240507/libhmac/libhmac_sha224_context.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_md5_context.h` & `libmodi-20240507/libhmac/libhmac_md5_context.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha256.c` & `libmodi-20240507/libhmac/libhmac_sha256.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha1_context.h` & `libmodi-20240507/libhmac/libhmac_sha1_context.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_libcerror.h` & `libmodi-20240507/libhmac/libhmac_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_error.c` & `libmodi-20240507/libhmac/libhmac_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_support.h` & `libmodi-20240507/libhmac/libhmac_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/Makefile.in` & `libmodi-20240507/libhmac/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -548,14 +548,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -628,16 +630,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBHMAC_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBHMAC_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBHMAC_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBHMAC_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBHMAC_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@LIBCRYPTO_CPPFLAGS@ \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBHMAC_TRUE@noinst_LTLIBRARIES = libhmac.la
 @HAVE_LOCAL_LIBHMAC_TRUE@libhmac_la_SOURCES = \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_byte_stream.h \
@@ -655,15 +657,16 @@
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha256_context.c libhmac_sha256_context.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha512.c libhmac_sha512.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha512_context.c libhmac_sha512_context.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_support.c libhmac_support.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_types.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -874,24 +877,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libhmac_error.Plo
+	-rm -f ./$(DEPDIR)/libhmac_md5.Plo
+	-rm -f ./$(DEPDIR)/libhmac_md5_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha1.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha1_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha224.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha224_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha256.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha256_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha512.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha512_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -986,17 +1003,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libhmac ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libhmac_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libhmac/libhmac_sha256.h` & `libmodi-20240507/libhmac/libhmac_sha256.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha224_context.h` & `libmodi-20240507/libhmac/libhmac_sha224_context.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha512_context.h` & `libmodi-20240507/libhmac/libhmac_sha512_context.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha512.h` & `libmodi-20240507/libhmac/libhmac_sha512.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_support.c` & `libmodi-20240507/libhmac/libhmac_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_sha1.c` & `libmodi-20240507/libhmac/libhmac_sha1.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libhmac/libhmac_md5_context.c` & `libmodi-20240507/libhmac/libhmac_md5_context.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_narrow_string.c` & `libmodi-20240507/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_definitions.h` & `libmodi-20240507/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libmodi-20240305/libcsplit/libcsplit_types.h` & `libmodi-20240507/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_wide_split_string.c` & `libmodi-20240507/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_support.h` & `libmodi-20240507/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/Makefile.am` & `libmodi-20240507/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libmodi-20240305/libcsplit/libcsplit_libcerror.h` & `libmodi-20240507/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_wide_string.c` & `libmodi-20240507/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_unused.h` & `libmodi-20240507/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_wide_split_string.h` & `libmodi-20240507/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_error.c` & `libmodi-20240507/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_narrow_split_string.c` & `libmodi-20240507/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_extern.h` & `libmodi-20240507/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_error.h` & `libmodi-20240507/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_support.c` & `libmodi-20240507/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_wide_string.h` & `libmodi-20240507/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/Makefile.in` & `libmodi-20240507/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -535,14 +535,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -615,16 +617,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -633,15 +635,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -846,24 +849,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -952,17 +963,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libcsplit/libcsplit_narrow_split_string.h` & `libmodi-20240507/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcsplit/libcsplit_narrow_string.h` & `libmodi-20240507/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/po/remove-potcdate.sin` & `libmodi-20240507/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/po/Makefile.in.in` & `libmodi-20240507/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/po/en@quot.header` & `libmodi-20240507/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/po/en@boldquot.header` & `libmodi-20240507/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/po/insert-header.sin` & `libmodi-20240507/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/po/Makevars` & `libmodi-20240507/po/Makevars`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/po/Makevars.in` & `libmodi-20240507/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/po/Rules-quot` & `libmodi-20240507/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1251.c` & `libmodi-20240507/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_utf16_string.c` & `libmodi-20240507/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_base16_stream.c` & `libmodi-20240507/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_utf8_stream.h` & `libmodi-20240507/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_2.h` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_932.c` & `libmodi-20240507/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_dingbats.h` & `libmodi-20240507/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_utf8_string.c` & `libmodi-20240507/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_base64_stream.c` & `libmodi-20240507/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_error.h` & `libmodi-20240507/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_turkish.h` & `libmodi-20240507/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_unicode_character.c` & `libmodi-20240507/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_gaelic.c` & `libmodi-20240507/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_arabic.h` & `libmodi-20240507/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_thai.c` & `libmodi-20240507/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_874.h` & `libmodi-20240507/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_15.h` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_utf8_string.h` & `libmodi-20240507/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_16.c` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1255.c` & `libmodi-20240507/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_utf7_stream.c` & `libmodi-20240507/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_byte_stream.h` & `libmodi-20240507/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_koi8_u.c` & `libmodi-20240507/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_unused.h` & `libmodi-20240507/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_6.c` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_14.c` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_base64_stream.h` & `libmodi-20240507/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_error.c` & `libmodi-20240507/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_centraleurroman.h` & `libmodi-20240507/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_romanian.c` & `libmodi-20240507/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_6.h` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_9.c` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_russian.h` & `libmodi-20240507/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_dingbats.c` & `libmodi-20240507/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_15.c` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_936.c` & `libmodi-20240507/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_croatian.h` & `libmodi-20240507/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_scsu.h` & `libmodi-20240507/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/Makefile.am` & `libmodi-20240507/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libmodi-20240305/libuna/libuna_utf32_stream.c` & `libmodi-20240507/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_936.h` & `libmodi-20240507/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_10.c` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_roman.c` & `libmodi-20240507/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_utf7_stream.h` & `libmodi-20240507/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_3.h` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_thai.h` & `libmodi-20240507/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_farsi.h` & `libmodi-20240507/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_ukrainian.c` & `libmodi-20240507/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_inuit.c` & `libmodi-20240507/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_932.h` & `libmodi-20240507/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_874.c` & `libmodi-20240507/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_5.c` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_10.h` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_definitions.h` & `libmodi-20240507/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libmodi-20240305/libuna/libuna_url_stream.h` & `libmodi-20240507/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_icelandic.h` & `libmodi-20240507/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_koi8_u.h` & `libmodi-20240507/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_utf16_stream.c` & `libmodi-20240507/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1253.c` & `libmodi-20240507/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_4.h` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_greek.c` & `libmodi-20240507/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_libcerror.h` & `libmodi-20240507/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_centraleurroman.c` & `libmodi-20240507/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1254.c` & `libmodi-20240507/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_13.h` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_7.h` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1255.h` & `libmodi-20240507/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_unicode_character.h` & `libmodi-20240507/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_8.h` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_13.c` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_949.h` & `libmodi-20240507/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_cyrillic.c` & `libmodi-20240507/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_celtic.c` & `libmodi-20240507/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_support.h` & `libmodi-20240507/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_4.c` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_949.c` & `libmodi-20240507/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_utf16_stream.h` & `libmodi-20240507/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_symbol.c` & `libmodi-20240507/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_roman.h` & `libmodi-20240507/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1257.c` & `libmodi-20240507/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1254.h` & `libmodi-20240507/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_950.c` & `libmodi-20240507/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_extern.h` & `libmodi-20240507/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1256.c` & `libmodi-20240507/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_types.h` & `libmodi-20240507/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_base32_stream.h` & `libmodi-20240507/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1253.h` & `libmodi-20240507/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_16.h` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_utf8_stream.c` & `libmodi-20240507/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1250.h` & `libmodi-20240507/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_2.c` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_support.c` & `libmodi-20240507/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_koi8_r.c` & `libmodi-20240507/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_5.h` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_utf16_string.h` & `libmodi-20240507/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_utf32_string.c` & `libmodi-20240507/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_icelandic.c` & `libmodi-20240507/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1256.h` & `libmodi-20240507/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_utf32_string.h` & `libmodi-20240507/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_romanian.h` & `libmodi-20240507/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_8.c` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_koi8_r.h` & `libmodi-20240507/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_cyrillic.h` & `libmodi-20240507/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_arabic.c` & `libmodi-20240507/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_croatian.c` & `libmodi-20240507/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_9.h` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_greek.h` & `libmodi-20240507/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1258.h` & `libmodi-20240507/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_7.c` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/Makefile.in` & `libmodi-20240507/libuna/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -703,14 +703,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -783,16 +785,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -858,15 +860,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1128,24 +1131,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1291,17 +1359,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_3.c` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1250.c` & `libmodi-20240507/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_scsu.c` & `libmodi-20240507/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1252.c` & `libmodi-20240507/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_turkish.c` & `libmodi-20240507/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_ukrainian.h` & `libmodi-20240507/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_russian.c` & `libmodi-20240507/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1258.c` & `libmodi-20240507/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_celtic.h` & `libmodi-20240507/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_byte_stream.c` & `libmodi-20240507/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_gaelic.h` & `libmodi-20240507/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_utf32_stream.h` & `libmodi-20240507/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_symbol.h` & `libmodi-20240507/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1257.h` & `libmodi-20240507/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_inuit.h` & `libmodi-20240507/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_mac_farsi.c` & `libmodi-20240507/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_950.h` & `libmodi-20240507/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_url_stream.c` & `libmodi-20240507/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1251.h` & `libmodi-20240507/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_windows_1252.h` & `libmodi-20240507/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_codepage_iso_8859_14.h` & `libmodi-20240507/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_base16_stream.h` & `libmodi-20240507/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libuna/libuna_base32_stream.c` & `libmodi-20240507/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/Makefile.in` & `libmodi-20240507/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -585,14 +585,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -733,16 +735,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libmodi.pc \
+	libmodi.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libmodi.pc
 
 all: all-recursive
 
@@ -1159,23 +1168,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1292,22 +1304,10 @@
 	(cd $(srcdir)/libfmos && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfplist && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libhmac && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcaes && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libmodi && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libmodi.pc
-	-rm -f libmodi.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmodi-20240305/libfvalue/libfvalue_filetime.c` & `libmodi-20240507/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_utf16_string.c` & `libmodi-20240507/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_libfwnt.h` & `libmodi-20240507/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_value.c` & `libmodi-20240507/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_value.h` & `libmodi-20240507/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_definitions.h` & `libmodi-20240507/libfvalue/libfvalue_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfvalue/definitions.h> are copied here
  * for local use of libfvalue
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFVALUE_VERSION						20240124
+#define LIBFVALUE_VERSION						20240415
 
 /* The libfvalue version string
  */
-#define LIBFVALUE_VERSION_STRING					"20240124"
+#define LIBFVALUE_VERSION_STRING					"20240415"
 
 /* The endian definitions
  */
 #define LIBFVALUE_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFVALUE_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 #define LIBFVALUE_ENDIAN_NATIVE						(uint8_t) 'n'
```

### Comparing `libmodi-20240305/libfvalue/libfvalue_codepage.h` & `libmodi-20240507/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_split_utf16_string.c` & `libmodi-20240507/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_error.c` & `libmodi-20240507/libfvalue/libfvalue_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_utf8_string.c` & `libmodi-20240507/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_unused.h` & `libmodi-20240507/libfvalue/libfvalue_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_split_utf16_string.h` & `libmodi-20240507/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_filetime.h` & `libmodi-20240507/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_support.c` & `libmodi-20240507/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_extern.h` & `libmodi-20240507/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/Makefile.am` & `libmodi-20240507/libfvalue/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFVALUE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
@@ -39,19 +39,17 @@
 	libfvalue_value_type.c libfvalue_value_type.h \
 	libfvalue_support.c libfvalue_support.h \
 	libfvalue_unused.h \
 	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 	libfvalue_utf16_string.c libfvalue_utf16_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
```

### Comparing `libmodi-20240305/libfvalue/libfvalue_value_type.h` & `libmodi-20240507/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_libcerror.h` & `libmodi-20240507/libfvalue/libfvalue_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_split_utf8_string.c` & `libmodi-20240507/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_data_handle.h` & `libmodi-20240507/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_libcnotify.h` & `libmodi-20240507/libfvalue/libfvalue_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_data_handle.c` & `libmodi-20240507/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_integer.c` & `libmodi-20240507/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_value_type.c` & `libmodi-20240507/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_integer.h` & `libmodi-20240507/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_binary_data.h` & `libmodi-20240507/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_value_entry.h` & `libmodi-20240507/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_utf16_string.h` & `libmodi-20240507/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_error.h` & `libmodi-20240507/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_table.h` & `libmodi-20240507/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_libfguid.h` & `libmodi-20240507/libfvalue/libfvalue_libfguid.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_split_utf8_string.h` & `libmodi-20240507/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_floating_point.h` & `libmodi-20240507/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_libfdatetime.h` & `libmodi-20240507/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_string.h` & `libmodi-20240507/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_binary_data.c` & `libmodi-20240507/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_value_entry.c` & `libmodi-20240507/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_libcdata.h` & `libmodi-20240507/libfvalue/libfvalue_libcdata.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_support.h` & `libmodi-20240507/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_table.c` & `libmodi-20240507/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/Makefile.in` & `libmodi-20240507/libfvalue/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -566,14 +566,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -646,16 +648,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBFVALUE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFGUID_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@PTHREAD_CPPFLAGS@ 
@@ -687,15 +689,16 @@
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_entry.c libfvalue_value_entry.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_type.c libfvalue_value_type.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_support.c libfvalue_support.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_unused.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.c libfvalue_utf16_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -910,24 +913,42 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfvalue_binary_data.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_error.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_floating_point.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_integer.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_support.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_table.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_entry.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1026,17 +1047,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libfvalue/libfvalue_utf8_string.h` & `libmodi-20240507/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_floating_point.c` & `libmodi-20240507/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_types.h` & `libmodi-20240507/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_string.c` & `libmodi-20240507/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libfvalue/libfvalue_libuna.h` & `libmodi-20240507/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcnotify/libcnotify_definitions.h` & `libmodi-20240507/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libmodi-20240305/libcnotify/libcnotify_extern.h` & `libmodi-20240507/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcnotify/libcnotify_support.c` & `libmodi-20240507/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcnotify/libcnotify_stream.h` & `libmodi-20240507/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcnotify/Makefile.am` & `libmodi-20240507/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libmodi-20240305/libcnotify/libcnotify_unused.h` & `libmodi-20240507/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcnotify/libcnotify_verbose.h` & `libmodi-20240507/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcnotify/libcnotify_print.h` & `libmodi-20240507/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcnotify/libcnotify_stream.c` & `libmodi-20240507/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcnotify/libcnotify_support.h` & `libmodi-20240507/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcnotify/libcnotify_verbose.c` & `libmodi-20240507/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcnotify/Makefile.in` & `libmodi-20240507/libcnotify/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -527,14 +527,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -607,30 +609,31 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -833,24 +836,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -937,17 +946,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libcnotify/libcnotify_libcerror.h` & `libmodi-20240507/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcnotify/libcnotify_print.c` & `libmodi-20240507/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libmodi.spec.in` & `libmodi-20240507/libmodi.spec.in`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcerror/libcerror_system.c` & `libmodi-20240507/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcerror/libcerror_error.c` & `libmodi-20240507/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcerror/libcerror_extern.h` & `libmodi-20240507/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcerror/Makefile.am` & `libmodi-20240507/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libmodi-20240305/libcerror/libcerror_types.h` & `libmodi-20240507/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcerror/libcerror_support.h` & `libmodi-20240507/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcerror/libcerror_error.h` & `libmodi-20240507/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcerror/libcerror_system.h` & `libmodi-20240507/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcerror/libcerror_definitions.h` & `libmodi-20240507/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libmodi-20240305/libcerror/libcerror_support.c` & `libmodi-20240507/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcerror/libcerror_unused.h` & `libmodi-20240507/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcerror/Makefile.in` & `libmodi-20240507/libcerror/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -524,14 +524,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -604,28 +606,29 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -827,24 +830,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -930,17 +938,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/aclocal.m4` & `libmodi-20240507/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/configure.ac` & `libmodi-20240507/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libmodi],
- [20240305],
+ [20240507],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libmodi.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_directory_entry.c` & `libmodi-20240507/libcdirectory/libcdirectory_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_system_string.c` & `libmodi-20240507/libcdirectory/libcdirectory_system_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_extern.h` & `libmodi-20240507/libcdirectory/libcdirectory_extern.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_system_string.h` & `libmodi-20240507/libcdirectory/libcdirectory_system_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_unused.h` & `libmodi-20240507/libcdirectory/libcdirectory_unused.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/Makefile.am` & `libmodi-20240507/libcdirectory/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDIRECTORY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdirectory.la
 
 libcdirectory_la_SOURCES = \
@@ -20,19 +20,17 @@
 	libcdirectory_support.c libcdirectory_support.h \
 	libcdirectory_system_string.c libcdirectory_system_string.h \
 	libcdirectory_types.h \
 	libcdirectory_unused.h \
 	libcdirectory_wide_string.c libcdirectory_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdirectory ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdirectory_la_SOURCES)
```

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_types.h` & `libmodi-20240507/libcdirectory/libcdirectory_types.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_support.c` & `libmodi-20240507/libcdirectory/libcdirectory_support.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_libclocale.h` & `libmodi-20240507/libcdirectory/libcdirectory_libclocale.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_definitions.h` & `libmodi-20240507/libcdirectory/libcdirectory_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdirectory/definitions.h>
 
 /* The definitions in <libcdirectory/definitions.h> are copied here
  * for local use of libcdirectory
  */
 #else
 
-#define LIBCDIRECTORY_VERSION				20240105
+#define LIBCDIRECTORY_VERSION				20240414
 
 /* The libcdirectory version string
  */
-#define LIBCDIRECTORY_VERSION_STRING			"20240105"
+#define LIBCDIRECTORY_VERSION_STRING			"20240414"
 
 /* The directory entry type definitions
  */
 enum LIBCDIRECTORY_ENTRY_TYPES
 {
 	LIBCDIRECTORY_ENTRY_TYPE_UNDEFINED,
 	LIBCDIRECTORY_ENTRY_TYPE_DEVICE,
```

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_error.c` & `libmodi-20240507/libcdirectory/libcdirectory_error.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_libcerror.h` & `libmodi-20240507/libcdirectory/libcdirectory_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_directory.h` & `libmodi-20240507/libcdirectory/libcdirectory_directory.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_wide_string.c` & `libmodi-20240507/libcdirectory/libcdirectory_wide_string.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_wide_string.h` & `libmodi-20240507/libcdirectory/libcdirectory_wide_string.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_support.h` & `libmodi-20240507/libcdirectory/libcdirectory_support.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_directory.c` & `libmodi-20240507/libcdirectory/libcdirectory_directory.c`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/Makefile.in` & `libmodi-20240507/libcdirectory/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -536,14 +536,16 @@
 bzip2_CFLAGS = @bzip2_CFLAGS@
 bzip2_LIBS = @bzip2_LIBS@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -616,16 +618,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDIRECTORY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDIRECTORY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDIRECTORY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDIRECTORY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@noinst_LTLIBRARIES = libcdirectory.la
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@libcdirectory_la_SOURCES = \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_definitions.h \
@@ -638,15 +640,16 @@
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_libuna.h \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_support.c libcdirectory_support.h \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_system_string.c libcdirectory_system_string.h \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_types.h \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_unused.h \
 @HAVE_LOCAL_LIBCDIRECTORY_TRUE@	libcdirectory_wide_string.c libcdirectory_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -851,24 +854,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdirectory_directory.Plo
+	-rm -f ./$(DEPDIR)/libcdirectory_directory_entry.Plo
+	-rm -f ./$(DEPDIR)/libcdirectory_error.Plo
+	-rm -f ./$(DEPDIR)/libcdirectory_support.Plo
+	-rm -f ./$(DEPDIR)/libcdirectory_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcdirectory_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -957,17 +968,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdirectory ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdirectory_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_error.h` & `libmodi-20240507/libcdirectory/libcdirectory_error.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_libuna.h` & `libmodi-20240507/libcdirectory/libcdirectory_libuna.h`

 * *Files identical despite different names*

### Comparing `libmodi-20240305/libcdirectory/libcdirectory_directory_entry.h` & `libmodi-20240507/libcdirectory/libcdirectory_directory_entry.h`

 * *Files identical despite different names*

