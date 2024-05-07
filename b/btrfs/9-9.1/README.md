# Comparing `tmp/btrfs-9.tar.gz` & `tmp/btrfs-9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/btrfs-9.tar", last modified: Fri Nov 24 13:04:33 2017, max compression
+gzip compressed data, was "dist/btrfs-9.1.tar", last modified: Mon Dec  3 22:45:39 2018, max compression
```

## Comparing `btrfs-9.tar` & `btrfs-9.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2017-11-24 13:04:33.000000 btrfs-9/
-drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2017-11-24 13:04:33.000000 btrfs-9/btrfs/
--rw-r--r--   0 knorrie   (1000) knorrie   (1000)     1392 2017-09-22 13:27:59.000000 btrfs-9/btrfs/__init__.py
--rw-r--r--   0 knorrie   (1000) knorrie   (1000)     4528 2017-11-23 22:57:17.000000 btrfs-9/btrfs/crc32c.py
--rw-r--r--   0 knorrie   (1000) knorrie   (1000)    44837 2017-11-23 22:57:17.000000 btrfs-9/btrfs/ctree.py
--rw-r--r--   0 knorrie   (1000) knorrie   (1000)     1370 2017-09-22 13:27:59.000000 btrfs-9/btrfs/free_space_tree.py
--rw-r--r--   0 knorrie   (1000) knorrie   (1000)    25544 2017-11-23 22:57:17.000000 btrfs-9/btrfs/ioctl.py
--rw-r--r--   0 knorrie   (1000) knorrie   (1000)     8856 2017-11-23 22:57:17.000000 btrfs-9/btrfs/utils.py
-drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2017-11-24 13:04:33.000000 btrfs-9/examples/
-drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2017-11-24 13:04:33.000000 btrfs-9/examples/munin/
-drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2017-11-24 13:04:33.000000 btrfs-9/examples/munin/plugin-conf.d/
--rw-r--r--   0 knorrie   (1000) knorrie   (1000)       24 2016-07-07 23:37:35.000000 btrfs-9/examples/munin/plugin-conf.d/btrfs_usage
-drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2017-11-24 13:04:33.000000 btrfs-9/examples/munin/plugins/
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     4366 2017-11-23 22:57:17.000000 btrfs-9/examples/munin/plugins/btrfs_usage
-drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2017-11-24 13:04:33.000000 btrfs-9/examples/nagios/
-drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2017-11-24 13:04:33.000000 btrfs-9/examples/nagios/plugins/
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     6581 2017-11-23 22:57:17.000000 btrfs-9/examples/nagios/plugins/check_btrfs
--rw-r--r--   0 knorrie   (1000) knorrie   (1000)      712 2017-08-29 21:35:05.000000 btrfs-9/examples/README.txt
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     2995 2017-09-22 13:27:59.000000 btrfs-9/examples/balance_least_used.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1812 2017-08-29 21:35:05.000000 btrfs-9/examples/block_group_search_timing.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      214 2017-08-29 21:35:05.000000 btrfs-9/examples/btrfs-fi-df-simple.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     2570 2017-08-29 21:35:05.000000 btrfs-9/examples/btrfs-fi-df.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      197 2017-08-29 21:35:05.000000 btrfs-9/examples/dir_item_name_hash.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1331 2017-11-23 22:57:17.000000 btrfs-9/examples/dump_tree.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      316 2017-08-29 21:35:05.000000 btrfs-9/examples/fs_info.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      261 2017-09-22 13:27:59.000000 btrfs-9/examples/inode_extref_hash.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1584 2017-11-23 22:57:17.000000 btrfs-9/examples/set_received_uuid.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1473 2017-08-29 21:35:05.000000 btrfs-9/examples/show_block_group_contents.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     2970 2017-11-23 22:57:17.000000 btrfs-9/examples/show_block_group_data_extent_filenames.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      491 2017-11-23 22:57:17.000000 btrfs-9/examples/show_block_group_free_space_extents.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      255 2017-08-29 21:35:05.000000 btrfs-9/examples/show_block_groups.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      272 2017-08-29 21:35:05.000000 btrfs-9/examples/show_chunk_tree_keys.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      630 2017-11-23 22:57:17.000000 btrfs-9/examples/show_default_subvolid.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      475 2017-11-12 12:33:03.000000 btrfs-9/examples/show_dev_extents.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1540 2017-11-18 14:40:55.000000 btrfs-9/examples/show_directory_contents.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      531 2017-08-29 21:35:05.000000 btrfs-9/examples/show_extent_tree_keys.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1661 2017-11-23 22:57:17.000000 btrfs-9/examples/show_file.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1535 2017-11-23 22:57:17.000000 btrfs-9/examples/show_file_by_inode.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     7209 2017-11-23 22:57:17.000000 btrfs-9/examples/show_file_csum.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     2963 2017-11-23 22:57:17.000000 btrfs-9/examples/show_free_space_fragmentation.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     2320 2017-09-22 13:27:59.000000 btrfs-9/examples/show_metadata_tree_sizes.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1653 2017-09-22 13:27:59.000000 btrfs-9/examples/show_orphan_cleaner_progress.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      205 2017-08-29 21:35:05.000000 btrfs-9/examples/show_orphaned_subvols.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      225 2017-08-29 21:35:05.000000 btrfs-9/examples/show_subvolumes.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      332 2017-10-16 19:43:40.000000 btrfs-9/examples/show_tree_keys.py
--rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      406 2017-08-29 21:35:05.000000 btrfs-9/examples/show_usage.py
--rw-r--r--   0 knorrie   (1000) knorrie   (1000)     1196 2017-08-29 21:35:05.000000 btrfs-9/README.md
--rw-r--r--   0 knorrie   (1000) knorrie   (1000)     1004 2017-11-23 22:57:17.000000 btrfs-9/setup.py
--rw-r--r--   0 knorrie   (1000) knorrie   (1000)     2299 2017-11-24 13:04:33.000000 btrfs-9/PKG-INFO
+drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2018-12-03 22:45:39.000000 btrfs-9.1/
+drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2018-12-03 22:45:39.000000 btrfs-9.1/btrfs/
+-rw-r--r--   0 knorrie   (1000) knorrie   (1000)     1392 2018-12-03 22:43:28.000000 btrfs-9.1/btrfs/__init__.py
+-rw-r--r--   0 knorrie   (1000) knorrie   (1000)     4528 2018-06-29 15:47:11.000000 btrfs-9.1/btrfs/crc32c.py
+-rw-r--r--   0 knorrie   (1000) knorrie   (1000)    45040 2018-12-03 22:43:28.000000 btrfs-9.1/btrfs/ctree.py
+-rw-r--r--   0 knorrie   (1000) knorrie   (1000)     1370 2017-09-22 13:27:59.000000 btrfs-9.1/btrfs/free_space_tree.py
+-rw-r--r--   0 knorrie   (1000) knorrie   (1000)    25468 2018-12-03 22:43:28.000000 btrfs-9.1/btrfs/ioctl.py
+-rw-r--r--   0 knorrie   (1000) knorrie   (1000)     8850 2018-12-03 22:43:28.000000 btrfs-9.1/btrfs/utils.py
+drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2018-12-03 22:45:39.000000 btrfs-9.1/examples/
+drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2018-12-03 22:45:39.000000 btrfs-9.1/examples/munin/
+drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2018-12-03 22:45:39.000000 btrfs-9.1/examples/munin/plugin-conf.d/
+-rw-r--r--   0 knorrie   (1000) knorrie   (1000)       24 2016-07-07 23:37:35.000000 btrfs-9.1/examples/munin/plugin-conf.d/btrfs_usage
+drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2018-12-03 22:45:39.000000 btrfs-9.1/examples/munin/plugins/
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     4366 2018-12-03 22:43:28.000000 btrfs-9.1/examples/munin/plugins/btrfs_usage
+drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2018-12-03 22:45:39.000000 btrfs-9.1/examples/nagios/
+drwxr-xr-x   0 knorrie   (1000) knorrie   (1000)        0 2018-12-03 22:45:39.000000 btrfs-9.1/examples/nagios/plugins/
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     6581 2018-12-03 22:43:28.000000 btrfs-9.1/examples/nagios/plugins/check_btrfs
+-rw-r--r--   0 knorrie   (1000) knorrie   (1000)      712 2017-08-29 21:35:05.000000 btrfs-9.1/examples/README.txt
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     2995 2018-11-24 17:59:45.000000 btrfs-9.1/examples/balance_least_used.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1812 2017-08-29 21:35:05.000000 btrfs-9.1/examples/block_group_search_timing.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      214 2018-11-10 00:08:04.000000 btrfs-9.1/examples/btrfs-fi-df-simple.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     2570 2018-12-03 22:43:28.000000 btrfs-9.1/examples/btrfs-fi-df.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      197 2017-08-29 21:35:05.000000 btrfs-9.1/examples/dir_item_name_hash.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1331 2018-11-10 00:08:04.000000 btrfs-9.1/examples/dump_tree.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      316 2018-11-10 00:08:04.000000 btrfs-9.1/examples/fs_info.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      261 2017-09-22 13:27:59.000000 btrfs-9.1/examples/inode_extref_hash.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1584 2018-11-10 00:08:04.000000 btrfs-9.1/examples/set_received_uuid.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1473 2018-11-10 00:08:04.000000 btrfs-9.1/examples/show_block_group_contents.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     2970 2018-06-29 15:47:11.000000 btrfs-9.1/examples/show_block_group_data_extent_filenames.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      491 2018-06-29 15:47:11.000000 btrfs-9.1/examples/show_block_group_free_space_extents.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      255 2018-12-03 22:43:28.000000 btrfs-9.1/examples/show_block_groups.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      272 2017-08-29 21:35:05.000000 btrfs-9.1/examples/show_chunk_tree_keys.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      630 2018-06-29 15:47:11.000000 btrfs-9.1/examples/show_default_subvolid.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      475 2017-11-12 12:33:03.000000 btrfs-9.1/examples/show_dev_extents.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1540 2017-11-18 14:40:55.000000 btrfs-9.1/examples/show_directory_contents.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      531 2017-08-29 21:35:05.000000 btrfs-9.1/examples/show_extent_tree_keys.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1661 2018-06-29 15:47:11.000000 btrfs-9.1/examples/show_file.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1535 2018-06-29 15:47:11.000000 btrfs-9.1/examples/show_file_by_inode.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     7209 2018-06-29 15:47:11.000000 btrfs-9.1/examples/show_file_csum.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     3159 2018-10-20 14:12:03.000000 btrfs-9.1/examples/show_free_space_fragmentation.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     2320 2017-09-22 13:27:59.000000 btrfs-9.1/examples/show_metadata_tree_sizes.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)     1653 2017-09-22 13:27:59.000000 btrfs-9.1/examples/show_orphan_cleaner_progress.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      205 2017-08-29 21:35:05.000000 btrfs-9.1/examples/show_orphaned_subvols.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      225 2017-08-29 21:35:05.000000 btrfs-9.1/examples/show_subvolumes.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      332 2018-05-11 21:59:51.000000 btrfs-9.1/examples/show_tree_keys.py
+-rwxr-xr-x   0 knorrie   (1000) knorrie   (1000)      406 2018-12-03 22:43:28.000000 btrfs-9.1/examples/show_usage.py
+-rw-r--r--   0 knorrie   (1000) knorrie   (1000)     1196 2017-08-29 21:35:05.000000 btrfs-9.1/README.md
+-rw-r--r--   0 knorrie   (1000) knorrie   (1000)     1008 2018-11-03 16:50:30.000000 btrfs-9.1/setup.py
+-rw-r--r--   0 knorrie   (1000) knorrie   (1000)     2303 2018-12-03 22:45:39.000000 btrfs-9.1/PKG-INFO
```

### Comparing `btrfs-9/btrfs/__init__.py` & `btrfs-9.1/btrfs/__init__.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/btrfs/crc32c.py` & `btrfs-9.1/btrfs/crc32c.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/btrfs/ctree.py` & `btrfs-9.1/btrfs/ctree.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public
 # License along with this program; if not, write to the
 # Free Software Foundation, Inc., 51 Franklin Street, Fifth Floor,
 # Boston, MA 02110-1301 USA
 
+import btrfs
 import collections.abc
 import copy
 import datetime
 import os
 import struct
 import uuid
 
@@ -27,14 +28,22 @@
 ULONG_MAX = (1 << 32) - 1
 
 
 def ULL(n):
     return n & ULLONG_MAX
 
 
+def struct_format(s):
+    f = s.format
+    # Python <= 3.6 returns bytes, 3.7 returns str, yay.
+    if type(f) == bytes:
+        return f.decode('utf-8')
+    return f
+
+
 ROOT_TREE_OBJECTID = 1
 EXTENT_TREE_OBJECTID = 2
 CHUNK_TREE_OBJECTID = 3
 DEV_TREE_OBJECTID = 4
 FS_TREE_OBJECTID = 5
 ROOT_TREE_DIR_OBJECTID = 6
 CSUM_TREE_OBJECTID = 7
@@ -348,18 +357,14 @@
         return _key_objectid_str_map.get(offset, str(offset))
     if offset == ULLONG_MAX:
         return '-1'
 
     return str(offset)
 
 
-import btrfs.ioctl  # noqa
-import btrfs.free_space_tree  # noqa
-
-
 class Key(object):
     def __init__(self, objectid, _type, offset):
         self._objectid = objectid
         self._type = _type
         self._offset = offset
         self._pack()
 
@@ -942,15 +947,16 @@
     _inode_item = [
         struct.Struct('<5Q4L3Q32x'),
         TimeSpec.timespec,
         TimeSpec.timespec,
         TimeSpec.timespec,
         TimeSpec.timespec,
     ]
-    inode_item = struct.Struct('<' + ''.join([s.format[1:].decode() for s in _inode_item]))
+    inode_item = struct.Struct('<' + ''.join([struct_format(s)[1:]
+                                              for s in _inode_item]))
 
     def __init__(self, header, data):
         super().__init__(header)
         self.generation, self.transid, self.size, self.nbytes, self.block_group, \
             self.nlink, self.uid, self.gid, self.mode, self.rdev, self.flags, self.sequence = \
             InodeItem._inode_item[0].unpack_from(data)
         pos = InodeItem._inode_item[0].size
@@ -1110,15 +1116,15 @@
 
 
 class DirItem(object):
     _dir_item = [
         DiskKey.disk_key,
         struct.Struct('<QHHB')
     ]
-    dir_item = struct.Struct('<' + ''.join([s.format[1:].decode() for s in _dir_item]))
+    dir_item = struct.Struct('<' + ''.join([struct_format(s)[1:] for s in _dir_item]))
 
     def __init__(self, data, pos):
         next_pos = pos + DiskKey.disk_key.size
         self.location = DiskKey(data[pos:next_pos])
         pos = next_pos
         self.transid, self.data_len, self.name_len, self.type = \
             DirItem._dir_item[1].unpack_from(data, pos)
@@ -1184,15 +1190,16 @@
         DiskKey.disk_key,
         struct.Struct('<BBQ16s16s16s4Q'),
         TimeSpec.timespec,
         TimeSpec.timespec,
         TimeSpec.timespec,
         TimeSpec.timespec,
     ]
-    root_item = struct.Struct('<' + ''.join([s.format[1:].decode() for s in _root_item]))
+    root_item = struct.Struct('<' + ''.join([struct_format(s)[1:]
+                                             for s in _root_item]))
 
     def __init__(self, header, data):
         super().__init__(header)
         self.inode = InodeItem(None, data[:InodeItem.inode_item.size])
         pos = InodeItem.inode_item.size
         self.generation, self.dirid, self.bytenr, self.byte_limit, self.bytes_used, \
             self.last_snapshot, self.flags, self.refs = \
@@ -1227,15 +1234,15 @@
 
 
 class FileExtentItem(ItemData):
     _file_extent_item = [
         struct.Struct('<QQBB2xB'),
         struct.Struct('<4Q'),
     ]
-    file_extent_item = struct.Struct('<' + ''.join([s.format[1:].decode()
+    file_extent_item = struct.Struct('<' + ''.join([struct_format(s)[1:]
                                                     for s in _file_extent_item]))
 
     def __init__(self, header, data):
         super().__init__(header)
         self.logical_offset = header.offset
         self.generation, self.ram_bytes, self.compression, self.encryption, self.type = \
             FileExtentItem._file_extent_item[0].unpack_from(data)
```

### Comparing `btrfs-9/btrfs/free_space_tree.py` & `btrfs-9.1/btrfs/free_space_tree.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/btrfs/ioctl.py` & `btrfs-9.1/btrfs/ioctl.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # You should have received a copy of the GNU General Public
 # License along with this program; if not, write to the
 # Free Software Foundation, Inc., 51 Franklin Street, Fifth Floor,
 # Boston, MA 02110-1301 USA
 
 from collections import namedtuple
 import array
+import btrfs
 import errno
 import fcntl
 import platform
 import struct
 import uuid
 
 ULLONG_MAX = (1 << 64) - 1
@@ -83,19 +84,14 @@
 
 def _IOWR(_type, nr, _struct):
     return _IOC(_IOC_READ | _IOC_WRITE, _type, nr, _struct.size)
 
 
 DEVICE_PATH_NAME_MAX = 1024
 
-from btrfs.ctree import BLOCK_GROUP_TYPE_MASK, SPACE_INFO_GLOBAL_RSV, BLOCK_GROUP_PROFILE_MASK  # noqa
-from btrfs.ctree import FIRST_FREE_OBJECTID  # noqa
-import btrfs.ctree  # noqa
-
-
 ioctl_fs_info_args = struct.Struct('=QQ16sLLL980x')
 IOC_FS_INFO = _IOR(BTRFS_IOCTL_MAGIC, 31, ioctl_fs_info_args)
 
 
 class FsInfo(object):
     def __init__(self, buf):
         self.max_id, self.num_devices, fsid_bytes, self.nodesize, self.sectorsize, \
@@ -176,16 +172,17 @@
 IOC_SPACE_INFO = _IOWR(BTRFS_IOCTL_MAGIC, 20, ioctl_space_args)
 SpaceArgs = namedtuple('SpaceArgs', ['space_slots', 'total_spaces'])
 
 
 class SpaceInfo(object):
     def __init__(self, buf, pos):
         self.flags, self.total_bytes, self.used_bytes = ioctl_space_info.unpack_from(buf, pos)
-        self.type = self.flags & (BLOCK_GROUP_TYPE_MASK | SPACE_INFO_GLOBAL_RSV)
-        self.profile = self.flags & BLOCK_GROUP_PROFILE_MASK
+        self.type = self.flags & \
+            (btrfs.ctree.BLOCK_GROUP_TYPE_MASK | btrfs.ctree.SPACE_INFO_GLOBAL_RSV)
+        self.profile = self.flags & btrfs.ctree.BLOCK_GROUP_PROFILE_MASK
         self.ratio = btrfs.utils.block_group_profile_ratio(self.profile)
         self.raw_total_bytes = self.total_bytes * self.ratio
         self.raw_used_bytes = self.used_bytes * self.ratio
 
     def __str__(self):
         return "{0}, {1}: total={2}, used={3}".format(
             btrfs.utils.block_group_type_str(self.flags),
@@ -208,15 +205,15 @@
     fcntl.ioctl(fd, IOC_SPACE_INFO, buf)
     return [SpaceInfo(buf, pos)
             for pos in range(ioctl_space_args.size, buf_size, ioctl_space_info.size)]
 
 
 ioctl_search_key = struct.Struct('=Q6QLLL4x32x')
 ioctl_search_args = struct.Struct('{0}{1}x'.format(
-    ioctl_search_key.format.decode(), 4096 - ioctl_search_key.size))
+    btrfs.ctree.struct_format(ioctl_search_key), 4096 - ioctl_search_key.size))
 ioctl_search_header = struct.Struct('=3Q2L')
 IOC_TREE_SEARCH = _IOWR(BTRFS_IOCTL_MAGIC, 17, ioctl_search_args)
 SearchHeader = namedtuple('SearchHeader', ['transid', 'objectid', 'offset', 'type', 'len'])
 
 
 def search(fd, tree, min_key=None, max_key=None,
            min_transid=0, max_transid=ULLONG_MAX,
@@ -225,15 +222,15 @@
                      nr_items, _v2=False)
 
 
 _ioctl_search_args_v2 = [
     ioctl_search_key,
     struct.Struct('=Q')
 ]
-ioctl_search_args_v2 = struct.Struct('=' + ''.join([s.format[1:].decode()
+ioctl_search_args_v2 = struct.Struct('=' + ''.join([btrfs.ctree.struct_format(s)[1:]
                                                     for s in _ioctl_search_args_v2]))
 IOC_TREE_SEARCH_V2 = _IOWR(BTRFS_IOCTL_MAGIC, 17, ioctl_search_args_v2)
 
 
 def search_v2(fd, tree, min_key=None, max_key=None,
               min_transid=0, max_transid=ULLONG_MAX,
               nr_items=ULONG_MAX, buf_size=None, _v2=True):
@@ -323,15 +320,15 @@
 
 INO_LOOKUP_PATH_MAX = 4080
 ioctl_ino_lookup_args = struct.Struct('=QQ{}s'.format(INO_LOOKUP_PATH_MAX))
 IOC_INO_LOOKUP = _IOWR(BTRFS_IOCTL_MAGIC, 18, ioctl_ino_lookup_args)
 InoLookupResult = namedtuple('InoLookupResult', ['treeid', 'name_bytes'])
 
 
-def ino_lookup(fd, treeid=0, objectid=FIRST_FREE_OBJECTID):
+def ino_lookup(fd, treeid=0, objectid=btrfs.ctree.FIRST_FREE_OBJECTID):
     args = bytearray(ioctl_ino_lookup_args.size)
     ioctl_ino_lookup_args.pack_into(args, 0, treeid, objectid, b'')
     fcntl.ioctl(fd, IOC_INO_LOOKUP, args)
     treeid, _, name_bytes = ioctl_ino_lookup_args.unpack_from(args, 0)
     return InoLookupResult(treeid, name_bytes.split(b'\0', 1)[0])
 
 
@@ -556,15 +553,15 @@
     struct.Struct('=Q'),  # 1 - state - out
     _balance_args,  # 2 - data - in/out
     _balance_args,  # 3 - meta - in/out
     _balance_args,  # 4 - sys - in/out
     _balance_progress,  # 5 - stat - out
     struct.Struct('=576x')
 ]
-ioctl_balance_args = struct.Struct('=' + ''.join([s.format[1:].decode()
+ioctl_balance_args = struct.Struct('=' + ''.join([btrfs.ctree.struct_format(s)[1:]
                                                   for s in _ioctl_balance_args]))
 IOC_BALANCE_V2 = _IOWR(BTRFS_IOCTL_MAGIC, 32, ioctl_balance_args)
 
 
 class BalanceError(Exception):
     def __init__(self, state, msg):
         self.state = state
```

### Comparing `btrfs-9/btrfs/utils.py` & `btrfs-9.1/btrfs/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public
 # License along with this program; if not, write to the
 # Free Software Foundation, Inc., 51 Franklin Street, Fifth Floor,
 # Boston, MA 02110-1301 USA
 
-import btrfs.ctree
+import btrfs
 import collections.abc
 import types
 from btrfs.ctree import (
     BLOCK_GROUP_DATA, BLOCK_GROUP_SYSTEM, BLOCK_GROUP_METADATA,
     SPACE_INFO_GLOBAL_RSV, BLOCK_GROUP_TYPE_MASK,
     BLOCK_GROUP_RAID0, BLOCK_GROUP_RAID1, BLOCK_GROUP_RAID5,
     BLOCK_GROUP_RAID6, BLOCK_GROUP_DUP, BLOCK_GROUP_RAID10,
```

### Comparing `btrfs-9/examples/munin/plugins/btrfs_usage` & `btrfs-9.1/examples/munin/plugins/btrfs_usage`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/nagios/plugins/check_btrfs` & `btrfs-9.1/examples/nagios/plugins/check_btrfs`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/README.txt` & `btrfs-9.1/examples/README.txt`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/balance_least_used.py` & `btrfs-9.1/examples/balance_least_used.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/block_group_search_timing.py` & `btrfs-9.1/examples/block_group_search_timing.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/btrfs-fi-df.py` & `btrfs-9.1/examples/btrfs-fi-df.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/dump_tree.py` & `btrfs-9.1/examples/dump_tree.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/set_received_uuid.py` & `btrfs-9.1/examples/set_received_uuid.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/show_block_group_contents.py` & `btrfs-9.1/examples/show_block_group_contents.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/show_block_group_data_extent_filenames.py` & `btrfs-9.1/examples/show_block_group_data_extent_filenames.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/show_default_subvolid.py` & `btrfs-9.1/examples/show_default_subvolid.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/show_directory_contents.py` & `btrfs-9.1/examples/show_directory_contents.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/show_extent_tree_keys.py` & `btrfs-9.1/examples/show_extent_tree_keys.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/show_file.py` & `btrfs-9.1/examples/show_file.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/show_file_by_inode.py` & `btrfs-9.1/examples/show_file_by_inode.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/show_file_csum.py` & `btrfs-9.1/examples/show_file_csum.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/show_free_space_fragmentation.py` & `btrfs-9.1/examples/show_free_space_fragmentation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 #!/usr/bin/python3
 
 import btrfs
 import math
 import sys
 
 if len(sys.argv) < 2:
-    print("Usage: {} <mountpoint>".format(sys.argv[0]))
+    print("Usage: {} [min_score] <mountpoint>".format(sys.argv[0]))
     sys.exit(1)
 
-fs = btrfs.FileSystem(sys.argv[1])
+fs = btrfs.FileSystem(sys.argv[-1])
+if len(sys.argv) == 3:
+    min_score = int(sys.argv[1])
+else:
+    min_score = 250
+print("Showing all block groups with free space fragmentation score >= {}".format(min_score))
 
 
 def extent_tree_free_space_extents(min_vaddr, max_vaddr):
     cur_end = min_vaddr
     for extent in fs.extents(min_vaddr, max_vaddr):
         next_start = extent.vaddr
         if isinstance(extent, btrfs.ctree.ExtentItem):
@@ -30,25 +35,22 @@
     list(fs.free_space_extents(0, 0))
     free_space_extents = fs.free_space_extents
 except:
     print("No Free Space Tree (space_cache=v2) found!")
     print("Falling back to using the extent tree to determine free space extents.")
     free_space_extents = extent_tree_free_space_extents
 
-skipped_max_usage = 0
+bad_chunks = 0
 for chunk in fs.chunks():
     if not chunk.type & btrfs.BLOCK_GROUP_DATA:
         continue
     try:
         block_group = fs.block_group(chunk.vaddr, chunk.length)
     except IndexError:
         continue
-    if block_group.used_pct >= 90:
-        skipped_max_usage += 1
-        continue
 
     min_vaddr = block_group.vaddr
     max_vaddr = block_group.vaddr + block_group.length - 1
 
     log2_bg_length = math.log2(block_group.length)
     half_width = (log2_bg_length - 11) / 2
     shift = (log2_bg_length + 11) / 2
@@ -69,11 +71,14 @@
     # space fragmentation is getting quite bad. Use btrfs-heatmap to create
     # images of specific block groups to see what's happening inside.
     fragments = 0
     score = 0
     for free_space_extent in free_space_extents(min_vaddr, max_vaddr):
         fragments += 1
         score += 1 - abs((math.log2(free_space_extent.length) - shift) / half_width)
-    print("vaddr {} length {} used_pct {} free space fragments {} score {}".format(
-        chunk.vaddr, chunk.length, block_group.used_pct, fragments, int(score)))
+    if score >= min_score:
+        bad_chunks += 1
+        print("vaddr {} length {} used_pct {} free space fragments {} score {}".format(
+            chunk.vaddr, chunk.length, block_group.used_pct, fragments, int(score)))
 
-print("Skipped because of usage > 90%: {} chunks".format(skipped_max_usage))
+if bad_chunks == 0:
+    print("No block groups found with free space fragmentation score >= {}".format(min_score))
```

### Comparing `btrfs-9/examples/show_metadata_tree_sizes.py` & `btrfs-9.1/examples/show_metadata_tree_sizes.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/examples/show_orphan_cleaner_progress.py` & `btrfs-9.1/examples/show_orphan_cleaner_progress.py`

 * *Files identical despite different names*

### Comparing `btrfs-9/README.md` & `btrfs-9.1/README.md`

 * *Files identical despite different names*

### Comparing `btrfs-9/setup.py` & `btrfs-9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='btrfs',
     packages=['btrfs'],
-    version='9',
+    version='9.1',
     description='Python module to inspect btrfs filesystems',
     long_description=long_description,
     author='Hans van Kranenburg',
     author_email='hans@knorrie.org',
     url='https://github.com/knorrie/python-btrfs',
-    download_url='https://github.com/knorrie/python-btrfs/tarball/v9',
+    download_url='https://github.com/knorrie/python-btrfs/tarball/v9.1',
     keywords=['btrfs', 'filesystem'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Programming Language :: Python :: 3 :: Only',
```

### Comparing `btrfs-9/PKG-INFO` & `btrfs-9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: btrfs
-Version: 9
+Version: 9.1
 Summary: Python module to inspect btrfs filesystems
 Home-page: https://github.com/knorrie/python-btrfs
 Author: Hans van Kranenburg
 Author-email: hans@knorrie.org
 License: UNKNOWN
-Download-URL: https://github.com/knorrie/python-btrfs/tarball/v9
+Download-URL: https://github.com/knorrie/python-btrfs/tarball/v9.1
 Description: python-btrfs
         ============
         
         Python 3 module to inspect btrfs filesystems.
         
         License: GPLv2.
```

